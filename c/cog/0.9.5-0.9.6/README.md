# Comparing `tmp/cog-0.9.5-py3-none-any.whl.zip` & `tmp/cog-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,107 +1,110 @@
-Zip file size: 90793 bytes, number of entries: 105
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-14 22:11 cog/.gitignore
--rw-r--r--  2.0 unx      362 b- defN 24-Mar-14 22:11 cog/__init__.py
--rw-r--r--  2.0 unx      411 b- defN 24-Mar-14 22:12 cog/_version.py
--rw-r--r--  2.0 unx      286 b- defN 24-Mar-14 22:11 cog/errors.py
--rw-r--r--  2.0 unx     2124 b- defN 24-Mar-14 22:11 cog/files.py
--rw-r--r--  2.0 unx     1945 b- defN 24-Mar-14 22:11 cog/json.py
--rw-r--r--  2.0 unx     3171 b- defN 24-Mar-14 22:11 cog/logging.py
--rw-r--r--  2.0 unx    15320 b- defN 24-Mar-14 22:11 cog/predictor.py
--rw-r--r--  2.0 unx     3308 b- defN 24-Mar-14 22:11 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 24-Mar-14 22:11 cog/suppress_output.py
--rw-r--r--  2.0 unx     8587 b- defN 24-Mar-14 22:11 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-14 22:11 cog/command/__init__.py
--rw-r--r--  2.0 unx    18782 b- defN 24-Mar-14 22:11 cog/command/ast_openapi_schema.py
--rw-r--r--  2.0 unx     1013 b- defN 24-Mar-14 22:11 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-14 22:11 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 24-Mar-14 22:11 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 24-Mar-14 22:11 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5349 b- defN 24-Mar-14 22:11 cog/server/helpers.py
--rw-r--r--  2.0 unx    17690 b- defN 24-Mar-14 22:11 cog/server/http.py
--rw-r--r--  2.0 unx      971 b- defN 24-Mar-14 22:11 cog/server/probes.py
--rw-r--r--  2.0 unx      689 b- defN 24-Mar-14 22:11 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    15246 b- defN 24-Mar-14 22:11 cog/server/runner.py
--rw-r--r--  2.0 unx     3326 b- defN 24-Mar-14 22:11 cog/server/webhook.py
--rw-r--r--  2.0 unx     8050 b- defN 24-Mar-14 22:11 cog/server/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-14 22:11 tests/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 24-Mar-14 22:11 tests/conftest.py
--rw-r--r--  2.0 unx     1737 b- defN 24-Mar-14 22:11 tests/test_json.py
--rw-r--r--  2.0 unx     1154 b- defN 24-Mar-14 22:11 tests/test_predictor.py
--rw-r--r--  2.0 unx     4689 b- defN 24-Mar-14 22:11 tests/test_types.py
--rw-r--r--  2.0 unx      113 b- defN 24-Mar-14 22:11 tests/fixtures/argv_override.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-14 22:11 tests/server/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 24-Mar-14 22:11 tests/server/conftest.py
--rw-r--r--  2.0 unx     4692 b- defN 24-Mar-14 22:11 tests/server/test_helpers.py
--rw-r--r--  2.0 unx    16956 b- defN 24-Mar-14 22:11 tests/server/test_http.py
--rw-r--r--  2.0 unx     8821 b- defN 24-Mar-14 22:11 tests/server/test_http_input.py
--rw-r--r--  2.0 unx     4020 b- defN 24-Mar-14 22:11 tests/server/test_http_output.py
--rw-r--r--  2.0 unx     1334 b- defN 24-Mar-14 22:11 tests/server/test_probes.py
--rw-r--r--  2.0 unx     1210 b- defN 24-Mar-14 22:11 tests/server/test_response_throttler.py
--rw-r--r--  2.0 unx    10931 b- defN 24-Mar-14 22:11 tests/server/test_runner.py
--rw-r--r--  2.0 unx     3225 b- defN 24-Mar-14 22:11 tests/server/test_webhook.py
--rw-r--r--  2.0 unx    16162 b- defN 24-Mar-14 22:11 tests/server/test_worker.py
--rw-r--r--  2.0 unx      209 b- defN 24-Mar-14 22:11 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
--rw-r--r--  2.0 unx      198 b- defN 24-Mar-14 22:11 tests/server/fixtures/catch_in_predict.py
--rw-r--r--  2.0 unx      232 b- defN 24-Mar-14 22:11 tests/server/fixtures/complex_output.py
--rw-r--r--  2.0 unx      131 b- defN 24-Mar-14 22:11 tests/server/fixtures/count_up.py
--rw-r--r--  2.0 unx      136 b- defN 24-Mar-14 22:11 tests/server/fixtures/exc_in_predict.py
--rw-r--r--  2.0 unx      133 b- defN 24-Mar-14 22:11 tests/server/fixtures/exc_in_setup.py
--rw-r--r--  2.0 unx      151 b- defN 24-Mar-14 22:11 tests/server/fixtures/exc_in_setup_and_predict.py
--rw-r--r--  2.0 unx       56 b- defN 24-Mar-14 22:11 tests/server/fixtures/exc_on_import.py
--rw-r--r--  2.0 unx      122 b- defN 24-Mar-14 22:11 tests/server/fixtures/exit_in_predict.py
--rw-r--r--  2.0 unx      124 b- defN 24-Mar-14 22:11 tests/server/fixtures/exit_in_setup.py
--rw-r--r--  2.0 unx       23 b- defN 24-Mar-14 22:11 tests/server/fixtures/exit_on_import.py
--rw-r--r--  2.0 unx       58 b- defN 24-Mar-14 22:11 tests/server/fixtures/function.py
--rw-r--r--  2.0 unx      159 b- defN 24-Mar-14 22:11 tests/server/fixtures/hello_world.py
--rw-r--r--  2.0 unx      197 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_choices_integer.py
--rw-r--r--  2.0 unx      139 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_file.py
--rw-r--r--  2.0 unx      160 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_ge_le.py
--rw-r--r--  2.0 unx      126 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_integer.py
--rw-r--r--  2.0 unx      152 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_integer_default.py
--rw-r--r--  2.0 unx      317 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_multiple.py
--rw-r--r--  2.0 unx      118 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_none.py
--rw-r--r--  2.0 unx      236 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_path.py
--rw-r--r--  2.0 unx      137 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_path_2.py
--rw-r--r--  2.0 unx      125 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_string.py
--rw-r--r--  2.0 unx      262 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_union_integer_or_list_of_integers.py
--rw-r--r--  2.0 unx      266 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_union_string_or_list_of_strings.py
--rw-r--r--  2.0 unx      205 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_unsupported_type.py
--rw-r--r--  2.0 unx      122 b- defN 24-Mar-14 22:11 tests/server/fixtures/input_untyped.py
--rw-r--r--  2.0 unx      160 b- defN 24-Mar-14 22:11 tests/server/fixtures/killed_in_predict.py
--rw-r--r--  2.0 unx      882 b- defN 24-Mar-14 22:11 tests/server/fixtures/logging.py
--rw-r--r--  2.0 unx      109 b- defN 24-Mar-14 22:11 tests/server/fixtures/missing_predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-14 22:11 tests/server/fixtures/missing_predictor.py
--rw-r--r--  2.0 unx      482 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_complex_input.py
--rw-r--r--  2.0 unx      332 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_custom_output_type.py
--rw-r--r--  2.0 unx      169 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_input_int_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_output_list.py
--rw-r--r--  2.0 unx      374 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_output_type.py
--rw-r--r--  2.0 unx      161 b- defN 24-Mar-14 22:11 tests/server/fixtures/openapi_output_yield.py
--rw-r--r--  2.0 unx      264 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_complex.py
--rw-r--r--  2.0 unx      148 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_file.py
--rw-r--r--  2.0 unx      192 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_file_named.py
--rw-r--r--  2.0 unx      257 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_iterator_complex.py
--rw-r--r--  2.0 unx      151 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_numpy.py
--rw-r--r--  2.0 unx      355 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_path_image.py
--rw-r--r--  2.0 unx      323 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_path_text.py
--rw-r--r--  2.0 unx      115 b- defN 24-Mar-14 22:11 tests/server/fixtures/output_wrong_type.py
--rw-r--r--  2.0 unx      175 b- defN 24-Mar-14 22:11 tests/server/fixtures/setup.py
--rw-r--r--  2.0 unx      262 b- defN 24-Mar-14 22:11 tests/server/fixtures/setup_uses_async.py
--rw-r--r--  2.0 unx      167 b- defN 24-Mar-14 22:11 tests/server/fixtures/setup_weights.py
--rw-r--r--  2.0 unx      118 b- defN 24-Mar-14 22:11 tests/server/fixtures/simple.py
--rw-r--r--  2.0 unx      193 b- defN 24-Mar-14 22:11 tests/server/fixtures/sleep.py
--rw-r--r--  2.0 unx      219 b- defN 24-Mar-14 22:11 tests/server/fixtures/slow_predict.py
--rw-r--r--  2.0 unx      122 b- defN 24-Mar-14 22:11 tests/server/fixtures/slow_setup.py
--rw-r--r--  2.0 unx      290 b- defN 24-Mar-14 22:11 tests/server/fixtures/steps.py
--rw-r--r--  2.0 unx      359 b- defN 24-Mar-14 22:11 tests/server/fixtures/train.py
--rw-r--r--  2.0 unx      263 b- defN 24-Mar-14 22:11 tests/server/fixtures/yield_concatenate_iterator.py
--rw-r--r--  2.0 unx      506 b- defN 24-Mar-14 22:11 tests/server/fixtures/yield_files.py
--rw-r--r--  2.0 unx      245 b- defN 24-Mar-14 22:11 tests/server/fixtures/yield_strings.py
--rw-r--r--  2.0 unx      339 b- defN 24-Mar-14 22:11 tests/server/fixtures/yield_strings_file_input.py
--rw-r--r--  2.0 unx    11347 b- defN 24-Mar-14 22:12 cog-0.9.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    36704 b- defN 24-Mar-14 22:12 cog-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 22:12 cog-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-Mar-14 22:12 cog-0.9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9284 b- defN 24-Mar-14 22:12 cog-0.9.5.dist-info/RECORD
-105 files, 256179 bytes uncompressed, 75919 bytes compressed:  70.4%
+Zip file size: 95519 bytes, number of entries: 108
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-19 20:25 cog/.gitignore
+-rw-r--r--  2.0 unx      362 b- defN 24-Apr-19 20:25 cog/__init__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-19 20:25 cog/_version.py
+-rw-r--r--  2.0 unx    10313 b- defN 24-Apr-19 20:25 cog/code_xforms.py
+-rw-r--r--  2.0 unx      286 b- defN 24-Apr-19 20:25 cog/errors.py
+-rw-r--r--  2.0 unx     2124 b- defN 24-Apr-19 20:25 cog/files.py
+-rw-r--r--  2.0 unx     1945 b- defN 24-Apr-19 20:25 cog/json.py
+-rw-r--r--  2.0 unx     3171 b- defN 24-Apr-19 20:25 cog/logging.py
+-rw-r--r--  2.0 unx    17091 b- defN 24-Apr-19 20:25 cog/predictor.py
+-rw-r--r--  2.0 unx     3308 b- defN 24-Apr-19 20:25 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 24-Apr-19 20:25 cog/suppress_output.py
+-rw-r--r--  2.0 unx     8587 b- defN 24-Apr-19 20:25 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 cog/command/__init__.py
+-rw-r--r--  2.0 unx    18782 b- defN 24-Apr-19 20:25 cog/command/ast_openapi_schema.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-Apr-19 20:25 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 24-Apr-19 20:25 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-19 20:25 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5349 b- defN 24-Apr-19 20:25 cog/server/helpers.py
+-rw-r--r--  2.0 unx    16945 b- defN 24-Apr-19 20:25 cog/server/http.py
+-rw-r--r--  2.0 unx      971 b- defN 24-Apr-19 20:25 cog/server/probes.py
+-rw-r--r--  2.0 unx      689 b- defN 24-Apr-19 20:25 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    15515 b- defN 24-Apr-19 20:25 cog/server/runner.py
+-rw-r--r--  2.0 unx     3326 b- defN 24-Apr-19 20:25 cog/server/webhook.py
+-rw-r--r--  2.0 unx     8050 b- defN 24-Apr-19 20:25 cog/server/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 24-Apr-19 20:25 tests/conftest.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-Apr-19 20:25 tests/test_json.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-Apr-19 20:25 tests/test_predictor.py
+-rw-r--r--  2.0 unx     4689 b- defN 24-Apr-19 20:25 tests/test_types.py
+-rw-r--r--  2.0 unx      113 b- defN 24-Apr-19 20:25 tests/fixtures/argv_override.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/server/__init__.py
+-rw-r--r--  2.0 unx     2800 b- defN 24-Apr-19 20:25 tests/server/conftest.py
+-rw-r--r--  2.0 unx     2564 b- defN 24-Apr-19 20:25 tests/server/test_code_xforms.py
+-rw-r--r--  2.0 unx     4692 b- defN 24-Apr-19 20:25 tests/server/test_helpers.py
+-rw-r--r--  2.0 unx    16956 b- defN 24-Apr-19 20:25 tests/server/test_http.py
+-rw-r--r--  2.0 unx     8821 b- defN 24-Apr-19 20:25 tests/server/test_http_input.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-Apr-19 20:25 tests/server/test_http_output.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-Apr-19 20:25 tests/server/test_predictor.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-Apr-19 20:25 tests/server/test_probes.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-Apr-19 20:25 tests/server/test_response_throttler.py
+-rw-r--r--  2.0 unx    10931 b- defN 24-Apr-19 20:25 tests/server/test_runner.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-Apr-19 20:25 tests/server/test_webhook.py
+-rw-r--r--  2.0 unx    16162 b- defN 24-Apr-19 20:25 tests/server/test_worker.py
+-rw-r--r--  2.0 unx      209 b- defN 24-Apr-19 20:25 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
+-rw-r--r--  2.0 unx      198 b- defN 24-Apr-19 20:25 tests/server/fixtures/catch_in_predict.py
+-rw-r--r--  2.0 unx      232 b- defN 24-Apr-19 20:25 tests/server/fixtures/complex_output.py
+-rw-r--r--  2.0 unx      131 b- defN 24-Apr-19 20:25 tests/server/fixtures/count_up.py
+-rw-r--r--  2.0 unx      136 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_predict.py
+-rw-r--r--  2.0 unx      133 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_setup.py
+-rw-r--r--  2.0 unx      151 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_in_setup_and_predict.py
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-19 20:25 tests/server/fixtures/exc_on_import.py
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_in_predict.py
+-rw-r--r--  2.0 unx      124 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_in_setup.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-19 20:25 tests/server/fixtures/exit_on_import.py
+-rw-r--r--  2.0 unx       58 b- defN 24-Apr-19 20:25 tests/server/fixtures/function.py
+-rw-r--r--  2.0 unx      159 b- defN 24-Apr-19 20:25 tests/server/fixtures/hello_world.py
+-rw-r--r--  2.0 unx      197 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_choices_integer.py
+-rw-r--r--  2.0 unx      139 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_file.py
+-rw-r--r--  2.0 unx      160 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_ge_le.py
+-rw-r--r--  2.0 unx      126 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_integer.py
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_integer_default.py
+-rw-r--r--  2.0 unx      317 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_multiple.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_none.py
+-rw-r--r--  2.0 unx      236 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_path.py
+-rw-r--r--  2.0 unx      137 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_path_2.py
+-rw-r--r--  2.0 unx      125 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_string.py
+-rw-r--r--  2.0 unx      262 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_union_integer_or_list_of_integers.py
+-rw-r--r--  2.0 unx      266 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_union_string_or_list_of_strings.py
+-rw-r--r--  2.0 unx      205 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_unsupported_type.py
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/input_untyped.py
+-rw-r--r--  2.0 unx      160 b- defN 24-Apr-19 20:25 tests/server/fixtures/killed_in_predict.py
+-rw-r--r--  2.0 unx      882 b- defN 24-Apr-19 20:25 tests/server/fixtures/logging.py
+-rw-r--r--  2.0 unx      109 b- defN 24-Apr-19 20:25 tests/server/fixtures/missing_predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-19 20:25 tests/server/fixtures/missing_predictor.py
+-rw-r--r--  2.0 unx      482 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_complex_input.py
+-rw-r--r--  2.0 unx      332 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_custom_output_type.py
+-rw-r--r--  2.0 unx      169 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_input_int_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_list.py
+-rw-r--r--  2.0 unx      374 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_type.py
+-rw-r--r--  2.0 unx      161 b- defN 24-Apr-19 20:25 tests/server/fixtures/openapi_output_yield.py
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_complex.py
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_file.py
+-rw-r--r--  2.0 unx      192 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_file_named.py
+-rw-r--r--  2.0 unx      257 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_iterator_complex.py
+-rw-r--r--  2.0 unx      151 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_numpy.py
+-rw-r--r--  2.0 unx      355 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_path_image.py
+-rw-r--r--  2.0 unx      323 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_path_text.py
+-rw-r--r--  2.0 unx      115 b- defN 24-Apr-19 20:25 tests/server/fixtures/output_wrong_type.py
+-rw-r--r--  2.0 unx      175 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup.py
+-rw-r--r--  2.0 unx      262 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup_uses_async.py
+-rw-r--r--  2.0 unx      167 b- defN 24-Apr-19 20:25 tests/server/fixtures/setup_weights.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-19 20:25 tests/server/fixtures/simple.py
+-rw-r--r--  2.0 unx      193 b- defN 24-Apr-19 20:25 tests/server/fixtures/sleep.py
+-rw-r--r--  2.0 unx      219 b- defN 24-Apr-19 20:25 tests/server/fixtures/slow_predict.py
+-rw-r--r--  2.0 unx      122 b- defN 24-Apr-19 20:25 tests/server/fixtures/slow_setup.py
+-rw-r--r--  2.0 unx      290 b- defN 24-Apr-19 20:25 tests/server/fixtures/steps.py
+-rw-r--r--  2.0 unx      359 b- defN 24-Apr-19 20:25 tests/server/fixtures/train.py
+-rw-r--r--  2.0 unx      263 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_concatenate_iterator.py
+-rw-r--r--  2.0 unx      506 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_files.py
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_strings.py
+-rw-r--r--  2.0 unx      339 b- defN 24-Apr-19 20:25 tests/server/fixtures/yield_strings_file_input.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    36704 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9536 b- defN 24-Apr-19 20:25 cog-0.9.6.dist-info/RECORD
+108 files, 274299 bytes uncompressed, 80257 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: cog/__init__.py
 Comment: 
 
 Filename: cog/_version.py
 Comment: 
 
