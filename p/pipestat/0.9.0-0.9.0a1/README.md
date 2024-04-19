# Comparing `tmp/pipestat-0.9.0.tar.gz` & `tmp/pipestat-0.9.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipestat-0.9.0.tar", last modified: Fri Apr 19 14:34:06 2024, max compression
+gzip compressed data, was "pipestat-0.9.0a1.tar", last modified: Thu Apr  4 17:46:46 2024, max compression
```

## Comparing `pipestat-0.9.0.tar` & `pipestat-0.9.0a1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.288411 pipestat-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-19 14:33:55.000000 pipestat-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-19 14:33:55.000000 pipestat-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-19 14:34:06.288411 pipestat-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-19 14:33:55.000000 pipestat-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.276411 pipestat-0.9.0/pipestat/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/argparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.280411 pipestat-0.9.0/pipestat/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.280411 pipestat-0.9.0/pipestat/backends/db_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/db_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/db_backend/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14287 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/db_backend/db_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    27351 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/db_backend/dbbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.280411 pipestat-0.9.0/pipestat/backends/file_backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/file_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32471 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/backends/file_backend/filebackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6413 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.284411 pipestat-0.9.0/pipestat/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/footer_index.html
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/glossary.html
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/glossary_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/head.html
--rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/logo.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/navbar.html
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/navbar_links.html
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/navbar_list_parent.html
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/project_object.html
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/sample.html
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/status.html
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/status_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/jinja_templates/status_table_no_links.html
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    40606 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/pipestat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.284411 pipestat-0.9.0/pipestat/pipestatreader/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/pipestatreader/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/pipestatreader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/pipestatreader/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    58267 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.284411 pipestat-0.9.0/pipestat/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/schemas/pipestat_config_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/schemas/status_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-19 14:33:55.000000 pipestat-0.9.0/pipestat/schemas/status_table_schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.288411 pipestat-0.9.0/pipestat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 14:34:06.000000 pipestat-0.9.0/pipestat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-19 14:33:55.000000 pipestat-0.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.284411 pipestat-0.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 14:33:55.000000 pipestat-0.9.0/requirements/requirements-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 14:33:55.000000 pipestat-0.9.0/requirements/requirements-db-backend.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 14:33:55.000000 pipestat-0.9.0/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 14:33:55.000000 pipestat-0.9.0/requirements/requirements-pipestatreader.txt
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 14:33:55.000000 pipestat-0.9.0/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 14:34:06.288411 pipestat-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 14:33:55.000000 pipestat-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 14:34:06.288411 pipestat-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-19 14:33:55.000000 pipestat-0.9.0/tests/test_db_only_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-19 14:33:55.000000 pipestat-0.9.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-19 14:33:55.000000 pipestat-0.9.0/tests/test_parsed_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    91024 2024-04-19 14:33:55.000000 pipestat-0.9.0/tests/test_pipestat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-19 14:33:55.000000 pipestat-0.9.0/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/argparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/db_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21016 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/db_backend/dbbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.067005 pipestat-0.9.0a1/pipestat/backends/file_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30130 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6618 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/jinja_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10727 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7843 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/sample.html
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37635 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/pipestatreader/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/pipestatreader/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58267 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.071005 pipestat-0.9.0a1/pipestat/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pipestat/schemas/status_table_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/pipestat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 17:46:46.000000 pipestat-0.9.0a1/pipestat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-db-backend.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-pipestatreader.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:46:46.075006 pipestat-0.9.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_db_only_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_parsed_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87713 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_pipestat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-04 17:46:35.000000 pipestat-0.9.0a1/tests/test_status.py
```

### Comparing `pipestat-0.9.0/LICENSE` & `pipestat-0.9.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/PKG-INFO` & `pipestat-0.9.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.9.0
+Version: 0.9.0a1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.9.0/README.md` & `pipestat-0.9.0a1/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/argparser.py` & `pipestat-0.9.0a1/pipestat/argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from .const import ENV_VARS, PKG_NAME, STATUS_SCHEMA
 
 REPORT_CMD = "report"
 INSPECT_CMD = "inspect"
 REMOVE_CMD = "remove"
 RETRIEVE_CMD = "retrieve"
-HISTORY_CMD = "history"
 STATUS_CMD = "status"
 INIT_CMD = "init"
 SUMMARIZE_CMD = "summarize"
 LINK_CMD = "link"
 SERVE_CMD = "serve"
 SUBPARSER_MESSAGES = {
     REPORT_CMD: "Report a result.",
@@ -23,15 +22,14 @@
     REMOVE_CMD: "Remove a result.",
     RETRIEVE_CMD: "Retrieve a result.",
     STATUS_CMD: "Manage pipeline status.",
     INIT_CMD: "Initialize generic config file",
     SUMMARIZE_CMD: "Generates HTML Report",
     LINK_CMD: "Create symlinks of reported files",
     SERVE_CMD: "Initializes pipestatreader API",
-    HISTORY_CMD: "Retrieve history of reported results for one record identifier",
 }
 
 STATUS_GET_CMD = "get"
 STATUS_SET_CMD = "set"
 STATUS_SUBPARSER_MESSAGES = {
     STATUS_SET_CMD: "Set status.",
     STATUS_GET_CMD: "Get status.",
@@ -167,15 +165,15 @@
             "--pipeline-type",
             type=str,
             metavar="P",
             help="project or sample level pipeline type. ",
         )
 
     # remove, report and inspect
-    for cmd in [REMOVE_CMD, REPORT_CMD, INSPECT_CMD, RETRIEVE_CMD, HISTORY_CMD]:
+    for cmd in [REMOVE_CMD, REPORT_CMD, INSPECT_CMD, RETRIEVE_CMD]:
         sps[cmd].add_argument(
             "-f",
             "--results-file",
             type=str,
             metavar="F",
             help=f"Path to the YAML file where the results will be stored. "
             f"This file will be used as {PKG_NAME} backend and to restore"
@@ -237,29 +235,21 @@
             "-r",
             "--record-identifier",
             type=str,
             metavar="R",
             help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
         )
 
-    for cmd in [RETRIEVE_CMD, HISTORY_CMD]:
-        sps[cmd].add_argument(
-            "-i",
-            "--result-identifier",
-            type=str,
-            metavar="I",
-            help="ID of the result to report; needs to be defined in the schema",
-        )
-        sps[cmd].add_argument(
-            "-r",
-            "--record-identifier",
-            type=str,
-            metavar="R",
-            help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
-        )
+    sps[RETRIEVE_CMD].add_argument(
+        "-r",
+        "--record-identifier",
+        type=str,
+        metavar="R",
+        help=f"ID of the record to report the result for. {_env_txt('record_identifier')}",
+    )
 
     # report
     sps[REPORT_CMD].add_argument(
         "-v",
         "--value",
         required=True,
         metavar="V",
```

### Comparing `pipestat-0.9.0/pipestat/backends/abstract.py` & `pipestat-0.9.0a1/pipestat/backends/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,14 @@
 
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: str,
         force_overwrite: bool = False,
         result_formatter: Optional[staticmethod] = None,
-        history_enabled: bool = True,
     ) -> str:
         _LOGGER.warning("Not implemented yet for this backend")
 
     def retrieve_distinct(
         self,
         columns: Optional[List[str]] = None,
     ) -> List[Any]:
```

### Comparing `pipestat-0.9.0/pipestat/backends/db_backend/db_helpers.py` & `pipestat-0.9.0a1/pipestat/backends/db_backend/db_helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/backends/db_backend/db_parsed_schema.py` & `pipestat-0.9.0a1/pipestat/backends/db_backend/db_parsed_schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -192,57 +192,14 @@
         # return ARRAY if t == list else t
         return t
 
     @property
     def file_like_table_name(self):
         return self._table_name("files")
 
-    def build_history_model(self, pipeline_type):
-        """Creates model for history ORM
-        :param str pipeline_type: project or sample-level pipeline
-        :return model: (model, table_name)
-        """
-        if pipeline_type == "project":
-            history_table_name = self.project_table_name + "_history"
-            data = self.project_level_data
-            main_table_id = self.project_table_name + ".id"
-
-        elif pipeline_type == "sample":
-            history_table_name = self.sample_table_name + "_history"
-            data = self.sample_level_data
-            main_table_id = self.sample_table_name + ".id"
-
-        else:
-            raise PipestatError(
-                f"Building model requires pipeline type. Provided type: '{pipeline_type}' "
-            )
-
-        if not self.sample_level_data and not self.project_level_data:
-            return None
-
-        field_defs = self._make_field_definitions(data, require_type=True)
-        field_defs = self._add_status_field(field_defs)
-        field_defs = self._add_record_identifier_field(field_defs)
-        field_defs = self._add_id_field(field_defs)
-        field_defs = self._add_pipeline_name_field(field_defs)
-        field_defs = self._add_created_time_field(field_defs)
-        field_defs = self._add_modified_time_field(field_defs)
-
-        field_defs["source_record_id"] = (
-            int,
-            Field(
-                default=None,
-                foreign_key=main_table_id,
-            ),
-        )
-
-        history_model = _create_model(history_table_name, **field_defs)
-
-        return history_model, history_table_name
-
     def build_model(self, pipeline_type):
         if pipeline_type == "project":
             data = self.project_level_data
             # if using the same output schema and thus, pipeline name for samples and project
             # we must ensure there are distinct table names in the same database.
             table_name = self.project_table_name
```

### Comparing `pipestat-0.9.0/pipestat/backends/db_backend/dbbackend.py` & `pipestat-0.9.0a1/pipestat/backends/file_backend/filebackend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,632 +1,608 @@
-import copy
 import datetime
