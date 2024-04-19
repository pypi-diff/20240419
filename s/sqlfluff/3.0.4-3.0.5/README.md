# Comparing `tmp/sqlfluff-3.0.4.tar.gz` & `tmp/sqlfluff-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlfluff-3.0.4.tar", last modified: Tue Apr  9 17:45:05 2024, max compression
+gzip compressed data, was "sqlfluff-3.0.5.tar", last modified: Fri Apr 19 13:48:27 2024, max compression
```

## Comparing `sqlfluff-3.0.4.tar` & `sqlfluff-3.0.5.tar`

### file list

```diff
@@ -1,273 +1,273 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)   499100 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 17:45:05.006647 sqlfluff-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.946646 sqlfluff-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.954646 sqlfluff-3.0.4/src/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.954646 sqlfluff-3.0.4/src/sqlfluff/api/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/api/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    49340 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/cli/outputstream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12430 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/default_config.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.958646 sqlfluff-3.0.4/src/sqlfluff/core/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/dialects/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.962646 sqlfluff-3.0.4/src/sqlfluff/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/helpers/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.962646 sqlfluff-3.0.4/src/sqlfluff/core/linter/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    45903 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/linting_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/linter/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11701 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/anyof.py
--rw-r--r--   0 runner    (1001) docker     (127)    19765 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/delimited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/noncode.py
--rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/markers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/match_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/match_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/matchable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10822 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.966646 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48833 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/bracketed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/keyword.py
--rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7807 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/parser/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/plugin/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/config_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/crawlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/doc_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/rules/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.970646 sqlfluff-3.0.4/src/sqlfluff/core/templaters/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)    46392 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.974646 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/core/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.982646 sqlfluff-3.0.4/src/sqlfluff/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   138386 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    22627 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    70760 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    35114 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    13869 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_duckdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    93118 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    32792 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    82206 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    28325 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)   191205 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    72987 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   240222 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_soql.py
--rw-r--r--   0 runner    (1001) docker     (127)   104915 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    18793 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    27893 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_teradata.py
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)   189301 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)    65703 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica.py
--rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica_keywords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/diff_quality_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.982646 sqlfluff-3.0.4/src/sqlfluff/rules/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.986646 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL05.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL06.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL07.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.986646 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM01.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM02.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM03.py
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM05.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM06.py
--rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM07.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP02.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP04.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP05.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/convention/
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV01.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV02.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV03.py
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV04.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV05.py
--rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV07.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV08.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV09.py
--rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV10.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV11.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/convention/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.990646 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/
--rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/JJ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/jinja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.994646 sqlfluff-3.0.4/src/sqlfluff/rules/layout/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT02.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT04.py
--rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT05.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT06.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT07.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT08.py
--rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT09.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT10.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT11.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT12.py
--rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/layout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.994646 sqlfluff-3.0.4/src/sqlfluff/rules/references/
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF01.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF02.py
--rw-r--r--   0 runner    (1001) docker     (127)    11300 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF03.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF04.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF05.py
--rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/RF06.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/references/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/rules/structure/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST01.py
--rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST02.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST03.py
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST04.py
--rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST05.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST06.py
--rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST07.py
--rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST08.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST09.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/TQ01.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/rules/tsql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:04.998647 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9101 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/analysis/select.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/segment_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/segments.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slices.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/identifers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/depthmap.py
--rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/rebreak.py
--rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/reindent.py
--rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/respace.py
--rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/reflow/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff/utils/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-09 17:44:54.000000 sqlfluff-3.0.4/src/sqlfluff/utils/testing/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/src/sqlfluff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-09 17:45:04.000000 sqlfluff-3.0.4/src/sqlfluff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 17:45:05.002647 sqlfluff-3.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-09 17:44:55.000000 sqlfluff-3.0.4/test/testing_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.644667 sqlfluff-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)   501370 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 13:48:27.644667 sqlfluff-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.584667 sqlfluff-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.592667 sqlfluff-3.0.5/src/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/api/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49340 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/cli/outputstream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12491 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/default_config.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.596667 sqlfluff-3.0.5/src/sqlfluff/core/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/dialects/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12243 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.600667 sqlfluff-3.0.5/src/sqlfluff/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/helpers/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.600667 sqlfluff-3.0.5/src/sqlfluff/core/linter/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9654 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45903 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/linting_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/linter/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13372 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/anyof.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19771 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/delimited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/noncode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36118 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9730 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/markers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28332 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/match_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/match_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/matchable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11439 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.604667 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49362 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/bracketed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/parser/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/plugin/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48881 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/config_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/crawlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/doc_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/rules/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.608667 sqlfluff-3.0.5/src/sqlfluff/core/templaters/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8716 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46392 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.612667 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35992 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/core/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.620667 sqlfluff-3.0.5/src/sqlfluff/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139271 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22826 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73562 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36216 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14195 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6658 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18370 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_duckdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    93480 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19408 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33399 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29892 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82604 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7584 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)   191523 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37092 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73019 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9669 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   242562 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_soql.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105180 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20606 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_teradata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11953 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   189871 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12681 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66185 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6277 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/diff_quality_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.620667 sqlfluff-3.0.5/src/sqlfluff/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11267 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL06.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10982 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4416 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.624667 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP05.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.628667 sqlfluff-3.0.5/src/sqlfluff/rules/convention/
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV05.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14963 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11947 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV10.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/convention/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.628667 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/
+-rw-r--r--   0 runner    (1001) docker     (127)     7886 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/JJ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/jinja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.632667 sqlfluff-3.0.5/src/sqlfluff/rules/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6092 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16989 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT11.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/layout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.632667 sqlfluff-3.0.5/src/sqlfluff/rules/references/
+-rw-r--r--   0 runner    (1001) docker     (127)     9008 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF02.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8506 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/RF06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/references/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/rules/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9445 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST02.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST04.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20587 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST06.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7002 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST07.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5171 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST08.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST09.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/TQ01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/rules/tsql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/analysis/select.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.636667 sqlfluff-3.0.5/src/sqlfluff/utils/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/segment_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/identifers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7051 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/depthmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32545 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23067 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/rebreak.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94663 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/reindent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/respace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25529 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/reflow/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff/utils/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/src/sqlfluff/utils/testing/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/src/sqlfluff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 13:48:27.000000 sqlfluff-3.0.5/src/sqlfluff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:48:27.640667 sqlfluff-3.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-19 13:48:18.000000 sqlfluff-3.0.5/test/testing_test.py
```

### Comparing `sqlfluff-3.0.4/CHANGELOG.md` & `sqlfluff-3.0.5/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,43 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!--
 Note: Changes are now automatically tracked in [GitHub](https://github.com/sqlfluff/sqlfluff/releases) and will be copied in here on each release (please remember to update the issues and contributors to links!). There is no need to manually edit this file going forward.
 -->
 <!--Start Of Releases (DO NOT DELETE THIS LINE)-->
 
+## [3.0.5] - 2024-04-19
+
+## Highlights
+
+This release contains one larger change, which is a big upgrade to case sensitivity in
+the alias use rules. Also allowing the customisation of how SQLFluff uses case sensitivity
+in rules like AL05. Beyond that, this also includes a handful of dialect improvements.
+
+Thanks especially to [@olshak](https://github.com/olshak), [@MarkPaulin](https://github.com/MarkPaulin),
+[@mhoogendoorn](https://github.com/mhoogendoorn) & [@kawashiro](https://github.com/kawashiro)
+who made their first contributions in this release! 🚀
+
+## What’s Changed
+
+* BigQuery: Support CREATE SNAPSHOT TABLE statement [#5779](https://github.com/sqlfluff/sqlfluff/pull/5779) [@kzosabe](https://github.com/kzosabe)
+* Upgrades to release actions. [#5774](https://github.com/sqlfluff/sqlfluff/pull/5774) [@alanmcruickshank](https://github.com/alanmcruickshank)
+* Improve Snowflake syntax support [#5770](https://github.com/sqlfluff/sqlfluff/pull/5770) [@kawashiro](https://github.com/kawashiro)
+* TSQL: allow 'OR ALTER' on 'CREATE TRIGGER' [#5772](https://github.com/sqlfluff/sqlfluff/pull/5772) [@mhoogendoorn](https://github.com/mhoogendoorn)
+* Enhancement: Improved Identifiers - casefolding, quoted values, and basic escaping [#5726](https://github.com/sqlfluff/sqlfluff/pull/5726) [@keraion](https://github.com/keraion)
+* TSQL: Fix bare functions in default constraints [#5771](https://github.com/sqlfluff/sqlfluff/pull/5771) [@MarkPaulin](https://github.com/MarkPaulin)
+* MySQL: Fix parsing 'ALTER TABLE ts ADD COLUMN modified_at TIMESTAMP NULL DEFAULT NULL ON UPDATE CURRENT_TIMESTAMP;' (#5766) [#5767](https://github.com/sqlfluff/sqlfluff/pull/5767) [@olshak](https://github.com/olshak)
+
+
+## New Contributors
+* [@olshak](https://github.com/olshak) made their first contribution in [#5767](https://github.com/sqlfluff/sqlfluff/pull/5767)
+* [@MarkPaulin](https://github.com/MarkPaulin) made their first contribution in [#5771](https://github.com/sqlfluff/sqlfluff/pull/5771)
+* [@mhoogendoorn](https://github.com/mhoogendoorn) made their first contribution in [#5772](https://github.com/sqlfluff/sqlfluff/pull/5772)
+* [@kawashiro](https://github.com/kawashiro) made their first contribution in [#5770](https://github.com/sqlfluff/sqlfluff/pull/5770)
+
 ## [3.0.4] - 2024-04-07
 
 ## Highlights
 
 This is a standard bugfix release bringing a bunch of dialect improvements and
 bugfixes. Almost every dialect sees some improvements and it also includes
 quality of life improvements to the CLI, pre-commit hooks, docs and several
```

### Comparing `sqlfluff-3.0.4/LICENSE.md` & `sqlfluff-3.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/PKG-INFO` & `sqlfluff-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.4
+Version: 3.0.5
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff-3.0.4/README.md` & `sqlfluff-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/pyproject.toml` & `sqlfluff-3.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sqlfluff"
-version = "3.0.4"
+version = "3.0.5"
 description = "The SQL Linter for Humans"
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.8"
 authors = [
   {name = "Alan Cruickshank", email = "alan@designingoverload.com"},
 ]
 license = {file = "LICENSE.md"}
@@ -125,15 +125,15 @@
 sqlfluff_rules_convention = "sqlfluff.rules.convention"
 sqlfluff_rules_jinja = "sqlfluff.rules.jinja"
 sqlfluff_rules_tsql = "sqlfluff.rules.tsql"
 
 
 [tool.sqlfluff_docs]
 # NOTE: Stable version is used by docs/conf.py
-stable_version = "3.0.4"
+stable_version = "3.0.5"
 
 
 [tool.setuptools.package-data]
 sqlfluff = ["core/default_config.cfg", "py.typed"]
 
 
 [tool.importlinter]
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/api/simple.py` & `sqlfluff-3.0.5/src/sqlfluff/api/simple.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/cli/autocomplete.py` & `sqlfluff-3.0.5/src/sqlfluff/cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/cli/commands.py` & `sqlfluff-3.0.5/src/sqlfluff/cli/commands.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/cli/formatters.py` & `sqlfluff-3.0.5/src/sqlfluff/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/cli/helpers.py` & `sqlfluff-3.0.5/src/sqlfluff/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/cli/outputstream.py` & `sqlfluff-3.0.5/src/sqlfluff/cli/outputstream.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/config.py` & `sqlfluff-3.0.5/src/sqlfluff/core/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/default_config.cfg` & `sqlfluff-3.0.5/src/sqlfluff/core/default_config.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,17 @@
 # Aliasing preference for tables
 aliasing = explicit
 
 [sqlfluff:rules:aliasing.column]
 # Aliasing preference for columns
 aliasing = explicit
 
+[sqlfluff:rules:aliasing.unused]
+alias_case_check = dialect
+
 [sqlfluff:rules:aliasing.length]
 min_alias_length = None
 max_alias_length = None
 
 [sqlfluff:rules:aliasing.forbid]
 # Avoid table aliases in from clauses and join conditions.
 # Disabled by default for all dialects unless explicitly enabled.
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/dialects/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/dialects/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/dialects/base.py` & `sqlfluff-3.0.5/src/sqlfluff/core/dialects/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/dialects/common.py` & `sqlfluff-3.0.5/src/sqlfluff/core/dialects/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/enums.py` & `sqlfluff-3.0.5/src/sqlfluff/core/enums.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/errors.py` & `sqlfluff-3.0.5/src/sqlfluff/core/errors.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/helpers/dict.py` & `sqlfluff-3.0.5/src/sqlfluff/core/helpers/dict.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/helpers/file.py` & `sqlfluff-3.0.5/src/sqlfluff/core/helpers/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/helpers/slice.py` & `sqlfluff-3.0.5/src/sqlfluff/core/helpers/slice.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/helpers/string.py` & `sqlfluff-3.0.5/src/sqlfluff/core/helpers/string.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/common.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/fix.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_dir.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_dir.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/linted_file.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/linted_file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/linter.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/linter.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/linting_result.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/linting_result.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/patch.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/patch.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/linter/runner.py` & `sqlfluff-3.0.5/src/sqlfluff/core/linter/runner.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/context.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/anyof.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/anyof.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,20 @@
         matched = MatchResult.empty_at(idx)
         max_idx = len(segments)  # What is the limit
 
         if self.parse_mode == ParseMode.GREEDY:
             max_idx = trim_to_terminator(
                 segments,
                 idx,
-                terminators=[*self.terminators, *parse_context.terminators],
+                terminators=(
+                    # Only pass through the context terminators if not resetting.
+                    self.terminators
+                    if self.reset_terminators
+                    else [*self.terminators, *parse_context.terminators]
+                ),
                 parse_context=parse_context,
             )
 
         while True:
             if n_matches >= self.min_times:
                 if (
                     # Either nothing left to match...
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/base.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             for k in self.equality_kwargs
         )
 
     def copy(
         self: T,
         insert: Optional[List[Matchable]] = None,
         at: Optional[int] = None,
-        before: Optional[Any] = None,
+        before: Optional[Matchable] = None,
         remove: Optional[List[Matchable]] = None,
         terminators: List[Union[str, Matchable]] = [],
         replace_terminators: bool = False,
         # NOTE: Optionally allow other kwargs to be provided to this
         # method for type compatibility. Any provided won't be used.
         **kwargs: Any,
     ) -> T:
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/conditional.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/conditional.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/delimited.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/delimited.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/noncode.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/noncode.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/grammar/sequence.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/grammar/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/helpers.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/lexer.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/markers.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/markers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/match_algorithms.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/match_algorithms.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/match_result.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/match_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,21 @@
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     Union,
-    cast,
 )
 
 from sqlfluff.core.helpers.slice import slice_length
 from sqlfluff.core.parser.markers import PositionMarker
 
 if TYPE_CHECKING:  # pragma: no cover
-    from sqlfluff.core.parser.segments import BaseSegment, MetaSegment, RawSegment
+    from sqlfluff.core.parser.segments import BaseSegment, MetaSegment
 
 
 def _get_point_pos_at_idx(
     segments: Sequence["BaseSegment"], idx: int
 ) -> PositionMarker:
     if idx < len(segments):
         _next_pos = segments[idx].pos_marker
@@ -283,23 +282,11 @@
         if max_idx < self.matched_slice.stop:
             result_segments += segments[max_idx : self.matched_slice.stop]
 
         if not self.matched_class:
             return result_segments
 
         # Otherwise construct the subsegment
-        new_seg: "BaseSegment"
-        if self.matched_class.class_is_type("raw"):
-            _raw_type = cast(Type["RawSegment"], self.matched_class)
-            assert len(result_segments) == 1
-            # TODO: Should this be a generic method on BaseSegment and RawSegment?
-            # It feels a little strange to be this specific here.
-            new_seg = _raw_type(
-                raw=result_segments[0].raw,
-                pos_marker=result_segments[0].pos_marker,
-                **self.segment_kwargs,
-            )
-        else:
-            new_seg = self.matched_class(
-                segments=result_segments, **self.segment_kwargs
-            )
+        new_seg: "BaseSegment" = self.matched_class.from_result_segments(
+            result_segments, self.segment_kwargs
+        )
         return (new_seg,)
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/matchable.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/matchable.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/parser.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/parser.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/parsers.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/parsers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Individual segment parsers.
 
 Matchable objects which return individual segments.
 """
 
 from abc import abstractmethod
-from typing import Any, Collection, Dict, Optional, Sequence, Tuple, Type
+from typing import Any, Callable, Collection, Dict, Optional, Sequence, Tuple, Type
 from uuid import uuid4
 
 import regex
 
 from sqlfluff.core.parser.context import ParseContext
 from sqlfluff.core.parser.match_result import MatchResult
 from sqlfluff.core.parser.matchable import Matchable
@@ -27,22 +27,24 @@
     def __init__(
         self,
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         # The following kwargs are passed on to the segment:
         trim_chars: Optional[Tuple[str, ...]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ) -> None:
         self.raw_class = raw_class
         # Store instance_types rather than just type to allow
         # for multiple possible types to be supported in derivative
         # classes.
         self._instance_types: Tuple[str, ...] = (type or raw_class.type,)
         self.optional = optional
         self._trim_chars = trim_chars
+        self._casefold = casefold
         # Generate a cache key
         self._cache_key = uuid4().hex
 
     def cache_key(self) -> str:
         """Get the cache key for this parser.
 
         For parsers, they're unique per-instance.
@@ -59,14 +61,16 @@
         This is a helper function for reuse by other parsers.
         """
         segment_kwargs: Dict[str, Any] = {}
         if self._instance_types:
             segment_kwargs["instance_types"] = self._instance_types
         if self._trim_chars:
             segment_kwargs["trim_chars"] = self._trim_chars
+        if self._casefold:
+            segment_kwargs["casefold"] = self._casefold
         return MatchResult(
             matched_slice=slice(idx, idx + 1),
             matched_class=self.raw_class,
             segment_kwargs=segment_kwargs,
         )
 
 
@@ -76,36 +80,39 @@
     def __init__(
         self,
         template: str,
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         trim_chars: Optional[Tuple[str, ...]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ) -> None:
         """Initialize a new instance of the class.
 
         Args:
             template (str): The template type.
             raw_class (Type[RawSegment]): The raw segment class.
             type (Optional[str]): The type of the instance.
             optional (bool): Whether the instance is optional.
             trim_chars (Optional[Tuple[str, ...]]): The characters to trim.
+            casefold: (Optional[Callable[[str],str]]): The default casing used.
 
         Returns:
             None
         """
         # NB: the template in this case is the _target_ type.
         # The type kwarg is the eventual type.
         self.template = template
         # Pre-calculate the appropriate frozenset for matching later.
         self._target_types = frozenset((template,))
         super().__init__(
             raw_class=raw_class,
             optional=optional,
             trim_chars=trim_chars,
+            casefold=casefold,
         )
         # NOTE: We override the instance types after initialising the base
         # class. We want to ensure that re-matching is possible by ensuring that
         # the `type` pre-matching is still present post-match even if it's not
         # part of the natural type hierarchy for the new `raw_class`.
         # The new `type` becomes the "primary" type, but the template will still
         # be part of the resulting `class_types`.
@@ -163,23 +170,25 @@
     def __init__(
         self,
         template: str,
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         trim_chars: Optional[Tuple[str, ...]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ):
         self.template = template.upper()
         # Create list version upfront to avoid recreating it multiple times.
         self._simple = frozenset((self.template,))
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             trim_chars=trim_chars,
+            casefold=casefold,
         )
 
     def __repr__(self) -> str:
         return f"<StringParser: {self.template!r}>"
 
     def simple(
         self, parse_context: "ParseContext", crumbs: Optional[Tuple[str, ...]] = None
@@ -213,23 +222,25 @@
     def __init__(
         self,
         templates: Collection[str],
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         trim_chars: Optional[Tuple[str, ...]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ):
         self.templates = {template.upper() for template in templates}
         # Create list version upfront to avoid recreating it multiple times.
         self._simple = frozenset(self.templates)
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             trim_chars=trim_chars,
+            casefold=casefold,
         )
 
     def __repr__(self) -> str:
         return f"<MultiStringParser: {self.templates!r}>"
 
     def simple(
         self, parse_context: "ParseContext", crumbs: Optional[Tuple[str, ...]] = None
@@ -264,33 +275,35 @@
         self,
         template: str,
         raw_class: Type[RawSegment],
         type: Optional[str] = None,
         optional: bool = False,
         anti_template: Optional[str] = None,
         trim_chars: Optional[Tuple[str, ...]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ):
         # Store the optional anti-template
         self.template = template
         self.anti_template = anti_template
         # Compile regexes upfront to avoid repeated overhead
         self._anti_template = regex.compile(anti_template or r"", regex.IGNORECASE)
         self._template = regex.compile(template, regex.IGNORECASE)
         super().__init__(
             raw_class=raw_class,
             type=type,
             optional=optional,
             trim_chars=trim_chars,
+            casefold=casefold,
         )
 
     def __repr__(self) -> str:
         return f"<RegexParser: {self.template!r}>"
 
     def simple(
-        cls, parse_context: ParseContext, crumbs: Optional[Tuple[str, ...]] = None
+        self, parse_context: ParseContext, crumbs: Optional[Tuple[str, ...]] = None
     ) -> None:
         """Does this matcher support a uppercase hash matching route?
 
         Regex segment does NOT for now. We might need to later for efficiency.
         """
         return None
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/base.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,14 +926,18 @@
         """
         return self.structural_simplify(self.to_tuple(**kwargs))
 
     def get_raw_segments(self) -> List["RawSegment"]:
         """Iterate raw segments, mostly for searching."""
         return [item for s in self.segments for item in s.raw_segments]
 
+    def raw_normalized(self, casefold: bool = True) -> str:
+        """Iterate raw segments, return normalized value."""
+        return "".join(seg.raw_normalized(casefold) for seg in self.get_raw_segments())
+
     def iter_segments(
         self, expanding: Optional[Sequence[str]] = None, pass_through: bool = False
     ) -> Iterator["BaseSegment"]:
         """Iterate segments, optionally expanding some children."""
         for s in self.segments:
             if expanding and s.is_type(*expanding):
                 yield from s.iter_segments(
@@ -1225,14 +1229,23 @@
 
     def edit(
         self, raw: Optional[str] = None, source_fixes: Optional[List[SourceFix]] = None
     ) -> BaseSegment:
         """Stub."""
         raise NotImplementedError()
 
+    @classmethod
+    def from_result_segments(
+        cls,
+        result_segments: Tuple[BaseSegment, ...],
+        segment_kwargs: Dict[str, Any],
+    ) -> "BaseSegment":
+        """Create an instance of this class from a tuple of matched segments."""
+        return cls(segments=result_segments, **segment_kwargs)
+
 
 class UnparsableSegment(BaseSegment):
     """This is a segment which can't be parsed. It indicates a error during parsing."""
 
     type = "unparsable"
     # From here down, comments are printed separately.
     comment_separate = True
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/bracketed.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/bracketed.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/common.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/common.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/file.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/file.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/generator.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/generator.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/keyword.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/keyword.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """The KeywordSegment class."""
 
-from typing import List, Optional, Tuple
+from typing import Callable, List, Optional, Tuple, Union
 
 from sqlfluff.core.parser.markers import PositionMarker
 from sqlfluff.core.parser.segments.base import SourceFix
 from sqlfluff.core.parser.segments.common import WordSegment
 
 
 class KeywordSegment(WordSegment):
@@ -20,21 +20,28 @@
     def __init__(
         self,
         raw: Optional[str] = None,
         pos_marker: Optional[PositionMarker] = None,
         instance_types: Tuple[str, ...] = (),
         source_fixes: Optional[List[SourceFix]] = None,
         trim_chars: Optional[Tuple[str, ...]] = None,
+        quoted_value: Optional[Tuple[str, Union[int, str]]] = None,
+        escape_replacements: Optional[List[Tuple[str, str]]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ):
         """If no other name is provided we extrapolate it from the raw."""
         super().__init__(
             raw=raw,
             pos_marker=pos_marker,
             instance_types=instance_types,
             source_fixes=source_fixes,
+            trim_chars=trim_chars,
+            quoted_value=quoted_value,
+            escape_replacements=escape_replacements,
+            casefold=casefold,
         )
 
     def edit(
         self, raw: Optional[str] = None, source_fixes: Optional[List[SourceFix]] = None
     ) -> "KeywordSegment":
         """Create a new segment, with exactly the same position but different content.
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/meta.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/meta.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/segments/raw.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/segments/raw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Raw segment definitions.
 
 This is designed to be the root segment, without
 any children, and the output of the lexer.
 """
 
-from typing import Any, FrozenSet, List, Optional, Tuple
+from typing import Any, Callable, Dict, FrozenSet, List, Optional, Tuple, Union, cast
 from uuid import uuid4
 
+import regex as re
+
 from sqlfluff.core.parser.markers import PositionMarker
 from sqlfluff.core.parser.segments.base import BaseSegment, SourceFix
 
 
 class RawSegment(BaseSegment):
     """This is a segment without any subsegments."""
 
@@ -31,14 +33,17 @@
         # we suggest using the `instance_types` option.
         type: Optional[str] = None,
         instance_types: Tuple[str, ...] = (),
         trim_start: Optional[Tuple[str, ...]] = None,
         trim_chars: Optional[Tuple[str, ...]] = None,
         source_fixes: Optional[List[SourceFix]] = None,
         uuid: Optional[int] = None,
+        quoted_value: Optional[Tuple[str, Union[int, str]]] = None,
+        escape_replacements: Optional[List[Tuple[str, str]]] = None,
+        casefold: Optional[Callable[[str], str]] = None,
     ):
         """Initialise raw segment.
 
         If raw is not provided, we default to _default_raw if present.
         If pos_marker is not provided, it is assume that this will be
         inserted later as part of a reposition phase.
         """
@@ -65,14 +70,18 @@
         # Keep track of any source fixes
         self._source_fixes = source_fixes
         # UUID for matching (the int attribute of it)
         self.uuid = uuid or uuid4().int
         self.representation = "<{}: ({}) {!r}>".format(
             self.__class__.__name__, self.pos_marker, self.raw
         )
+        self.quoted_value = quoted_value
+        self.escape_replacements = escape_replacements
+        self.casefold = casefold
+        self._raw_value: str = self._raw_normalized()
 
     def __repr__(self) -> str:
         # This is calculated at __init__, because all elements are immutable
         # and this was previously recalculating the pos marker,
         # and became very expensive
         return self.representation
 
@@ -167,14 +176,48 @@
                     raw_buff = raw_buff[len(seq) :]
                 # trim end
                 while raw_buff.endswith(seq):
                     raw_buff = raw_buff[: -len(seq)]
             return raw_buff
         return raw_buff
 
+    def _raw_normalized(self) -> str:
+        """Returns the string of the raw content's value.
+
+        E.g. This removes leading and trailing quote characters, removes escapes
+
+        Return:
+        str: The raw content's value
+        """
+        raw_buff = self.raw
+        if self.quoted_value:
+            _match = re.match(self.quoted_value[0], raw_buff)
+            if _match:
+                _group_match = _match.group(self.quoted_value[1])
+                if isinstance(_group_match, str):
+                    raw_buff = _group_match
+        if self.escape_replacements:
+            for old, new in self.escape_replacements:
+                raw_buff = re.sub(old, new, raw_buff)
+        return raw_buff
+
+    def raw_normalized(self, casefold: bool = True) -> str:
+        """Returns a normalized string of the raw content.
+
+        E.g. This removes leading and trailing quote characters, removes escapes,
+        optionally casefolds to the dialect's casing
+
+        Return:
+        str: The normalized version of the raw content
+        """
+        raw_buff = self._raw_value
+        if self.casefold and casefold:
+            raw_buff = self.casefold(raw_buff)
+        return raw_buff
+
     def stringify(
         self, ident: int = 0, tabsize: int = 4, code_only: bool = False
     ) -> str:
         """Use indentation to render this segment and its children as a string.
 
         Args:
             ident (int, optional): The indentation level. Defaults to 0.
@@ -219,16 +262,45 @@
         """
         return self.__class__(
             raw=raw or self.raw,
             pos_marker=self.pos_marker,
             instance_types=self.instance_types,
             trim_start=self.trim_start,
             trim_chars=self.trim_chars,
+            quoted_value=self.quoted_value,
+            escape_replacements=self.escape_replacements,
+            casefold=self.casefold,
             source_fixes=source_fixes or self.source_fixes,
         )
 
+    def _get_raw_segment_kwargs(self) -> Dict[str, Any]:
+        return {
+            "quoted_value": self.quoted_value,
+            "escape_replacements": self.escape_replacements,
+            "casefold": self.casefold,
+        }
+
+    # ################ CLASS METHODS
+
+    @classmethod
+    def from_result_segments(
+        cls,
+        result_segments: Tuple[BaseSegment, ...],
+        segment_kwargs: Dict[str, Any],
+    ) -> "RawSegment":
+        """Create a RawSegment from result segments."""
+        assert len(result_segments) == 1
+        raw_seg = cast("RawSegment", result_segments[0])
+        new_segment_kwargs = raw_seg._get_raw_segment_kwargs()
+        new_segment_kwargs.update(segment_kwargs)
+        return cls(
+            raw=raw_seg.raw,
+            pos_marker=raw_seg.pos_marker,
+            **new_segment_kwargs,
+        )
+
 
 __all__ = [
     "PositionMarker",
     "RawSegment",
     "SourceFix",
 ]
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/parser/types.py` & `sqlfluff-3.0.5/src/sqlfluff/core/parser/types.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/plugin/hookspecs.py` & `sqlfluff-3.0.5/src/sqlfluff/core/plugin/hookspecs.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/plugin/host.py` & `sqlfluff-3.0.5/src/sqlfluff/core/plugin/host.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/plugin/lib.py` & `sqlfluff-3.0.5/src/sqlfluff/core/plugin/lib.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/base.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/config_info.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/config_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -191,14 +191,24 @@
         "validation": ["consistent", "single_quotes", "double_quotes"],
         "definition": (
             "Preferred quoting style to use for the quoted literals. If set to "
             "``consistent`` quoting style is derived from the first quoted literal"
             "in the file."
         ),
     },
+    "alias_case_check": {
+        "validation": [
+            "dialect",
+            "case_insensitive",
+            "quoted_cs_naked_upper",
+            "quoted_cs_naked_lower",
+            "case_sensitive",
+        ],
+        "definition": "How to handle comparison casefolding in an alias.",
+    },
     "min_alias_length": {
         "validation": range(1000),
         "definition": (
             "The minimum length of an alias to allow without raising a violation."
         ),
     },
     "max_alias_length": {
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/context.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/crawlers.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/crawlers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/doc_decorators.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/doc_decorators.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/fix.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/fix.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/loader.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/loader.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/noqa.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/noqa.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/rules/reference.py` & `sqlfluff-3.0.5/src/sqlfluff/core/rules/reference.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/base.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/base.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/jinja.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/jinja.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/placeholder.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/placeholder.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/python.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/python.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/templaters/slicers/tracer.py` & `sqlfluff-3.0.5/src/sqlfluff/core/templaters/slicers/tracer.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/core/timing.py` & `sqlfluff-3.0.5/src/sqlfluff/core/timing.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,19 +89,50 @@
             ),
             trim_post_subdivide=RegexLexer(
                 "whitespace",
                 r"[^\S\r\n]+",
                 WhitespaceSegment,
             ),
         ),
-        RegexLexer("single_quote", r"'([^'\\]|\\.|'')*'", CodeSegment),
-        RegexLexer("double_quote", r'"([^"\\]|\\.)*"', CodeSegment),
-        RegexLexer("back_quote", r"`[^`]*`", CodeSegment),
+        RegexLexer(
+            "single_quote",
+            r"'([^'\\]|\\.|'')*'",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^'\\]|\\.|'')*)'", 1),
+                "escape_replacements": [(r"\\'|''", "'")],
+            },
+        ),
+        RegexLexer(
+            "double_quote",
+            r'"([^"\\]|\\.)*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"\\]|\\.)*)"', 1),
+                "escape_replacements": [(r'\\"|""', '"')],
+            },
+        ),
+        RegexLexer(
+            "back_quote",
+            r"`(?:[^`\\]|\\.)*`",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"`((?:[^`\\]|\\.)*)`", 1),
+                "escape_replacements": [(r"\\`", "`")],
+            },
+        ),
         # See https://www.geeksforgeeks.org/postgresql-dollar-quoted-string-constants/
-        RegexLexer("dollar_quote", r"\$(\w*)\$[^\1]*?\$\1\$", CodeSegment),
+        RegexLexer(
+            "dollar_quote",
+            r"\$(\w*)\$(.*?)\$\1\$",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"\$(\w*)\$(.*?)\$\1\$", 2),
+            },
+        ),
         # Numeric literal matches integers, decimals, and exponential formats,
         # Pattern breakdown:
         # (?>                      Atomic grouping
         #                          (https://www.regular-expressions.info/atomic.html).
         #     \d+\.\d+             e.g. 123.456
         #     |\d+\.(?![\.\w])     e.g. 123.
         #                          (N.B. negative lookahead assertion to ensure we
@@ -268,14 +299,15 @@
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             r"[A-Z0-9_]*[A-Z][A-Z0-9_]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.upper,
         )
     ),
     ParameterNameSegment=RegexParser(
         r"\"?[A-Z][A-Z0-9_]*\"?", CodeSegment, type="parameter"
     ),
     FunctionNameIdentifierSegment=TypedParser(
         "word", WordSegment, type="function_name_identifier"
@@ -1549,14 +1581,15 @@
 
         # Handle any aliases
         alias_expression = self.get_child("alias_expression")
         if alias_expression:
             # If it has an alias, return that
             segment = alias_expression.get_child("identifier")
             if segment:
+                segment = cast(IdentifierSegment, segment)
                 return AliasInfo(
                     segment.raw, segment, True, self, alias_expression, ref
                 )
 
         # If not return the object name (or None if there isn't one)
         if ref:
             references: List = list(ref.iter_raw_references())
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_ansi_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_ansi_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,17 @@
                     ),
                 )
             )
         ),
     ),
     BackQuotedIdentifierSegment=TypedParser(
         "back_quote",
-        LiteralSegment,
+        IdentifierSegment,
         type="quoted_identifier",
+        casefold=str.lower,
     ),
     DatetimeWithTZSegment=Sequence(OneOf("TIMESTAMP", "TIME"), "WITH", "TIME", "ZONE"),
 )
 
 athena_dialect.replace(
     LiteralGrammar=ansi_dialect.get_grammar("LiteralGrammar").copy(
         insert=[
@@ -227,16 +228,20 @@
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             r"[A-Z0-9_]*[A-Z_][A-Z0-9_]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.lower,
         )
     ),
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.lower
+    ),
     SingleIdentifierGrammar=ansi_dialect.get_grammar("SingleIdentifierGrammar").copy(
         insert=[
             Ref("BackQuotedIdentifierSegment"),
         ]
     ),
     BinaryOperatorGrammar=OneOf(
         Ref("ArithmeticBinaryOperatorGrammar"),
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_athena_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_athena_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,21 +75,41 @@
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#string_and_bytes_literals
         # Triple quoted variant first, then single quoted
         RegexLexer(
             "single_quote",
             r"([rR]?[bB]?|[bB]?[rR]?)?('''((?<!\\)(\\{2})*\\'|'{,2}(?!')|[^'])"
             r"*(?<!\\)(\\{2})*'''|'((?<!\\)(\\{2})*\\'|[^'])*(?<!\\)(\\{2})*')",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (
+                    r"(?:[rR]?[bB]?|[bB]?[rR]?)?"
+                    r"(?:'''(?<value>(?:(?<!\\)(?:\\{2})*\\'|'{,2}(?!')|[^'])*"
+                    r"(?<!\\)(?:\\{2})*)'''|'(?<value>(?:(?<!\\)(?:\\{2})*\\'"
+                    r"|[^'])*(?<!\\)(?:\\{2})*)')",
+                    "value",
+                ),
+                "escape_replacements": [(r"\\([\\`\"'?])", "\1")],
+            },
         ),
         RegexLexer(
             "double_quote",
             r"([rR]?[bB]?|[bB]?[rR]?)?(\"\"\"((?<!\\)(\\{2})*\\\"|\"{,2}(?!\")"
             r'|[^\"])*(?<!\\)(\\{2})*\"\"\"|"((?<!\\)(\\{2})*\\"|[^"])*(?<!\\)'
             r'(\\{2})*")',
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (
+                    r"([rR]?[bB]?|[bB]?[rR]?)?"
+                    r"(\"\"\"(?<value>((?<!\\)(\\{2})*\\\"|\"{,2}(?!\")"
+                    r'|[^\"])*(?<!\\)(\\{2})*)\"\"\"|"(?<value>((?<!\\)'
+                    r'(\\{2})*\\"|[^"])*(?<!\\)(\\{2})*)")',
+                    "value",
+                ),
+                "escape_replacements": [(r"\\([\\`\"'?])", "\1")],
+            },
         ),
     ]
 )
 
 bigquery_dialect.add(
     DoubleQuotedLiteralSegment=TypedParser(
         "double_quote",
@@ -145,14 +165,41 @@
     NakedIdentifierPart=RegexParser(
         # The part of a an identifier after a hyphen.
         # NOTE: This one can match an "all numbers" variant.
         # https://cloud.google.com/resource-manager/docs/creating-managing-projects
         r"[A-Z0-9_]+",
         IdentifierSegment,
         type="naked_identifier",
+        casefold=str.upper,
+    ),
+    NakedCSIdentifierPart=RegexParser(
+        # Same as NakedIdentifierPart, but case-sensitive.
+        r"[A-Z0-9_]+",
+        IdentifierSegment,
+        type="naked_identifier",
+    ),
+    NakedCSIdentifierSegment=SegmentGenerator(
+        # Generate the anti template from the set of reserved keywords
+        lambda dialect: RegexParser(
+            r"[A-Z_][A-Z0-9_]*",
+            IdentifierSegment,
+            type="naked_identifier",
+            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+        )
+    ),
+    QuotedCSIdentifierSegment=TypedParser(
+        "back_quote",
+        IdentifierSegment,
+        type="quoted_identifier",
+        trim_chars=("`",),
+    ),
+    SingleCSIdentifierGrammar=OneOf(
+        Ref("NakedCSIdentifierSegment"),
+        Ref("QuotedCSIdentifierSegment"),
+        terminators=[Ref("DotSegment")],
     ),
     SingleIdentifierFullGrammar=OneOf(
         Ref("NakedIdentifierSegment"),
         Ref("QuotedIdentifierSegment"),
         Ref("NakedIdentifierFullSegment"),
     ),
     DefaultDeclareOptionsGrammar=Sequence(
@@ -209,14 +256,15 @@
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             r"[A-Z_][A-Z0-9_]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.upper,
         )
     ),
     FunctionContentsExpressionGrammar=OneOf(
         Ref("DatetimeUnitSegment"),
         Ref("DatePartWeekSegment"),
         Sequence(
             Ref("ExpressionSegment"),
@@ -335,14 +383,30 @@
             Ref("DatatypeSegment"),
             bracket_type="angle",
             bracket_pairs_set="angle_bracket_pairs",
         ),
     )
 
 
+class ForSystemTimeAsOfSegment(BaseSegment):
+    """A `FOR SYSTEM_TIME AS OF` syntax.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/query-syntax#for_system_time_as_of
+    """
+
+    type = "for_system_time_as_of_segment"
+    match_grammar = Sequence(
+        "FOR",
+        OneOf("SYSTEM_TIME", Sequence("SYSTEM", "TIME")),
+        "AS",
+        "OF",
+        Ref("ExpressionSegment"),
+    )
+
+
 class QualifyClauseSegment(BaseSegment):
     """A `QUALIFY` clause like in `SELECT`."""
 
     type = "qualify_clause"
     match_grammar = Sequence(
         "QUALIFY",
         Indent,
@@ -431,14 +495,15 @@
 
     match_grammar = ansi.StatementSegment.match_grammar.copy(
         insert=[
             Ref("DeclareStatementSegment"),
             Ref("SetStatementSegment"),
             Ref("ExportStatementSegment"),
             Ref("CreateExternalTableStatementSegment"),
+            Ref("CreateSnapshotTableStatementSegment"),
             Ref("AssertStatementSegment"),
             Ref("CallStatementSegment"),
             Ref("ReturnStatementSegment"),
             Ref("BreakStatementSegment"),
             Ref("LeaveStatementSegment"),
             Ref("ContinueStatementSegment"),
             Ref("RaiseStatementSegment"),
@@ -714,14 +779,15 @@
 
 bigquery_dialect.replace(
     QuotedIdentifierSegment=TypedParser(
         "back_quote",
         IdentifierSegment,
         type="quoted_identifier",
         trim_chars=("`",),
+        casefold=str.upper,
     ),
     # Add ParameterizedSegment to the ansi NumericLiteralSegment
     NumericLiteralSegment=OneOf(
         TypedParser("numeric_literal", LiteralSegment, type="numeric_literal"),
         Ref("ParameterizedSegment"),
     ),
     QuotedLiteralSegment=OneOf(
@@ -732,22 +798,15 @@
     LiteralGrammar=ansi_dialect.get_grammar("LiteralGrammar").copy(
         insert=[
             Ref("ParameterizedSegment"),
             Ref("SystemVariableSegment"),
         ]
     ),
     PostTableExpressionGrammar=Sequence(
-        Sequence(
-            "FOR",
-            OneOf("SYSTEM_TIME", Sequence("SYSTEM", "TIME")),
-            "AS",
-            "OF",
-            Ref("ExpressionSegment"),
-            optional=True,
-        ),
+        Ref("ForSystemTimeAsOfSegment", optional=True),
         Sequence(
             "WITH",
             "OFFSET",
             Sequence("AS", Ref("SingleIdentifierGrammar"), optional=True),
             optional=True,
         ),
     ),
@@ -1294,19 +1353,19 @@
 class TableReferenceSegment(ansi.ObjectReferenceSegment):
     """A reference to an object that may contain embedded hyphens."""
 
     type = "table_reference"
 
     match_grammar: Matchable = Delimited(
         Sequence(
-            Ref("SingleIdentifierGrammar"),
+            Ref("SingleCSIdentifierGrammar"),
             AnyNumberOf(
                 Sequence(
                     Ref("DashSegment"),
-                    Ref("NakedIdentifierPart"),
+                    Ref("NakedCSIdentifierPart"),
                     allow_gaps=False,
                 ),
                 optional=True,
             ),
             allow_gaps=False,
         ),
         delimiter=Ref("ObjectReferenceDelimiterGrammar"),
@@ -1703,14 +1762,35 @@
                 optional=True,
             ),
             Ref("OptionsSegment", optional=True),
         ),
     )
 
 
+class CreateSnapshotTableStatementSegment(BaseSegment):
+    """A `CREATE SNAPSHOT TABLE` statement.
+
+    https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#create_snapshot_table_statement
+    """
+
+    type = "create_snapshot_table_statement"
+
+    match_grammar = Sequence(
+        "CREATE",
+        "SNAPSHOT",
+        "TABLE",
+        Ref("IfNotExistsGrammar", optional=True),
+        Ref("TableReferenceSegment"),
+        "CLONE",
+        Ref("TableReferenceSegment"),
+        Ref("ForSystemTimeAsOfSegment", optional=True),
+        Ref("OptionsSegment", optional=True),
+    )
+
+
 class CreateViewStatementSegment(ansi.CreateViewStatementSegment):
     """A `CREATE VIEW` statement.
 
     https://cloud.google.com/bigquery/docs/reference/standard-sql/data-definition-language#view_option_list
     """
 
     match_grammar = Sequence(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_bigquery_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_bigquery_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 ASC
 ASSERT_ROWS_MODIFIED
 AT
 BETWEEN
 BY
 CASE
 CAST
+CLONE
 COLLATE
 CONTAINS
 CREATE
 CROSS
 CUBE
 CURRENT
 DEFAULT
@@ -252,14 +253,15 @@
 SCHEMAS
 SECOND
 SEPARATOR
 SERVER
 SEQUENCE
 SESSION_USER
 SHARE
+SNAPSHOT
 SOURCE
 STAGE
 START
 STREAM
 SUNDAY
 SYSTEM
 SYSTEM_TIME
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,26 +5,30 @@
 
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.core.parser import (
     AnyNumberOf,
     AnySetOf,
     BaseSegment,
     Bracketed,
+    CodeSegment,
     Conditional,
     Dedent,
     Delimited,
     IdentifierSegment,
     Indent,
     LiteralSegment,
     Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
     Ref,
+    RegexLexer,
+    RegexParser,
+    SegmentGenerator,
     Sequence,
     StringLexer,
     SymbolSegment,
     TypedParser,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects.dialect_clickhouse_keywords import UNRESERVED_KEYWORDS
@@ -37,14 +41,37 @@
 
 clickhouse_dialect.insert_lexer_matchers(
     # https://clickhouse.com/docs/en/sql-reference/functions#higher-order-functions---operator-and-lambdaparams-expr-function
     [StringLexer("lambda", r"->", SymbolSegment)],
     before="newline",
 )
 
+clickhouse_dialect.patch_lexer_matchers(
+    [
+        RegexLexer(
+            "double_quote",
+            r'"([^"\\]|""|\\.)*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"\\]|""|\\.)*)"', 1),
+                "escape_replacements": [(r'(""|\\")', '"')],
+            },
+        ),
+        RegexLexer(
+            "back_quote",
+            r"`(?:[^`\\]|``|\\.)*`",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"`((?:[^`\\]|``|\\.)*)`", 1),
+                "escape_replacements": [(r"(``|\\`)", "`")],
+            },
+        ),
+    ]
+)
+
 clickhouse_dialect.add(
     BackQuotedIdentifierSegment=TypedParser(
         "back_quote",
         IdentifierSegment,
         type="quoted_identifier",
     ),
     LambdaFunctionSegment=TypedParser("lambda", SymbolSegment, type="lambda"),
@@ -170,14 +197,24 @@
         ),
         TypedParser(
             "dollar_quote",
             LiteralSegment,
             type="quoted_literal",
         ),
     ),
+    # Drop casefold from ANSI
+    NakedIdentifierSegment=SegmentGenerator(
+        # Generate the anti template from the set of reserved keywords
+        lambda dialect: RegexParser(
+            r"[A-Z0-9_]*[A-Z][A-Z0-9_]*",
+            IdentifierSegment,
+            type="naked_identifier",
+            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+        )
+    ),
     SingleIdentifierGrammar=OneOf(
         Ref("NakedIdentifierSegment"),
         Ref("QuotedIdentifierSegment"),
         Ref("SingleQuotedIdentifierSegment"),
         Ref("BackQuotedIdentifierSegment"),
     ),
     InOperatorGrammar=ansi_dialect.get_grammar("InOperatorGrammar").copy(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_clickhouse_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_clickhouse_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_databricks.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_databricks.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     NakedIdentifierSegment=SegmentGenerator(
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             r"[A-Z0-9_#]*[A-Z#][A-Z0-9_#]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.upper,
         )
     ),
     FunctionContentsExpressionGrammar=OneOf(
         Ref("ExpressionSegment"),
         Ref("NamedArgumentSegment"),
     ),
     ConditionalCrossJoinKeywordsGrammar=Nothing(),
@@ -117,22 +118,30 @@
             r"(--)[^\n]*",
             CommentSegment,
             segment_kwargs={"trim_start": ("--")},
         ),
         # In Db2, the only escape character is ' for single quote strings
         RegexLexer(
             "single_quote",
-            r"(?s)('')+?(?!')|('.*?(?<!')(?:'')*'(?!'))",
+            r"'((?:[^']|'')*)'",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^']|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
         ),