+Filename: cog/code_xforms.py
+Comment: 
+
 Filename: cog/errors.py
 Comment: 
 
 Filename: cog/files.py
 Comment: 
 
 Filename: cog/json.py
@@ -90,26 +93,32 @@
 
 Filename: tests/server/__init__.py
 Comment: 
 
 Filename: tests/server/conftest.py
 Comment: 
 
+Filename: tests/server/test_code_xforms.py
+Comment: 
+
 Filename: tests/server/test_helpers.py
 Comment: 
 
 Filename: tests/server/test_http.py
 Comment: 
 
 Filename: tests/server/test_http_input.py
 Comment: 
 
 Filename: tests/server/test_http_output.py
 Comment: 
 
+Filename: tests/server/test_predictor.py
+Comment: 
+
 Filename: tests/server/test_probes.py
 Comment: 
 
 Filename: tests/server/test_response_throttler.py
 Comment: 
 
 Filename: tests/server/test_runner.py
@@ -294,23 +303,23 @@
 
 Filename: tests/server/fixtures/yield_strings.py
 Comment: 
 
 Filename: tests/server/fixtures/yield_strings_file_input.py
 Comment: 
 
-Filename: cog-0.9.5.dist-info/LICENSE
+Filename: cog-0.9.6.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.9.5.dist-info/METADATA
+Filename: cog-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.9.5.dist-info/WHEEL
+Filename: cog-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.9.5.dist-info/top_level.txt
+Filename: cog-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.9.5.dist-info/RECORD
+Filename: cog-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.5'
-__version_tuple__ = version_tuple = (0, 9, 5)
+__version__ = version = '0.9.6'
+__version_tuple__ = version_tuple = (0, 9, 6)
```

## cog/predictor.py

```diff
@@ -1,14 +1,15 @@
 import enum
 import importlib.util
 import inspect
 import io
 import os.path
 import sys
 import types