+import os.path
+import operator
+from copy import deepcopy
+from functools import reduce
+from itertools import chain
+from ...helpers import get_all_result_files
+
+
+from glob import glob
 from logging import getLogger
-from contextlib import contextmanager
-from typing import List, Dict, Any, Optional, Union, NoReturn, Tuple
+from yacman import FutureYAMLConfigManager as YAMLConfigManager
+from yacman import read_lock, write_lock
+
+from ubiquerg import create_lock, remove_lock
 
-from sqlmodel import SQLModel, Session, create_engine, select as sql_select
+from typing import List, Dict, Any, Optional, Union, Literal, Callable, Tuple
 
-from pipestat.backends.db_backend.db_helpers import selection_filter
-from pipestat.backends.abstract import PipestatBackend
-from ...exceptions import (
-    PipestatDatabaseError,
-    RecordNotFoundError,
-    SchemaError,
-    ColumnNotFoundError,
-    UnrecognizedStatusError,
-    SchemaNotFoundError,
-)
-from ...const import PKG_NAME, STATUS, RECORD_IDENTIFIER, CREATED_TIME, MODIFIED_TIME
+from ...exceptions import UnrecognizedStatusError, PipestatError
+from ...backends.abstract import PipestatBackend
+from ...const import DATE_FORMAT, PKG_NAME, CREATED_TIME, MODIFIED_TIME
 
 
 _LOGGER = getLogger(PKG_NAME)
 
 
-class DBBackend(PipestatBackend):
+class FileBackend(PipestatBackend):
     def __init__(
         self,
+        results_file_path: str,
         record_identifier: Optional[str] = None,
         pipeline_name: Optional[str] = None,
-        show_db_logs: bool = False,
-        pipeline_type: Optional[str] = False,
+        pipeline_type: Optional[str] = None,
         parsed_schema: Optional[str] = None,
         status_schema: Optional[str] = None,
-        db_url: Optional[str] = None,
-        status_schema_source: Optional[dict] = None,
+        status_file_dir: Optional[str] = None,
         result_formatter: Optional[staticmethod] = None,
+        multi_pipelines: Optional[bool] = None,
     ):
         """
-        Class representing a Database backend
+        Class representing a File backend
+        :param str results_file_path: YAML file to report into, if file is
+            used as the object back-end
         :param str record_identifier: record identifier to report for. This
             creates a weak bound to the record, which can be overridden in
             this object method calls
         :param str pipeline_name: name of pipeline associated with result
-        :param str show_db_logs: Defaults to False, toggles showing database logs
         :param str pipeline_type: "sample" or "project"
         :param str parsed_schema: results output schema. Used to construct DB columns.
         :param str status_schema: schema containing pipeline statuses e.g. 'running'
-        :param str db_url: url used for connection to Postgres DB
-        :param dict status_schema_source: filepath of status schema
+        :param str status_file_dir: directory for placing status flags
         :param str result_formatter: function for formatting result
-        """
+        :param bool multi_pipelines: allows for running multiple pipelines for one file backend
 
+        """
         super().__init__(pipeline_type)
-        _LOGGER.warning(f"Initializing DBBackend for pipeline '{pipeline_name}'")
+        _LOGGER.warning("Initialize FileBackend")
+
+        self.results_file_path = results_file_path
         self.pipeline_name = pipeline_name
-        self.pipeline_type = pipeline_type or "sample"
+        self.pipeline_type = pipeline_type
         self.record_identifier = record_identifier
         self.parsed_schema = parsed_schema
         self.status_schema = status_schema
-        self.db_url = db_url
-        self.show_db_logs = show_db_logs
-        self.status_schema_source = status_schema_source
+        self.status_file_dir = status_file_dir
         self.result_formatter = result_formatter
+        self.multi_pipelines = multi_pipelines
 
-        self.orms = self._create_orms(pipeline_type=pipeline_type)
-        self.history_table = self._create_history_orms(pipeline_type=pipeline_type)
+        self.determine_results_file(self.results_file_path)
 
-        self.table_name = list(self.orms.keys())[0]
-        SQLModel.metadata.create_all(self._engine)
+    def determine_results_file(self, results_file_path: str) -> None:
+        """Initialize or load results_file from given path
+        :param str results_file_path: YAML file to report into, if file is
+        used as the object back-end
+        """
+        if not os.path.exists(self.results_file_path):
+            _LOGGER.debug(
+                f"Results file doesn't yet exist. Initializing: {self.results_file_path}"
+            )
+            self._init_results_file()
+        else:
+            _LOGGER.debug(f"Loading results file: {self.results_file_path}")
+            self._load_results_file()
 
     def check_record_exists(
         self,
         record_identifier: str,
     ) -> bool:
         """
-        Check if the specified record exists in the table
+        Check if the specified record exists in self._data
 
         :param str record_identifier: record to check for
         :return bool: whether the record exists in the table
         """
 
-        query_hit = self.select_records(
-            filter_conditions=[
-                {
-                    "key": "record_identifier",
-                    "operator": "eq",
-                    "value": record_identifier,
-                }
-            ]
+        return (
+            self.pipeline_name in self._data
+            and record_identifier in self._data[self.pipeline_name][self.pipeline_type]
         )
 
-        return bool(query_hit["records"])
+    def clear_status(
+        self, record_identifier: str = None, flag_names: List[str] = None
+    ) -> List[Union[str, None]]:
+        """
+        Remove status flags
+
+        :param str record_identifier: name of the record to remove flags for
+        :param Iterable[str] flag_names: Names of flags to remove, optional; if
+            unspecified, all schema-defined flag names will be used.
+        :return List[str]: Collection of names of flags removed
+        """
+
+        flag_names = flag_names or list(self.status_schema.keys())
+        if isinstance(flag_names, str):
+            flag_names = [flag_names]
+        removed = []
+        for f in flag_names:
+            path_flag_file = self.get_status_flag_path(
+                status_identifier=f, record_identifier=record_identifier
+            )
+            try:
+                os.remove(path_flag_file)
+            except:
+                pass
+            else:
+                _LOGGER.info(f"Removed existing flag: {path_flag_file}")
+                removed.append(f)
+        return removed
 
     def count_records(self):
         """
-        Count rows in a selected table
+        Count records
         :return int: number of records
         """
 
-        mod = self.get_model(table_name=self.table_name)
-        with self.session as s:
-            stmt = sql_select(mod)
-            records = s.exec(stmt).all()
-            return len(records)
-
-    def get_model(self, table_name: str):
-        """
-        Get model based on table_name
-        :param str table_name: pipelinename__sample or pipelinename__project
-        :return mod: model/orm associated with the table name
-        """
-        if self.orms is None:
-            raise PipestatDatabaseError("Object relational mapper classes not defined.")
-
-        mod = self.orms.get(table_name)
-
-        if mod is None:
-            raise PipestatDatabaseError(
-                f"No object relational mapper class defined for table '{table_name}'. "
-                f"{len(self.orms)} defined: {', '.join(self.orms.keys())}"
-            )
-        return mod
+        return len(self._data[self.pipeline_name])
+
+    def get_flag_file(self, record_identifier: str = None) -> Union[str, List[str], None]:
+        """
+        Get path to the status flag file for the specified record
+
+        :param str record_identifier: unique record identifier
+        :return str | list[str] | None: path to the status flag file
+        """
+
+        r_id = record_identifier
+        regex = os.path.join(self.status_file_dir, f"{self.pipeline_name}_{r_id}_*.flag")
+        file_list = glob(regex)
+        if len(file_list) > 1:
+            _LOGGER.warning("Multiple flag files found")
+            return file_list
+        elif len(file_list) == 1:
+            return file_list[0]
+        else:
+            _LOGGER.debug("No flag files found")
+            return None
+        pass
 
     def get_status(self, record_identifier: str) -> Optional[str]:
         """
-        Get pipeline status
+        Get the current pipeline status
 
         :param str record_identifier: record identifier to set the
             pipeline status for
-        :return str status
+        :return str: status identifier, e.g. 'running'
         """
-
-        try:
-            result = self.select_records(
-                columns=[STATUS],
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": record_identifier,
-                    }
-                ],
+        r_id = record_identifier or self.record_identifier
+        flag_file = self.get_flag_file(record_identifier=record_identifier)
+        if flag_file is not None:
+            assert isinstance(flag_file, str), TypeError(
+                "Flag file path is expected to be a str, were multiple flags found?"
             )
-        except RecordNotFoundError:
-            return None
-        try:
-            status = result["records"][0]["status"]
-        except IndexError:
-            status = None
+            with open(flag_file, "r") as f:
+                status = f.read()
+            return status
+        _LOGGER.debug(
+            f"Could not determine status for '{r_id}' record. "
+            f"No flags found in: {self.status_file_dir}"
+        )
+        return None
+
+    def get_status_flag_path(self, status_identifier: str, record_identifier=None) -> str:
+        """
+        Get the path to the status file flag
 
-        return status
+        :param str status_identifier: one of the defined status IDs in schema
+        :param str record_identifier: unique record ID
+        :return str: absolute path to the flag file or None if object is
+            backed by a DB
+        """
+
+        r_id = record_identifier
+        return os.path.join(
+            self.status_file_dir,
+            f"{self.pipeline_name}_{r_id}_{status_identifier}.flag",
+        )
 
     def list_results(
         self,
         restrict_to: Optional[List[str]] = None,
-        record_identifier: str = None,
+        record_identifier: Optional[str] = None,
     ) -> List[str]:
         """
-        Check if the specified results exist in the table
+        Lists all, or a selected set of, reported results
 
