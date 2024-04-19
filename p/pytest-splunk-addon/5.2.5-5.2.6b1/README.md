# Comparing `tmp/pytest_splunk_addon-5.2.5.tar.gz` & `tmp/pytest_splunk_addon-5.2.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.2.5.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.2.6b1.tar", max compression
```

## Comparing `pytest_splunk_addon-5.2.5.tar` & `pytest_splunk_addon-5.2.6b1.tar`

### file list

```diff
@@ -1,86 +1,87 @@
--rw-r--r--   0        0        0    11341 2024-01-12 14:51:10.906850 pytest_splunk_addon-5.2.5/LICENSE
--rw-r--r--   0        0        0     2455 2024-01-12 14:51:45.266891 pytest_splunk_addon-5.2.5/pyproject.toml
--rw-r--r--   0        0        0     1886 2024-01-12 14:51:10.910850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      740 2024-01-12 14:51:45.262891 pytest_splunk_addon-5.2.5/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     8539 2024-01-12 14:51:10.910850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    31974 2024-01-12 14:51:10.910850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      575 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46777 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1216 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2787 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3308 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2078 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3132 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13280 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2756 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2443 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5387 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6164 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      750 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1247 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1126 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9582 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2347 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2797 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2438 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      966 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2020 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2382 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3933 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3263 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4222 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9214 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2961 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11200 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20764 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9400 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     6608 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    17483 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      885 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      858 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7335 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     4998 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4414 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4991 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3611 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3011 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      808 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3301 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5416 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11033 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10356 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21980 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      762 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      707 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11983 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11453 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      905 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7287 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46396 2024-01-12 14:51:10.914850 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15409 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2286 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16788 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6028 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6213 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      830 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4630 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1623 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3030 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3410 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17581 2024-01-12 14:51:10.918851 pytest_splunk_addon-5.2.5/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     1496 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-04-19 15:14:44.549955 pytest_splunk_addon-5.2.6b1/LICENSE
+-rw-r--r--   0        0        0     2322 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      751 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     5364 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/docker_class.py
+-rw-r--r--   0        0        0     8543 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    34048 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      579 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46781 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1220 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2791 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3312 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2082 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3136 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13284 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2760 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2447 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5391 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6168 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      754 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1130 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9586 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2351 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2801 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2442 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      970 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2386 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3937 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3267 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4226 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9218 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2965 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11204 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20768 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     9400 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     6608 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    17483 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      889 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7339 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     5002 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4418 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4995 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3615 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3015 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      812 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3305 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5420 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11040 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10360 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21984 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      766 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      711 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11987 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11457 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      909 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7291 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46400 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15413 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2290 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16792 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     6032 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6217 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      834 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4634 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1627 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3034 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3414 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0    17585 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.2.6b1/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.2.5/LICENSE` & `pytest_splunk_addon-5.2.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pyproject.toml` & `pytest_splunk_addon-5.2.6b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.2.5"
+version = "5.2.6-beta.1"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
@@ -36,29 +36,25 @@
 pytest = ">5.4.0,<8"
 splunk-sdk = ">=1.6"
 requests = "^2.31.0"
 jsonschema = ">=4,<5"
 pytest-xdist = ">=2.3.0"
 filelock = "^3.0"
 pytest-ordering = "~0.6"
-lovely-pytest-docker = { version="^0", optional = true }
 junitparser = "^2.2.0"
 addonfactory-splunk-conf-parser-lib = "*"
 defusedxml = "^0.7.1"
 Faker = ">=13.12,<19.0.0"
 xmltodict = "^0.13.0"
 xmlschema = "^1.11.3"
 splunksplwrapper = "^1.1.1"
 urllib3 = "<2"
 
-[tool.poetry.extras]
-docker = ['lovely-pytest-docker']
 
 [tool.poetry.group.dev.dependencies]
-lovely-pytest-docker = "~0.3.0"
 pytest-cov = "^3.0.0"
 requests-mock = "^1.8.0"
 freezegun = "^1.2.1"
 pytz = "^2022.1"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 # -*- coding: utf-8 -*-
 """Top-level package for splunk-app-test-lib."""
 
 __author__ = """Splunk Inc."""
 __email__ = "addonfactory@splunk.com"
-__version__ = "5.2.5"
+__version__ = "5.2.6-beta.1"
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
@@ -17,19 +17,21 @@
 import os
 import shutil
 from collections import defaultdict
 from time import sleep
 import json
 import pytest
 import requests
+import re
 import splunklib.client as client
 from splunksplwrapper.manager.jobs import Jobs
 from splunksplwrapper.splunk.cloud import CloudSplunk
 from splunksplwrapper.SearchUtil import SearchUtil
 from .standard_lib.event_ingestors import IngestorHelper
+from .docker_class import Services
 from .standard_lib.CIM_Models.datamodel_definition import datamodels
 import configparser
 from filelock import FileLock
 
 RESPONSIVE_SPLUNK_TIMEOUT = 300  # seconds
 
 LOGGER = logging.getLogger("pytest-splunk-addon")
@@ -319,14 +321,21 @@
     group.addoption(
         "--execute-test",
         action="store",
         dest="execute_test",
         help="Should execute test or not (True|False)",
         default="True",
     )