-        # In Db2, there is no escape character for double quote strings
+        # In Db2, the escape character is "" for double quote strings
         RegexLexer(
             "double_quote",
-            r'(?s)".+?"',
+            r'"((?:[^"]|"")*)"',
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
         ),
         # In Db2, a field could have a # pound/hash sign
         RegexLexer("word", r"[0-9a-zA-Z_#]+", WordSegment),
     ]
 )
 
 db2_dialect.add(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_db2_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_db2_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_duckdb.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_duckdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,28 @@
     AnyNumberOf,
     BaseSegment,
     BinaryOperatorSegment,
     Bracketed,
     CodeSegment,
     Dedent,
     Delimited,
+    IdentifierSegment,
     Indent,
     Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
     Ref,
+    RegexLexer,
     Sequence,
     StringLexer,
     StringParser,
     SymbolSegment,
+    TypedParser,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects import dialect_postgres as postgres
 
 ansi_dialect = load_raw_dialect("ansi")
 postgres_dialect = load_raw_dialect("postgres")
 duckdb_dialect = postgres_dialect.copy_as("duckdb")
@@ -51,19 +54,14 @@
 )
 
 duckdb_dialect.add(
     LambdaArrowSegment=StringParser("->", SymbolSegment, type="lambda_arrow"),
 )
 
 duckdb_dialect.replace(
-    SingleIdentifierGrammar=OneOf(
-        Ref("NakedIdentifierSegment"),
-        Ref("QuotedIdentifierSegment"),
-        Ref("SingleQuotedIdentifierSegment"),
-    ),
     DivideSegment=OneOf(
         StringParser("//", BinaryOperatorSegment),
         StringParser("/", BinaryOperatorSegment),
     ),
     CreateTableAsStatementSegment=Nothing(),
     UnionGrammar=ansi_dialect.get_grammar("UnionGrammar").copy(
         insert=[
@@ -110,23 +108,55 @@
     ColumnsExpressionGrammar=Sequence(
         Ref("ColumnsExpressionFunctionNameSegment"),
         Bracketed(
             Ref("ColumnsExpressionFunctionContentsSegment"),
             parse_mode=ParseMode.GREEDY,
         ),
     ),
+    # Matching postgres lower casefold, as it is case-insensitive
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.lower
+    ),
+    SingleQuotedIdentifierSegment=TypedParser(
+        "single_quote", IdentifierSegment, type="quoted_identifier", casefold=str.lower
+    ),
 )
 
 duckdb_dialect.insert_lexer_matchers(
     [
         StringLexer("double_divide", "//", CodeSegment),
     ],
     before="divide",
 )
 
+duckdb_dialect.patch_lexer_matchers(
+    [
+        # In DuckDB, a double single/double quote resolves as a single/double quote in
+        # the string.
+        RegexLexer(
+            "single_quote",
+            r"'([^']|'')*'",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^']|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
+        ),
+        RegexLexer(
+            "double_quote",
+            r'"([^"]|"")*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
+        ),
+    ]
+)
+
 
 class ColumnConstraintSegment(ansi.ColumnConstraintSegment):
     """A column option; each CREATE TABLE column can have 0 or more.
 
     https://duckdb.org/docs/sql/statements/create_table
     https://duckdb.org/docs/sql/statements/alter_table
     """
@@ -359,14 +389,34 @@
             Ref("SetOperatorSegment"),
             Ref("OrderByClauseSegment"),
             Ref("LimitClauseSegment"),
         ],
     )
 
 