-        :param List[str] restrict_to: results identifiers to check for
-        :param str record_identifier: record to check for
-        :return List[str] existing: if no result identifier specified, return all results for the record
-        :return List[str]: results identifiers that exist
+        :param List[str] restrict_to: selected subset of names of results to list
+        :param str record_identifier: unique identifier of the record
+        :return List[str]: names of results which exist
         """
+        record_identifier = record_identifier or self.record_identifier
 
-        rid = record_identifier
-        record = self.select_records(
-            filter_conditions=[
-                {
-                    "key": "record_identifier",
-                    "operator": "eq",
-                    "value": rid,
-                }
-            ]
-        )
         try:
-            record = record["records"][0]
-        except IndexError:
-            return []
-
-        if restrict_to is None:
-            return (
-                [
-                    key
-                    for key in self.parsed_schema.results_data.keys()
-                    if getattr(record, key, None) is not None
-                ]
-                if record
-                else []
+            results = list(
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier].keys()
             )
-        else:
-            return [r for r in restrict_to if record.get(r, None) is not None] if record else []
+        except KeyError:
+            return []
+        if restrict_to:
+            return [r for r in restrict_to if r in results]
+        return results
 
     def remove(
         self,
         record_identifier: Optional[str] = None,
         result_identifier: Optional[str] = None,
     ) -> bool:
         """
         Remove a result.
 
-        If no result ID specified, the entire record
+        If no result ID specified or last result is removed, the entire record
         will be removed.
 
         :param str record_identifier: unique identifier of the record
         :param str result_identifier: name of the result to be removed or None
              if the record should be removed.
         :return bool: whether the result has been removed
         """
 
-        # TODO removing last result identifier (apart from created, modified time should remove record)
         record_identifier = record_identifier or self.record_identifier
+
         rm_record = True if result_identifier is None else False
 
-        if not self.check_record_exists(record_identifier=record_identifier):
+        if not self.check_record_exists(
+            record_identifier=record_identifier,
+        ):
             _LOGGER.error(f"Record '{record_identifier}' not found")
             return False
 
         if result_identifier and not self.check_result_exists(
-            result_identifier=result_identifier,
-            record_identifier=record_identifier,
+            result_identifier, record_identifier
         ):
             _LOGGER.error(f"'{result_identifier}' has not been reported for '{record_identifier}'")
             return False
 
-        try:
-            ORMClass = self.get_model(table_name=self.table_name)
-            if self.check_record_exists(
+        if rm_record:
+            self.remove_record(
                 record_identifier=record_identifier,
+                rm_record=rm_record,
+            )
+        else:
+            del self._data[self.pipeline_name][self.pipeline_type][record_identifier][
+                result_identifier
+            ]
+            _LOGGER.info(
+                f"Removed result '{result_identifier}' for record "
+                f"'{record_identifier}' from '{self.pipeline_name}' namespace"
+            )
+            if not self._data[self.pipeline_name][self.pipeline_type][record_identifier]:
+                _LOGGER.info(
+                    f"Last result removed for '{record_identifier}'. " f"Removing the record"
+                )
+                rm_record = True
+                self.remove_record(
+                    record_identifier=record_identifier,
+                    rm_record=rm_record,
+                )
+            # Check if the last remaining attributes are the timestamps
+            remaining_attributes = list(
+                self._data[self.pipeline_name][self.pipeline_type][record_identifier].keys()
+            )
+            if (
+                len(remaining_attributes) == 2
+                and CREATED_TIME in remaining_attributes
+                and MODIFIED_TIME in remaining_attributes
             ):
-                with self.session as s:
-                    records = s.exec(
-                        sql_select(ORMClass).where(
-                            getattr(ORMClass, "record_identifier") == record_identifier
-                        )
-                    )
-                    if rm_record is True:
-                        self.remove_record(
-                            record_identifier=record_identifier,
-                            rm_record=rm_record,
-                        )
-                    else:
-                        if not self.check_result_exists(
-                            record_identifier=record_identifier,
-                            result_identifier=result_identifier,
-                        ):
-                            raise RecordNotFoundError(
-                                f"Result '{result_identifier}' not found for record "
-                                f"'{record_identifier}'"
-                            )
-                        setattr(records.first(), result_identifier, None)
-                    s.commit()
-            else:
-                raise RecordNotFoundError(f"Record '{record_identifier}' not found")
-        except Exception as e:
-            _LOGGER.error(f"Could not remove the result from the database. Exception: {e}")
-            raise
-
+                _LOGGER.info(
+                    f"Last result removed for '{record_identifier}'. " f"Removing the record"
+                )
+                rm_record = True
+                self.remove_record(
+                    record_identifier=record_identifier,
+                    rm_record=rm_record,
+                )
+            with write_lock(self._data) as locked_data:
+                locked_data.write()
         return True
 
     def remove_record(
         self,
         record_identifier: Optional[str] = None,
         rm_record: Optional[bool] = False,
-    ) -> NoReturn:
+    ) -> bool:
         """
         Remove a record, requires rm_record to be True
 
         :param str record_identifier: unique identifier of the record
         :param bool rm_record: bool for removing record.
         :return bool: whether the result has been removed
-        :raises RecordNotFoundError: if record not found
         """
-
-        record_identifier = record_identifier or self.record_identifier
         if rm_record:
             try:
-                ORMClass = self.get_model(table_name=self.table_name)
-                ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
-                if self.check_record_exists(
-                    record_identifier=record_identifier,
-                ):
-                    with self.session as s:
-                        source_record_id = (
-                            s.exec(
-                                sql_select(ORMClass).where(
-                                    getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
-                                )
-                            )
-                            .first()
-                            .id
-                        )
-                        linked_records = s.exec(
-                            sql_select(ORMClass_History).where(
-                                getattr(ORMClass_History, "source_record_id") == source_record_id
-                            )
-                        ).all()
-                        for r in linked_records:
-                            s.delete(r)
-                        s.commit()
-                    with self.session as s:
-                        record = s.exec(
-                            sql_select(ORMClass).where(
-                                getattr(ORMClass, "record_identifier") == record_identifier
-                            )
-                        ).first()
-                        s.delete(record)
-                        s.commit()
-                else:
-                    raise RecordNotFoundError(f"Record '{record_identifier}' not found")
-            except Exception as e:
-                _LOGGER.error(f"Could not remove the result from the database. Exception: {e}")
-                raise
+                _LOGGER.info(f"Removing '{record_identifier}' record")
+                del self._data[self.pipeline_name][self.pipeline_type][record_identifier]
+                with write_lock(self._data) as data_locked:
+                    data_locked.write()
+                return True
+            except:
+                _LOGGER.warning(
+                    f" Unable to remove record, aborting Removing '{record_identifier}' record"
+                )
+                return False
         else:
             _LOGGER.info(f" rm_record flag False, aborting Removing '{record_identifier}' record")
 
     def report(
         self,
         values: Dict[str, Any],
-        record_identifier: str,
+        record_identifier: Optional[str] = None,
         force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
-        history_enabled: bool = True,
     ) -> Union[List[str], bool]:
         """
         Update the value of a result in a current namespace.
 
         This method overwrites any existing data and creates the required
          hierarchical mapping structure if needed.
 
         :param Dict[str, Any] values: dict of results identifiers and values
             to be reported
         :param str record_identifier: unique identifier of the record
-        :param bool force_overwrite: force overwriting of results, defaults to False.
+        :param bool force_overwrite: Toggles force overwriting results, defaults to False
         :param str result_formatter: function for formatting result
-        :return list[str] list results_formatted | bool: return list of formatted string
+        :return bool | list[str] results_formatted: return list of formatted string
         """
 
-        record_identifier = record_identifier or self.record_identifier
+        # record_identifier = record_identifier or self.record_identifier
+        record_identifier = record_identifier
 
         result_formatter = result_formatter or self.result_formatter
         results_formatted = []
-        result_identifiers = list(values.keys())
-        if self.parsed_schema is None:
-            raise SchemaNotFoundError("DB Backend report results requires schema")
-        self.assert_results_defined(results=result_identifiers, pipeline_type=self.pipeline_type)
+        current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
+        result_identifiers = list(values.keys())
+        if self.parsed_schema is not None:
+            self.assert_results_defined(
+                results=result_identifiers, pipeline_type=self.pipeline_type
+            )
         existing = self.list_results(
             record_identifier=record_identifier,
             restrict_to=result_identifiers,
         )
         if existing:
             existing_str = ", ".join(existing)
             _LOGGER.warning(f"These results exist for '{record_identifier}': {existing_str}")
             if not force_overwrite:
                 return False
             _LOGGER.info(f"Overwriting existing results: {existing_str}")
-
-        try:
-            ORMClass = self.get_model(table_name=self.table_name)
-            ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
-            values.update({RECORD_IDENTIFIER: record_identifier})
-
-            if not self.check_record_exists(
-                record_identifier=record_identifier,
-            ):
-                current_time = datetime.datetime.now()
-                values.update({CREATED_TIME: current_time})
+            values.update({MODIFIED_TIME: current_time})
+        if not existing:
+            if record_identifier in self._data[self.pipeline_name][self.pipeline_type].keys():
                 values.update({MODIFIED_TIME: current_time})
-                new_record = ORMClass(**values)
-                with self.session as s:
-                    s.add(new_record)
-                    s.commit()
             else:
-                with self.session as s:
-                    record_to_update = s.exec(
-                        sql_select(ORMClass).where(
-                            getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
-                        )
-                    ).first()
-                    old_record_attributes = record_to_update.model_dump()
-                    values.update({MODIFIED_TIME: datetime.datetime.now()})
-                    for result_id, result_value in values.items():
-                        setattr(record_to_update, result_id, result_value)
-                    s.commit()
-                if history_enabled:
-                    if "id" in old_record_attributes:
-                        del old_record_attributes["id"]
-                    with self.session as s:
-                        source_record = s.exec(
-                            sql_select(ORMClass).where(
-                                getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
-                            )
-                        ).first()
-                        new_record_history = ORMClass_History(**old_record_attributes)
-                        new_record_history.source_record_id = source_record.id
-                        s.add(new_record_history)
-                        s.commit()
-
-            for res_id, val in values.items():
-                results_formatted.append(
-                    result_formatter(
-                        pipeline_name=self.pipeline_name,
-                        record_identifier=record_identifier,
-                        res_id=res_id,
-                        value=val,
-                    )
+                values.update({CREATED_TIME: current_time})
+                values.update({MODIFIED_TIME: current_time})
+
+        self._data[self.pipeline_name][self.pipeline_type].setdefault(record_identifier, {})
+
+        for res_id, val in values.items():
+            self._data[self.pipeline_name][self.pipeline_type][record_identifier][res_id] = val
+            results_formatted.append(
+                result_formatter(
+                    pipeline_name=self.pipeline_name,
+                    record_identifier=record_identifier,
+                    res_id=res_id,
+                    value=val,
                 )
-            return results_formatted
-        except Exception as e:
-            _LOGGER.error(f"Could not insert the result into the database. Exception: {e}")
-            raise
+            )
+
+        with write_lock(self._data) as locked_data:
+            locked_data.write()
+
+        return results_formatted
+
+    def select_distinct(self, columns: Union[str, List[str]]) -> List[Tuple]:
+        """
+        Retrieve distinct results given a list of columns
+
+        :param str | List[str] columns: column columns to include in the result
+        :return List[Tuple]: returns distinct values.
+        """
+        if isinstance(columns, str):
+            columns = [columns]
+
+        record_data = self._data.data[self.pipeline_name][self.pipeline_type]
+
+        final_values_list = []
+        for record_id in record_data.keys():
+            record_value_list = []
+            for column in columns:
+                if column in list(record_data[record_id].keys()):
+                    record_value_list.append(record_data[record_id][column])
+                else:
+                    if column != "record_identifier":
+                        _LOGGER.warning(msg=f"Column {column} not reported, skipping....")
+
+            if "record_identifier" in columns:
+                # record_identifier is not a column in the file backend but the user may want it
+                record_value_list.append(record_id)
+            final_values_list.append(tuple(record_value_list))
+
+        # make sure that the order is correct
+        unique_lists = list(set(final_values_list))
+        return unique_lists
 
     def select_records(
         self,
         columns: Optional[List[str]] = None,
         filter_conditions: Optional[List[Dict[str, Any]]] = None,
         limit: Optional[int] = 1000,
         cursor: Optional[int] = None,
         bool_operator: Optional[str] = "AND",
     ) -> Dict[str, Any]:
         """