+    group.addoption(
+        "--keepalive",
+        "-K",
+        action="store_true",
+        default=False,
+        help="Keep docker containers alive",
+    )
 
 
 @pytest.fixture(scope="session")
 def splunk_setup(splunk):
     """
     Override this fixture in conftest.py, if any setup is required before the test session.
     splunk fixture can provide the details of the splunk instance in dict format.
@@ -737,26 +746,29 @@
             "session_headers": splunk_hec_uri[0].headers,
             "splunk_hec_uri": splunk_hec_uri[1],
             "sc4s_host": sc4s[0],  # for sc4s
             "sc4s_port": sc4s[1][514],  # for sc4s
         }
         thread_count = int(request.config.getoption("thread_count"))
         store_events = request.config.getoption("store_events")
-        IngestorHelper.ingest_events(
-            ingest_meta_data,
-            addon_path,
-            config_path,
-            thread_count,
-            store_events,
-        )
-        sleep(50)
-        if "PYTEST_XDIST_WORKER" in os.environ:
-            with open(os.environ.get("PYTEST_XDIST_TESTRUNUID") + "_wait", "w+"):
-                PYTEST_XDIST_TESTRUNUID = os.environ.get("PYTEST_XDIST_TESTRUNUID")
-
+        try:
+            IngestorHelper.ingest_events(
+                ingest_meta_data,
+                addon_path,
+                config_path,
+                thread_count,
+                store_events,
+            )
+            sleep(50)
+        except Exception as e:
+            raise e
+        finally:
+            if "PYTEST_XDIST_WORKER" in os.environ:
+                with open(os.environ.get("PYTEST_XDIST_TESTRUNUID") + "_wait", "w+"):
+                    PYTEST_XDIST_TESTRUNUID = os.environ.get("PYTEST_XDIST_TESTRUNUID")
     else:
         while not os.path.exists(os.environ.get("PYTEST_XDIST_TESTRUNUID") + "_wait"):
             sleep(1)
 
 
 @pytest.fixture(scope="session")
 def splunk_events_cleanup(request, splunk_search_util):
@@ -826,14 +838,64 @@
                     recommended_fields[model_key] += value
 
         return recommended_fields
 
     return update_recommended_fields
 
 
+@pytest.fixture(scope="session")
+def docker_ip():
+    """Determine IP address for TCP connections to Docker containers."""
+
+    # When talking to the Docker daemon via a UNIX socket, route all TCP
+    # traffic to docker containers via the TCP loopback interface.
+    docker_host = os.environ.get("DOCKER_HOST", "").strip()
+    if not docker_host:
+        return "127.0.0.1"
+
+    match = re.match("^tcp://(.+?):\d+$", docker_host)
+    if not match:
+        raise ValueError('Invalid value for DOCKER_HOST: "%s".' % (docker_host,))
+    return match.group(1)
+
+
+@pytest.fixture(scope="session")
+def docker_compose_files(pytestconfig):
+    """Get the docker-compose.yml absolute path.
+    Override this fixture in your tests if you need a custom location.
+    """
+    return [os.path.join(str(pytestconfig.rootdir), "tests", "docker-compose.yml")]
+
+
+@pytest.fixture(scope="session")
+def docker_services_project_name(pytestconfig):
+    """
+    Create unique project name for docker compose based on the pytestconfig root directory.
+    Characters prohibited by Docker compose project names are replaced with hyphens.
+    """
+    slug = re.sub(r"[^a-z0-9]+", "-", str(pytestconfig.rootdir).lower())
+    project_name = "pytest{}".format(slug)
+    return project_name
+
+
+@pytest.fixture(scope="session")
+def docker_services(
+    request, docker_compose_files, docker_ip, docker_services_project_name
+):
+    """Provide the docker services as a pytest fixture.
+
+    The services will be stopped after all tests are run.
+    """
+    keep_alive = request.config.getoption("--keepalive", False)
+    services = Services(docker_compose_files, docker_ip, docker_services_project_name)
+    yield services
+    if not keep_alive:
+        services.shutdown()
+
+
 def is_responsive_uf(uf):
     """
     Verify if the management port of Universal Forwarder is responsive or not
 
     Args:
         uf (dict): details of the Universal Forwarder instance
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+# -*- coding: utf-8 -*-
+"""
+There are 2 utilities included:
+
+1. CIM Compliance report generator for pytest-splunk-addon
+2. pytest-splunk-addon-data.conf generator
+
+"""
+
+from .junit_parser import JunitParser
+from .xml_event_parser import escape_char_event
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright 2022 Splunk Inc.
+#
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
 import logging
 import re
 import os
 
 from defusedxml import cElementTree as ET
 from defusedxml.cElementTree import ParseError
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/__init__.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-# -*- coding: utf-8 -*-
-"""
-There are 2 utilities included:
-
-1. CIM Compliance report generator for pytest-splunk-addon
-2. pytest-splunk-addon-data.conf generator
-
-"""
-
-from .junit_parser import JunitParser
-from .xml_event_parser import escape_char_event
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
-# Copyright 2021 Splunk Inc.
+# Copyright 2024 Splunk Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
```

### Comparing `pytest_splunk_addon-5.2.5/PKG-INFO` & `pytest_splunk_addon-5.2.6b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.2.5
+Version: 5.2.6b1
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
-Provides-Extra: docker
 Requires-Dist: Faker (>=13.12,<19.0.0)
 Requires-Dist: addonfactory-splunk-conf-parser-lib
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: filelock (>=3.0,<4.0)
 Requires-Dist: jsonschema (>=4,<5)
 Requires-Dist: junitparser (>=2.2.0,<3.0.0)
-Requires-Dist: lovely-pytest-docker (>=0,<1) ; extra == "docker"
 Requires-Dist: pytest (>5.4.0,<8)
 Requires-Dist: pytest-ordering (>=0.6,<0.7)
 Requires-Dist: pytest-xdist (>=2.3.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: splunk-sdk (>=1.6)
 Requires-Dist: splunksplwrapper (>=1.1.1,<2.0.0)
 Requires-Dist: urllib3 (<2)
```

