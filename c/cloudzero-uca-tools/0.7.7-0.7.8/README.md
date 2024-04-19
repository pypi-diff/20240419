# Comparing `tmp/cloudzero_uca_tools-0.7.7.tar.gz` & `tmp/cloudzero_uca_tools-0.7.8.tar.gz`

## Comparing `cloudzero_uca_tools-0.7.7.tar` & `cloudzero_uca_tools-0.7.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/__version__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/constants.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/exceptions.py
--rwxr-xr-x   0        0        0    11150 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/main.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/commands/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/commands/convert.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/__init__.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/aws.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/cli.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/custom_types.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/files.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/formatters.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/common/standards.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/alb_configuration.json
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/configuration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/csv_configuration.json
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/data.csv
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/example_alb_logs
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/sample_uca_data.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/test_configuration.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/test_data.csv
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/data/transform.jq
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/features/__init__.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/features/convert.py
--rw-r--r--   0        0        0     6341 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/features/generate.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/features/transform.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/features/transmit.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/interfaces/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/interfaces/uca_api.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/exceptions.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/interface.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/models.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/parser.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/util.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/__init__.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/client.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/plugin.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/cli/__init__.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/cli/main.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/LICENSE
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/README.md
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/pyproject.toml
--rw-r--r--   0        0        0    15827 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/__version__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/constants.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/exceptions.py
+-rwxr-xr-x   0        0        0    11510 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/main.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/commands/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/commands/convert.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/__init__.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/aws.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/cli.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/custom_types.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/files.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/formatters.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/standards.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/alb_configuration.json
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/configuration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/csv_configuration.json
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/data.csv
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/example_alb_logs
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/sample_uca_data.json
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/test_configuration.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/test_data.csv
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/transform.jq
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/__init__.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/convert.py
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/generate.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/transform.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/transmit.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/interfaces/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/interfaces/uca_api.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/exceptions.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/interface.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/models.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/parser.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/util.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/__init__.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/client.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/plugin.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/__init__.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/main.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/LICENSE
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/README.md
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0    15827 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/PKG-INFO
```

### Comparing `cloudzero_uca_tools-0.7.7/uca/constants.py` & `cloudzero_uca_tools-0.7.8/uca/constants.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/main.py` & `cloudzero_uca_tools-0.7.8/uca/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,29 +116,34 @@
         eprint("Please specify a --configuration file")
         sys.exit()
 
     output = os.path.abspath(output)
     configuration.output_path = output
     configuration.destination = "File"
 
+    configuration.template.pop("metric-name", None)
+    configuration.template.pop("telemetry-stream", None)
+
     if today:
         today = datetime.today().replace(hour=0, minute=0, second=0, microsecond=0)
         range_requested = TimeRange(start=today, end=today + timedelta(days=1))
+
     elif all([start, end]):
         try:
             start_date = utc_datetime_from_anything(start)
         except InvalidDate as error:
             print(f"Invalid start date: {error}")
             sys.exit(-1)
         try:
             end_date = utc_datetime_from_anything(end)
         except InvalidDate as error:
             print(f"Invalid end date: {error}")
             sys.exit(-1)
         range_requested = TimeRange(start=start_date, end=end_date)
+
     else:
         range_requested = None
 
     try:
         generate_settings = configuration.settings["generate"]
 
         if not isinstance(generate_settings, dict):
@@ -152,25 +157,32 @@
             raise ValueError(
                 f"Missing required key(s) in 'generate' config: {', '.join(missing_keys)}"
             )
 
         print("CloudZero UCA Data Generator")
         print("-" * 140)
         print(f"   Date Range : {range_requested or 'data driven'}")
+
         if "metric-name" not in configuration.template:
             print(f"  Granularity : {configuration.template['granularity']}")
+
         print(f"         Mode : {generate_settings['mode']}")
+
         if generate_settings["mode"] == "jitter":
             print(f"       Jitter : {generate_settings['jitter']}")