-        Perform a `SELECT` on the table
+        Select records from the FileBackend
 
         :param list[str] columns: columns to include in the result
         :param list[dict]  filter_conditions: e.g. [{"key": ["id"], "operator": "eq", "value": 1)], operator list:
             - eq for ==
             - lt for <
             - ge for >=
             - in for in_
-            - like for like
         :param int limit: maximum number of results to retrieve per page
         :param int cursor: cursor position to begin retrieving records
         :param bool bool_operator: Perform filtering with AND or OR Logic.
         :return dict records_dict = {
             "total_size": int,
             "page_size": int,
             "next_page_token": int,
             "records": List[Dict[{key, Any}]],
         }
         """
+        if cursor:
+            _LOGGER.warning("Cursor not supported for FileBackend, ignoring cursor")
 
-        ORM = self.get_model(table_name=self.table_name)
-
-        with self.session as s:
-            total_count = len(s.exec(sql_select(ORM)).all())
-
-            if columns is not None:
-                columns = copy.deepcopy(columns)
-                for i in ["id", "record_identifier"]:  # Must add id, need it for cursor
-                    if i not in columns:
-                        columns.insert(0, i)
-                try:
-                    statement = sql_select(*[getattr(ORM, column) for column in columns]).order_by(
-                        ORM.id
-                    )
-                except AttributeError:
-                    raise ColumnNotFoundError(
-                        msg=f"One of the supplied columns does not exist in current table: {columns}"
-                    )
+        def get_operator(op: Literal["eq", "lt", "ge", "gt", "in"]) -> Any:
+            """
+            Get python operator for a given string
+
+            :param str op: desired operator, "eq", "lt"
+            :return: operator function
+            """
+
+            if op == "eq":
+                return operator.__eq__
+            if op == "lt":
+                return operator.__lt__
+            if op == "ge":
+                return operator.__ge__
+            if op == "gt":
+                return operator.__gt__
+            if op == "in":
+                return operator.contains
+            raise ValueError(f"Invalid filter operator: {op}")
+
+        def get_nested_column(result_value: dict, key_list: list, retrieved_operator: Callable):
+            """
+            Recursive function that evaluates a nested list of keys vs a value dict
+
+            :param dict result_value: nested dictionary
+            :param key_list: list of keys, e.g. keys that may be in the nested dictionary e.g. ['id', 'name']
+            :param retrieved_operator: operator function (ge, gt...)
+            :return bool:
+            """
+            if len(key_list) == 1:
+                if result_value.get(key_list[0], None):
+                    if retrieved_operator(key_list, result_value.get(key_list[0])):
+                        return True
+                return False
             else:
-                statement = sql_select(ORM).order_by(ORM.id)
-
-            if cursor is not None:
-                statement = statement.where(ORM.id > cursor)
-
-            statement = selection_filter(
-                ORM=ORM,
-                statement=statement,
-                filter_conditions=filter_conditions,
-                bool_operator=bool_operator,
-            )
-
-            if isinstance(limit, int):
-                statement = statement.limit(limit)
-
-            results = s.exec(statement).all()
-
-        if results != []:
-            next_cursor = results[-1].id
-        else:
-            next_cursor = None
-
-        end_results = []
+                return get_nested_column(
+                    result_value[key_list[0]], key_list[1:], retrieved_operator
+                )
 
-        # SQL model returns either a SQLModelMetaCLass OR a sqlalchemy Row.
-        # We must create a dictionary containing the record before returning
-        if not columns:
-            end_results = [r.model_dump() for r in results]
+        records_list = []
 
-        else:
-            for record in results:
-                record_dict = dict(record._mapping)
-                del record_dict["id"]
-                end_results.append(record_dict)
+        data = deepcopy(self._data.data[self.pipeline_name][self.pipeline_type])
 
-        records_dict = {
-            "total_size": total_count,
-            "page_size": limit,
-            "next_page_token": next_cursor,
-            "records": end_results,
-        }
+        if columns:
+            if not isinstance(columns, list):
+                raise ValueError(
+                    "Columns must be a list of strings, e.g. ['record_identifier', 'number_of_things']"
+                )
 
-        return records_dict
+        total_count = len(data.keys())
 
-    def retrieve_history_db(
-        self,
-        record_identifier: str,
-        result_identifier: Optional[Union[str, List[str]]] = None,
-    ) -> Dict[str, Any]:
-        """
+        filtered_records_list = []
+        if filter_conditions:
+            for filter_condition in filter_conditions:
+                if list(filter_condition.keys()) != ["key", "operator", "value"]:
+                    raise ValueError(
+                        "Filter conditions must be a dictionary with keys 'key', 'operator', and 'value'"
+                    )
 
