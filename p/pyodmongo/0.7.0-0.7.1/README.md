# Comparing `tmp/pyodmongo-0.7.0.tar.gz` & `tmp/pyodmongo-0.7.1.tar.gz`

## Comparing `pyodmongo-0.7.0.tar` & `pyodmongo-0.7.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/code_of_conduct.md
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/coverage.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyproject.py
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/requirements.txt
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/black_formatter.yml
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/publishing_docs_s3.yml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/python_publish.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/insomnia_request.png
--rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/logo.png
--rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png
--rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_White.png
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/aggregation.md
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/contributing.md
--rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/db_model.md
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/delete.md
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/fastapi.md
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/find.md
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/getting_started.md
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/index.md
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/indexes.md
--rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/query.md
--rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/en/save.md
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/aggregation.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/contributing.md
--rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/db_model.md
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/delete.md
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/fastapi.md
--rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/find.md
--rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/getting_started.md
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/index.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/indexes.md
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/query.md
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/pt-BR/save.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/docs/stylesheets/extras.css
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/version.py
--rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/async_engine/engine.py
--rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/engine/engine.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/engine/utils.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/db_field_info.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/db_model.py
--rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/fields.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/id_model.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/paginate.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/query_operators.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/models/responses.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/__init__.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/comparison_operators.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/logical_operators.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/query_string.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/queries/sort_operator.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/aggregate_stages.py
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/model_init.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyodmongo/services/query_operators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_async_aggregate.py
--rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_async_crud_db.py
--rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_class.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_db_field_info.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_db_index.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_dict_empty.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_fastapi.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_model_init_functions.py
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_object_id.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_project_pipeline.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_pydantic_validators.py
--rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_queries.py
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_reference_pipeline.py
--rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_save_dict.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_sync_aggregate.py
--rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_sync_crud_db.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/tests/test_version.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/LICENSE
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/README.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4976 2020-02-02 00:00:00.000000 pyodmongo-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/code_of_conduct.md
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/coverage.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/mkdocs.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyproject.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/requirements.txt
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/workflows/black_formatter.yml
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/workflows/publishing_docs_s3.yml
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/workflows/python_publish.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0    56292 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    94192 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/assets/images/insomnia_request.png
+-rw-r--r--   0        0        0    57259 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/assets/images/logo.png
+-rw-r--r--   0        0        0    70935 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png
+-rw-r--r--   0        0        0    72399 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/assets/images/pyodmongo_Logo_BG_White.png
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/aggregation.md
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/contributing.md
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/db_model.md
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/delete.md
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/fastapi.md
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/find.md
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/getting_started.md
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/index.md
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/indexes.md
+-rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/query.md
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/en/save.md
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/aggregation.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/contributing.md
+-rw-r--r--   0        0        0     5121 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/db_model.md
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/delete.md
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/fastapi.md
+-rw-r--r--   0        0        0     7543 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/find.md
+-rw-r--r--   0        0        0     5379 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/getting_started.md
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/index.md
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/indexes.md
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/query.md
+-rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/pt-BR/save.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/docs/stylesheets/extras.css
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/version.py
+-rw-r--r--   0        0        0     9674 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/async_engine/engine.py
+-rw-r--r--   0        0        0     9399 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/engine/engine.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/engine/utils.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/db_field_info.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/db_model.py
+-rw-r--r--   0        0        0     9486 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/fields.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/id_model.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/paginate.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/query_operators.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/models/responses.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/queries/__init__.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/queries/comparison_operators.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/queries/logical_operators.py
+-rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/queries/query_string.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/queries/sort_operator.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/services/aggregate_stages.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/services/model_init.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyodmongo/services/query_operators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_async_aggregate.py
+-rw-r--r--   0        0        0    18182 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_async_crud_db.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_class.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_db_field_info.py
+-rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_db_index.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_dict_empty.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_fastapi.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_model_init_functions.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_object_id.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_project_pipeline.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_pydantic_validators.py
+-rw-r--r--   0        0        0     9990 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_queries.py
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_reference_pipeline.py
+-rw-r--r--   0        0        0     8320 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_save_dict.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_sync_aggregate.py
+-rw-r--r--   0        0        0    12269 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_sync_crud_db.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/tests/test_version.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 pyodmongo-0.7.1/PKG-INFO
```

### Comparing `pyodmongo-0.7.0/code_of_conduct.md` & `pyodmongo-0.7.1/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/mkdocs.yml` & `pyodmongo-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyproject.py` & `pyodmongo-0.7.1/pyproject.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/requirements.txt` & `pyodmongo-0.7.1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,17 +41,16 @@
 paginate==0.5.6
 pathspec==0.11.2
 Pillow==10.0.1
 platformdirs==3.10.0
 pluggy==1.3.0
 pycodestyle==2.11.0
 pycparser==2.21