+class TableReferenceSegment(ansi.TableReferenceSegment):
+    """A reference to an table, CTE, subquery or alias.
+
+    Overload for DuckDB as only tables can be single quoted identifiers
+    when used by the httpfs extension.
+    """
+
+    match_grammar = ansi.TableReferenceSegment.match_grammar.copy(
+        insert=[Ref("SingleQuotedIdentifierSegment")],
+    )
+
+
+class AliasExpressionSegment(ansi.AliasExpressionSegment):
+    """A reference to an object with an `AS` clause.
+
+    The optional AS keyword allows both implicit and explicit aliasing.
+    Inherit from ANSI instead of Postgres.
+    """
+
+
 class OrderByClauseSegment(ansi.OrderByClauseSegment):
     """A `ORDER BY` clause like in `SELECT`."""
 
     match_grammar: Matchable = Sequence(
         "ORDER",
         "BY",
         Indent,
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,21 +23,21 @@
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
     Ref,
     RegexLexer,
     RegexParser,
+    SegmentGenerator,
     Sequence,
     StringLexer,
     StringParser,
     SymbolSegment,
     TypedParser,
 )
-from sqlfluff.core.parser.segments.generator import SegmentGenerator
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects.dialect_exasol_keywords import (
     BARE_FUNCTIONS,
     RESERVED_KEYWORDS,
     SESSION_PARAMETERS,
     SYSTEM_PARAMETERS,
     UNRESERVED_KEYWORDS,
@@ -77,14 +77,17 @@
         RegexLexer("lua_multiline_quotes", r"\[{2}([^[\\]|\\.)*\]{2}", CodeSegment),
         # This matches escaped identifier e.g. [day]. There can be reserved keywords
         # within the square brackets.
         RegexLexer(
             "escaped_identifier",
             r"\[\w+\]",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"\[(\w+)\]", 1),
+            },
         ),
         RegexLexer(
             "udf_param_dot_syntax",
             r"\.{3}",
             CodeSegment,
         ),
         RegexLexer(
@@ -117,19 +120,27 @@
         # strings like in the IMPORT function
         # https://docs.exasol.com/sql_references/basiclanguageelements.htm#Delimited_Identifiers
         # https://docs.exasol.com/sql_references/literals.htm
         RegexLexer(
             "single_quote",
             r"'([^']|'')*'",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^']|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
         ),
         RegexLexer(
             "double_quote",
             r'"([^"]|"")*"',
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
         ),
         RegexLexer(
             "inline_comment",
             r"--[^\n]*",
             CommentSegment,
             segment_kwargs={"trim_start": ("--")},
         ),
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_exasol_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_exasol_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_greenplum_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_greenplum_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Matchable,
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
     Ref,
     RegexParser,
+    SegmentGenerator,
     Sequence,
     StringParser,
     SymbolSegment,
     TypedParser,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 from sqlfluff.dialects.dialect_hive_keywords import (
@@ -133,26 +134,44 @@
             )
         ),
     ),
     BackQuotedIdentifierSegment=TypedParser(
         "back_quote",
         IdentifierSegment,
         type="quoted_identifier",
+        casefold=str.lower,
     ),
 )
 
 # https://cwiki.apache.org/confluence/display/hive/languagemanual+joins
 hive_dialect.replace(
     JoinKeywordsGrammar=Sequence(Sequence("SEMI", optional=True), "JOIN"),
     QuotedLiteralSegment=OneOf(
-        TypedParser("single_quote", LiteralSegment, type="quoted_literal"),
-        TypedParser("double_quote", LiteralSegment, type="quoted_literal"),
-        TypedParser("back_quote", LiteralSegment, type="quoted_literal"),
+        TypedParser(
+            "single_quote", LiteralSegment, type="quoted_literal", casefold=str.lower
+        ),
+        TypedParser(
+            "double_quote", LiteralSegment, type="quoted_literal", casefold=str.lower
+        ),
+        TypedParser(
+            "back_quote", LiteralSegment, type="quoted_literal", casefold=str.lower
+        ),
     ),
     TrimParametersGrammar=Nothing(),
+    # ANSI with lower casefold
+    NakedIdentifierSegment=SegmentGenerator(
+        # Generate the anti template from the set of reserved keywords
+        lambda dialect: RegexParser(
+            r"[A-Z0-9_]*[A-Z][A-Z0-9_]*",
+            IdentifierSegment,
+            type="naked_identifier",
+            anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.lower,
+        )
+    ),
     SingleIdentifierGrammar=ansi_dialect.get_grammar("SingleIdentifierGrammar").copy(
         insert=[
             Ref("BackQuotedIdentifierSegment"),
         ]
     ),
     SelectClauseTerminatorGrammar=ansi_dialect.get_grammar(
         "SelectClauseTerminatorGrammar"
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_hive_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_hive_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_materialize_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_materialize_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,27 @@
         #         '                single quote (end of the single-quoted string)
         #         (?!')            negative lookahead: not single quote
         #     )                    group1 end
         RegexLexer(
             "single_quote",
             r"(?s)('(?:\\'|''|\\\\|[^'])*'(?!'))",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"(?s)('((?:\\'|''|\\\\|[^'])*)'(?!'))", 2),
+                "escape_replacements": [(r"\\'|''", "'")],
+            },
         ),
         RegexLexer(
             "double_quote",
             r'(?s)("(?:\\"|""|\\\\|[^"])*"(?!"))',
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'(?s)("((?:\\"|""|\\\\|[^"])*)"(?!"))', 2),
+                "escape_replacements": [(r'\\"|""', '"')],
+            },
         ),
     ]
 )
 
 mysql_dialect.insert_lexer_matchers(
     [
         RegexLexer(
@@ -334,14 +342,15 @@
                                 Bracketed(
                                     Ref("NumericLiteralSegment", optional=True),
                                     optional=True,
                                 ),
                             ),
                             Ref("NumericLiteralSegment"),
                             Ref("QuotedLiteralSegment"),
+                            "NULL",
                         ),
                         optional=True,
                     ),
                     Sequence(
                         "ON",
                         "UPDATE",
                         OneOf(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_mysql_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_mysql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_oracle.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,27 @@
 oracle_dialect.patch_lexer_matchers(
     [
         RegexLexer("word", r"[a-zA-Z][0-9a-zA-Z_$#]*", WordSegment),
         RegexLexer(
             "single_quote",
             r"'([^'\\]|\\|\\.|'')*'",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^'\\]|\\|\\.|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
+        ),
+        RegexLexer(
+            "double_quote",
+            r'"([^"]|"")*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
         ),
     ]
 )
 
 oracle_dialect.insert_lexer_matchers(
     [
         RegexLexer(
@@ -171,14 +184,15 @@
     ),
     NakedIdentifierSegment=SegmentGenerator(
         lambda dialect: RegexParser(
             r"[A-Z0-9_]*[A-Z][A-Z0-9_#$]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.upper,
         )
     ),
     PostFunctionGrammar=AnyNumberOf(
         Ref("WithinGroupClauseSegment"),
         Ref("FilterClauseGrammar"),
         Ref("OverClauseSegment", optional=True),
     ),
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,22 +175,30 @@
             r"(--)[^\n]*",
             CommentSegment,
             segment_kwargs={"trim_start": ("--")},
         ),
         # In Postgres, the only escape character is ' for single quote strings
         RegexLexer(
             "single_quote",
-            r"(?s)('')+?(?!')|('.*?(?<!')(?:'')*'(?!'))",
+            r"'([^']|'')*'",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^']|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
         ),
-        # In Postgres, there is no escape character for double quote strings
+        # In Postgres, the escape character is "" for double quote strings
         RegexLexer(
             "double_quote",
-            r'(?s)".+?"',
+            r'"([^"]|"")*"',
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
         ),
         # Patching block comments to account for nested blocks.
         # N.B. this syntax is only possible via the non-standard-library
         # (but still backwards compatible) `regex` package.
         # https://pypi.org/project/regex/
         # Pattern breakdown:
         # /\*                    Match opening slash.
@@ -375,14 +383,15 @@
         lambda dialect: RegexParser(
             # Can’t begin with $, must only contain digits, letters, underscore it $ but
             # can’t be all digits.
             r"([A-Z_]+|[0-9]+[A-Z_$])[A-Z0-9_$]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.lower,
         )
     ),
     Expression_C_Grammar=Sequence(
         Ref("WalrusOperatorSegment", optional=True),
         ansi_dialect.get_grammar("Expression_C_Grammar"),
     ),
     ParameterNameSegment=RegexParser(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_postgres_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_postgres_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
             # Optionally begins with # for temporary tables. Otherwise
             # must only contain digits, letters, underscore, and $ but
             # can’t be all digits.
             r"#?([A-Z_]+|[0-9]+[A-Z_$])[A-Z0-9_$]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.lower,
         )
     ),
 )
 
 redshift_dialect.patch_lexer_matchers(
     [
         # add optional leading # to word for temporary tables
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_redshift_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_redshift_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,14 +566,15 @@
         # Generate the anti template from the set of reserved keywords
         lambda dialect: RegexParser(
             # See https://docs.snowflake.com/en/sql-reference/identifiers-syntax.html
             r"[a-zA-Z_][a-zA-Z0-9_$]*",
             IdentifierSegment,
             type="naked_identifier",
             anti_template=r"^(" + r"|".join(dialect.sets("reserved_keywords")) + r")$",
+            casefold=str.upper,
         )
     ),
     LiteralGrammar=ansi_dialect.get_grammar("LiteralGrammar").copy(
         insert=[
             Ref("ReferencedVariableNameSegment"),
         ]
     ),
@@ -613,14 +614,15 @@
         Ref("StagePath"),
         Sequence(
             "IDENTIFIER",
             Bracketed(
                 OneOf(
                     Ref("SingleQuotedIdentifierSegment"),
                     Ref("ReferencedVariableNameSegment"),
+                    Ref("BindVariableSegment"),
                 ),
             ),
         ),
     ),
     PostFunctionGrammar=Sequence(
         Ref("WithinGroupClauseSegment", optional=True),
         Sequence(OneOf("IGNORE", "RESPECT"), "NULLS", optional=True),
@@ -1250,23 +1252,30 @@
     )
 
 
 class StatementSegment(ansi.StatementSegment):
     """A generic segment, to any of its child subsegments."""
 
     match_grammar = ansi.StatementSegment.match_grammar.copy(
+        # NOTE: The Scripting Block segment must be tried before
+        # we get to the transaction statement (from the ansi dialect)
+        # because they both start with BEGIN.
+        insert=[
+            Ref("ScriptingBlockStatementSegment"),
+        ],
+        before=Ref("TransactionStatementSegment"),
+    ).copy(
         insert=[
             Ref("AccessStatementSegment"),
             Ref("CreateStatementSegment"),
             Ref("CreateTaskSegment"),
             Ref("CreateUserSegment"),
             Ref("CreateCloneStatementSegment"),
             Ref("CreateProcedureStatementSegment"),
             Ref("AlterProcedureStatementSegment"),
-            Ref("ScriptingBlockStatementSegment"),
             Ref("ScriptingLetStatementSegment"),
             Ref("ReturnStatementSegment"),
             Ref("ShowStatementSegment"),
             Ref("AlterAccountStatementSegment"),
             Ref("AlterUserStatementSegment"),
             Ref("AlterSessionStatementSegment"),
             Ref("AlterTaskStatementSegment"),
@@ -1321,14 +1330,15 @@
             Ref("AlterSequenceStatementSegment"),
             Ref("AlterDatabaseSegment"),
             Ref("AlterMaskingPolicySegment"),
             Ref("AlterNetworkPolicyStatementSegment"),
             Ref("CreateExternalVolumeStatementSegment"),
             Ref("DropExternalVolumeStatementSegment"),
             Ref("AlterExternalVolumeStatementSegment"),
+            Ref("ForInLoopSegment"),
         ],
         remove=[
             Ref("CreateIndexStatementSegment"),
             Ref("DropIndexStatementSegment"),
         ],
     )
 
