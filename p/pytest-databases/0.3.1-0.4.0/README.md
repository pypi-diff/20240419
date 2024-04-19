# Comparing `tmp/pytest_databases-0.3.1.tar.gz` & `tmp/pytest_databases-0.4.0.tar.gz`

## Comparing `pytest_databases-0.3.1.tar` & `pytest_databases-0.4.0.tar`

### file list

```diff
@@ -1,62 +1,66 @@
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/.sourcery.yaml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/CODEOWNERS
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/Makefile
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/sonar-project.properties
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/.vscode/settings.json
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/requirements/requirements-dev.txt
--rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/requirements/requirements-docs.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/requirements/requirements.txt
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/scripts/__init__.py
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/scripts/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/scripts/convert_docs.sh
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/__metadata__.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/py.typed
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/__init__.py
--rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/alloydb_omni.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/cockroachdb.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.cockroachdb.yml
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.dragonfly.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.keydb.yml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.mariadb.yml
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.mssql.yml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.mysql.yml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.oracle.yml
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.postgres.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.redis.yml
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.spanner.yml
--rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/dragonfly.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/elastic_search.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/keydb.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/mariadb.py
--rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/mssql.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/mysql.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/oracle.py
--rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/postgres.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/redis.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/src/pytest_databases/docker/spanner.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/conftest.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/__init__.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_alloydb_omni.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_cockroachdb.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_dragonfly.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_elasticsearch.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_keydb.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_mariadb.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_mssql.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_mysql.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_oracle.py
--rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_postgres.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_redis.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/tests/docker/test_spanner.py
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/LICENSE
--rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/README.md
--rw-r--r--   0        0        0    17357 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    13325 2020-02-02 00:00:00.000000 pytest_databases-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.sourcery.yaml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/CODEOWNERS
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/Makefile
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/sonar-project.properties
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.vscode/launch.json
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.vscode/settings.json
+-rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0     8544 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements-docs.txt
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/requirements/requirements.txt
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/__init__.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/scripts/convert_docs.sh
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/__metadata__.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/py.typed
+-rw-r--r--   0        0        0     5252 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/__init__.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/alloydb_omni.py
+-rw-r--r--   0        0        0     4067 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/bigquery.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/cockroachdb.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.bigquery.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.cockroachdb.yml
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.dragonfly.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.keydb.yml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mariadb.yml
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mssql.yml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mysql.yml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.oracle.yml
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.postgres.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.redis.yml
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.spanner.yml
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/dragonfly.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/elastic_search.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/keydb.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mariadb.py
+-rw-r--r--   0        0        0     4248 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mssql.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/mysql.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/oracle.py
+-rw-r--r--   0        0        0     7643 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/postgres.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/redis.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/src/pytest_databases/docker/spanner.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/__init__.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_alloydb_omni.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_bigquery.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_cockroachdb.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_dragonfly.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_elasticsearch.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_keydb.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mariadb.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mssql.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_mysql.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_oracle.py
+-rw-r--r--   0        0        0     6013 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_postgres.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_redis.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/tests/docker/test_spanner.py
+-rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/LICENSE
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/README.md
+-rw-r--r--   0        0        0    17832 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 pytest_databases-0.4.0/PKG-INFO
```

### Comparing `pytest_databases-0.3.1/.pre-commit-config.yaml` & `pytest_databases-0.4.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: ["--fix=auto"] # replace 'auto' with 'lf' to enforce Linux/Mac line endings or 'crlf' for Windows
 
   # Ruff replaces black, flake8, autoflake and isort
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.3.7" # make sure this is always consistent with hatch configs
+    rev: "v0.4.0" # make sure this is always consistent with hatch configs
     hooks:
       - id: ruff
         args: [--config, ./pyproject.toml]
 
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v4.0.0-alpha.8
     hooks:
```

### Comparing `pytest_databases-0.3.1/.sourcery.yaml` & `pytest_databases-0.4.0/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/CONTRIBUTING.rst` & `pytest_databases-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/Makefile` & `pytest_databases-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/.vscode/settings.json` & `pytest_databases-0.4.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/requirements/requirements-dev.txt` & `pytest_databases-0.4.0/requirements/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #
 # This file is autogenerated by hatch-pip-compile with Python 3.11
 #
-# [constraints] requirements/requirements-docs.txt (SHA256: bc66ec3f548a65764214d7adf74c74992465c90498f84a07b19b829ae70e0bfb)
+# [constraints] requirements/requirements-docs.txt (SHA256: a093b9560889a29cbc3c8aa0b34a88712507f753d6e17b1f14300bb5327d479e)
 #
 # - nodeenv
 # - cython
 # - anyio
 # - coverage[toml]>=6.2
 # - pytest
 # - pytest-cov