-        :param record_identifier: single record_identifier
-        :param result_identifier: single or list of result identifiers
-        :return: dict records_dict = {
-            "history": List[Dict[{key, Any}]],
-        }
-        """
+                retrieved_operator = get_operator(filter_condition["operator"])
+                retrieved_results = []
 
-        record_identifier = record_identifier or self.record_identifier
+                # Check each sample's dict
+                for record_identifier in list(data.keys())[0:limit]:
+                    if filter_condition["key"] != "record_identifier":
+                        for key, value in data[record_identifier].items():
+                            result = False
+                            if isinstance(value, dict):
+                                if key == filter_condition["key"][0]:
+                                    result = get_nested_column(
+                                        value,
+                                        filter_condition["key"][1:],
+                                        retrieved_operator,
+                                    )
+                            else:
+                                if filter_condition["key"] == key:
+                                    # Filter datetime objects
+                                    if key in CREATED_TIME or key in MODIFIED_TIME:
+                                        try:
+                                            time_stamp = datetime.datetime.strptime(
+                                                data[record_identifier][key],
+                                                DATE_FORMAT,
+                                            )
+                                            result = retrieved_operator(
+                                                time_stamp, filter_condition["value"]
+                                            )
+                                        except TypeError:
+                                            result = False
+                                    else:
+                                        result = retrieved_operator(
+                                            value, filter_condition["value"]
+                                        )
 
-        ORMClass = self.get_model(table_name=self.table_name)
-        ORMClass_History = self.history_table[list(self.history_table.keys())[0]]
+                            if result:
+                                retrieved_results.append(record_identifier)
+                    else:
+                        # If user wants record_identifier
+                        if isinstance(filter_condition["value"], list):
+                            for v in filter_condition["value"]:
+                                if (
+                                    record_identifier == v
+                                    and record_identifier not in retrieved_results
+                                ):
+                                    retrieved_results.append(record_identifier)
+                        elif record_identifier == filter_condition["value"]:
+                            retrieved_results.append(record_identifier)
 
-        if not result_identifier:
-            columns = None
+                if retrieved_results:
+                    filtered_records_list.append(retrieved_results)
         else:
-            if isinstance(result_identifier, str):
-                columns = [result_identifier]
-            elif isinstance(result_identifier, list):
-                columns = copy.deepcopy(result_identifier)
-            else:
-                raise ValueError("Result identifier must be a str or list[str]")
-            for i in ["id", MODIFIED_TIME]:
-                if i not in columns:
-                    columns.insert(0, i)
+            # Assume user wants all the records if no filter was given.
+            filtered_records_list = [list(data.keys())[0:limit]]
 
-        if not self.check_record_exists(
-            record_identifier=record_identifier,
-        ):
-            raise RecordNotFoundError(f"{record_identifier} does not exist.")
-        else:
-            with self.session as s:
-                source_record_id = (
-                    s.exec(
-                        sql_select(ORMClass).where(
-                            getattr(ORMClass, RECORD_IDENTIFIER) == record_identifier
-                        )
-                    )
-                    .first()
-                    .id
-                )
-                if columns is not None:
-                    try:
-                        statement = sql_select(
-                            *[getattr(ORMClass_History, column) for column in columns]
-                        ).order_by(ORMClass_History.id)
-                    except AttributeError:
-                        raise ColumnNotFoundError(
-                            msg=f"One of the supplied columns does not exist in current table: {columns}"
-                        )
+        # There is now a list of dicts for each filtered condition.
+        # Depending on Union or Intersection we want to pare down the list.
+        shared_keys = []
+
+        if bool_operator.lower() == "and" and filtered_records_list:
+            shared_keys = list(reduce(lambda i, j: i & j, (set(x) for x in filtered_records_list)))
+
+        if bool_operator.lower() == "or" and filtered_records_list:
+            shared_keys = list(set(chain(*filtered_records_list)))
+
+        if shared_keys:
+            for record_identifier in sorted(shared_keys):
+                record = {}
+                if columns:  # Did the user specify a list of columns as well?
+                    for key, value in list(data[record_identifier].items()):
+                        if key in columns:
+                            record.update({key: value})
+                    if "record_identifier" in columns:
+                        record.update({"record_identifier": record_identifier})
                 else:
-                    statement = sql_select(ORMClass_History).order_by(ORMClass_History.id)
-
-                statement = statement.where(
-                    getattr(ORMClass_History, "source_record_id") == source_record_id
-                )
-
-                history_records = s.exec(statement).all()
-
-        end_results = []
-
-        # SQL model returns either a SQLModelMetaCLass OR a sqlalchemy Row.
-        # We must create a dictionary containing the record before returning
-
-        if not columns:
-            end_results = [r.model_dump() for r in history_records]
-
-        else:
-            for record in history_records:
-                record_dict = dict(record._mapping)
-                end_results.append(record_dict)
-
-        # This next step is to process the results such that they will match output similar to the filebackend
-
-        collected_keys = []
-        new_history_dict = {}
-        for result in end_results:
-            for key, value in result.items():
-                if key == MODIFIED_TIME:
-                    continue
-                elif value:
-                    if key not in new_history_dict:
-                        collected_keys.append(key)
-                        new_history_dict[key] = {result[MODIFIED_TIME]: value}
-                    else:
-                        new_history_dict[key].update({result[MODIFIED_TIME]: value})
+                    record = data[record_identifier]
+                if record != {}:
+                    record.update({"record_identifier": record_identifier})
+                    records_list.append(record)
 
         records_dict = {
-            "history": new_history_dict,
+            "total_size": total_count,
+            "page_size": limit,
+            "next_page_token": 0,
+            "records": records_list,
         }
 
         return records_dict
 
-    def select_distinct(
-        self,
-        columns: Union[str, List[str]],
-    ) -> List[Tuple]:
-        """
-        Perform a `SELECT DISTINCT` on given table and column
-
-        :param str | List[str] columns: columns to include in the result
-        :return List[Tuple]: returns distinct values.
-        """
-        if isinstance(columns, str):
-            columns = [columns]
-
-        ORM = self.get_model(table_name=self.table_name)
-        with self.session as s:
-            list_columns = [getattr(ORM, column) for column in columns]
-            result = s.exec(sql_select(*list_columns).distinct()).all()
-
-        return result
-
     def set_status(
         self,
         status_identifier: str,
         record_identifier: str = None,
     ) -> None:
         """
         Set pipeline run status.
@@ -636,89 +612,129 @@
         this package.
 
         :param str status_identifier: status to set, one of statuses defined
             in the status schema
         :param str record_identifier: record identifier to set the
             pipeline status for
         """
+        r_id = record_identifier or self.record_identifier
+        if self.status_schema is not None:
+            known_status_identifiers = self.status_schema.keys()
+            if status_identifier not in known_status_identifiers:
+                raise UnrecognizedStatusError(
+                    f"'{status_identifier}' is not a defined status identifier. "
+                    f"These are allowed: {known_status_identifiers}"
+                )
+        prev_status = self.get_status(r_id)
+
+        if prev_status is not None:
+            prev_flag_path = self.get_status_flag_path(prev_status, record_identifier)
+            os.remove(prev_flag_path)
+        flag_path = self.get_status_flag_path(status_identifier, record_identifier)
+        create_lock(flag_path)
+        with open(flag_path, "w") as f:
+            f.write(status_identifier)
+        remove_lock(flag_path)
 
-        record_identifier = record_identifier or self.record_identifier
-        known_status_identifiers = self.status_schema.keys()
-        if status_identifier not in known_status_identifiers:
-            raise UnrecognizedStatusError(
-                f"'{status_identifier}' is not a defined status identifier. "
-                f"These are allowed: {known_status_identifiers}"
-            )
-        prev_status = self.get_status(record_identifier)
-        try:
-            self.report(
-                values={STATUS: status_identifier},
-                record_identifier=record_identifier,
-            )
-        except Exception as e:
-            _LOGGER.error(
-                f"Could not insert into the status table ('{self.table_name}'). Exception: {e}"
-            )
-            raise
         if prev_status:
             _LOGGER.debug(f"Changed status from '{prev_status}' to '{status_identifier}'")
 
-    def _create_orms(self, pipeline_type):
-        """Create ORMs.
-        :param str pipeline_type: project or sample-level pipeline
-        :return dict: {table_name: model}
-        """
-        _LOGGER.debug(f"Creating models for '{self.pipeline_name}' table in '{PKG_NAME}' database")
-        model = self.parsed_schema.build_model(pipeline_type=pipeline_type)
-        table_name = self.parsed_schema._table_name(pipeline_type)
-        # TODO reconsider line below. Why do we need to return a dict?
-        if model:
-            return {table_name: model}
-        else:
-            raise SchemaError(
-                f"Neither project nor samples model could be built from schema source: {self.status_schema_source}"
-            )
+    def _htmlreportbuilder(self):
+        """
+        build html report based on all reported results
+        """
 
-    def _create_history_orms(self, pipeline_type):
-        """Creates the additional ORMs for auditing result modifications
-        :param str pipeline_type: project or sample-level pipeline
-        :return dict: {table_name: model}
-        """
-        model, table_name = self.parsed_schema.build_history_model(pipeline_type=pipeline_type)
-        if model:
-            return {table_name: model}
-        else:
-            raise SchemaError(
-                f"Neither project nor samples model could be built from schema source: {self.status_schema_source}"
-            )
+        # build new folder for the report
+        self.reports_dir = os.path.join(self.results_file_path, "reports")
+        _LOGGER.debug(f"Reports dir: {self.reports_dir}")
 
-    @property
-    def _engine(self):
-        """Access the database engine backing this manager."""
-        try:
-            return self.db_engine_key
-        except AttributeError:
-            # Do it this way rather than .setdefault to avoid evaluating
-            # the expression for the default argument (i.e., building
-            # the engine) if it's not necessary.
-            self.db_engine_key = create_engine(self.db_url, echo=self.show_db_logs)
-            return self.db_engine_key
-
-    @property
-    @contextmanager
-    def session(self):
+    def _init_results_file(self) -> None:
         """