@@ -3114,22 +3124,41 @@
 class ScriptingBlockStatementSegment(BaseSegment):
     """A snowflake `BEGIN ... END` statement for SQL scripting.
 
     https://docs.snowflake.com/en/sql-reference/snowflake-scripting/begin
     """
 
     type = "scripting_block_statement"
-    match_grammar = OneOf(
+    match_grammar = Sequence(
         Sequence(
             "BEGIN",
-            Delimited(
+            Indent,
+            Ref("StatementSegment"),
+        ),
+        AnyNumberOf(
+            Sequence(
+                Ref("DelimiterGrammar"),
                 Ref("StatementSegment"),
             ),
+            terminators=[
+                OneOf(
+                    Sequence(Ref("DelimiterGrammar"), "END"),
+                    # Don't terminate on an "END FOR", because that's a different
+                    # expression.
+                    exclude=Sequence(Ref("DelimiterGrammar"), "END", "FOR"),
+                ),
+            ],
+            # NOTE: We can't be greedy because there may be nested loops. This
+            # does make understanding any failed parsing loops difficult but I
+            # don't think there's an easy way around that.
         ),
-        Sequence("END"),
+        Ref("DelimiterGrammar"),
+        Dedent,
+        "END",
+        reset_terminators=True,
     )
 
 
 class ScriptingLetStatementSegment(BaseSegment):
     """A snowflake `LET` statement for SQL scripting.
 
     https://docs.snowflake.com/en/sql-reference/snowflake-scripting/let
@@ -7127,14 +7156,16 @@
     """`BEGIN`, `START TRANSACTION`, `COMMIT`, AND `ROLLBACK` statement grammar.
 
     Overwrites ANSI to match correct Snowflake grammar.
 
     https://docs.snowflake.com/en/sql-reference/sql/begin.html
     https://docs.snowflake.com/en/sql-reference/sql/commit.html
     https://docs.snowflake.com/en/sql-reference/sql/rollback.html
+
+    NOTE: "END" is not currently a supported keyword here.
     """
 
     match_grammar = OneOf(
         Sequence(
             "BEGIN",
             OneOf("WORK", "TRANSACTION", optional=True),
             Sequence("NAME", Ref("ObjectReferenceSegment"), optional=True),
@@ -7823,7 +7854,52 @@
             Sequence("UNSET", "TAG", Delimited(Ref("TagReferenceSegment"))),
             Sequence(
                 "SET", "COMMENT", Ref("EqualsSegment"), Ref("QuotedLiteralSegment")
             ),
             Sequence("UNSET", "COMMENT"),
         ),
     )
+
+
+class ForInLoopSegment(BaseSegment):
+    """FOR...IN...DO...END FOR statement.
+
+    https://docs.snowflake.com/en/developer-guide/snowflake-scripting/loops#for-loop
+    """
+
+    type = "for_in_statement"
+
+    match_grammar = Sequence(
+        Sequence(
+            Sequence(
+                "FOR",
+                Ref("LocalVariableNameSegment"),
+                "IN",
+                Ref("LocalVariableNameSegment"),
+                "DO",
+                Indent,
+            ),
+            Delimited(
+                Ref("StatementSegment"),
+                delimiter=Ref("DelimiterGrammar"),
+            ),
+            parse_mode=ParseMode.GREEDY_ONCE_STARTED,
+            reset_terminators=True,
+            terminators=[Sequence(Ref("DelimiterGrammar"), "END", "FOR")],
+        ),
+        # There must be a trailing semicolon
+        Ref("DelimiterGrammar"),
+        Dedent,
+        "END",
+        "FOR",
+    )
+
+
+class BindVariableSegment(BaseSegment):
+    """A :VARIABLE_NAME expression."""
+
+    type = "bind_variable"
+
+    match_grammar = Sequence(
+        Ref("ColonSegment"),
+        Ref("LocalVariableNameSegment"),
+    )
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_snowflake_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_snowflake_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_soql.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_soql.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,18 @@
         # including `
         # Ex: select `delimited `` with escaped` from `just delimited`
         # https://spark.apache.org/docs/latest/sql-ref-identifier.html#delimited-identifier
         RegexLexer(
             "back_quote",
             r"`([^`]|``)*`",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"`((?:[^`]|``)*)`", 1),
+                "escape_replacements": [(r"``", "`")],
+            },
         ),
         # Numeric literal matches integers, decimals, and exponential formats.
         # https://spark.apache.org/docs/latest/sql-ref-literals.html#numeric-literal
         # Pattern breakdown:
         # (?>                                    Atomic grouping
         #                           (https://www.regular-expressions.info/atomic.html).
         #                                        3 distinct groups here:
@@ -412,14 +416,16 @@
 sparksql_dialect.add(
     FileLiteralSegment=TypedParser("file_literal", LiteralSegment, type="file_literal"),
     BackQuotedIdentifierSegment=TypedParser(
         "back_quote",
         IdentifierSegment,
         type="quoted_identifier",
         trim_chars=("`",),
+        # match ANSI's naked identifier casefold, sparksql is case-insensitive.
+        casefold=str.upper,
     ),
     NakedSemiStructuredElementSegment=RegexParser(
         r"[A-Z0-9_]*",
         CodeSegment,
         type="semi_structured_element",
     ),
     QuotedSemiStructuredElementSegment=TypedParser(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sparksql_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sparksql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 
 from sqlfluff.core.dialects import load_raw_dialect
 from sqlfluff.core.parser import (
     AnyNumberOf,
     Anything,
     BaseSegment,
     Bracketed,
+    CodeSegment,
     CommentSegment,
     Delimited,
+    IdentifierSegment,
     LiteralSegment,
     Matchable,
     NewlineSegment,
     Nothing,
     OneOf,
     OptionallyBracketed,
     ParseMode,
@@ -53,17 +55,54 @@
             ),
             trim_post_subdivide=RegexLexer(
                 "whitespace",
                 r"[^\S\r\n]+",
                 WhitespaceSegment,
             ),
         ),
+        RegexLexer(
+            "single_quote",
+            r"'([^']|'')*'",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"'((?:[^']|'')*)'", 1),
+                "escape_replacements": [(r"''", "'")],
+            },
+        ),
+        RegexLexer(
+            "double_quote",
+            r'"([^"]|"")*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
+        ),
+        RegexLexer(
+            "back_quote",
+            r"`([^`]|``)*`",
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"`((?:[^`]|``)*)`", 1),
+                "escape_replacements": [(r"``", "`")],
+            },
+        ),
     ]
 )
 
+sqlite_dialect.add(
+    BackQuotedIdentifierSegment=TypedParser(
+        "back_quote",
+        IdentifierSegment,
+        type="quoted_identifier",
+        # match ANSI's naked identifier casefold, sqlite is case-insensitive.
+        casefold=str.upper,
+    ),
+)
+
 sqlite_dialect.replace(
     PrimaryKeyGrammar=Sequence(
         "PRIMARY", "KEY", Sequence("AUTOINCREMENT", optional=True)
     ),
     TemporaryTransientGrammar=Ref("TemporaryGrammar"),
     DateTimeLiteralGrammar=Sequence(
         OneOf("DATE", "DATETIME"),
@@ -75,14 +114,18 @@
         Ref("FunctionSegment"),
         Ref("ColumnReferenceSegment"),
         Ref("ExpressionSegment"),
         Sequence(
             Ref("DatatypeSegment"),
             Ref("LiteralGrammar"),
         ),
+        terminators=[
+            Ref("CommaSegment"),
+            Ref.keyword("AS"),
+        ],
     ),
     AutoIncrementGrammar=Nothing(),
     CommentClauseSegment=Nothing(),
     IntervalExpressionSegment=Nothing(),
     TimeZoneGrammar=Nothing(),
     FetchClauseSegment=Nothing(),
     TrimParametersGrammar=Nothing(),
@@ -191,14 +234,28 @@
         Sequence("DISTINCT", "FROM", optional=True),
     ),
     NanLiteralSegment=Nothing(),
     PatternMatchingGrammar=Sequence(
         Ref.keyword("NOT", optional=True),
         OneOf("GLOB", "REGEXP", "MATCH"),
     ),
+    SingleIdentifierGrammar=OneOf(
+        Ref("NakedIdentifierSegment"),
+        Ref("SingleQuotedIdentifierSegment"),
+        Ref("QuotedIdentifierSegment"),
+        Ref("BackQuotedIdentifierSegment"),
+        terminators=[Ref("DotSegment")],
+    ),
+    # match ANSI's naked identifier casefold, sqlite is case-insensitive.
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
+    ),
+    SingleQuotedIdentifierSegment=TypedParser(
+        "single_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
+    ),
 )
 
 
 class SetOperatorSegment(BaseSegment):
     """A set operator such as Union, Minus, Except or Intersect."""
 
     type = "set_operator"
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_sqlite_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_sqlite_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_teradata.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_teradata.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     BaseSegment,
     Bracketed,
     CodeSegment,
     ComparisonOperatorSegment,
     CompositeComparisonOperatorSegment,
     Dedent,
     Delimited,
+    IdentifierSegment,
     Indent,
     Matchable,
     OneOf,
     OptionallyBracketed,
     Ref,
     RegexLexer,
     Sequence,
     StringParser,
+    TypedParser,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
 
 ansi_dialect = load_raw_dialect("ansi")
 teradata_dialect = ansi_dialect.copy_as("teradata")
 
 teradata_dialect.patch_lexer_matchers(
@@ -118,15 +120,19 @@
         Ref("NotEqualToSegment"),
         Ref("NotEqualToSegment_a"),
         Ref("NotEqualToSegment_b"),
         Ref("NotEqualToSegment_c"),
         Ref("LikeOperatorSegment"),
         Sequence("IS", "DISTINCT", "FROM"),
         Sequence("IS", "NOT", "DISTINCT", "FROM"),
-    )
+    ),
+    # match ANSI's naked identifier casefold, teradata is case-insensitive.
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
+    ),
 )
 
 teradata_dialect.add(
     # Add Teradata comparison operator extensions
     EqualsSegment_a=StringParser("EQ", ComparisonOperatorSegment),
     GreaterThanSegment_a=StringParser("GT", ComparisonOperatorSegment),
     LessThanSegment_a=StringParser("LT", ComparisonOperatorSegment),
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 from sqlfluff.core.parser import (
     AnyNumberOf,
     Anything,
     BaseSegment,
     Bracketed,
     CodeSegment,
     Delimited,
+    IdentifierSegment,
     LiteralSegment,
     Matchable,
     Nothing,
     OneOf,
     Ref,
+    RegexLexer,
     Sequence,
     StringLexer,
     StringParser,
     SymbolSegment,
     TypedParser,
 )
 from sqlfluff.dialects import dialect_ansi as ansi
@@ -55,14 +57,28 @@
     before="like_operator",
 )
 
 trino_dialect.add(
     RightArrowOperator=StringParser("->", SymbolSegment, type="binary_operator"),
 )
 
+trino_dialect.patch_lexer_matchers(
+    [
+        RegexLexer(
+            "double_quote",
+            r'"([^"]|"")*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
+        ),
+    ]
+)
+
 trino_dialect.replace(
     DateTimeLiteralGrammar=OneOf(
         Sequence(
             OneOf("DATE", "TIME", "TIMESTAMP"),
             TypedParser(
                 "single_quote", LiteralSegment, type="date_constructor_literal"
             ),
@@ -190,14 +206,18 @@
         Ref("ArithmeticBinaryOperatorGrammar"),
         Ref("StringBinaryOperatorGrammar"),
         Ref("BooleanBinaryOperatorGrammar"),
         Ref("ComparisonOperatorGrammar"),
         # Add arrow operators for functions (e.g. regexp_replace)
         Ref("RightArrowOperator"),
     ),
+    # match ANSI's naked identifier casefold, trino is case-insensitive.
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
+    ),
 )
 
 
 class DatatypeSegment(BaseSegment):
     """Data type segment.
 
     See https://trino.io/docs/current/language/types.html
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_trino_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_trino_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,20 +161,26 @@
             r"[$][a-zA-Z0-9_]+",
             CodeSegment,
         ),
         RegexLexer(
             "square_quote",
             r"\[([^\[\]]*)*\]",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"\[([^\[\]]*)\]", 1),
+            },
         ),
         # T-SQL unicode strings
         RegexLexer(
             "single_quote_with_n",
             r"N'([^']|'')*'",
             CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r"N'((?:[^']|'')*)'", 1),