@@ -34,14 +34,15 @@
 # - types-six
 # - types-decorator
 # - types-pyyaml
 # - asyncpg-stubs
 # - types-docutils
 # - types-redis
 # - pytest
+# - google-cloud-bigquery
 # - psycopg
 # - elasticsearch7[async]
 # - elasticsearch8[async]
 # - aioodbc
 # - asyncmy>=0.2.9
 # - oracledb
 # - asyncpg>=0.29.0
@@ -120,16 +121,14 @@
     # via
     #   oracledb
     #   types-pyopenssl
     #   types-redis
 cssutils==2.10.2
     # via dict2css
 cython==3.0.10
-deprecated==1.2.14
-    # via google-cloud-spanner
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 dill==0.3.8
     # via pylint
 distlib==0.3.8
     # via virtualenv
 docutils==0.21.1
@@ -146,55 +145,64 @@
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 duckdb==0.10.2
     # via harlequin
 elastic-transport==8.13.0
     # via elasticsearch8
-elasticsearch7==7.9.1
+elasticsearch7==7.17.9
 elasticsearch8==8.13.0
 execnet==2.1.1
     # via pytest-xdist
 filelock==3.13.4
     # via
     #   cachecontrol
     #   sphinx-toolbox
     #   virtualenv
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 google-api-core==2.18.0
     # via
+    #   google-cloud-bigquery
     #   google-cloud-core
     #   google-cloud-spanner
 google-auth==2.29.0
     # via
     #   google-api-core
+    #   google-cloud-bigquery
     #   google-cloud-core
+google-cloud-bigquery==3.21.0
 google-cloud-core==2.4.1
-    # via google-cloud-spanner
-google-cloud-spanner==3.44.0
+    # via
+    #   google-cloud-bigquery
+    #   google-cloud-spanner
+google-cloud-spanner==3.45.0
+google-crc32c==1.5.0
+    # via google-resumable-media
+google-resumable-media==2.7.0
+    # via google-cloud-bigquery
 googleapis-common-protos==1.63.0
     # via
     #   google-api-core
     #   grpc-google-iam-v1
     #   grpcio-status
 grpc-google-iam-v1==0.13.0
     # via google-cloud-spanner
 grpc-interceptor==0.15.4
     # via google-cloud-spanner
-grpcio==1.62.1
+grpcio==1.62.2
     # via
     #   google-api-core
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpc-interceptor
     #   grpcio-status
-grpcio-status==1.62.1
+grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via uvicorn
 harlequin==1.17.0
 html5lib==1.1
     # via sphinx-toolbox
 identify==2.5.35
@@ -250,14 +258,15 @@
 numpy==1.26.4
     # via
     #   harlequin
     #   pyarrow
 oracledb==2.1.2
 packaging==24.0
     # via
+    #   google-cloud-bigquery
     #   pydata-sphinx-theme
     #   pytest
     #   pytest-sugar
     #   sphinx
 platformdirs==4.2.0
     # via
     #   apeye
@@ -318,47 +327,52 @@
     #   pytest-xdist
 pytest-click==1.1.0
 pytest-cov==5.0.0
 pytest-mock==3.14.0
 pytest-sugar==1.0.0
 pytest-vcr==1.0.2
 pytest-xdist==3.5.0
+python-dateutil==2.9.0.post0
+    # via google-cloud-bigquery
 pyyaml==6.0.1
     # via
     #   pre-commit
     #   vcrpy
 questionary==2.0.1
     # via harlequin
 redis==5.0.3
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   google-api-core
+    #   google-cloud-bigquery
     #   sphinx
 rich==13.7.1
     # via
     #   rich-click
     #   textual
 rich-click==1.7.4
     # via harlequin
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.3.7
+ruff==0.4.0
     # via auto-pytabs
 setuptools==69.5.1
     # via nodeenv
 shandy-sqlfmt==0.21.2
     # via harlequin
 six==1.16.0
-    # via html5lib
+    # via
+    #   html5lib
+    #   python-dateutil
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.3.6
@@ -452,15 +466,15 @@
     #   psycopg
     #   pydata-sphinx-theme
     #   rich-click
     #   sphinx-toolbox
     #   textual
 uc-micro-py==1.0.3
     # via linkify-it-py
-urllib3==2.2.1
+urllib3==1.26.18
     # via
     #   elastic-transport
     #   elasticsearch7
     #   requests
 uvicorn==0.29.0
     # via sphinx-autobuild
 vcrpy==6.0.1