-pydantic==2.6.4
-pydantic-dbmodel-core==0.0.3
-pydantic_core==2.16.3
+pydantic==2.7.0
+pydantic_core==2.18.1
 pyflakes==3.1.0
 Pygments==2.16.1
 pylint==2.17.6
 pymdown-extensions==10.3
 pymongo==4.5.0
 pytest==7.4.1
 pytest-asyncio==0.21.1
```

### Comparing `pyodmongo-0.7.0/.github/ISSUE_TEMPLATE/bug.yml` & `pyodmongo-0.7.1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/.github/workflows/black_formatter.yml` & `pyodmongo-0.7.1/.github/workflows/black_formatter.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/.github/workflows/publishing_docs_s3.yml` & `pyodmongo-0.7.1/.github/workflows/publishing_docs_s3.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/.github/workflows/python_publish.yml` & `pyodmongo-0.7.1/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/.github/workflows/tests.yml` & `pyodmongo-0.7.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/assets/images/favicon.png` & `pyodmongo-0.7.1/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/assets/images/insomnia_request.png` & `pyodmongo-0.7.1/docs/assets/images/insomnia_request.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/assets/images/logo.png` & `pyodmongo-0.7.1/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_Dark.png` & `pyodmongo-0.7.1/docs/assets/images/pyodmongo_Logo_BG_Dark.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/assets/images/pyodmongo_Logo_BG_White.png` & `pyodmongo-0.7.1/docs/assets/images/pyodmongo_Logo_BG_White.png`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/aggregation.md` & `pyodmongo-0.7.1/docs/en/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/contributing.md` & `pyodmongo-0.7.1/docs/en/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/db_model.md` & `pyodmongo-0.7.1/docs/en/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/delete.md` & `pyodmongo-0.7.1/docs/en/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/fastapi.md` & `pyodmongo-0.7.1/docs/en/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/find.md` & `pyodmongo-0.7.1/docs/en/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/getting_started.md` & `pyodmongo-0.7.1/docs/en/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/index.md` & `pyodmongo-0.7.1/docs/en/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/indexes.md` & `pyodmongo-0.7.1/docs/en/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/query.md` & `pyodmongo-0.7.1/docs/en/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/en/save.md` & `pyodmongo-0.7.1/docs/en/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/aggregation.md` & `pyodmongo-0.7.1/docs/pt-BR/aggregation.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/contributing.md` & `pyodmongo-0.7.1/docs/pt-BR/contributing.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/db_model.md` & `pyodmongo-0.7.1/docs/pt-BR/db_model.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/delete.md` & `pyodmongo-0.7.1/docs/pt-BR/delete.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/fastapi.md` & `pyodmongo-0.7.1/docs/pt-BR/fastapi.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/find.md` & `pyodmongo-0.7.1/docs/pt-BR/find.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/getting_started.md` & `pyodmongo-0.7.1/docs/pt-BR/getting_started.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/index.md` & `pyodmongo-0.7.1/docs/pt-BR/index.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/indexes.md` & `pyodmongo-0.7.1/docs/pt-BR/indexes.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/query.md` & `pyodmongo-0.7.1/docs/pt-BR/query.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/docs/pt-BR/save.md` & `pyodmongo-0.7.1/docs/pt-BR/save.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/async_engine/engine.py` & `pyodmongo-0.7.1/pyodmongo/async_engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/engine/engine.py` & `pyodmongo-0.7.1/pyodmongo/engine/engine.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/engine/utils.py` & `pyodmongo-0.7.1/pyodmongo/engine/utils.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/models/db_model.py` & `pyodmongo-0.7.1/pyodmongo/models/db_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,60 @@
 from pydantic import ConfigDict
-from pydantic_dbmodel_core import DbModelCore
 from .id_model import Id
 from datetime import datetime
 from typing import ClassVar
 from ..services.model_init import (
     resolve_indexes,
     resolve_class_fields_db_info,
     resolve_reference_pipeline,
 )
+from pydantic import BaseModel
+from pydantic._internal._model_construction import ModelMetaclass
+from abc import ABCMeta
+from typing_extensions import dataclass_transform
+from typing import ClassVar
+
+
+class PyOdmongoMeta(ABCMeta):
+    def __getattr__(cls, name: str):
+        if cls.__dict__.get("pyodmongo_complete"):
+            is_attr = name in cls.__dict__["model_fields"].keys()
+            if is_attr:
+                return cls.__dict__.get(name + "__pyodmongo")
+        ModelMetaclass.__getattr__(cls, name)
 
 
-class DbModel(DbModelCore):
+@dataclass_transform()
+class DbMeta(PyOdmongoMeta, ModelMetaclass): ...
+
+
+class DbModel(BaseModel, metaclass=DbMeta):
     id: Id | None = None
     created_at: datetime | None = None
     updated_at: datetime | None = None
     model_config = ConfigDict(populate_by_name=True)
     _pipeline: ClassVar = []
 
+    @classmethod
+    def __init_subclass__(cls):
+        setattr(cls, "pyodmongo_complete", False)
+        for base in cls.__bases__:
+            setattr(base, "pyodmongo_complete", False)
+
+    @classmethod
+    def __pydantic_init_subclass__(cls):
+        setattr(cls, "pyodmongo_complete", True)
+        for base in cls.__bases__:
+            setattr(base, "pyodmongo_complete", True)
+        resolve_class_fields_db_info(cls=cls)
+        pipeline = resolve_reference_pipeline(cls=cls, pipeline=[])
+        setattr(cls, "_reference_pipeline", pipeline)
+        indexes = resolve_indexes(cls=cls)
+        setattr(cls, "_init_indexes", indexes)
+
     def __remove_empty_dict(self, dct: dict):
         for key, value in dct.items():
             if value == {}:
                 dct[key] = None
             elif type(value) == dict:
                 self.__remove_empty_dict(dct=value)
                 is_full_empty = all(
@@ -36,15 +70,7 @@
     def __init__(self, **attrs):
         for key, value in attrs.items():
             if type(value) == dict:
                 attrs[key] = self.__remove_empty_dict(dct=value)
         if attrs.get("_id") is not None:
             attrs["id"] = attrs.pop("_id")
         super().__init__(**attrs)
-
-    @classmethod
-    def __pydantic_init_subclass__(cls):
-        resolve_class_fields_db_info(cls=cls)
-        pipeline = resolve_reference_pipeline(cls=cls, pipeline=[])
-        setattr(cls, "_reference_pipeline", pipeline)
-        indexes = resolve_indexes(cls=cls)
-        setattr(cls, "_init_indexes", indexes)
```