+            },
         ),
         RegexLexer(
             "hash_prefix",
             r"[#][#]?[a-zA-Z0-9_]+",
             CodeSegment,
         ),
         RegexLexer(
@@ -244,21 +250,30 @@
             "word", r"[0-9a-zA-Z_#@]+", WordSegment
         ),  # overriding to allow hash mark and at-sign in code
     ]
 )
 
 tsql_dialect.add(
     BracketedIdentifierSegment=TypedParser(
-        "square_quote", IdentifierSegment, type="quoted_identifier"
+        "square_quote",
+        IdentifierSegment,
+        type="quoted_identifier",
+        casefold=str.upper,
     ),
     HashIdentifierSegment=TypedParser(
-        "hash_prefix", IdentifierSegment, type="hash_identifier"
+        "hash_prefix",
+        IdentifierSegment,
+        type="hash_identifier",
+        casefold=str.upper,
     ),
     VariableIdentifierSegment=TypedParser(
-        "var_prefix", IdentifierSegment, type="variable_identifier"
+        "var_prefix",
+        IdentifierSegment,
+        type="variable_identifier",
+        casefold=str.upper,
     ),
     BatchDelimiterGrammar=Ref("GoStatementSegment"),
     QuotedLiteralSegmentWithN=TypedParser(
         "single_quote_with_n", LiteralSegment, type="quoted_literal"
     ),
     QuotedLiteralSegmentOptWithN=OneOf(
         Ref("QuotedLiteralSegment"),
@@ -372,16 +387,23 @@
             type="naked_identifier",
             anti_template=r"^("
             + r"|".join(
                 dialect.sets("reserved_keywords")
                 | dialect.sets("future_reserved_keywords")
             )
             + r")$",
+            casefold=str.upper,
         )
     ),
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote",
+        IdentifierSegment,
+        type="quoted_identifier",
+        casefold=str.upper,
+    ),
     # Overring ANSI BaseExpressionElement to remove Interval Expression Segment
     BaseExpressionElementGrammar=ansi_dialect.get_grammar(
         "BaseExpressionElementGrammar"
     ).copy(
         remove=[
             Ref("IntervalExpressionSegment"),
         ]
@@ -2431,14 +2453,15 @@
                     optional=True,
                 ),
                 # DEFAULT <value>
                 "DEFAULT",
                 OptionallyBracketed(
                     OneOf(
                         OptionallyBracketed(Ref("LiteralGrammar")),  # ((-1))
+                        Ref("BareFunctionSegment"),
                         Ref("FunctionSegment"),
                         Ref("NextValueSequenceSegment"),
                     ),
                 ),
             ),
             Ref("IdentityGrammar"),
             Sequence("NOT", "FOR", "REPLICATION"),