@@ -472,15 +486,12 @@
 wcwidth==0.2.13
     # via prompt-toolkit
 webencodings==0.5.1
     # via html5lib
 websockets==12.0
     # via sphinx-autobuild
 wrapt==1.16.0
-    # via
-    #   deprecated
-    #   vcrpy
+    # via vcrpy
 yarl==1.9.4
     # via
     #   aiohttp
-    #   elasticsearch7
     #   vcrpy
```

### Comparing `pytest_databases-0.3.1/requirements/requirements-docs.txt` & `pytest_databases-0.4.0/requirements/requirements-docs.txt`

 * *Files 21% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # - litestar-sphinx-theme@ git+https://github.com/litestar-org/litestar-sphinx-theme.git
 # - sphinx-click>=5.0.1
 # - sphinx-toolbox>=3.5.0
 # - sphinx-design>=0.5.0
 # - sphinxcontrib-mermaid>=0.9.2
 # - auto-pytabs[sphinx]>=0.4.0
 # - pytest
+# - google-cloud-bigquery
 # - psycopg
 # - elasticsearch7[async]
 # - elasticsearch8[async]
 # - aioodbc
 # - asyncmy>=0.2.9
 # - oracledb
 # - asyncpg>=0.29.0
@@ -38,33 +39,38 @@
 accessible-pygments==0.0.4
     # via pydata-sphinx-theme
 aiohttp==3.9.5
     # via
     #   elasticsearch7
     #   elasticsearch8
 aioodbc==0.5.0
+    # via hatch.envs.docs
 aiosignal==1.3.1
     # via aiohttp
 alabaster==0.7.16
     # via sphinx
 anyio==4.3.0
     # via
+    #   hatch.envs.docs
     #   starlette
     #   watchfiles
 apeye==1.4.1
     # via sphinx-toolbox
 apeye-core==1.1.5
     # via apeye
 async-timeout==4.0.3
     # via asyncpg
 asyncmy==0.2.9
+    # via hatch.envs.docs
 asyncpg==0.29.0
+    # via hatch.envs.docs
 attrs==23.2.0
     # via aiohttp
 auto-pytabs==0.4.0
+    # via hatch.envs.docs
 autodocsumm==0.2.12
     # via sphinx-toolbox
 babel==2.14.0
     # via
     #   pydata-sphinx-theme
     #   sphinx
 beautifulsoup4==4.12.3
@@ -88,22 +94,23 @@
     # via
     #   pytest-click
     #   sphinx-click
     #   uvicorn
 colorama==0.4.6
     # via sphinx-autobuild
 coverage==7.4.4
-    # via pytest-cov
+    # via
+    #   hatch.envs.docs
+    #   pytest-cov
 cryptography==42.0.5
     # via oracledb
 cssutils==2.10.2
     # via dict2css
 cython==3.0.10
-deprecated==1.2.14
-    # via google-cloud-spanner
+    # via hatch.envs.docs
 dict2css==0.3.0.post1
     # via sphinx-toolbox
 docutils==0.21.1
     # via
     #   pydata-sphinx-theme
     #   sphinx
     #   sphinx-click
@@ -114,111 +121,134 @@
     # via
     #   apeye
     #   apeye-core
     #   dict2css
     #   sphinx-toolbox
 elastic-transport==8.13.0
     # via elasticsearch8
-elasticsearch7==7.9.1
+elasticsearch7==7.17.9
+    # via hatch.envs.docs
 elasticsearch8==8.13.0
+    # via hatch.envs.docs
 execnet==2.1.1
     # via pytest-xdist
 filelock==3.13.4
     # via
     #   cachecontrol
     #   sphinx-toolbox
 frozenlist==1.4.1
     # via
     #   aiohttp
     #   aiosignal
 google-api-core==2.18.0
     # via
+    #   google-cloud-bigquery
     #   google-cloud-core
     #   google-cloud-spanner
 google-auth==2.29.0
     # via
     #   google-api-core
+    #   google-cloud-bigquery
     #   google-cloud-core
+google-cloud-bigquery==3.21.0
+    # via hatch.envs.docs
 google-cloud-core==2.4.1
-    # via google-cloud-spanner
-google-cloud-spanner==3.44.0
+    # via
+    #   google-cloud-bigquery
+    #   google-cloud-spanner
+google-cloud-spanner==3.45.0
+    # via hatch.envs.docs
+google-crc32c==1.5.0
+    # via google-resumable-media
+google-resumable-media==2.7.0
+    # via google-cloud-bigquery
 googleapis-common-protos==1.63.0
     # via
     #   google-api-core
     #   grpc-google-iam-v1
     #   grpcio-status
 grpc-google-iam-v1==0.13.0
     # via google-cloud-spanner
 grpc-interceptor==0.15.4
     # via google-cloud-spanner
-grpcio==1.62.1
+grpcio==1.62.2
     # via
     #   google-api-core
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpc-interceptor
     #   grpcio-status
-grpcio-status==1.62.1
+grpcio-status==1.62.2
     # via google-api-core
 h11==0.14.0
     # via uvicorn
 html5lib==1.1
     # via sphinx-toolbox
 idna==3.7
     # via
     #   anyio
     #   apeye-core
     #   requests
     #   yarl
 imagesize==1.4.1
     # via sphinx
 iniconfig==2.0.0
-    # via pytest
+    # via
+    #   -c requirements/requirements.txt
+    #   pytest
 jinja2==3.1.3
     # via
     #   sphinx
     #   sphinx-jinja2-compat
-litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git@c5ce66aadc8f910c24f54bf0d172798c237a67eb
+litestar-sphinx-theme @ git+https://github.com/litestar-org/litestar-sphinx-theme.git
+    # via hatch.envs.docs
 markupsafe==2.1.5
     # via
     #   jinja2
     #   sphinx-jinja2-compat
 msgpack==1.0.8
     # via cachecontrol
 multidict==6.0.5
     # via
     #   aiohttp
     #   yarl
 natsort==8.4.0
     # via domdf-python-tools
 nodeenv==1.8.0
+    # via hatch.envs.docs
 oracledb==2.1.2
+    # via hatch.envs.docs
 packaging==24.0
     # via
+    #   -c requirements/requirements.txt
+    #   google-cloud-bigquery
     #   pydata-sphinx-theme
     #   pytest
     #   pytest-sugar
     #   sphinx
 platformdirs==4.2.0
     # via apeye
 pluggy==1.4.0
-    # via pytest
+    # via
+    #   -c requirements/requirements.txt
+    #   pytest
 proto-plus==1.23.0
     # via
     #   google-api-core
     #   google-cloud-spanner
 protobuf==4.25.3
     # via
     #   google-api-core
     #   google-cloud-spanner
     #   googleapis-common-protos
     #   grpc-google-iam-v1
     #   grpcio-status
     #   proto-plus
 psycopg==3.1.18
+    # via hatch.envs.docs
 pyasn1==0.6.0
     # via
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.4.0
     # via google-auth
 pycparser==2.22
@@ -232,89 +262,109 @@
     #   sphinx
     #   sphinx-prompt
     #   sphinx-tabs
 pyodbc==5.1.0
     # via aioodbc
 pytest==8.1.1
     # via
+    #   -c requirements/requirements.txt
+    #   hatch.envs.docs
     #   pytest-click
     #   pytest-cov
     #   pytest-mock
     #   pytest-sugar
     #   pytest-vcr
     #   pytest-xdist
 pytest-click==1.1.0
+    # via hatch.envs.docs
 pytest-cov==5.0.0
+    # via hatch.envs.docs
 pytest-mock==3.14.0
+    # via hatch.envs.docs
 pytest-sugar==1.0.0
+    # via hatch.envs.docs
 pytest-vcr==1.0.2
+    # via hatch.envs.docs
 pytest-xdist==3.5.0
+    # via hatch.envs.docs
+python-dateutil==2.9.0.post0
+    # via google-cloud-bigquery
 pyyaml==6.0.1
     # via vcrpy
 redis==5.0.3
+    # via hatch.envs.docs
 requests==2.31.0
     # via
     #   apeye
     #   cachecontrol
     #   google-api-core
+    #   google-cloud-bigquery
     #   sphinx
 rsa==4.9
     # via google-auth
 ruamel-yaml==0.18.6
     # via sphinx-toolbox
 ruamel-yaml-clib==0.2.8
     # via ruamel-yaml
-ruff==0.3.7
+ruff==0.4.0
     # via auto-pytabs
-setuptools==69.5.1
-    # via nodeenv
 six==1.16.0
-    # via html5lib
+    # via
+    #   html5lib
+    #   python-dateutil
 sniffio==1.3.1
     # via anyio
 snowballstemmer==2.2.0
     # via sphinx
 soupsieve==2.5
     # via beautifulsoup4
 sphinx==7.3.6
     # via
+    #   hatch.envs.docs
     #   auto-pytabs
     #   autodocsumm
     #   pydata-sphinx-theme
     #   sphinx-autobuild
     #   sphinx-autodoc-typehints
     #   sphinx-click
     #   sphinx-copybutton
     #   sphinx-design
     #   sphinx-prompt
     #   sphinx-tabs
     #   sphinx-toolbox
 sphinx-autobuild==2024.4.16
+    # via hatch.envs.docs
 sphinx-autodoc-typehints==2.1.0
     # via sphinx-toolbox
 sphinx-click==5.1.0
+    # via hatch.envs.docs
 sphinx-copybutton==0.5.2
+    # via hatch.envs.docs
 sphinx-design==0.5.0
-    # via litestar-sphinx-theme
+    # via
+    #   hatch.envs.docs
+    #   litestar-sphinx-theme
 sphinx-jinja2-compat==0.2.0.post1
     # via sphinx-toolbox
 sphinx-prompt==1.8.0
     # via sphinx-toolbox
 sphinx-tabs==3.4.5
     # via sphinx-toolbox
 sphinx-toolbox==3.5.0
+    # via hatch.envs.docs
 sphinxcontrib-applehelp==1.0.8
     # via sphinx
 sphinxcontrib-devhelp==1.0.6
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-mermaid==0.9.2
+    # via hatch.envs.docs
 sphinxcontrib-qthelp==1.0.7
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
 sqlparse==0.5.0
     # via google-cloud-spanner
 starlette==0.37.2
@@ -325,15 +375,15 @@
     # via pytest-sugar
 typing-extensions==4.11.0
     # via
     #   domdf-python-tools
     #   psycopg
     #   pydata-sphinx-theme
     #   sphinx-toolbox
-urllib3==2.2.1
+urllib3==1.26.18
     # via
     #   elastic-transport
     #   elasticsearch7
     #   requests
 uvicorn==0.29.0
     # via sphinx-autobuild
 vcrpy==6.0.1
@@ -341,15 +391,15 @@
 watchfiles==0.21.0
     # via sphinx-autobuild
 webencodings==0.5.1
     # via html5lib
 websockets==12.0
     # via sphinx-autobuild
 wrapt==1.16.0
-    # via
-    #   deprecated
-    #   vcrpy
+    # via vcrpy
 yarl==1.9.4
     # via
     #   aiohttp
-    #   elasticsearch7
     #   vcrpy
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `pytest_databases-0.3.1/scripts/__init__.py` & `pytest_databases-0.4.0/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/scripts/build_docs.py` & `pytest_databases-0.4.0/scripts/build_docs.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/__init__.py` & `pytest_databases-0.4.0/src/pytest_databases/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/__metadata__.py` & `pytest_databases-0.4.0/src/pytest_databases/__metadata__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/helpers.py` & `pytest_databases-0.4.0/src/pytest_databases/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/__init__.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,19 +121,19 @@
             timeout=timeout,
             pause=pause,
             host=self.docker_ip,
             **kwargs,
         )
 
     def stop(self, name: str) -> None:
-        self.run_command("down", "--remove-orphans", "--volumes", "-t", "10", name)
+        self.run_command("down", "--volumes", "-t", "10", name)
 
     def down(self) -> None:
         if not SKIP_DOCKER_COMPOSE:
-            self.run_command("down", "--remove-orphans", "--volumes", "-t", "10")
+            self.run_command("down", "-t", "10")
 
 
 @pytest.fixture(scope="session")
 def compose_project_name() -> str:
     return os.environ.get("COMPOSE_PROJECT_NAME", COMPOSE_PROJECT_NAME)
```

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/alloydb_omni.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/cockroachdb.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.alloydb-omni.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.alloydb-omni.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.dragonfly.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.dragonfly.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.elasticsearch.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.elasticsearch.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.mysql.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.mysql.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.oracle.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.oracle.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.postgres.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.postgres.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/docker-compose.spanner.yml` & `pytest_databases-0.4.0/src/pytest_databases/docker/docker-compose.spanner.yml`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/dragonfly.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/elastic_search.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/elastic_search.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/keydb.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/mariadb.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/mssql.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/mysql.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/oracle.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/postgres.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/redis.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/src/pytest_databases/docker/spanner.py` & `pytest_databases-0.4.0/src/pytest_databases/docker/spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/__init__.py` & `pytest_databases-0.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/conftest.py` & `pytest_databases-0.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/__init__.py` & `pytest_databases-0.4.0/tests/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_alloydb_omni.py` & `pytest_databases-0.4.0/tests/docker/test_alloydb_omni.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_cockroachdb.py` & `pytest_databases-0.4.0/tests/docker/test_cockroachdb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_dragonfly.py` & `pytest_databases-0.4.0/tests/docker/test_dragonfly.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_elasticsearch.py` & `pytest_databases-0.4.0/tests/docker/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_keydb.py` & `pytest_databases-0.4.0/tests/docker/test_keydb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_mariadb.py` & `pytest_databases-0.4.0/tests/docker/test_mariadb.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_mssql.py` & `pytest_databases-0.4.0/tests/docker/test_mssql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_mysql.py` & `pytest_databases-0.4.0/tests/docker/test_mysql.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_oracle.py` & `pytest_databases-0.4.0/tests/docker/test_oracle.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_postgres.py` & `pytest_databases-0.4.0/tests/docker/test_postgres.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_redis.py` & `pytest_databases-0.4.0/tests/docker/test_redis.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/tests/docker/test_spanner.py` & `pytest_databases-0.4.0/tests/docker/test_spanner.py`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/.gitignore` & `pytest_databases-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/LICENSE` & `pytest_databases-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_databases-0.3.1/README.md` & `pytest_databases-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# pytest-databases
+# Pytest Databases
 
 Reusable test fixtures for any and all databases.
 
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
@@ -34,14 +34,15 @@
 
 - **Postgres**: Version 12, 13, 14, 15, and 16 are available
 - **MySQL**: Version 5.6, 5.7 and 8 are available
 - **Oracle**: Version 18c XE and 23C Free are available
 - **SQL Server**: Version 2022 is available
 - **Google AlloyDB Omni**: Simplified Omni installation for easy testing.
 - **Google Spanner**: The latest cloud-emulator from Google is available
+- **Google BigQuery**: Unofficial BigQuery emulator
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
 
 ## Contributing
```