-        Provide a transactional scope around a series of query
-        operations.
+        Initialize YAML results file if it does not exist.
+        Read the data stored in the existing file into the memory otherwise.
+
+        :return bool: whether the file has been created
         """
-        session = Session(self._engine)
-        _LOGGER.debug("Created session")
+        _LOGGER.info(f"Initializing results file '{self.results_file_path}'")
+
+        # Must ensure sub-directories exist if they do not
+        # TODO should this actually be handled by yacman?
         try:
-            yield session
-        except:
-            _LOGGER.info("session.rollback")
-            session.rollback()
-            raise
-        finally:
-            # _LOGGER.info("session.close")
-            session.close()
-        _LOGGER.debug("Ending session")
+            os.makedirs(os.path.dirname(self.results_file_path))
+        except FileExistsError:
+            pass
+
+        self._data = YAMLConfigManager.from_yaml_file(
+            self.results_file_path,
+            create_file=True,
+        )
+        self._data.update_from_obj({self.pipeline_name: {}})
+        self._data.setdefault(self.pipeline_name, {})
+        self._data[self.pipeline_name].setdefault("project", {})
+        self._data[self.pipeline_name].setdefault("sample", {})
+        with write_lock(self._data) as data_locked:
+            data_locked.write()
+
+    def aggregate_multi_results(self, results_directory) -> None:
+        """
+        Collects single results files and aggregates them into a new aggregate_results.yaml file
+        :param str results_directory: directory containing subdirectories containing results.yaml files
+        :return: None
+        """
+        all_result_files = get_all_result_files(results_directory)
+        if len(all_result_files) == 0:
+            _LOGGER.warning(
+                "Attempting to aggregate multiple results files but no result files found. Ensure they are in subdirectories, e.g. 'record1/record1_results.yaml'"
+            )
+        aggregate_results_file_path = os.path.join(results_directory, "aggregate_results.yaml")
+
+        # THIS WILL OVERWRITE self.results_file_path and self._data on the current psm!
+        self.results_file_path = aggregate_results_file_path
+        self._init_results_file()
+
+        for file in all_result_files:
+            try:
+                temp_data = YAMLConfigManager.from_yaml_file(file)
+            except ValueError:
+                temp_data = YAMLConfigManager()
+            if self.pipeline_name in temp_data:
+                if "project" in temp_data[self.pipeline_name]:
+                    self._data[self.pipeline_name]["project"].update(
+                        temp_data[self.pipeline_name]["project"]
+                    )
+                if "sample" in temp_data[self.pipeline_name]:
+                    self._data[self.pipeline_name]["sample"].update(
+                        temp_data[self.pipeline_name]["sample"]
+                    )
+
+        with write_lock(self._data) as data_locked:
+            data_locked.write()
+
+    def _load_results_file(self) -> None:
+        _LOGGER.debug(f"Reading data from '{self.results_file_path}'")
+        data = YAMLConfigManager.from_yaml_file(self.results_file_path)
+        if not bool(data):
+            self._data = data
+            self._data.setdefault(self.pipeline_name, {})
+            self._data[self.pipeline_name].setdefault("project", {})
+            self._data[self.pipeline_name].setdefault("sample", {})
+            with write_lock(self._data) as data_locked:
+                data_locked.write()
+        namespaces_reported = [k for k in data.keys() if not k.startswith("_")]
+        num_namespaces = len(namespaces_reported)
+        if num_namespaces == 0:
+            self._data = data
+        elif num_namespaces > 0:
+            if self.pipeline_name in namespaces_reported:
+                self._data = data
+            elif self.pipeline_name not in namespaces_reported and self.multi_pipelines is True:
+                self._data = data
+                self._data.setdefault(self.pipeline_name, {})
+                self._data[self.pipeline_name].setdefault("project", {})
+                self._data[self.pipeline_name].setdefault("sample", {})
+                _LOGGER.warning("MULTI PIPELINES FOR SINGLE RESULTS FILE")
+            else:
+                raise PipestatError(
+                    f"Trying to report result for namespace '{self.pipeline_name}' at '{self.results_file_path}', but "
+                    f"{num_namespaces} other namespaces are already in the file: [{', '.join(namespaces_reported)}]. "
+                    f"Pipestat will not report multiple namespaces to one file unless `multi_pipelines` is True."
+                )
```

### Comparing `pipestat-0.9.0/pipestat/cli.py` & `pipestat-0.9.0a1/pipestat/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     STATUS_CMD,
     STATUS_GET_CMD,
     STATUS_SET_CMD,
     INIT_CMD,
     SUMMARIZE_CMD,
     SERVE_CMD,
     LINK_CMD,
-    HISTORY_CMD,
 )
 from .const import (
     SCHEMA_KEY,
     SCHEMA_TYPE_KEY,
     CANONICAL_TYPES,
     PKG_NAME,
 )
@@ -118,15 +117,15 @@
         database_only=args.database_only,
         flag_file_dir=args.flag_dir,
         pipeline_type=args.pipeline_type,
     )
     types_to_read_from_json = ["object"] + list(CANONICAL_TYPES.keys())
 
     # The next few commands require a record_identifier. Need to also check ENV variables for its existence.
-    if not hasattr(args, "record_identifier") or getattr(args, "record_identifier", None) is None:
+    if args.record_identifier is None:
         args.record_identifier = os.getenv("PIPESTAT_RECORD_IDENTIFIER")
 
     if args.command == REPORT_CMD:
         value = args.value
         if psm.cfg[SCHEMA_KEY] is None:
             raise SchemaNotFoundError(msg="report", cli=True)
         result_metadata = psm.cfg[SCHEMA_KEY].results_data[args.result_identifier]
@@ -171,16 +170,9 @@
         if args.subcommand == STATUS_GET_CMD:
             print(psm.get_status(record_identifier=args.record_identifier))
         if args.subcommand == STATUS_SET_CMD:
             psm.set_status(
                 status_identifier=args.status_identifier,
                 record_identifier=args.record_identifier,
             )
-    if args.command == HISTORY_CMD:
-        print(f"\nHistory for Record: {args.record_identifier}")
-        print(
-            psm.retrieve_history(
-                record_identifier=args.record_identifier, result_identifier=args.result_identifier
-            )
-        )
 
     sys.exit(0)
```

### Comparing `pipestat-0.9.0/pipestat/const.py` & `pipestat-0.9.0a1/pipestat/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,17 +59,14 @@
     "TEMPLATES_DIRNAME",
     "NO_DATA_PLACEHOLDER",
     "PROFILE_COLNAMES",
     "OUTPUT_DIR",
     "RECORD_IDENTIFIER",
     "CREATED_TIME",
     "MODIFIED_TIME",
-    "DATE_FORMAT",
-    "META_KEY",
-    "HISTORY_KEY",
 ]
 
 PKG_NAME = "pipestat"
 LOCK_PREFIX = "lock."
 
 # object attribute names
 SAMPLE_NAME_ID_KEY = "_sample_name"
@@ -83,17 +80,14 @@
 # DB column names
 SAMPLE_NAME = "sample_name"
 RECORD_IDENTIFIER = "record_identifier"
 STATUS = "status"
 CREATED_TIME = "pipestat_created_time"
 MODIFIED_TIME = "pipestat_modified_time"
 
-META_KEY = "meta"
-HISTORY_KEY = "history"
-
 CANONICAL_TYPES = {
     "image": {
         "type": "object",
         "properties": {
             "path": {"type": "string"},
             "thumbnail_path": {"type": "string"},
             "title": {"type": "string"},
```

### Comparing `pipestat-0.9.0/pipestat/exceptions.py` & `pipestat-0.9.0a1/pipestat/exceptions.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/helpers.py` & `pipestat-0.9.0a1/pipestat/helpers.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/footer_index.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/footer_index.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/glossary_table.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/glossary_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/head.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/head.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/index.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/index.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/logo.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/logo.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/navbar.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/navbar_links.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/navbar_list_parent.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/navbar_list_parent.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/object.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/project_object.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/project_object.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/sample.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/sample.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/status_table.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/status_table.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/jinja_templates/status_table_no_links.html` & `pipestat-0.9.0a1/pipestat/jinja_templates/status_table_no_links.html`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/parsed_schema.py` & `pipestat-0.9.0a1/pipestat/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/pipestat.py` & `pipestat-0.9.0a1/pipestat/pipestat.py`

 * *Files 4% similar despite different names*

```diff
@@ -472,15 +472,14 @@
             except ValueError:
                 raise InvalidTimeFormatError(msg=f"Incorrect time format, requires: {date_format}")
 
         if time_column == "created":
             col_name = CREATED_TIME
         else:
             col_name = MODIFIED_TIME
-
         results = self.select_records(
             limit=limit,
             filter_conditions=[
                 {
                     "key": col_name,
                     "operator": "lt",
                     "value": start,
@@ -488,14 +487,15 @@
                 {
                     "key": col_name,
                     "operator": "gt",
                     "value": end,
                 },
             ],
         )
+
         return results
 
     def process_schema(self, schema_path):
         # Load pipestat schema in two parts: 1) main and 2) status
         self._schema_path = self.cfg[CONFIG_KEY].priority_get(
             "schema_path", env_var=ENV_VARS["schema"], override=schema_path
         )
@@ -543,47 +543,34 @@
         r_id = record_identifier or self.cfg[RECORD_IDENTIFIER]
         return self.backend.remove(
             record_identifier=r_id,
             result_identifier=result_identifier,
         )
 
     @require_backend
-    def remove_record(
-        self,
-        record_identifier: Optional[str] = None,
-        rm_record: Optional[bool] = False,
-    ) -> bool:
-        return self.backend.remove_record(
-            record_identifier=record_identifier,
-            rm_record=rm_record,
-        )
-
-    @require_backend
     def report(
         self,
         values: Dict[str, Any],
         record_identifier: Optional[str] = None,
         force_overwrite: bool = True,
         result_formatter: Optional[staticmethod] = None,
         strict_type: bool = True,
-        history_enabled: bool = True,
     ) -> Union[List[str], bool]:
         """
         Report a result.
 
         :param Dict[str, any] values: dictionary of result-value pairs
         :param str record_identifier: unique identifier of the record, value
             in 'record_identifier' column to look for to determine if the record
             already exists
         :param bool force_overwrite: whether to overwrite the existing record
         :param str result_formatter: function for formatting result
         :param bool strict_type: whether the type of the reported values should
             remain as is. Pipestat would attempt to convert to the
             schema-defined one otherwise
-        :param bool history_enabled: Should history of reported results be enabled?
         :return str reported_results: return list of formatted string
         """
 
         result_formatter = result_formatter or self.cfg[RESULT_FORMATTER]
         values = deepcopy(values)
         r_id = record_identifier or self.cfg[RECORD_IDENTIFIER]
         if r_id is None:
@@ -606,15 +593,14 @@
                 )
 
         reported_results = self.backend.report(
             values=values,
             record_identifier=r_id,
             force_overwrite=force_overwrite,
             result_formatter=result_formatter,
-            history_enabled=history_enabled,
         )
 
         return reported_results
 
     @require_backend
     def select_distinct(
         self,
@@ -675,18 +661,21 @@
         self,
         record_identifier: str = None,
         result_identifier: Optional[Union[str, List[str]]] = None,
     ) -> Union[Any, Dict[str, Any]]:
         """
         Retrieve a single record
         :param str record_identifier: single record_identifier