### Comparing `pyodmongo-0.7.0/pyodmongo/models/fields.py` & `pyodmongo-0.7.1/pyodmongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/models/id_model.py` & `pyodmongo-0.7.1/pyodmongo/models/id_model.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/queries/comparison_operators.py` & `pyodmongo-0.7.1/pyodmongo/queries/comparison_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/queries/logical_operators.py` & `pyodmongo-0.7.1/pyodmongo/queries/logical_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/queries/query_string.py` & `pyodmongo-0.7.1/pyodmongo/queries/query_string.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/services/aggregate_stages.py` & `pyodmongo-0.7.1/pyodmongo/services/aggregate_stages.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyodmongo/services/model_init.py` & `pyodmongo-0.7.1/pyodmongo/services/model_init.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,8 +183,8 @@
     for field, field_info in cls.model_fields.items():
         db_field_info = field_annotation_infos(field=field, field_info=field_info)
         path = db_field_info.field_alias
         db_field_info.path_str = path
         field_to_set = _recursice_db_fields_info(
             db_field_info=db_field_info, path=[path]
         )
-        setattr(cls, field, field_to_set)
+        setattr(cls, field + "__pyodmongo", field_to_set)
```

### Comparing `pyodmongo-0.7.0/pyodmongo/services/query_operators.py` & `pyodmongo-0.7.1/pyodmongo/services/query_operators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_async_aggregate.py` & `pyodmongo-0.7.1/tests/test_async_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_async_crud_db.py` & `pyodmongo-0.7.1/tests/test_async_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_class.py` & `pyodmongo-0.7.1/tests/test_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,7 +163,25 @@
 def test_field_with_email_str():
     class MyClass(DbModel):
         attr_1: str
         email: EmailStr
 
     with pytest.raises(ValidationError):
         obj = MyClass(attr_1="Value one", email="shunda")