### Comparing `pytest_databases-0.3.1/pyproject.toml` & `pytest_databases-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [project]
 description = 'Reusable database fixtures for any and all databases.'
 license = "MIT"
 name = "pytest-databases"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.3.1"
+version = "0.4.0"
 #
 authors = [{ name = "Cody Fincher", email = "cody.fincher@gmail.com" }]
 keywords = [
   "database",
   "migration",
   "postgres",
   "mysql",
@@ -48,14 +48,15 @@
 
 [project.urls]
 Documentation = "https://github.com/litestar-org/pytest-databases#readme"
 Issues = "https://github.com/litestar-org/pytest-databases/issues"
 Source = "https://github.com/litestar-org/pytest-databases"
 
 [project.optional-dependencies]
+bigquery = ["google-cloud-bigquery"]
 cockroachdb = ["psycopg"]
 dragonfly = ["redis"]
 elasticsearch7 = ["elasticsearch7[async]"]
 elasticsearch8 = ["elasticsearch8[async]"]
 keydb = ["redis"]
 mssql = ["aioodbc"]
 mysql = ["asyncmy>=0.2.9"]
@@ -113,29 +114,30 @@
   "postgres",
   "spanner",
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
+  "bigquery",
 ]
 template = "default"
 type = "virtual"
 
 [tool.hatch.envs.test.env-vars]