+import uuid
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
@@ -16,14 +17,18 @@
     Optional,
     Type,
     Union,
     cast,
 )
 from unittest.mock import patch
 
+import structlog
+
+import cog.code_xforms as code_xforms
+
 try:
     from typing import get_args, get_origin
 except ImportError:  # Python < 3.8
     from typing_compat import get_args, get_origin  # type: ignore
 
 import yaml
 from pydantic import BaseModel, Field, create_model
@@ -40,14 +45,16 @@
     Input,
     URLPath,
 )
 from .types import (
     Path as CogPath,
 )
 
+log = structlog.get_logger("cog.server.predictor")
+
 ALLOWED_INPUT_TYPES: List[Type[Any]] = [str, int, float, bool, CogFile, CogPath]
 
 
 class BasePredictor(ABC):
     def setup(self, weights: Optional[Union[CogFile, CogPath, str]] = None) -> None:
         """
         An optional method to prepare the model so multiple predictions run efficiently.
@@ -169,34 +176,77 @@
         raise PredictorNotSet(
             f"Can't run predictions: '{mode}' option not found in cog.yaml"
         )
 
     return config[mode]
 
 
-def load_predictor_from_ref(ref: str) -> BasePredictor:
-    module_path, class_name = ref.split(":", 1)
-    module_name = os.path.basename(module_path).split(".py", 1)[0]
+def load_full_predictor_from_file(
+    module_path: str, module_name: str
+) -> types.ModuleType:
     spec = importlib.util.spec_from_file_location(module_name, module_path)
     assert spec is not None
     module = importlib.util.module_from_spec(spec)
     assert spec.loader is not None
-
     # Remove any sys.argv while importing predictor to avoid conflicts when
     # user code calls argparse.Parser.parse_args in production
     with patch("sys.argv", sys.argv[:1]):
         spec.loader.exec_module(module)
+    return module
+
+
+def load_slim_predictor_from_file(
+    module_path: str, class_name: str, method_name: str
+) -> Union[types.ModuleType, None]:
+    with open(module_path, encoding="utf-8") as file:
+        source_code = file.read()
+    stripped_source = code_xforms.strip_model_source_code(
+        source_code, class_name, method_name
+    )
+    module = code_xforms.load_module_from_string(uuid.uuid4().hex, stripped_source)
+    return module
 
+
+def get_predictor(module: types.ModuleType, class_name: str) -> Any:
     predictor = getattr(module, class_name)
     # It could be a class or a function
     if inspect.isclass(predictor):
         return predictor()
     return predictor
 
 
+def load_slim_predictor_from_ref(ref: str, method_name: str) -> BasePredictor:
+    module_path, class_name = ref.split(":", 1)
+    module_name = os.path.basename(module_path).split(".py", 1)[0]
+    module = None
+    try:
+        if sys.version_info >= (3, 9):
+            module = load_slim_predictor_from_file(module_path, class_name, method_name)
+            if not module:
+                log.debug(f"[{module_name}] fast loader returned None")
+        else:
+            log.debug(f"[{module_name}] cannot use fast loader as current Python <3.9")
+    except Exception as e:
+        log.debug(f"[{module_name}] fast loader failed: {e}")
+    finally:
+        if not module:
+            log.debug(f"[{module_name}] falling back to slow loader")
+            module = load_full_predictor_from_file(module_path, module_name)
+    predictor = get_predictor(module, class_name)
+    return predictor
+
+
+def load_predictor_from_ref(ref: str) -> BasePredictor:
+    module_path, class_name = ref.split(":", 1)
+    module_name = os.path.basename(module_path).split(".py", 1)[0]
+    module = load_full_predictor_from_file(module_path, module_name)
+    predictor = get_predictor(module, class_name)
+    return predictor
+
+
 # Base class for inputs, constructed dynamically in get_input_type().
 # (This can't be a docstring or it gets passed through to the schema.)
 class BaseInput(BaseModel):
     class Config:
         # When using `choices`, the type is converted into an enum to validate
         # But, after validation, we want to pass the actual value to predict(), not the enum object
         use_enum_values = True
```

## cog/command/openapi_schema.py

```diff
@@ -1,31 +1,52 @@
 """
 python -m cog.command.specification
 
 This prints a JSON object describing the inputs of the model.
 """
 
 import json
+from typing import Any, Dict, List, Union
 
 from ..errors import CogError, ConfigDoesNotExist, PredictorNotSet
 from ..predictor import load_config
 from ..schema import Status
 from ..server.http import create_app
 from ..suppress_output import suppress_output
 
+
+def remove_title_next_to_ref(
+    schema_node: Union[Dict[str, Any], List[Any]],
+) -> Union[Dict[str, Any], List[Any]]:
+    """
+    Recursively remove 'title' from schema components that have a '$ref'.
+    This function addresses a non-compliance issue in FastAPI's OpenAPI schema generation, where
+    'title' fields adjacent to '$ref' fields can cause validation problems with some OpenAPI tools.
+    """
+    if isinstance(schema_node, dict):
+        if "$ref" in schema_node and "title" in schema_node:
+            del schema_node["title"]
+        for _key, value in schema_node.items():
+            remove_title_next_to_ref(value)
+    elif isinstance(schema_node, list):  # type: ignore[reportUnnecessaryIsInstance]
+        for i, item in enumerate(schema_node):
+            schema_node[i] = remove_title_next_to_ref(item)
+    return schema_node
+
+
 if __name__ == "__main__":
     schema = {}
     try:
         with suppress_output():
             config = load_config()
             app = create_app(config, shutdown_event=None, is_build=True)
             if (
                 app.state.setup_result
                 and app.state.setup_result.status == Status.FAILED
             ):
                 raise CogError(app.state.setup_result.logs)
-            schema = app.openapi()
+            schema = remove_title_next_to_ref(app.openapi())
     except (ConfigDoesNotExist, PredictorNotSet):
         # If there is no cog.yaml or 'predict' has not been set, then there is no type signature.
         # Not an error, there just isn't anything.
         pass
     print(json.dumps(schema, indent=2))
```

## cog/server/http.py

```diff
@@ -43,15 +43,15 @@
 from ..predictor import (
     get_input_type,
     get_output_type,
     get_predictor_ref,
     get_training_input_type,
     get_training_output_type,
     load_config,
-    load_predictor_from_ref,
+    load_slim_predictor_from_ref,
 )
 from .runner import (
     PredictionRunner,
     RunnerBusyError,
     SetupResult,
     SetupTask,
     UnknownPredictionError,
@@ -123,24 +123,17 @@
         log.info("shutdown requested via http")
         if shutdown_event is not None:
             shutdown_event.set()
         return JSONResponse({}, status_code=200)
 
     try:
         predictor_ref = get_predictor_ref(config, mode)
-        # use bundled schema if it exists
-        schema_module = None  # schema.create_schema_module() - breaks complex types, always use slow path for now
-        if schema_module is not None:
-            log.info("using bundled schema")
-            InputType = schema_module.Input
-            OutputType = schema_module.Output
-        else:
-            predictor = load_predictor_from_ref(predictor_ref)
-            InputType = get_input_type(predictor)
-            OutputType = get_output_type(predictor)
+        predictor = load_slim_predictor_from_ref(predictor_ref, "predict")
+        InputType = get_input_type(predictor)
+        OutputType = get_output_type(predictor)
     except Exception:
         msg = "Error while loading predictor:\n\n" + traceback.format_exc()
         add_setup_failed_routes(app, started_at, msg)
         return app
 
     runner = PredictionRunner(
         predictor_ref=predictor_ref,
@@ -168,24 +161,17 @@
                 return await f(*args, **kwargs)
 
         return wrapped
 
     if "train" in config:
         try:
             trainer_ref = get_predictor_ref(config, "train")
-            # use bundled schema if it exists
-            schema_module = None  # schema.create_schema_module() - breaks complex types, always use slow path for now
-            if schema_module is not None:
-                log.info("using bundled schema")
-                TrainingInputType = schema_module.TrainingInputType
-                TrainingOutputType = schema_module.TrainingOutputType
-            else:
-                trainer = load_predictor_from_ref(trainer_ref)
-                TrainingInputType = get_training_input_type(trainer)
-                TrainingOutputType = get_training_output_type(trainer)
+            trainer = load_slim_predictor_from_ref(trainer_ref, "train")
+            TrainingInputType = get_training_input_type(trainer)
+            TrainingOutputType = get_training_output_type(trainer)
 
             class TrainingRequest(
                 schema.TrainingRequest.with_types(input_type=TrainingInputType)
             ):
                 pass
 
             TrainingResponse = schema.TrainingResponse.with_types(
```

## cog/server/runner.py

```diff
@@ -378,23 +378,29 @@
 ) -> schema.PredictionResponse:
     initial_prediction = request.dict()
 
     output_type = None
     input_dict = initial_prediction["input"]
 
     for k, v in input_dict.items():
-        if isinstance(v, types.URLPath):
-            try:
+        try:
+            # Check if v is an instance of URLPath
+            if isinstance(v, types.URLPath):
                 input_dict[k] = v.convert()
-            except requests.exceptions.RequestException as e:
-                tb = traceback.format_exc()
-                event_handler.append_logs(tb)
-                event_handler.failed(error=str(e))
-                log.warn("failed to download url path from input", exc_info=True)
-                return event_handler.response
+            # Check if v is a list of URLPath instances
+            elif isinstance(v, list) and all(
+                isinstance(item, types.URLPath) for item in v
+            ):
+                input_dict[k] = [item.convert() for item in v]
+        except requests.exceptions.RequestException as e:
+            tb = traceback.format_exc()
+            event_handler.append_logs(tb)
+            event_handler.failed(error=str(e))
+            log.warn("Failed to download url path from input", exc_info=True)
+            return event_handler.response
 
     for event in worker.predict(input_dict, poll=0.1):
         if should_cancel.is_set():
             worker.cancel()
             should_cancel.clear()
 
         if isinstance(event, Heartbeat):
```

## tests/server/test_worker.py

```diff
@@ -18,15 +18,15 @@
 from hypothesis.stateful import (
     RuleBasedStateMachine,
     precondition,
     rule,
 )
 
 # Set a longer deadline on CI as the instances are a bit slower.
-settings.register_profile("ci", max_examples=100, deadline=1000)
+settings.register_profile("ci", max_examples=100, deadline=1500)
 settings.register_profile("default", max_examples=10, deadline=1000)
 settings.register_profile("slow", max_examples=10, deadline=2000)
 settings.load_profile(os.getenv("HYPOTHESIS_PROFILE", "default"))
 
 ST_NAMES = st.sampled_from(["John", "Barry", "Elspeth", "Hamid", "Ronnie", "Yasmeen"])
 
 SETUP_FATAL_FIXTURES = [
```

## Comparing `cog-0.9.5.dist-info/LICENSE` & `cog-0.9.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.9.5.dist-info/METADATA` & `cog-0.9.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.9.5
+Version: 0.9.6
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `cog-0.9.5.dist-info/RECORD` & `cog-0.9.6.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 cog/.gitignore,sha256=OIzCsCr9oYv3wBtJU_TppxWi-OhuDmwCBrrUqcE6kfY,13
 cog/__init__.py,sha256=qDIBBVsf5tfoaCGu49zQyYQb_AWtCwIxQrp9RLZlbbI,362
-cog/_version.py,sha256=mGWHnd7vlgJDPI-PIRFkte_okQf1MI2ryZANxv7K9gY,411
+cog/_version.py,sha256=11ciOFzse5i9Y6lr7kosD6U2UdIm5Bsf7hdpK0Hg_2I,411
+cog/code_xforms.py,sha256=ZCiXn1bN5fIoY_GU91mwNeZr7B4rmE_GXiJVcZONyaM,10313
 cog/errors.py,sha256=pB29TjzvXmyqbqi3zPOlLobFJnVWb6GJ9WsLE-77TIQ,286
 cog/files.py,sha256=8PENbdvtuVl6sbgsoZSAHId60TSM8iU-dNMpNPS9h1A,2124
 cog/json.py,sha256=xNwlgqYY7egcHZzcWs94S17q3KbtZVyaDe5gCyZG-Vo,1945
 cog/logging.py,sha256=3I7jOG1HKU5oh6-xJF1dh_qFMJMBrjo9Z60zM6sr3qU,3171
-cog/predictor.py,sha256=8aAhS2bM1FVZH6LJ0VgSPy4aqr9QhdZ68bBPMmo15wQ,15320
+cog/predictor.py,sha256=JIgJzax9smlIDH-bax0PSY31NoUiD6b_92eOvgEFMfY,17091
 cog/schema.py,sha256=NaVXnqMQ-duhWkS8vomg2NrXhdLn9nEkFKHPnhRtb7A,3308
 cog/suppress_output.py,sha256=HHSNGR9j4rkyLL4mGnkluxzSQAYYIUcEWGdNCtYfwZc,645
 cog/types.py,sha256=nYMt6hHND-tEvfdvKXoBEzRwatBrKKHHPxJDVZnOUAI,8587
 cog/command/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/command/ast_openapi_schema.py,sha256=J42SekXuXHDmVbNKD29kMjWaRyxKnwFHY2BG8cVn28s,18782
-cog/command/openapi_schema.py,sha256=MvurAZeEUBKLSDKCtDccNDDkXm4dvftc3xy8KcC_wDk,1013
+cog/command/openapi_schema.py,sha256=h-bfqVHkdOjnK469-mKhY9U18JaGK59W4Ur9bFWoM1U,1934
 cog/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/server/eventtypes.py,sha256=s2iJKjiXFG_cRIS_a4VQE_wVQosoyppRqTJfevBD_XI,593
 cog/server/exceptions.py,sha256=HknokO6g7gIlbIAMBM8685gE4Xgb8lykC-gTF6SLEYM,149
 cog/server/helpers.py,sha256=Z0mRZJOonbqc7Kir3JiGSbg-0svmtJCVpp3IaET3MlM,5349
-cog/server/http.py,sha256=2OERUzbfpZQ-jXCUgJapQSS3Dppsc8cYyLBV45dT1ms,17690
+cog/server/http.py,sha256=-xoaDzal7FV7_pAIATOM-TQZi90iEZeupw36MlPfjZY,16945
 cog/server/probes.py,sha256=QV_AaKzKM64euwiFuo0Fw8kjA6GYSzBkZ4kXy7QS7vE,971
 cog/server/response_throttler.py,sha256=sDjMj_hvJyiB4IywBB9zl-D_EcRKSK4SIT_mujORAXk,689
-cog/server/runner.py,sha256=4k2GSaIYcqXWK-7fwoMXTAZlfTK6AkTO5K9W0PCPzgc,15246
+cog/server/runner.py,sha256=-fXchhxcPeuXMWtKbgajuIyePSxEKF5r-pe7cNo84xQ,15515
 cog/server/webhook.py,sha256=alohqVPU8aOsPz10N77uv2eFlvGMk8RBUj37eWFzLjY,3326
 cog/server/worker.py,sha256=VybuJ3bAFdNsOcqAkhv8M2-FkSx7sr8atN_fFAx2yLc,8050
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=KbeqWWshZoqqT6aLcZGB3_zLMe1G0IQ61BhoKQU1Xro,536
 tests/test_json.py,sha256=fkrKcif7qoHoSoQNwK24267MWeO5Lwyz8EMRUUT122Q,1737
 tests/test_predictor.py,sha256=K6yc1Va8isKetQxMIyQJ6WG92HJHKI8vvxGj4sA3rDY,1154
 tests/test_types.py,sha256=Okt_mbTcsVQapR5su0CIQEhMV-5xuFpXjzxKldFgR_Q,4689
 tests/fixtures/argv_override.py,sha256=dGjPI-zOkXaA0PVG1n_uKTxGB7WlSuuoa8WxBz6ZGoo,113
 tests/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/server/conftest.py,sha256=Njsjm2jgUf-4RaDMa3msxqgp0RMQIz0DZQtdP5i0sFQ,2800
+tests/server/test_code_xforms.py,sha256=3oBRcqz2UgzkBKvIIpicR0hWYpk5hTDHl6W9qVpCdYE,2564
 tests/server/test_helpers.py,sha256=XVpcv42AYwUmo1wAoR73FMdN4tOoRYkqaTjduKE_aDA,4692
 tests/server/test_http.py,sha256=3TqUNYjYkTktHE-8WskvTWQDRGWGFHSvqeuBgj6dr04,16956
 tests/server/test_http_input.py,sha256=7yRu_bUiUnT9-g_RaGlSXrP3X_SFlUjs1DPD7kD0rp4,8821
 tests/server/test_http_output.py,sha256=AViMdeDEoSNfNtkftmtvyYG2A4DCP0ViGrmnZjYXuy4,4020
+tests/server/test_predictor.py,sha256=x7xpvWtJkY1N4lvk1SzhQpY57e_tNrk-atzTS2Lliog,2775
 tests/server/test_probes.py,sha256=L1ncJKDELevnxFq_Nr4hiZtNrLhkbClzbvAIGJ-RTzA,1334
 tests/server/test_response_throttler.py,sha256=5Dfslni4ioDrNbMJ2xNt-3La4K1SBm6LlV1UTosTlbg,1210
 tests/server/test_runner.py,sha256=dQymyMKrpYUpfifF_0R294520ZG7MdBDA9XlZHcKJ0s,10931
 tests/server/test_webhook.py,sha256=gt8XfJ-gizqKd__K2sCKTNkWJ1iYm29h1YDIYxxJo3Y,3225
-tests/server/test_worker.py,sha256=tOjI9ToxPpnNVdSWCtiEct-wXPVvE9W7X-eTAMwzjbI,16162
+tests/server/test_worker.py,sha256=XH_B63JAmFniAQzYxO0Ee_2VKGa5S01NwVIq5iBo6Oo,16162
 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py,sha256=UcuNOP_0ZSW5M8ijN8fHPhCoSRZ96SswSx6TOn3GEZs,209
 tests/server/fixtures/catch_in_predict.py,sha256=jLjudcAuFfpgAgNhMQXD2VaXvDm9Rk6vhxUfbc52K7U,198
 tests/server/fixtures/complex_output.py,sha256=IY3KfpdtAwMi2K9At-65RXW4CYRAn8xmXD0_YDqM9W0,232
 tests/server/fixtures/count_up.py,sha256=y8JEmFEKnTDm64Qj1w5mtFRZ4gumkINSfHCU7qpw_GQ,131
 tests/server/fixtures/exc_in_predict.py,sha256=uKNB7i0tvwUvfIxzH8oD8RM9kBlxEFF0B2mLWSlWlIc,136
 tests/server/fixtures/exc_in_setup.py,sha256=ieQMqxgCNUmLTXLODhq5ANDBiDNDZ6FqS-egbmI6ZlU,133
 tests/server/fixtures/exc_in_setup_and_predict.py,sha256=Nx05ViOQj1LFGgeVcxehWJXUv_umVsWHZhBvO8iDfME,151
@@ -94,12 +97,12 @@
 tests/server/fixtures/slow_setup.py,sha256=vHIq6spLzpo-bLmgXlyazLWljQz53JamJDHcpTl_XJo,122
 tests/server/fixtures/steps.py,sha256=WbD27CUVQE8Zj_SVOtOqtleG3Y8meSJVAn-vkhpKst8,290
 tests/server/fixtures/train.py,sha256=5LmmIK9Cd7uSJIIjl-6zZkz4BRNbXCpMW5iBYRXLhKU,359
 tests/server/fixtures/yield_concatenate_iterator.py,sha256=2X582IGdiprIALwIs5e-EZO4i1eBUdM7CI4FCPf-CAo,263
 tests/server/fixtures/yield_files.py,sha256=QpIl1SOFsaakNZJlShl_XkjBGyB_MyuQgv5-J2Vm75U,506
 tests/server/fixtures/yield_strings.py,sha256=7Y9cTGZ7WE0iKlr-ZQmhkeg30mXt-fEpY9U0AQ0QMAQ,245
 tests/server/fixtures/yield_strings_file_input.py,sha256=rNxZHFXLhzqkNiG35JfcyihSA4Lx6s3bp86YRGPztX8,339
-cog-0.9.5.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
-cog-0.9.5.dist-info/METADATA,sha256=bNX8zwvzO3ui8L6SRev9gwM4U9YzYIXKFsM-1O2FlWk,36704
-cog-0.9.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cog-0.9.5.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
-cog-0.9.5.dist-info/RECORD,,
+cog-0.9.6.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
+cog-0.9.6.dist-info/METADATA,sha256=m4brIMf2CDYtMAqI68h4UTDeE-n5Nrw8e8Zxkapx1Cw,36704
+cog-0.9.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cog-0.9.6.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
+cog-0.9.6.dist-info/RECORD,,
```