+
+
+def test_polymorphism():
+    class FirstClass(DbModel):
+        attr_1: str = "one"
+        attr_2: int = 2
+
+    class SecondClass(FirstClass):
+        attr_1: int = 1
+        attr_3: int = 3
+
+    obj_1 = FirstClass()
+    obj_2 = SecondClass()
+
+    assert obj_1.attr_1 == "one"
+    assert type(obj_1.attr_1) is str
+    assert obj_2.attr_1 == 1
+    assert type(obj_2.attr_1) is int
```

### Comparing `pyodmongo-0.7.0/tests/test_db_field_info.py` & `pyodmongo-0.7.1/tests/test_db_field_info.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_db_index.py` & `pyodmongo-0.7.1/tests/test_db_index.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_dict_empty.py` & `pyodmongo-0.7.1/tests/test_dict_empty.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_fastapi.py` & `pyodmongo-0.7.1/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_model_init_functions.py` & `pyodmongo-0.7.1/tests/test_model_init_functions.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_object_id.py` & `pyodmongo-0.7.1/tests/test_object_id.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_project_pipeline.py` & `pyodmongo-0.7.1/tests/test_project_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_pydantic_validators.py` & `pyodmongo-0.7.1/tests/test_pydantic_validators.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_queries.py` & `pyodmongo-0.7.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_reference_pipeline.py` & `pyodmongo-0.7.1/tests/test_reference_pipeline.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_save_dict.py` & `pyodmongo-0.7.1/tests/test_save_dict.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_sync_aggregate.py` & `pyodmongo-0.7.1/tests/test_sync_aggregate.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/tests/test_sync_crud_db.py` & `pyodmongo-0.7.1/tests/test_sync_crud_db.py`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/.gitignore` & `pyodmongo-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/LICENSE` & `pyodmongo-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/README.md` & `pyodmongo-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyodmongo-0.7.0/pyproject.toml` & `pyodmongo-0.7.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyodmongo"
-version = "0.7.0"
+version = "0.7.1"
 license = "MIT"
 authors = [
   { name="Mauro André", email="eng.mauroandre@gmail.com" },
 ]
 description = "A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic"
 readme = "README.md"
 requires-python = ">=3.11"
@@ -17,14 +17,14 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Database",
     "Topic :: Database :: Database Engines/Servers"
 ]
 
 dependencies = [
-    "pydantic-dbmodel-core>=0.0.1,<0.2.0",
+    "pydantic>=2.0.0,<3.0.0",
     "motor>=3.2.0,<4.0.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/mauro-andre/pyodmongo"
 "Documentation" = "https://pyodmongo.dev"
```

### Comparing `pyodmongo-0.7.0/PKG-INFO` & `pyodmongo-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: pyodmongo
-Version: 0.7.0
+Version: 0.7.1
 Summary: A syncrounous and asyncrounous Python ODM for MongoDB based on Pydantic
 Project-URL: Homepage, https://github.com/mauro-andre/pyodmongo
 Project-URL: Documentation, https://pyodmongo.dev
 Author-email: Mauro André <eng.mauroandre@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Database :: Database Engines/Servers
 Requires-Python: >=3.11
 Requires-Dist: motor<4.0.0,>=3.2.0
-Requires-Dist: pydantic-dbmodel-core<0.2.0,>=0.0.1
+Requires-Dist: pydantic<3.0.0,>=2.0.0
 Description-Content-Type: text/markdown
 
 
 <div align="center">
     <a href="https://pyodmongo.dev" target="_blank">
       <img src="https://raw.githubusercontent.com/mauro-andre/pyodmongo/master/docs/assets/images/pyodmongo_Logo_BG_White.png" alt="coverage">
     </a>
```