-PYTHONPATH = "."
+PYTHONPATH = ".:src/"
 PYTHONUNBUFFERED = "1"
 SOURCE_DATE_EPOCH = "1580601600"
 
 # Test matrix for various Python versions replacing the functionality of tox
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 [tool.hatch.envs.test.scripts]
-cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov-report=xml"
+cov = "pytest --cov=pytest_databases --cov-report=xml"
 debug = "cov --no-cov -s --pdb --pdbcls=IPython.core.debugger:Pdb"
 no-cov = "cov --no-cov"
 
 
 # Docs environment
 [tool.hatch.envs.docs]
 extra-dependencies = [
@@ -170,14 +172,15 @@
   "postgres",
   "spanner",
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
+  "bigquery",
 ]
 lock-filename = "requirements/requirements-docs.txt"
 pip-compile-constraint = "default"
 python = "3.11"
 template = "test"
 type = "pip-compile"
 
@@ -241,14 +244,15 @@
   "mssql",
   "postgres",
   "cockroachdb",
   "spanner",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
+  "bigquery",
 ]
 lock-filename = "requirements/requirements-dev.txt"
 path = ".venv/"
 pip-compile-constraint = "docs"
 python = "3.11"
 template = "docs"
 type = "pip-compile"
@@ -279,14 +283,15 @@
   "mssql",
   "postgres",
   "spanner",
   "cockroachdb",
   "redis",
   "elasticsearch7",
   "elasticsearch8",