@@ -4039,15 +4062,15 @@
             ),
         ),
         Ref("OptionClauseSegment", optional=True),
         Ref("DelimiterGrammar", optional=True),
     )
 
 
-class FromClauseSegment(BaseSegment):
+class FromClauseSegment(ansi.FromClauseSegment):
     """A `FROM` clause like in `SELECT`.
 
     NOTE: this is a delimited set of table expressions, with a variable
     number of optional join clauses with those table expressions. The
     delmited aspect is the higher of the two such that the following is
     valid (albeit unusual):
 
@@ -4063,16 +4086,14 @@
     type = "from_clause"
     match_grammar = Sequence(
         "FROM",
         Delimited(Ref("FromExpressionSegment")),
         Ref("DelimiterGrammar", optional=True),
     )
 
-    get_eventual_aliases = ansi.FromClauseSegment.get_eventual_aliases
-
 
 class FromExpressionElementSegment(ansi.FromExpressionElementSegment):
     """FROM Expression Element Segment.
 
     Overriding ANSI to add Temporal Query.
     """
 
@@ -5035,14 +5056,15 @@
     https://docs.microsoft.com/en-us/sql/t-sql/statements/create-trigger-transact-sql?view=sql-server-ver15
     """
 
     type = "create_trigger"
 
     match_grammar: Matchable = Sequence(
         "CREATE",
+        Sequence("OR", "ALTER", optional=True),
         "TRIGGER",
         Ref("TriggerReferenceSegment"),
         "ON",
         OneOf(
             Ref("TableReferenceSegment"),
             Sequence("ALL", "SERVER"),
             "DATABASE",
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_tsql_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_tsql_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     BaseSegment,
     Bracketed,
     BracketedSegment,
     CodeSegment,
     CompositeComparisonOperatorSegment,
     Dedent,
     Delimited,
+    IdentifierSegment,
     Indent,
     KeywordSegment,
     LiteralSegment,
     Matchable,
     MultiStringParser,
     OneOf,
     OptionallyBracketed,
@@ -86,14 +87,28 @@
             r"(?<!')(?:'')*')'(?!'))",
             CodeSegment,
         ),
     ],
     before="like_operator",
 )
 
+vertica_dialect.patch_lexer_matchers(
+    [
+        RegexLexer(
+            "double_quote",
+            r'"([^"]|"")*"',
+            CodeSegment,
+            segment_kwargs={
+                "quoted_value": (r'"((?:[^"]|"")*)"', 1),
+                "escape_replacements": [(r'""', '"')],
+            },
+        ),
+    ]
+)
+
 # Set Keywords
 vertica_dialect.update_keywords_set_from_multiline_string(
     "unreserved_keywords", vertica_unreserved_keywords
 )
 
 vertica_dialect.update_keywords_set_from_multiline_string(
     "reserved_keywords", vertica_reserved_keywords
@@ -452,14 +467,17 @@
             TypedParser(
                 "escaped_single_quote",
                 LiteralSegment,
                 type="quoted_literal",
             ),
         ),
     ),