-        :param str result_identifier: single record_identifier or list of result identifiers
-        :return: Dict[str, any]: a mapping with filtered results reported for the record
+        :param str result_identifier: single record_identifier
+        :return: Dict[str, any]: a mapping with filtered
+
+
+            results reported for the record
         """
-        record_identifier = record_identifier or self.record_identifier
+        r_id = record_identifier or self.record_identifier
 
         filter_conditions = [
             {
                 "key": "record_identifier",
                 "operator": "eq",
                 "value": record_identifier,
             },
@@ -728,77 +717,14 @@
                     except IndexError:
                         raise RecordNotFoundError(f"Record '{record_identifier}' not found")
                 else:
                     raise RecordNotFoundError(f"Record '{record_identifier}' not found")
             except IndexError:
                 raise RecordNotFoundError(f"Record '{record_identifier}' not found")
 
-    def retrieve_history(
-        self,
-        record_identifier: str = None,
-        result_identifier: Optional[Union[str, List[str]]] = None,
-    ) -> Union[Any, Dict[str, Any]]:
-        """
-        Retrieve a single record's history
-        :param str record_identifier: single record_identifier
-        :param str result_identifier: single result_identifier or list of result identifiers
-        :return: Dict[str, any]: a mapping with filtered historical results
-        """
-
-        record_identifier = record_identifier or self.record_identifier
-
-        if self.file:
-            result = self.backend.select_records(
-                filter_conditions=[
-                    {
-                        "key": "record_identifier",
-                        "operator": "eq",
-                        "value": record_identifier,
-                    }
-                ],
-                meta_data_bool=True,
-            )["records"][0]
-
-            if "meta" in result and "history" in result["meta"]:
-                history = {}
-                if isinstance(result_identifier, str) and result_identifier in result:
-                    history.update(
-                        {result_identifier: result["meta"]["history"][result_identifier]}
-                    )
-                elif isinstance(result_identifier, list):
-                    for r in result_identifier:
-                        if r in result["meta"]["history"]:
-                            history.update({r: result["meta"]["history"][r]})
-                else:
-                    history = result["meta"]["history"]
-            else:
-                _LOGGER.warning(f"No history available for Record: {record_identifier}")
-                return {}
-
-        else:
-            if result_identifier:
-                history = self.backend.retrieve_history_db(record_identifier, result_identifier)[
-                    "history"
-                ]
-            else:
-                history = self.backend.retrieve_history_db(record_identifier)["history"]
-
-            # DB backend returns some extra_keys that we can remove before returning them to the user.
-            extra_keys_to_delete = [
-                "id",
-                "pipestat_created_time",
-                "source_record_id",
-                "record_identifier",
-            ]
-            history = {
-                key: value for key, value in history.items() if key not in extra_keys_to_delete
-            }
-
-        return history
-
     def retrieve_many(
         self,
         record_identifiers: List[str],
         result_identifier: Optional[str] = None,
     ) -> Union[Any, Dict[str, Any]]:
         """
         :param record_identifiers: list of record identifiers
```

### Comparing `pipestat-0.9.0/pipestat/pipestatreader/README.md` & `pipestat-0.9.0a1/pipestat/pipestatreader/README.md`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/pipestatreader/reader.py` & `pipestat-0.9.0a1/pipestat/pipestatreader/reader.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/reports.py` & `pipestat-0.9.0a1/pipestat/reports.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat/schemas/pipestat_config_schema.yaml` & `pipestat-0.9.0a1/pipestat/schemas/pipestat_config_schema.yaml`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/pipestat.egg-info/PKG-INFO` & `pipestat-0.9.0a1/pipestat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipestat
-Version: 0.9.0
+Version: 0.9.0a1
 Summary: A pipeline results reporter
 Home-page: https://github.com/pepkit/pipestat
 Author: Michal Stolarczyk, Nathan Sheffield
 License: BSD2
 Keywords: project,metadata,bioinformatics,sequencing,ngs,workflow
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pipestat-0.9.0/pipestat.egg-info/SOURCES.txt` & `pipestat-0.9.0a1/pipestat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/setup.py` & `pipestat-0.9.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/tests/test_db_only_mode.py` & `pipestat-0.9.0a1/tests/test_db_only_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             try:
                 SamplePipestatManager(
                     schema_path=schema_file_path,
                     record_identifier="irrelevant",
                     database_only=True,
                     config_file=config_file_path,
                 )
-                print("done")
             except Exception as e:
                 pytest.fail(f"Pipestat manager construction failed: {e})")
 
     @pytest.mark.parametrize(["rec_id", "res_id"], [("sample2", "number_of_things")])
     def test_select_invalid_filter_column__raises_expected_exception(
         self,
         rec_id,
```

### Comparing `pipestat-0.9.0/tests/test_init.py` & `pipestat-0.9.0a1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/tests/test_parsed_schema.py` & `pipestat-0.9.0a1/tests/test_parsed_schema.py`

 * *Files identical despite different names*

### Comparing `pipestat-0.9.0/tests/test_pipestat.py` & `pipestat-0.9.0a1/tests/test_pipestat.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             ("sample2", {"number_of_things": 2}),
             ("sample2", {"percentage_of_things": 10.1}),
             ("sample2", {"name_of_something": "test_name"}),
             ("sample3", {"name_of_something": "test_name"}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
-    def test_basics_all(
+    def test_basics(
         self,
         rec_id,
         val,
         config_file_path,
         schema_file_path,
         results_file_path,
         backend,
@@ -86,15 +86,14 @@
             assert status == "running"
             assert psm.retrieve_one(record_identifier=rec_id)[val_name] == val[val_name]
             psm.remove(record_identifier=rec_id, result_identifier=val_name)
             if backend == "file":
                 psm.clear_status(record_identifier=rec_id)
                 status = psm.get_status(record_identifier=rec_id)
                 assert status is None
-                psm.remove_record(record_identifier=rec_id, rm_record=True)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
             if backend == "db":
                 assert psm.retrieve_one(record_identifier=rec_id).get(val_name, None) is None
                 psm.remove(record_identifier=rec_id)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
@@ -174,16 +173,16 @@
             assert status == "running"
             assert psm.retrieve_one(record_identifier=rec_id)[val_name] == val[val_name]
             psm.remove(record_identifier=rec_id, result_identifier=val_name)
             if backend == "file":
                 psm.clear_status(record_identifier=rec_id)
                 status = psm.get_status(record_identifier=rec_id)
                 assert status is None
-                # with pytest.raises(RecordNotFoundError):
-                #     psm.retrieve_one(record_identifier=rec_id)
+                with pytest.raises(RecordNotFoundError):
+                    psm.retrieve_one(record_identifier=rec_id)
             if backend == "db":
                 psm.remove(record_identifier=rec_id)
                 with pytest.raises(RecordNotFoundError):
                     psm.retrieve_one(record_identifier=rec_id)
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
@@ -196,15 +195,15 @@
             ("sample1", {"number_of_things": 1}),
             ("sample2", {"number_of_things": 2}),
             ("sample2", {"percentage_of_things": 10.1}),
             ("sample2", {"name_of_something": "test_name"}),
             ("sample3", {"name_of_something": "test_name"}),
         ],
     )
-    @pytest.mark.parametrize("backend", ["db"])
+    @pytest.mark.parametrize("backend", ["file", "db"])
     def test_report_basic(
         self,
         rec_id,
         val,
         config_file_path,
         schema_file_path,
         results_file_path,
@@ -324,15 +323,15 @@
                     "properties": {
                         "prop1": {"properties": {"path": "pathstring", "title": "titlestring"}}
                     }
                 }
             },
         ],
     )