+
         elif generate_settings["mode"] == "allocation":
             print(f"   Allocation : {generate_settings['allocation']}")
+
             if generate_settings.get("jitter"):
                 print(f"              : with Jitter {generate_settings['jitter']}")
+
         if generate_settings.get("precision"):
             print(f"    Precision : {generate_settings['precision']}")
+
         print(f"Configuration : {configuration.configuration_path}")
         print(f"   Input Data : {input}")
         print(f"  Output File : {configuration.output_path}")
         print("-" * 140)
 
     except KeyError as error:
         eprint(f"Missing configurations: {error}")
@@ -225,57 +237,66 @@
 )
 @pass_root_configuration
 def transmit_uca_command(configuration, data, output, transform):
     if output:
         configuration.output_path = output
         configuration.destination = "File"
 
-    if 'telemetry-stream' in configuration.template:
-        stream_name = configuration.template['telemetry-stream']
-        stream_type = 'allocation'
-
-    elif 'metric-name' in configuration.template:
-        stream_name = configuration.template['metric-name']
-        stream_type = 'metric'
+    if "telemetry-stream" in configuration.template:
+        stream_name = configuration.template["telemetry-stream"].lower()
+        stream_type = "allocation"
+
+    elif "metric-name" in configuration.template:
+        stream_name = configuration.template["metric-name"].lower()
+        stream_type = "metric"
 
     else:
-        print("Missing 'telemetry-stream' or 'metric-name' key in 'template' config:")
+        print("Missing 'telemetry-stream' or 'metric-name' key in 'template' config")
         sys.exit(-1)
 
     print(f"Transmitting UCA data from {data} to {configuration.destination}")
     print("-" * 140)
 
     records = load_data_files(data, file_format="JSON")
     transform_script = load_transform_script(transform)
     uca_to_send, transformed_records, filtered_records = transform_data(
         records, transform_script
     )
 
-    transmit_type = "sum"
-    if "transmit_type" in configuration.settings and configuration.settings["transmit_type"].lower() in ["sum", "update", "delete"]:
-        transmit_type = configuration.settings["transmit_type"]
-
-        if configuration.settings["transmit_type"] == "delete":
-            for record in uca_to_send:
-                try:
-                    del record["value"]
+    if "transmit_type" not in configuration.settings:
+        print("Missing 'transmit_type' key in 'settings' config")
+        sys.exit(-1)
+
+    transmit_type = configuration.settings["transmit_type"].lower()
+    if transmit_type not in ["sum", "replace", "delete", "update"]:
+        print(f"Invalid value, '{transmit_type}', for 'transmit_type' key in 'settings' config")
+        print("Valid values: 'sum', 'replace', 'delete'")
+        sys.exit(-1)
+
+    if transmit_type == "delete":
+        for record in uca_to_send:
+            try:
+                del record["value"]
+
+            except KeyError:
+                pass
 
-                except KeyError:
-                    pass
+    if transmit_type == "update":
+        transmit_type = "replace"
 
     print(
         f" - Processed {len(records)} records "
         f"| {transformed_records} Transformed | {filtered_records} Filtered"
     )
     print(f" - {len(records) - filtered_records} records ready for transmission")
     print_uca_sample(uca_to_send)
     transmit(
-        stream_name.lower(),
-        stream_type.lower(),
-        transmit_type.lower(),
+        stream_name,
+        stream_type,
+        transmit_type,
         uca_to_send,
         configuration.output_path,
         configuration.api_key,
         configuration.dry_run,
     )