+  "bigquery",
 ]
 python = "3.11"
 template = "docs"
 
 [tool.hatch.envs.lint.scripts]
 check = ["style", "typing"]
 fix = [
@@ -388,25 +393,46 @@
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 warn_no_return = false
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
+disable_error_code = "attr-defined"
+module = "pytest_databases.docker.spanner"
+
+[[tool.mypy.overrides]]
+disable_error_code = "attr-defined"
+module = "pytest_databases.docker.bigquery"
+
+[[tool.mypy.overrides]]
+disable_error_code = "attr-defined"
 disallow_untyped_decorators = false
-module = ["tests.*"]
+module = "tests.*"
 warn_unused_ignores = false
 
 [[tool.mypy.overrides]]
 disable_error_code = ["arg-type"]
 disallow_untyped_calls = false
 disallow_untyped_decorators = false
 module = ["docutils.nodes.*"]
 
 
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = [
+  "asyncmy",
+  "pyodbc",
+  "google.auth.*",
+  "google.cloud.*",
+  "google.protobuf.*",
+  "googleapiclient",
+  "googleapiclient.*",
+]
+
 [tool.ruff]
 exclude = [
   ".bzr",
   ".direnv",
   ".eggs",
   ".git",
   ".hg",
@@ -470,20 +496,21 @@
   "ANN101",  # ruff - Missing type annotation for `self` in method
   "PLR0913", # ruff - Too many arguments to function call
   "PLR2004", # Magic value used in comparison
   "FBT001",  # Boolean typed positional argument in function definition
   "FBT002",  # Boolean default positional argument in function definition
   "FBT003",  # Boolean Boolean default positional argument in function definition
   "ARG002",  # Unused method argument
-  "ARG001",  #  Unused function argument
+  "ARG001",  # Unused function argument
   "TD002",
   "TD003",
   "FIX002",
   "PGH003",
   "RUF006",
+  "RUF029",  # Ruff - Function is declared `async`, but doesn't `await` or use `async` features. # ignore
   "SLF001",
   "PT007",
   'PT004',
   'PT005',
   'S603',
   "E501",    # pycodestyle line too long, handled by black
   "PLW2901", # pylint - for loop variable overwritten by assignment target
@@ -564,45 +591,38 @@
 '''
 include = '\.pyi?$'
 line-length = 120
 
 ## Testing Tools
 
 [tool.pytest.ini_options]
-addopts = "-ra -q --doctest-glob='*.md'"
+addopts = "--dist loadfile -n 2 -ra -q --doctest-glob='*.md'"
 filterwarnings = ["ignore::DeprecationWarning:pkg_resources", "ignore::DeprecationWarning:xdist.*"]
 markers = [
   "mysql: MySQL Tests",
   "postgres: Postgres Tests",
   "oracle: Oracle Tests",
   "spanner: Google Cloud Spanner Tests",
   "duckdb: DuckDB Tests",
   "mssql: Microsoft SQL Server Tests",
   "elasticsearch: Elasticsearch Tests",
 ]
-minversion = "6.0"
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
-concurrency = ["multiprocessing", "thread"]
-disable_warnings = ["no-data-collected", "module-not-measured"]
+concurrency = ["multiprocessing"]
+disable_warnings = ["no-data-collected", "module-not-measured", "module-not-imported"]
 omit = [
   "_version.py",                          # automatically created by hatch-vcs, not in repo
   "src/pytest_databases/__metadata__.py",
   "tests/*",
   "scripts/*",
 ]
 parallel = true
-source = ["src/pytest_databases"]
-source_pkgs = ["pytest_databases"]
-
-[tool.coverage.paths]
-pytest_databases = ["src/pytest_databases"]
-tests = ["tests"]
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_lines = [
   # Have to re-enable the standard pragma
   "pragma: no cover",
```

### Comparing `pytest_databases-0.3.1/PKG-INFO` & `pytest_databases-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-databases
-Version: 0.3.1
+Version: 0.4.0
 Summary: Reusable database fixtures for any and all databases.
 Project-URL: Documentation, https://github.com/litestar-org/pytest-databases#readme
 Project-URL: Issues, https://github.com/litestar-org/pytest-databases/issues
 Project-URL: Source, https://github.com/litestar-org/pytest-databases
 Author-email: Cody Fincher <cody.fincher@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: pytest
+Provides-Extra: bigquery
+Requires-Dist: google-cloud-bigquery; extra == 'bigquery'
 Provides-Extra: cockroachdb
 Requires-Dist: psycopg; extra == 'cockroachdb'
 Provides-Extra: dragonfly
 Requires-Dist: redis; extra == 'dragonfly'
 Provides-Extra: elasticsearch7
 Requires-Dist: elasticsearch7[async]; extra == 'elasticsearch7'
 Provides-Extra: elasticsearch8
@@ -42,25 +44,25 @@
 Requires-Dist: redis; extra == 'redis'
 Provides-Extra: spanner
 Requires-Dist: google-cloud-spanner; extra == 'spanner'
 Provides-Extra: sqlite
 Requires-Dist: aiosqlite; extra == 'sqlite'
 Description-Content-Type: text/markdown
 
-# pytest-databases
+# Pytest Databases
 
 Reusable test fixtures for any and all databases.
 
 <div align="center">
 
 <!-- prettier-ignore-start -->
 
 | Project   |     | Status                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
 |-----------|:----|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| CI/CD     |     | [![Latest Release](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/release.yaml) [![ci](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml/badge.svg)](https://github.com/litestar-org/pytest-databases/actions/workflows/ci.yaml) [![Documentation Building](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml/badge.svg?branch=main)](https://github.com/litestar-org/pytest-databases/actions/workflows/docs.yaml)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 | Quality   |     | [![Coverage](https://codecov.io/github/litestar-org/pytest-databases/graph/badge.svg?token=vKez4Pycrc)](https://codecov.io/github/litestar-org/pytest-databases) [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases) [![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=litestar-org_pytest_databases&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=litestar-org_pytest_databases)                                                                                                                                                                                                                                                                                                                               |
 | Package   |     | [![PyPI - Version](https://img.shields.io/pypi/v/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)](https://badge.fury.io/py/pytest-databases) ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pytest-databases?labelColor=202235&color=edb641&logo=python&logoColor=edb641)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 | Community |     | [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/litestarapi?label=r%2FLitestar&logo=reddit&labelColor=202235&color=edb641&logoColor=edb641)](https://reddit.com/r/litestarapi) [![Discord](https://img.shields.io/discord/919193495116337154?labelColor=202235&color=edb641&label=chat%20on%20discord&logo=discord&logoColor=edb641)](https://discord.gg/litestar-919193495116337154) [![Matrix](https://img.shields.io/badge/chat%20on%20Matrix-bridged-202235?labelColor=202235&color=edb641&logo=matrix&logoColor=edb641)](https://matrix.to/#/#litestar:matrix.org) [![Medium](https://img.shields.io/badge/Medium-202235?labelColor=202235&color=edb641&logo=medium&logoColor=edb641)](https://blog.litestar.dev) [![Twitter](https://img.shields.io/twitter/follow/LitestarAPI?labelColor=202235&color=edb641&logo=twitter&logoColor=edb641&style=flat)](https://twitter.com/LitestarAPI) [![Blog](https://img.shields.io/badge/Blog-litestar.dev-202235?logo=blogger&labelColor=202235&color=edb641&logoColor=edb641)](https://blog.litestar.dev)                                                                                                                                                                                                       |
 | Meta      |     | [![Litestar Project](https://img.shields.io/badge/Litestar%20Org-%E2%AD%90%20Litestar-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/litestar-org/pytest-databases) [![types - Mypy](https://img.shields.io/badge/types-Mypy-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://github.com/python/mypy) [![License - MIT](https://img.shields.io/badge/license-MIT-202235.svg?logo=python&labelColor=202235&color=edb641&logoColor=edb641)](https://spdx.org/licenses/) [![Litestar Sponsors](https://img.shields.io/badge/Sponsor-%E2%9D%A4-%23edb641.svg?&logo=github&logoColor=edb641&labelColor=202235)](https://github.com/sponsors/litestar-org) [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json&labelColor=202235)](https://github.com/astral-sh/ruff) [![code style - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/format.json&labelColor=202235)](https://github.com/psf/black)|
 
 <!-- prettier-ignore-end -->
 </div>
@@ -82,14 +84,15 @@
 
 - **Postgres**: Version 12, 13, 14, 15, and 16 are available
 - **MySQL**: Version 5.6, 5.7 and 8 are available
 - **Oracle**: Version 18c XE and 23C Free are available
 - **SQL Server**: Version 2022 is available
 - **Google AlloyDB Omni**: Simplified Omni installation for easy testing.
 - **Google Spanner**: The latest cloud-emulator from Google is available
+- **Google BigQuery**: Unofficial BigQuery emulator
 - **Cockroach**: Version 23.1-latest is available
 - **Redis**: Latest server
 - **Dragonfly**: Latest server
 - **KeyDB**: Latest server
 - **Elasticsearch**: Version 7 and 8 are available
 
 ## Contributing
```

