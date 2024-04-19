# Comparing `tmp/pytest_databases-0.4.0.tar.gz` & `tmp/pytest_databases-0.4.1.tar.gz`

## Comparing `pytest_databases-0.4.0.tar` & `pytest_databases-0.4.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/CODEOWNERS
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/Makefile
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/sonar-project.properties
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.vscode/launch.json
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/alloydb_omni.py
--rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/bigquery.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.bigquery.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.keydb.yml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mariadb.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mssql.yml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mysql.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.oracle.yml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.postgres.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.redis.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.spanner.yml
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/elastic_search.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_alloydb_omni.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_bigquery.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_elasticsearch.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/LICENSE
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/README.md
--rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/CODEOWNERS
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/Makefile
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/sonar-project.properties
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.vscode/launch.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.vscode/settings.json
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/alloydb_omni.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/bigquery.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.bigquery.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.cockroachdb.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.dragonfly.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.keydb.yml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mariadb.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mssql.yml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.oracle.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.postgres.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.redis.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.spanner.yml
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/elastic_search.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_alloydb_omni.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_bigquery.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_elasticsearch.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/LICENSE
+-rw-r--r--   0        0        0    11163 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/README.md
+-rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 pytest_databases-0.4.1/PKG-INFO
```

### Comparing `pytest_databases-0.4.0/.pre-commit-config.yaml` & `pytest_databases-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/.sourcery.yaml` & `pytest_databases-0.4.1/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/CONTRIBUTING.rst` & `pytest_databases-0.4.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/Makefile` & `pytest_databases-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/.vscode/settings.json` & `pytest_databases-0.4.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/requirements/requirements-dev.txt` & `pytest_databases-0.4.1/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/requirements/requirements-docs.txt` & `pytest_databases-0.4.1/requirements/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/scripts/__init__.py` & `pytest_databases-0.4.1/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/scripts/build_docs.py` & `pytest_databases-0.4.1/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/__init__.py` & `pytest_databases-0.4.1/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/__metadata__.py` & `pytest_databases-0.4.1/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/helpers.py` & `pytest_databases-0.4.1/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/alloydb_omni.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/bigquery.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/bigquery.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.bigquery.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.bigquery.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.dragonfly.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.dragonfly.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mysql.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.oracle.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.oracle.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.postgres.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.postgres.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.spanner.yml` & `pytest_databases-0.4.1/src/pytest_databases/docker/docker-compose.spanner.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/elastic_search.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/elastic_search.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/redis.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.4.1/src/pytest_databases/docker/spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/__init__.py` & `pytest_databases-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/conftest.py` & `pytest_databases-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/__init__.py` & `pytest_databases-0.4.1/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_alloydb_omni.py` & `pytest_databases-0.4.1/tests/docker/test_alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_bigquery.py` & `pytest_databases-0.4.1/tests/docker/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_cockroachdb.py` & `pytest_databases-0.4.1/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_dragonfly.py` & `pytest_databases-0.4.1/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_elasticsearch.py` & `pytest_databases-0.4.1/tests/docker/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_keydb.py` & `pytest_databases-0.4.1/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_mariadb.py` & `pytest_databases-0.4.1/tests/docker/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_mssql.py` & `pytest_databases-0.4.1/tests/docker/test_mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_mysql.py` & `pytest_databases-0.4.1/tests/docker/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_oracle.py` & `pytest_databases-0.4.1/tests/docker/test_oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_postgres.py` & `pytest_databases-0.4.1/tests/docker/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_redis.py` & `pytest_databases-0.4.1/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/tests/docker/test_spanner.py` & `pytest_databases-0.4.1/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/.gitignore` & `pytest_databases-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/LICENSE` & `pytest_databases-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.4.0/README.md` & `pytest_databases-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
+| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
+| Community |     | [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
 
 > [!WARNING]
 >
```

### Comparing `pytest_databases-0.4.0/pyproject.toml` & `pytest_databases-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.4.0"
+version = "0.4.1"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
```

### Comparing `pytest_databases-0.4.0/PKG-INFO` & `pytest_databases-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.4.0
+Version: 0.4.1
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -55,17 +55,17 @@
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
-| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
+| Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest-databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest-databases)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
+| Community |     | [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
 
 > [!WARNING]
 >
```