```

### Comparing `cloudzero_uca_tools-0.7.7/uca/commands/convert.py` & `cloudzero_uca_tools-0.7.8/uca/commands/convert.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/aws.py` & `cloudzero_uca_tools-0.7.8/uca/common/aws.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/cli.py` & `cloudzero_uca_tools-0.7.8/uca/common/cli.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/custom_types.py` & `cloudzero_uca_tools-0.7.8/uca/common/custom_types.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/files.py` & `cloudzero_uca_tools-0.7.8/uca/common/files.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/formatters.py` & `cloudzero_uca_tools-0.7.8/uca/common/formatters.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/common/standards.py` & `cloudzero_uca_tools-0.7.8/uca/common/standards.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/data/alb_configuration.json` & `cloudzero_uca_tools-0.7.8/uca/data/alb_configuration.json`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/data/example_alb_logs` & `cloudzero_uca_tools-0.7.8/uca/data/example_alb_logs`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/data/sample_uca_data.json` & `cloudzero_uca_tools-0.7.8/uca/data/sample_uca_data.json`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/features/convert.py` & `cloudzero_uca_tools-0.7.8/uca/features/convert.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/features/generate.py` & `cloudzero_uca_tools-0.7.8/uca/features/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,14 @@
         else:
             uca_events = _render_uca_data(uca_data, settings, uca_template)
 
     return uca_events
 
 
 def _render_uca_data(uca_data, settings, uca_template, timestamp=None):
-    uca_template.pop("telemetry-stream", "None")
-    uca_template.pop("metric-name", "None")
 
     unit_value_header = uca_template['value'].replace('$', '')
     timestamp_header = uca_template['timestamp'].replace('$', '')
 
     if settings.get("precision"):
         precision = int("1" + "0" * settings.get("precision"))
 
@@ -137,14 +135,15 @@
             uca_events.append(json.loads(rendered_template.strip().replace("\n", "")))
 
         except KeyError as err:
             print(f"Missing key in CSV data: {err}")
             sys.exit(-1)
         except Exception as err:
             print(f"Error: {err}")
+            print(row)
             sys.exit(-1)
 
     return uca_events
 
 
 def round_decimal(input_number: Decimal, precision):
     """
```

### Comparing `cloudzero_uca_tools-0.7.7/uca/features/transform.py` & `cloudzero_uca_tools-0.7.8/uca/features/transform.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/features/transmit.py` & `cloudzero_uca_tools-0.7.8/uca/features/transmit.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/interfaces/uca_api.py` & `cloudzero_uca_tools-0.7.8/uca/interfaces/uca_api.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/interface.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/interface.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/models.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/models.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/parser.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/client.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/client.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/plugin.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/aws/s3.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/s3.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/uca/vendored/aws_log_parser/cli/main.py` & `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/main.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/.gitignore` & `cloudzero_uca_tools-0.7.8/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/LICENSE` & `cloudzero_uca_tools-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/README.md` & `cloudzero_uca_tools-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.7/pyproject.toml` & `cloudzero_uca_tools-0.7.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 
 [project.scripts]
 uca = "uca.main:cli"
 
 [project.urls]
 Homepage = "https://github.com/Cloudzero/cloudzero-uca-tools"
 
+[tool]
+rye = { dev-dependencies = [
+    "hatch>=1.9.4",
+] }
+
 [tool.hatch.version]
 path = "uca/__version__.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["uca"]
 [tool.hatch.build.targets.sdist]
 include = [
@@ -119,8 +124,8 @@
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
     "ruff>=0.0.243"
 ]
 [tool.hatch.envs.lint.scripts]
 fix = "ruff . --fix"
-check = "ruff ."
+check = "ruff ."
```

### Comparing `cloudzero_uca_tools-0.7.7/PKG-INFO` & `cloudzero_uca_tools-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudzero-uca-tools
-Version: 0.7.7
+Version: 0.7.8
 Summary: CloudZero UCA Toolkit
 Project-URL: Homepage, https://github.com/Cloudzero/cloudzero-uca-tools
 Author-email: CloudZero <support@cloudzero.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: CloudZero,Toolkit,UCA,analysis,cost,economics,unit
 Classifier: Development Status :: 4 - Beta
```