-    @pytest.mark.parametrize("backend", ["file"])
+    @pytest.mark.parametrize("backend", ["file", "db"])
     def test_complex_object_report(
         self, val, config_file_path, recursive_schema_file_path, results_file_path, backend
     ):
         with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
             results_file_path = f.name
             args = dict(schema_path=recursive_schema_file_path, database_only=False)
             backend_data = (
@@ -588,47 +587,14 @@
             assert str(list(val.keys())[0]) in list(retrieved_val.keys())
             # Test Retrieve Whole Record
             assert isinstance(psm.retrieve_one(record_identifier=rec_id), Mapping)
 
     @pytest.mark.parametrize(
         ["rec_id", "val"],
         [
-            ("sample1", {"name_of_something": "test_name"}),
-            ("sample1", {"number_of_things": 2}),
-        ],
-    )
-    @pytest.mark.parametrize("backend", ["file", "db"])
-    def test_retrieve_basic_no_record_identifier(
-        self,
-        rec_id,
-        val,
-        config_file_path,
-        results_file_path,
-        schema_file_path,
-        backend,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            args.update(record_identifier=rec_id)
-            psm = SamplePipestatManager(**args)
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-            assert (
-                psm.retrieve_one(result_identifier=list(val.keys())[0]) == list(val.items())[0][1]
-            )
-
-    @pytest.mark.parametrize(
-        ["rec_id", "val"],
-        [
             ("sample1", {"number_of_things": 2}),
         ],
     )
     @pytest.mark.parametrize("backend", ["file", "db"])
     def test_retrieve_one_single_result_as_list(
         self,
         rec_id,
@@ -895,14 +861,45 @@
                 if backend == "db"
                 else {"results_file_path": results_file_path}
             )
             args.update(backend_data)
             psm = SamplePipestatManager(**args)
             assert not psm.remove(record_identifier=rec_id)
 
+    @pytest.mark.parametrize(["rec_id", "res_id"], [("sample3", "name_of_something")])
+    @pytest.mark.parametrize("backend", ["file"])
+    def test_last_result_removal_removes_record(
+        self,
+        rec_id,
+        res_id,
+        schema_file_path,
+        config_file_path,
+        results_file_path,
+        backend,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+            psm.report(
+                record_identifier=rec_id,
+                values={res_id: "something"},
+                force_overwrite=True,
+            )
+            assert psm.remove(record_identifier=rec_id, result_identifier=res_id)
+
+            with pytest.raises(RecordNotFoundError):
+                result = psm.retrieve_one(record_identifier=rec_id)
+
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires postgres service to be available")
 class TestNoRecordID:
     @pytest.mark.parametrize(
         "val",
         [
@@ -1034,14 +1031,15 @@
         monkeypatch.setenv(ENV_VARS["results_file"], results_file_path)
         monkeypatch.setenv(ENV_VARS["schema"], schema_file_path)
         try:
             SamplePipestatManager()
         except Exception as e:
             pytest.fail(f"Error during pipestat manager creation: {e}")
 
+    # @pytest.mark.skip(reason="known failure for now with config file")
     def test_config__psm_is_built_from_config_file_env_var(self, monkeypatch, config_file_path):
         """PSM can be created from config parsed from env var value."""
         monkeypatch.setenv(ENV_VARS["config"], config_file_path)
         try:
             SamplePipestatManager()
         except Exception as e:
             pytest.fail(f"Error during pipestat manager creation: {e}")
@@ -1391,15 +1389,15 @@
                     "report",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
                     "--value",
                     list(val.values())[0],
-                    "--config",
+                    "--config-file",
                     config_file_path,
                     "--schema",
                     schema_file_path,
                 ]
 
             with pytest.raises(
                 SystemExit
@@ -1410,54 +1408,31 @@
             if backend != "db":
                 x = [
                     "retrieve",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
+                    "--value",
+                    list(val.values())[0],
                     "--results-file",
                     results_file_path,
                     "--schema",
                     schema_file_path,
                 ]
             else:
                 x = [
                     "retrieve",
                     "--record-identifier",
                     rec_id,
                     "--result-identifier",
                     list(val.keys())[0],
-                    "--config",
-                    config_file_path,
-                    "--schema",
-                    schema_file_path,
-                ]
-
-            with pytest.raises(
-                SystemExit
-            ):  # pipestat cli normal behavior is to end with a "sys.exit(0)"
-                main(test_args=x)
-
-            # history
-            if backend != "db":
-                x = [
-                    "history",
-                    "--record-identifier",
-                    rec_id,
-                    "--results-file",
-                    results_file_path,
-                    "--schema",
-                    schema_file_path,
-                ]
-            else:
-                x = [
-                    "history",
-                    "--record-identifier",
-                    rec_id,
-                    "--config",
+                    "--value",
+                    list(val.values())[0],
+                    "--config-file",
                     config_file_path,
                     "--schema",
                     schema_file_path,
                 ]
 
             with pytest.raises(
                 SystemExit
@@ -1514,14 +1489,99 @@
                 # TODO This example will have collision if the file names and property names are the same
                 print(files)
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
 class TestTimeStamp:
+    @pytest.mark.parametrize(
+        ["rec_id", "val"],
+        [
+            ("sample1", {"name_of_something": "test_name"}),
+        ],
+    )
+    @pytest.mark.parametrize("backend", ["file", "db"])
+    def test_basic_time_stamp(
+        self,
+        rec_id,
+        val,
+        config_file_path,
+        schema_file_path,
+        results_file_path,
+        backend,
+    ):
+        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
+            results_file_path = f.name
+            args = dict(schema_path=schema_file_path, database_only=False)
+            backend_data = (
+                {"config_file": config_file_path}
+                if backend == "db"
+                else {"results_file_path": results_file_path}
+            )
+            args.update(backend_data)
+            psm = SamplePipestatManager(**args)
+            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
+
+            # CHECK CREATION AND MODIFY TIME EXIST
+
+            created = psm.select_records(
+                filter_conditions=[
+                    {
+                        "key": "record_identifier",
+                        "operator": "eq",
+                        "value": rec_id,
+                    },
+                ],
+                columns=[CREATED_TIME],
+            )["records"][0][CREATED_TIME]
+
+            modified = psm.select_records(
+                filter_conditions=[
+                    {
+                        "key": "record_identifier",
+                        "operator": "eq",
+                        "value": rec_id,
+                    },
+                ],
+                columns=[MODIFIED_TIME],
+            )["records"][0][MODIFIED_TIME]
+
+            assert created is not None
+            assert modified is not None
+            assert created == modified
+            # Report new
+            val = {"number_of_things": 1}
+            time.sleep(
+                1
+            )  # The filebackend is so fast that the updated time will equal the created time
+            psm.report(record_identifier="sample1", values=val, force_overwrite=True)
+            # CHECK MODIFY TIME DIFFERS FROM CREATED TIME
+            created = psm.select_records(
+                filter_conditions=[
+                    {
+                        "key": "record_identifier",
+                        "operator": "eq",
+                        "value": rec_id,
+                    },
+                ],
+                columns=[CREATED_TIME],
+            )["records"][0][CREATED_TIME]
+
+            modified = psm.select_records(
+                filter_conditions=[
+                    {
+                        "key": "record_identifier",
+                        "operator": "eq",
+                        "value": rec_id,
+                    },
+                ],
+                columns=[MODIFIED_TIME],
+            )["records"][0][MODIFIED_TIME]
+
+            assert created != modified
 
     @pytest.mark.parametrize("backend", ["db", "file"])
     def test_list_recent_results(
         self,
         config_file_path,
         schema_file_path,
         results_file_path,
@@ -1565,15 +1625,15 @@
             results = psm.list_recent_results(start="2100-01-01 0:0:0", end="1970-01-01 0:0:0")
             assert len(results["records"]) == 10
 
 
 @pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
 @pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
 class TestSelectRecords:
-    @pytest.mark.parametrize("backend", ["db", "file"])
+    @pytest.mark.parametrize("backend", ["file", "db"])
     def test_select_records_basic(
         self,
         config_file_path,
         results_file_path,
         recursive_schema_file_path,
         backend,
         range_values,
@@ -2307,177 +2367,7 @@
                 r_id = i[0]
                 val = i[1]
                 psm.report(record_identifier=r_id, values=val, force_overwrite=True)
 
             mod = psm.backend.get_model(table_name=psm.backend.table_name)
             assert mod.md5sum.index is True
             assert mod.number_of_things.index is False
-
-
-@pytest.mark.skipif(not DB_DEPENDENCIES, reason="Requires dependencies")
-@pytest.mark.skipif(SERVICE_UNAVAILABLE, reason="requires service X to be available")
-class TestRetrieveHistory:
-    @pytest.mark.parametrize(
-        ["rec_id", "val"],
-        [
-            ("sample1", {"name_of_something": "test_name"}),
-        ],
-    )
-    @pytest.mark.parametrize("backend", ["db", "file"])
-    def test_select_history_basic(
-        self,
-        config_file_path,
-        results_file_path,
-        schema_file_path,
-        backend,
-        range_values,
-        rec_id,
-        val,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            psm = SamplePipestatManager(**args)
-
-            val["number_of_things"] = 1
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            val = {"name_of_something": "MODIFIED_test_name", "number_of_things": 2}
-
-            time.sleep(1)
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            history_result = psm.retrieve_history(
-                record_identifier="sample1", result_identifier="name_of_something"
-            )
-
-            all_history_result = psm.retrieve_history(record_identifier="sample1")
-
-            assert len(all_history_result.keys()) == 2
-            assert len(history_result.keys()) == 1
-            assert len(history_result["name_of_something"].keys()) == 1
-
-    @pytest.mark.parametrize(
-        ["rec_id", "val"],
-        [
-            ("sample1", {"name_of_something": "test_name"}),
-        ],
-    )
-    @pytest.mark.parametrize("backend", ["db", "file"])
-    def test_select_history_multi_results(
-        self,
-        config_file_path,
-        results_file_path,
-        schema_file_path,
-        backend,
-        range_values,
-        rec_id,
-        val,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            psm = SamplePipestatManager(**args)
-
-            val["number_of_things"] = 1
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            val = {"name_of_something": "MODIFIED_test_name", "number_of_things": 2}
-
-            time.sleep(1)
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            history_result = psm.retrieve_history(
-                record_identifier="sample1",
-                result_identifier=["name_of_something", "number_of_things"],
-            )
-
-            assert len(history_result.keys()) == 2
-            assert len(history_result["name_of_something"].keys()) == 1
-
-    @pytest.mark.parametrize(
-        ["rec_id", "val"],
-        [
-            (
-                "sample1",
-                {
-                    "output_image": {
-                        "path": "path_string",
-                        "thumbnail_path": "thumbnail_path_string",
-                        "title": "title_string",
-                    }
-                },
-            ),
-        ],
-    )
-    @pytest.mark.parametrize("backend", ["db", "file"])
-    def test_select_history_complex_objects(
-        self,
-        config_file_path,
-        results_file_path,
-        recursive_schema_file_path,
-        backend,
-        range_values,
-        rec_id,
-        val,
-    ):
-        with NamedTemporaryFile() as f, ContextManagerDBTesting(DB_URL):
-            results_file_path = f.name
-            args = dict(schema_path=recursive_schema_file_path, database_only=False)
-            backend_data = (
-                {"config_file": config_file_path}
-                if backend == "db"
-                else {"results_file_path": results_file_path}
-            )
-            args.update(backend_data)
-            psm = SamplePipestatManager(**args)
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            val = {
-                "output_image": {
-                    "path": "path_string2",
-                    "thumbnail_path": "thumbnail_path_string2",
-                    "title": "title_string2",
-                }
-            }
-
-            time.sleep(1)
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            val = {
-                "output_image": {
-                    "path": "path_string3",
-                    "thumbnail_path": "thumbnail_path_string3",
-                    "title": "title_string3",
-                }
-            }
-
-            time.sleep(1)
-
-            psm.report(record_identifier=rec_id, values=val, force_overwrite=True)
-
-            history_result = psm.retrieve_history(
-                record_identifier="sample1",
-                result_identifier="output_image",
-            )
-
-            assert len(history_result.keys()) == 1
-            assert "output_image" in history_result
-            assert len(history_result["output_image"].keys()) == 2
```

### Comparing `pipestat-0.9.0/tests/test_status.py` & `pipestat-0.9.0a1/tests/test_status.py`

 * *Files identical despite different names*