+    QuotedIdentifierSegment=TypedParser(
+        "double_quote", IdentifierSegment, type="quoted_identifier", casefold=str.upper
+    ),
 )
 
 
 class ShorthandCastSegment(ansi.ShorthandCastSegment):
     """A casting operation using '::' or '::!'."""
 
     match_grammar: Matchable = Sequence(
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/dialects/dialect_vertica_keywords.py` & `sqlfluff-3.0.5/src/sqlfluff/dialects/dialect_vertica_keywords.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/diff_quality_plugin.py` & `sqlfluff-3.0.5/src/sqlfluff/diff_quality_plugin.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL04.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,18 +64,18 @@
     aliases = ("L020",)
     groups: Tuple[str, ...] = ("all", "core", "aliasing", "aliasing.unique")
     crawl_behaviour = SegmentSeekerCrawler({"select_statement"})
 
     def _lint_references_and_aliases(
         self,
         table_aliases: List[AliasInfo],
-        standalone_aliases: List[str],
+        standalone_aliases: List[BaseSegment],
         references: List[ObjectReferenceSegment],
         col_aliases: List[ColumnAliasInfo],
-        using_cols: List[str],
+        using_cols: List[BaseSegment],
         parent_select: Optional[BaseSegment],
     ) -> Optional[List[LintResult]]:
         """Check whether any aliases are duplicates.
 
         NB: Subclasses of this error should override this function.
 
         """
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL05.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Implementation of Rule AL05."""
 
+from collections import Counter
 from dataclasses import dataclass, field
 from typing import List, Set, cast
 
-from sqlfluff.core.dialects.base import Dialect
 from sqlfluff.core.dialects.common import AliasInfo
-from sqlfluff.core.parser.segments import BaseSegment
+from sqlfluff.core.parser.segments import BaseSegment, RawSegment
 from sqlfluff.core.rules import (
     BaseRule,
     EvalResultType,
     LintFix,
     LintResult,
     RuleContext,
 )
@@ -56,75 +56,146 @@
         FROM foo
 
     """
 
     name = "aliasing.unused"
     aliases = ("L025",)
     groups = ("all", "core", "aliasing")
+    config_keywords = ["alias_case_check"]
     crawl_behaviour = SegmentSeekerCrawler({"select_statement"})
     _dialects_requiring_alias_for_values_clause = [
+        "athena",
         "snowflake",
         "tsql",
         "postgres",
     ]
     is_fix_compatible = True
 
+    # config
+    alias_case_check: str
+
     def _eval(self, context: RuleContext) -> EvalResultType:
         violations: List[LintResult] = []
         assert context.segment.is_type("select_statement")
         # Exit early if the SELECT does not define any aliases.
         select_info = get_select_statement_info(context.segment, context.dialect)
         if not select_info or not select_info.table_aliases:
             return None
 
         # Analyze the SELECT.
         alias: AliasInfo
-        query = AL05Query.from_segment(context.segment, dialect=context.dialect)
-        self._analyze_table_aliases(query, context.dialect)
+        query = cast(
+            AL05Query, AL05Query.from_segment(context.segment, dialect=context.dialect)
+        )
+        self._analyze_table_aliases(query)
 
-        if context.dialect.name == "redshift":
+        if context.dialect.name in ("redshift", "bigquery"):
             # Redshift supports un-nesting using aliases.
             # Detect that situation and ignore.
             # https://docs.aws.amazon.com/redshift/latest/dg/query-super.html#unnest
 
             # Do any references refer to aliases in the same list?
             references = set()
             aliases = set()
 
             for alias in query.aliases:
                 aliases.add(alias.ref_str)
+                if alias.segment:
+                    aliases.add(self._cs_str_id(alias.segment))
                 if not alias.object_reference:
                     continue  # pragma: no cover
                 for seg in alias.object_reference.segments:
                     if seg.is_type("identifier"):
-                        references.add(seg.raw)
+                        references.add(self._cs_str_id(seg))
 
             # If there's any overlap between aliases and reference
             if aliases.intersection(references):
                 self.logger.debug(
-                    "Overlapping references found. Assuming redshift semi-structured."
+                    "Overlapping references found. Assuming %s semi-structured.",
+                    context.dialect.name,
                 )
                 return None
 
+        # Get the number of times an object (table/view) is referenced. While some
+        # dialects can handle the same table name reference with different schemas,
+        # we don't want to allow a conflict with AL04's uniqueness rule so we grab
+        # the base table name instead of the fully qualified one to determine naming
+        # collisions.
+        ref_counter = Counter(
+            self._cs_str_id(a.object_reference.segments[-1])
+            for a in query.aliases
+            if a.object_reference and a.object_reference.segments
+        )
         for alias in query.aliases:
             # Skip alias if it's required (some dialects require aliases for
             # VALUES clauses).
             if alias.from_expression_element and self._is_alias_required(
                 alias.from_expression_element, context.dialect.name
             ):
                 continue
+            # Skip alias if the table is referenced more than once, some dialects
+            # require the referenced table names to be unique even if not returned
+            # by the statement.
+            if (
+                alias.object_reference
+                and alias.object_reference.segments
+                and ref_counter.get(
+                    self._cs_str_id(alias.object_reference.segments[-1]),
+                    0,
+                )
+                > 1
+            ):
+                continue
+            # Redshift requires an alias when a `QUALIFY` statement immediately follows
+            # the `FROM` clause.
+            # https://docs.aws.amazon.com/redshift/latest/dg/r_QUALIFY_clause.html
+            if (
+                context.dialect.name == "redshift"
+                and alias.alias_expression
+                and self._followed_by_qualify(context, alias)
+            ):
+                continue
 
-            if alias.aliased and alias.ref_str not in query.tbl_refs:
+            if (
+                alias.aliased
+                and alias.segment
+                and self._cs_str_id(alias.segment) not in query.tbl_refs
+            ):
                 # Unused alias. Report and fix.
                 violations.append(self._report_unused_alias(alias))
         return violations or None
 
-    @classmethod
+    def _cs_str_id(self, identifier: BaseSegment):
+        _normal_val = identifier.raw_normalized(self.alias_case_check == "dialect")
+        if self.alias_case_check == "case_insensitive":
+            _normal_val = _normal_val.upper()
+        elif self.alias_case_check == "quoted_cs_naked_upper":
+            if identifier.is_type("naked_identifier"):
+                _normal_val = _normal_val.upper()
+        elif self.alias_case_check == "quoted_cs_naked_lower":
+            if identifier.is_type("naked_identifier"):
+                _normal_val = _normal_val.lower()
+        return _normal_val
+
+    def _followed_by_qualify(self, context: RuleContext, alias: AliasInfo) -> bool:
+        curr_from_seen = False
+        assert alias.alias_expression
+        for seg in context.segment.segments:
+            if alias.alias_expression.get_end_loc() == seg.get_end_loc():
+                curr_from_seen = True
+            elif curr_from_seen and not seg.is_code:
+                continue
+            elif curr_from_seen and seg.is_type("qualify_clause"):
+                return True
+            elif curr_from_seen:
+                return False
+        return False
+
     def _is_alias_required(
-        cls, from_expression_element: BaseSegment, dialect_name: str
+        self, from_expression_element: BaseSegment, dialect_name: str
     ) -> bool:
         """Given an alias, is it REQUIRED to be present?
 
         Aliases are required in SOME, but not all dialects when there's a VALUES
         clause.
         """
         # Look for a table_expression (i.e. VALUES clause) as a descendant of
@@ -134,15 +205,15 @@
         for segment in from_expression_element.iter_segments(expanding=("bracketed",)):
             if segment.is_type("table_expression"):
                 # Found a table expression. Does it have a VALUES clause?
                 if segment.get_child("values_clause"):
                     # Found a VALUES clause. Is this a dialect that requires
                     # VALUE clauses to be aliased?
                     return (
-                        dialect_name in cls._dialects_requiring_alias_for_values_clause
+                        dialect_name in self._dialects_requiring_alias_for_values_clause
                     )
                 elif any(
                     seg.is_type(
                         "select_statement", "set_expression", "with_compound_statement"
                     )
                     for seg in segment.iter_segments(expanding=("bracketed",))
                 ):
@@ -155,49 +226,51 @@
                     # None of the special cases above applies, so the alias is
                     # not required.
                     return False
 
         # This should never happen. Return False just to be safe.
         return False  # pragma: no cover
 
-    @classmethod
-    def _analyze_table_aliases(cls, query: AL05Query, dialect: Dialect) -> None:
+    def _analyze_table_aliases(self, query: AL05Query) -> None:
         # Get table aliases defined in query.
         for selectable in query.selectables:
             select_info = selectable.select_info
             if select_info:
                 # Record the aliases.
                 query.aliases += select_info.table_aliases
 
                 # Look at each table reference; if it's an alias reference,
                 # resolve the alias: could be an alias defined in "query"
                 # itself or an "ancestor" query.
-                for r in select_info.reference_buffer:
+                for r in (
+                    select_info.reference_buffer + select_info.table_reference_buffer
+                ):
                     for tr in r.extract_possible_references(
                         level=r.ObjectReferenceLevel.TABLE
                     ):
                         # This function walks up the query's parent stack if necessary.
-                        cls._resolve_and_mark_reference(query, tr.part)
+                        self._resolve_and_mark_reference(
+                            query, cast(RawSegment, tr.segments[0])
+                        )
 
         # Visit children.
         for child in query.children:
-            cls._analyze_table_aliases(cast(AL05Query, child), dialect)
+            self._analyze_table_aliases(cast(AL05Query, child))
 
-    @classmethod
-    def _resolve_and_mark_reference(cls, query: AL05Query, ref: str) -> None:
+    def _resolve_and_mark_reference(self, query: AL05Query, ref: RawSegment) -> None:
         # Does this query define the referenced alias?
-        if any(ref == a.ref_str for a in query.aliases):
+        _ref = self._cs_str_id(ref)
+        if any(_ref == self._cs_str_id(a.segment) for a in query.aliases if a.segment):
             # Yes. Record the reference.
-            query.tbl_refs.add(ref)
+            query.tbl_refs.add(_ref)
         elif query.parent:
             # No. Recursively check the query's parent hierarchy.
-            cls._resolve_and_mark_reference(cast(AL05Query, query.parent), ref)
+            self._resolve_and_mark_reference(query.parent, ref)
 
-    @classmethod
-    def _report_unused_alias(cls, alias: AliasInfo) -> LintResult:
+    def _report_unused_alias(self, alias: AliasInfo) -> LintResult:
         fixes = [LintFix.delete(alias.alias_expression)]  # type: ignore
         # Walk back to remove indents/whitespaces
         to_delete = (
             Segments(*alias.from_expression_element.segments)
             .reversed()
             .select(
                 start_seg=alias.alias_expression,
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL07.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL08.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/AL09.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/AL09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/aliasing/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/aliasing/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/AM07.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/AM07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/ambiguous/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/ambiguous/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/CP05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/CP05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/capitalisation/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/capitalisation/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV07.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV08.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV09.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV10.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/CV11.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/CV11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/convention/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/jinja/JJ01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/jinja/JJ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT07.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT08.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT09.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT10.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT10.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT11.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT11.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT12.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT12.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/LT13.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/LT13.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/layout/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF01.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Implementation of Rule RF01."""
 
 from dataclasses import dataclass, field
 from typing import List, Optional, Tuple, cast
 
 from sqlfluff.core.dialects.base import Dialect
 from sqlfluff.core.dialects.common import AliasInfo
+from sqlfluff.core.parser import BaseSegment
 from sqlfluff.core.rules import (
     BaseRule,
     LintResult,
     RuleContext,
 )
 from sqlfluff.core.rules.crawlers import SegmentSeekerCrawler
 from sqlfluff.core.rules.reference import object_ref_matches_table
@@ -23,15 +24,15 @@
 
 
 @dataclass
 class RF01Query(Query):
     """Query with custom RF01 info."""
 
     aliases: List[AliasInfo] = field(default_factory=list)
-    standalone_aliases: List[str] = field(default_factory=list)
+    standalone_aliases: List[BaseSegment] = field(default_factory=list)
 
 
 class Rule_RF01(BaseRule):
     """References cannot reference objects not present in ``FROM`` clause.
 
     .. note::
 
@@ -139,15 +140,15 @@
             if select_info:
                 # Record the available tables.
                 query.aliases += select_info.table_aliases
                 query.standalone_aliases += select_info.standalone_aliases
                 self.logger.debug(
                     "Aliases: %s %s",
                     [alias.ref_str for alias in select_info.table_aliases],
-                    select_info.standalone_aliases,
+                    [standalone.raw for standalone in select_info.standalone_aliases],
                 )
 
                 # Try and resolve each reference to a value in query.aliases (or
                 # in an ancestor query).
                 for r in select_info.reference_buffer:
                     if not self._should_ignore_reference(r, selectable):
                         # This function walks up the query's parent stack if necessary.
@@ -211,15 +212,15 @@
     ):
         # Does this query define the referenced table?
         possible_references = [tbl_ref[1] for tbl_ref in tbl_refs]
         targets = []
         for alias in query.aliases:
             targets += self._alias_info_as_tuples(alias)
         for standalone_alias in query.standalone_aliases:
-            targets.append((standalone_alias,))
+            targets.append((standalone_alias.raw,))
         if not object_ref_matches_table(possible_references, targets):
             # No. Check the parent query, if there is one.
             if query.parent:
                 return self._resolve_reference(
                     r, tbl_refs, dml_target_table, cast(RF01Query, query.parent)
                 )
             # No parent query. If there's a DML statement at the root, check its
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF02.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,18 +42,18 @@
     aliases = ("L027",)
     groups = ("all", "references")
     # Crawl behaviour is defined in AL04
 
     def _lint_references_and_aliases(
         self,
         table_aliases: List[AliasInfo],
-        standalone_aliases: List[str],
+        standalone_aliases: List[BaseSegment],
         references,
         col_aliases: List[ColumnAliasInfo],
-        using_cols: List[str],
+        using_cols: List[BaseSegment],
         parent_select: Optional[BaseSegment],
     ) -> Optional[List[LintResult]]:
         # Config type hints
         self.ignore_words_regex: str
 
         # Do we have more than one? If so, all references should be qualified.
         if len(table_aliases) <= 1:
@@ -90,18 +90,18 @@
             if (
                 this_ref_type == "unqualified"
                 # Allow unqualified columns that
                 # are actually aliases defined
                 # in a different select clause element.
                 and r.raw not in col_alias_names
                 # Allow columns defined in a USING expression.
-                and r.raw not in using_cols
+                and r.raw not in [using_col.raw for using_col in using_cols]
                 # Allow columns defined as standalone aliases
                 # (e.g. value table functions from bigquery)
-                and r.raw not in standalone_aliases
+                and r.raw not in [a.raw for a in standalone_aliases]
             ):
                 violation_buff.append(
                     LintResult(
                         anchor=r,
                         description=f"Unqualified reference {r.raw!r} found in "
                         "select with more than one referenced table/view.",
                     )
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF03.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     # because they will more accurately process any internal references.
     crawl_behaviour = SegmentSeekerCrawler(set(_START_TYPES), allow_recurse=False)
     _is_struct_dialect = False
     _dialects_with_structs = ["bigquery", "hive", "redshift"]
     # This could be turned into an option
     _fix_inconsistent_to = "qualified"
     is_fix_compatible = True
+    single_table_references: str
 
     def _eval(self, context: RuleContext) -> EvalResultType:
         """Override base class for dialects that use structs, or SELECT aliases."""
         # Config type hints
         self.force_enable: bool
         # Some dialects use structs (e.g. column.field) which look like
         # table references and so incorrectly trigger this rule.
@@ -129,15 +130,15 @@
                     fixable = False
 
                 yield from _check_references(
                     select_info.table_aliases,
                     select_info.standalone_aliases,
                     select_info.reference_buffer,
                     select_info.col_aliases,
-                    self.single_table_references,  # type: ignore
+                    self.single_table_references,
                     self._is_struct_dialect,
                     self._fix_inconsistent_to,
                     fixable,
                 )
         children = list(query.children)
         # 'query.children' includes CTEs and "main" queries, but not queries in
         # the "FROM" list. We want to visit those as well.
@@ -156,15 +157,15 @@
                     children.append(q)
         for child in children:
             yield from self._visit_queries(child, visited)
 
 
 def _check_references(
     table_aliases: List[AliasInfo],
-    standalone_aliases: List[str],
+    standalone_aliases: List[BaseSegment],
     references: List[ObjectReferenceSegment],
     col_aliases: List[ColumnAliasInfo],
     single_table_references: str,
     is_struct_dialect: bool,
     fix_inconsistent_to: Optional[str],
     fixable: bool,
 ) -> Iterator[LintResult]:
@@ -216,15 +217,15 @@
         yield lint_res
 
 
 def _validate_one_reference(
     single_table_references: str,
     ref: BaseSegment,
     this_ref_type: str,
-    standalone_aliases: List[str],
+    standalone_aliases: List[BaseSegment],
     table_ref_str: str,
     table_ref_str_source: Optional[BaseSegment],
     col_alias_names: List[str],
     seen_ref_types: Set[str],
     fixable: bool,
 ) -> Optional[LintResult]:
     # We skip any unqualified wildcard references (i.e. *). They shouldn't
@@ -232,15 +233,15 @@
     if not ref.is_qualified() and ref.is_type("wildcard_identifier"):  # type: ignore
         return None
     # Oddball case: Column aliases provided via function calls in by
     # FROM or JOIN. References to these don't need to be qualified.
     # Note there could be a table with a column by the same name as
     # this alias, so avoid bogus warnings by just skipping them
     # entirely rather than trying to enforce anything.
-    if ref.raw in standalone_aliases:
+    if ref.raw in [a.raw for a in standalone_aliases]:
         return None
 
     # Oddball case: tsql table variables can't be used to qualify references.
     # This appears here as an empty string for table_ref_str.
     if not table_ref_str:
         return None
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/RF06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/RF06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/references/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/references/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST02.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST02.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST03.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST03.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST04.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST04.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST05.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST05.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST06.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST06.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST07.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST07.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST08.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST08.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/ST09.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/ST09.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/structure/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/tsql/TQ01.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/tsql/TQ01.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/rules/tsql/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/rules/tsql/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/analysis/query.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/analysis/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,15 @@
                 select_statement=self.selectable,
                 table_aliases=[alias_info],
                 standalone_aliases=[],
                 reference_buffer=[],
                 select_targets=[],
                 col_aliases=[],
                 using_cols=[],
+                table_reference_buffer=[],
             )
 
     def get_wildcard_info(self) -> List[WildcardInfo]:
         """Find wildcard (*) targets in the SELECT."""
         buff: List[WildcardInfo] = []
         # Some select-like statements don't have select_info
         # (e.g. test_exasol_invalid_foreign_key_from)
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/analysis/select.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/analysis/select.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """Basic code analysis tools for SELECT statements."""
 
-from typing import List, NamedTuple, Optional, cast
+from typing import List, NamedTuple, Optional, Tuple, cast
 
 from sqlfluff.core.dialects.base import Dialect
 from sqlfluff.core.dialects.common import AliasInfo, ColumnAliasInfo
-from sqlfluff.core.parser.segments.base import BaseSegment
+from sqlfluff.core.parser.segments import BaseSegment
 from sqlfluff.dialects.dialect_ansi import (
+    FromClauseSegment,
+    JoinClauseSegment,
     ObjectReferenceSegment,
     SelectClauseElementSegment,
 )
 
 
 class SelectStatementColumnsAndTables(NamedTuple):
     """Structure returned by get_select_statement_info()."""
 
     select_statement: BaseSegment
     table_aliases: List[AliasInfo]
-    standalone_aliases: List[str]  # value table function aliases
+    standalone_aliases: List[BaseSegment]  # value table function aliases
     reference_buffer: List[ObjectReferenceSegment]
     select_targets: List[SelectClauseElementSegment]
     col_aliases: List[ColumnAliasInfo]
-    using_cols: List[str]
+    using_cols: List[BaseSegment]
+    table_reference_buffer: List[ObjectReferenceSegment]
 
 
 def _get_object_references(segment: BaseSegment) -> List[ObjectReferenceSegment]:
     return list(
         cast(ObjectReferenceSegment, _seg)
         for _seg in segment.recursive_crawl(
             "object_reference", no_recursive_seg_type="select_statement"
@@ -48,14 +51,15 @@
     if not sc:  # pragma: no cover
         # TODO: Review whether this clause should be removed. It might only
         # have existed for an old way of structuring the Exasol dialect.
         return None
     # NOTE: In this first crawl, don't crawl inside any sub-selects, that's very
     # important for both isolation and performance reasons.
     reference_buffer = _get_object_references(sc)
+    table_reference_buffer = []
     for potential_clause in (
         "where_clause",
         "groupby_clause",
         "having_clause",
         "orderby_clause",
         "qualify_clause",
     ):
@@ -76,14 +80,27 @@
     col_aliases = [_alias for _alias in _pre_aliases if _alias is not None]
 
     # Get any columns referred to in a using clause, and extract anything
     # from ON clauses.
     using_cols = []
     fc = segment.get_child("from_clause")
     if fc:
+        for table_expression in fc.recursive_crawl(
+            "table_expression", no_recursive_seg_type="select_statement"
+        ):
+            for seg in table_expression.iter_segments():
+                # table references can get tricky with what is a schema, table,
+                # project, or column. It may be best for now to use the redshift
+                # unnest logic for dialects that support arrays or objects/structs
+                # in AL05. However, this solves finding other types of references
+                # in functions such as LATERAL FLATTEN.
+                if not seg.is_type("table_reference"):
+                    reference_buffer += _get_object_references(seg)
+                elif cast(ObjectReferenceSegment, seg).is_qualified():
+                    table_reference_buffer += _get_object_references(seg)
         for join_clause in fc.recursive_crawl(
             "join_clause", no_recursive_seg_type="select_statement"
         ):
             seen_using = False
             for seg in join_clause.iter_segments():
                 if seg.is_type("keyword") and seg.raw_upper == "USING":
                     seen_using = True
@@ -91,52 +108,56 @@
                     for on_seg in seg.segments:
                         if on_seg.is_type("bracketed", "expression"):
                             # Deal with expressions
                             reference_buffer += _get_object_references(seg)
                 elif seen_using and seg.is_type("bracketed"):
                     for subseg in seg.segments:
                         if subseg.is_type("identifier"):
-                            using_cols.append(subseg.raw)
+                            using_cols.append(subseg)
                     seen_using = False
 
     return SelectStatementColumnsAndTables(
         select_statement=segment,
         table_aliases=table_aliases or [],
         standalone_aliases=standalone_aliases or [],
         reference_buffer=reference_buffer,
         select_targets=select_targets,
         col_aliases=col_aliases,
         using_cols=using_cols,
+        table_reference_buffer=table_reference_buffer,
     )
 
 
-def get_aliases_from_select(segment, dialect=None):
+def get_aliases_from_select(
+    segment: BaseSegment, dialect: Optional[Dialect] = None
+) -> Tuple[Optional[list], Optional[list]]:
     """Gets the aliases referred to in the FROM clause.
 
     Returns a tuple of two lists:
     - Table aliases
     - Value table function aliases
     """
     fc = segment.get_child("from_clause")
     if not fc:
         # If there's no from clause then just abort.
         return None, None
+    assert isinstance(fc, (FromClauseSegment, JoinClauseSegment))
     aliases = fc.get_eventual_aliases()
 
     # We only want table aliases, so filter out aliases for value table
     # functions, lambda parameters and pivot columns.
-    standalone_aliases = []
+    standalone_aliases: List[BaseSegment] = []
     standalone_aliases += _get_pivot_table_columns(segment, dialect)
     standalone_aliases += _get_lambda_argument_columns(segment, dialect)
 
     table_aliases = []
     for table_expr, alias_info in aliases:
         if _has_value_table_function(table_expr, dialect):
-            if alias_info[0] not in standalone_aliases:
-                standalone_aliases.append(alias_info[0])
+            if alias_info.segment and alias_info.segment not in standalone_aliases:
+                standalone_aliases.append(alias_info.segment)
         elif alias_info not in table_aliases:
             table_aliases.append(alias_info)
 
     return table_aliases, standalone_aliases
 
 
 def _has_value_table_function(table_expr, dialect) -> bool:
@@ -151,73 +172,75 @@
         # remove
         # See: https://github.com/sqlfluff/sqlfluff/issues/1304
         if function_name.raw.upper().strip() in dialect.sets("value_table_functions"):
             return True
     return False
 
 
-def _get_pivot_table_columns(segment, dialect) -> list:
+def _get_pivot_table_columns(
+    segment: BaseSegment, dialect: Optional[Dialect]
+) -> List[BaseSegment]:
     if not dialect:
         # We need the dialect to get the pivot table column names. If
         # we don't have it, assume the clause does not have a pivot table
         return []  # pragma: no cover
 
     fc = segment.recursive_crawl("from_pivot_expression")
     if not fc:
         # If there's no pivot clause then just abort.
         return []  # pragma: no cover
 
-    pivot_table_column_aliases = []
+    pivot_table_column_aliases: list[BaseSegment] = []
 
     for pivot_table_column_alias in segment.recursive_crawl("pivot_column_reference"):
-        if pivot_table_column_alias.raw not in pivot_table_column_aliases:
-            pivot_table_column_aliases.append(pivot_table_column_alias.raw)
+        if pivot_table_column_alias.raw not in [
+            a.raw for a in pivot_table_column_aliases
+        ]:
+            pivot_table_column_aliases.append(pivot_table_column_alias)
 
     return pivot_table_column_aliases
 
 
 # Lambda arguments,
 # e.g. `x` and `y` in `x -> x is not null` and `(x, y) -> x + y`
 # are declared in-place, and are as such standalone – i.e. they do not reference
 # identifiers or columns that we should expect to be declared somewhere else.
 # These columns are interesting to identify since they can get special
 # treatment in some rules.
 def _get_lambda_argument_columns(
-    segment: BaseSegment, dialect: Dialect
-) -> Optional[List[str]]:
+    segment: BaseSegment, dialect: Optional[Dialect]
+) -> List[BaseSegment]:
     if not dialect or dialect.name not in ["athena", "sparksql"]:
         # Only athena and sparksql are known to have lambda expressions,
         # so all other dialects will have zero lambda columns
         return []
 
-    lambda_argument_columns = []
+    lambda_argument_columns: list[BaseSegment] = []
     for potential_lambda in segment.recursive_crawl("expression"):
         potential_arrow = potential_lambda.get_child("binary_operator")
         if potential_arrow and potential_arrow.raw == "->":
             arrow_operator = potential_arrow
             # The arguments will be before the arrow operator, so we get anything
             # that is a column reference or a set of bracketed column references before
             # the arrow. There should be exactly one segment matching this, if there are
             # more, this doesn't cleanly match a lambda expression
             argument_segments = potential_lambda.select_children(
                 stop_seg=arrow_operator,
-                select_if=(
-                    lambda x: x.is_type("bracketed") or x.is_type("column_reference")
-                ),
+                select_if=(lambda x: x.is_type("bracketed", "column_reference")),
             )
 
             assert len(argument_segments) == 1
             child_segment = argument_segments[0]
 
             if child_segment.is_type("bracketed"):
                 start_bracket = child_segment.get_child("start_bracket")
                 # There will be a start bracket if it's bracketed.
                 assert start_bracket
                 if start_bracket.raw == "(":
                     bracketed_arguments = child_segment.get_children("column_reference")
-                    raw_arguments = [argument.raw for argument in bracketed_arguments]
+                    raw_arguments = [argument for argument in bracketed_arguments]
                     lambda_argument_columns += raw_arguments
 
             elif child_segment.is_type("column_reference"):
-                lambda_argument_columns.append(child_segment.raw)
+                lambda_argument_columns.append(child_segment)
 
     return lambda_argument_columns
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/__init__.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/context.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/context.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slice_predicates.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/raw_file_slices.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/raw_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/segment_predicates.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/segment_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/segments.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/segments.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slice_predicates.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slice_predicates.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/functional/templated_file_slices.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/functional/templated_file_slices.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/identifers.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/identifers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/config.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/config.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/depthmap.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/depthmap.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/elements.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/elements.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/helpers.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/rebreak.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/rebreak.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/reindent.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/reindent.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/respace.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/respace.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/reflow/sequence.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/reflow/sequence.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/testing/cli.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/testing/cli.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/testing/logging.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/testing/logging.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff/utils/testing/rules.py` & `sqlfluff-3.0.5/src/sqlfluff/utils/testing/rules.py`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff.egg-info/PKG-INFO` & `sqlfluff-3.0.5/src/sqlfluff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlfluff
-Version: 3.0.4
+Version: 3.0.5
 Summary: The SQL Linter for Humans
 Author-email: Alan Cruickshank <alan@designingoverload.com>
 License: MIT License
         
         Copyright (c) 2023 Alan Cruickshank
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sqlfluff-3.0.4/src/sqlfluff.egg-info/SOURCES.txt` & `sqlfluff-3.0.5/src/sqlfluff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/src/sqlfluff.egg-info/entry_points.txt` & `sqlfluff-3.0.5/src/sqlfluff.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `sqlfluff-3.0.4/test/testing_test.py` & `sqlfluff-3.0.5/test/testing_test.py`

 * *Files identical despite different names*

