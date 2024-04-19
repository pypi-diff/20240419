# Comparing `tmp/collective.elastic.ingest-2.0.1.tar.gz` & `tmp/collective_elastic_ingest-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.elastic.ingest-2.0.1.tar", last modified: Tue Jan 16 12:26:47 2024, max compression
+gzip compressed data, was "collective_elastic_ingest-2.1.0.tar", last modified: Fri Apr 19 10:09:16 2024, max compression
```

## Comparing `collective.elastic.ingest-2.0.1.tar` & `collective_elastic_ingest-2.1.0.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.641759 collective.elastic.ingest-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/CONTRIBUTORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/LICENSE.GPL
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-01-16 12:26:47.641759 collective.elastic.ingest-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20583 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.633758 collective.elastic.ingest-2.0.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.633758 collective.elastic.ingest-2.0.1/examples/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/analysis/analysis-german.json
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/analysis/elasticsearch-lexicon-german.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/analysis/mappings-german-analysis.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.637758 collective.elastic.ingest-2.0.1/examples/docker-es/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-es/.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.637758 collective.elastic.ingest-2.0.1/examples/docker-es/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-es/configuration/mappings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-es/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.637758 collective.elastic.ingest-2.0.1/examples/docker-os/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-os/.env
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-os/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.637758 collective.elastic.ingest-2.0.1/examples/docker-os/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-os/configuration/mappings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/docker-os/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.637758 collective.elastic.ingest-2.0.1/examples/local/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/local/.env-es
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/local/.env-os
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/examples/local/mappings.json
--rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 12:26:47.641759 collective.elastic.ingest-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.633758 collective.elastic.ingest-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.633758 collective.elastic.ingest-2.0.1/src/collective/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.633758 collective.elastic.ingest-2.0.1/src/collective/elastic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.641759 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/celery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/ingestion.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/plone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/plone_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/postprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5550 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessings.json
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-16 12:26:39.000000 collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/removal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 12:26:47.641759 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22713 2024-01-16 12:26:47.000000 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-01-16 12:26:47.000000 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 12:26:47.000000 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-16 12:26:47.000000 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-16 12:26:47.000000 collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.696911 collective_elastic_ingest-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/CONTRIBUTORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/LICENSE.GPL
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-04-19 10:09:16.696911 collective_elastic_ingest-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20565 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.684911 collective_elastic_ingest-2.1.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.688911 collective_elastic_ingest-2.1.0/examples/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/analysis/analysis-german.json
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/analysis/elasticsearch-keywords-german.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/analysis/elasticsearch-lexicon-german.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/analysis/mappings-german-analysis.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.688911 collective_elastic_ingest-2.1.0/examples/docker-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-es/.env
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.688911 collective_elastic_ingest-2.1.0/examples/docker-es/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-es/configuration/mappings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-es/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.688911 collective_elastic_ingest-2.1.0/examples/docker-os/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-os/.env
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-os/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.688911 collective_elastic_ingest-2.1.0/examples/docker-os/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-os/configuration/mappings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/docker-os/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.692911 collective_elastic_ingest-2.1.0/examples/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/local/.env-es
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/local/.env-os
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/examples/local/mappings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:09:16.696911 collective_elastic_ingest-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.684911 collective_elastic_ingest-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.684911 collective_elastic_ingest-2.1.0/src/collective/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.684911 collective_elastic_ingest-2.1.0/src/collective/elastic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.696911 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/celery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/deleteindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/plone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/plone_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/postprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-19 10:09:12.000000 collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/removal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:16.696911 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22579 2024-04-19 10:09:16.000000 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-19 10:09:16.000000 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:09:16.000000 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-19 10:09:16.000000 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 10:09:16.000000 collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/top_level.txt
```

### Comparing `collective.elastic.ingest-2.0.1/CHANGES.rst` & `collective_elastic_ingest-2.1.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+2.1.0 (2024-04-19)
+------------------
+
+- "behaviors/plone.categorization/subjects" both searchable and also usable as facet. [ksuess]
+- Add celery task "deleteindex". [ksuess]
+- Fix field type of review_state to keyword: review_state can be used as facet. [ksuess]
+- Update analysis example configuration. [ksuess]
+
+
 2.0.1 (2024-01-16)
 ------------------
 
 - Fix: Do not fail on `field_remove` or `full_remove` if section or name does not exist. [jensens]
 - Fix: Fail and exit worker if there is `mappings.json` is missing or has a syntax error. [jensens]
 - Enhancement: additional_schema documentation. [jensens]
```

### Comparing `collective.elastic.ingest-2.0.1/CONTRIBUTING.md` & `collective_elastic_ingest-2.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/LICENSE.GPL` & `collective_elastic_ingest-2.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/LICENSE.rst` & `collective_elastic_ingest-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/PKG-INFO` & `collective_elastic_ingest-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: collective.elastic.ingest
-Version: 2.0.1
+Version: 2.1.0
 Summary: Ingestion service queue runner between Plone RestAPI and ElasticSearch or OpenSearch.
 Author: Katja Süss, Peter Holzer
 Author-email: Jens Klein <jk@kleinundpartner.at>
 Maintainer-email: Jens Klein <jk@kleinundpartner.at>
 License: GPL 2.0
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.ingest
 Project-URL: Changelog, https://github.com/collective/collective.elastic.ingest/blob/main/CHANGES.rst
 Project-URL: Source, https://github.com/collective/collective.elastic.ingest
 Project-URL: Issues, https://github.com/collective/collective.elastic.ingest/issues
 Keywords: elasticsearch,opensearch,plone,celery,search,indexer
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 5.2
-Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
@@ -310,15 +307,15 @@
 ``rewrite``
     Moves content data from one position in the field-tree to another.
     The configuration must be a mapping with ``source`` and ``target`` keys.
     The value of ``source`` is the path to the data to move.
     The value of ``target`` is the path to the new location of the data (missing containers are created).
     The value of ``enforce`` is a boolean value (default: False). If True, the source must exist, otherwise an error is raised.
 
-    Example: ``"configuration": {"source": "@components/collectiveelastic/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
+    Example: ``"configuration": {"source": "@components/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
 
 ``remove``
     Deletes a field or sub-field from the content data.
     The value of ``target`` is the path to the data to delete.
 
 ``field_remove``
     Deletes a field from the full schema and its field value from the content.
```

### Comparing `collective.elastic.ingest-2.0.1/README.rst` & `collective_elastic_ingest-2.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -260,15 +260,15 @@
 ``rewrite``
     Moves content data from one position in the field-tree to another.
     The configuration must be a mapping with ``source`` and ``target`` keys.
     The value of ``source`` is the path to the data to move.
     The value of ``target`` is the path to the new location of the data (missing containers are created).
     The value of ``enforce`` is a boolean value (default: False). If True, the source must exist, otherwise an error is raised.
 
-    Example: ``"configuration": {"source": "@components/collectiveelastic/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
+    Example: ``"configuration": {"source": "@components/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
 
 ``remove``
     Deletes a field or sub-field from the content data.
     The value of ``target`` is the path to the data to delete.
 
 ``field_remove``
     Deletes a field from the full schema and its field value from the content.
```

### Comparing `collective.elastic.ingest-2.0.1/examples/analysis/analysis-german.json` & `collective_elastic_ingest-2.1.0/examples/analysis/analysis-german.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9338541666666667%*

 * *Differences: {"'settings'": "{'analysis': {'analyzer': {'german_analyzer': {'filter': {insert: [(2, "*

 * *               "'no_stem')], delete: [3]}}, 'german_exact_analyzer': OrderedDict([('tokenizer', "*

 * *               "'standard'), ('filter', ['lowercase'])]), delete: ['german_exact']}, 'filter': "*

 * *               "{'custom_dictionary_decompounder': {'word_list_path': "*

 * *               "'elasticsearch-lexicon-german.txt'}, 'no_stem': OrderedDict([('type', "*

 * *               "'keyword_marker'), ('keywords_path', 'elasticsearch- […]*

```diff
@@ -2,32 +2,36 @@
     "settings": {
         "analysis": {
             "analyzer": {
                 "german_analyzer": {
                     "filter": [
                         "lowercase",
                         "custom_dictionary_decompounder",
-                        "light_german_stemmer",
-                        "unique"
+                        "no_stem",
+                        "light_german_stemmer"
                     ],
                     "tokenizer": "standard"
                 },
-                "german_exact": {
+                "german_exact_analyzer": {
                     "filter": [
                         "lowercase"
                     ],
                     "tokenizer": "standard"
                 }
             },
             "filter": {
                 "custom_dictionary_decompounder": {
                     "type": "dictionary_decompounder",
-                    "word_list_path": "elasticsearch-lexicon.txt"
+                    "word_list_path": "elasticsearch-lexicon-german.txt"
                 },
                 "light_german_stemmer": {
                     "language": "light_german",
                     "type": "stemmer"
+                },
+                "no_stem": {
+                    "keywords_path": "elasticsearch-keywords-german.txt",
+                    "type": "keyword_marker"
                 }
             }
         }
     }
 }
```

### Comparing `collective.elastic.ingest-2.0.1/examples/analysis/mappings-german-analysis.json` & `collective_elastic_ingest-2.1.0/examples/analysis/mappings-german-analysis.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8245923913043478%*

 * *Differences: {"'behaviors/plone.categorization/subjects'": "{'fields': {'keyword': OrderedDict([('type', "*

 * *                                              "'keyword')])}}",*

 * * "'plone.namedfile.field.NamedBlobFile'": "{'pipeline': {'type': {delete: ['include_in_parent']}}}",*

 * * 'delete': "['behaviors/plone.basic/title', 'behaviors/plone.basic/description', "*

 * *           "'blocks_plaintext', 'behaviors/plone.allowdiscussion/allow_discussion']"}*

```diff
@@ -1,54 +1,18 @@
 {
-    "behaviors/plone.allowdiscussion/allow_discussion": {
-        "type": "boolean"
-    },
-    "behaviors/plone.basic/description": {
-        "analyzer": "german_analyzer",
-        "fields": {
-            "exact": {
-                "analyzer": "german_exact_analyzer",
-                "term_vector": "with_positions_offsets",
-                "type": "text"
-            }
-        },
-        "term_vector": "with_positions_offsets",
-        "type": "text"
-    },
-    "behaviors/plone.basic/title": {
-        "analyzer": "german_analyzer",
-        "fields": {
-            "exact": {
-                "analyzer": "german_exact_analyzer",
-                "term_vector": "with_positions_offsets",
-                "type": "text"
-            }
-        },
-        "term_vector": "with_positions_offsets",
-        "type": "text"
-    },
     "behaviors/plone.categorization/subjects": {
         "analyzer": "german_analyzer",
         "fields": {
             "exact": {
                 "analyzer": "german_exact_analyzer",
                 "term_vector": "with_positions_offsets",
                 "type": "text"
-            }
-        },
-        "term_vector": "with_positions_offsets",
-        "type": "text"
-    },
-    "blocks_plaintext": {
-        "analyzer": "german_analyzer",
-        "fields": {
-            "exact": {
-                "analyzer": "german_exact_analyzer",
-                "term_vector": "with_positions_offsets",
-                "type": "text"
+            },
+            "keyword": {
+                "type": "keyword"
             }
         },
         "term_vector": "with_positions_offsets",
         "type": "text"
     },
     "plone.app.textfield.RichText": {
         "definition": {
@@ -162,15 +126,14 @@
                     }
                 }
             ],
             "source": "{name}__data",
             "target": "{name}__extracted",
             "type": {
                 "dynamic": false,
-                "include_in_parent": true,
                 "properties": {
                     "author": {
                         "type": "text"
                     },
                     "content": {
                         "type": "text"
                     },
```

### Comparing `collective.elastic.ingest-2.0.1/examples/docker-es/configuration/mappings.json` & `collective_elastic_ingest-2.1.0/examples/docker-es/configuration/mappings.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/docker-es/docker-compose.yml` & `collective_elastic_ingest-2.1.0/examples/docker-es/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/docker-os/configuration/mappings.json` & `collective_elastic_ingest-2.1.0/examples/docker-os/configuration/mappings.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/docker-os/docker-compose.yml` & `collective_elastic_ingest-2.1.0/examples/docker-os/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/local/.env-es` & `collective_elastic_ingest-2.1.0/examples/local/.env-es`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/local/.env-os` & `collective_elastic_ingest-2.1.0/examples/local/.env-os`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/examples/local/mappings.json` & `collective_elastic_ingest-2.1.0/examples/local/mappings.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/pyproject.toml` & `collective_elastic_ingest-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "collective.elastic.ingest"
-version = "2.0.1"
+version = "2.1.0"
 description = "Ingestion service queue runner between Plone RestAPI and ElasticSearch or OpenSearch."
 keywords = ["elasticsearch", "opensearch", "plone", "celery", "search", "indexer"]
 readme = "README.rst"
 maintainers = [
     {name = "Jens Klein", email = "jk@kleinundpartner.at"},
 ]
 authors = [
@@ -13,17 +13,14 @@
     {name = "Peter Holzer"},
 ]
 requires-python = ">=3.8"
 license = { text = "GPL 2.0" }
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Plone",
-    "Framework :: Plone :: Addon",
-    "Framework :: Plone :: 5.2",
-    "Framework :: Plone :: 6.0",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/analysis.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/analysis.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/celery.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/celery.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from .deleteindex import delete_index
 from .ingestion import process_ingest
 from .logging import logger
 from .plone import fetch_content
 from .plone import fetch_schema
 from .removal import remove
 from celery import Celery
 
@@ -80,7 +81,21 @@
         sys.exit(1)
     except Exception:
         # xxx: retry handling!
         msg = "Error while removing data from ElasticSearch"
         logger.exception(msg)
         return msg
     return "unindexed {}".format(uid)
+
+
+@app.task(name="collective.elastic.ingest.deleteindex")
+def deleteindex(index_name):
+    try:
+        delete_index(index_name)
+    except RuntimeError:
+        logger.error("Fatal error, stop worker")
+        sys.exit(1)
+    except Exception:
+        msg = "Error while deleting index '{}'".format(index_name)
+        logger.exception(msg)
+        return msg
+    return "Index deleted: {}".format(index_name)
```

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/client.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/client.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/ingestion.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/ingestion.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/mapping.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/mapping.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/plone.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/plone.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/plone_test.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/plone_test.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/postprocessing.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/postprocessing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/postprocessing_test.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/postprocessing_test.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessing.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessing_test.py` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.ingest-2.0.1/src/collective/elastic/ingest/preprocessings.json` & `collective_elastic_ingest-2.1.0/src/collective/elastic/ingest/preprocessings.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9023297491039426%*

 * *Differences: {'9': "{'configuration': {'source': '@components/blocks_plaintext'}}",*

 * * 'insert': "[(11, OrderedDict([('comment', '... needs this information, essential rewrite, do not "*

 * *           "remove'), ('action', 'rewrite'), ('configuration', OrderedDict([('source', "*

 * *           "'@components/collectiveelastic/section_id'), ('target', 'section'), ('enforce', "*

 * *           "True)]))])), (12, OrderedDict([('comment', 'Schema for above section_id, do not "*

 * *           "remove'), ('action', 'additional_schema'), ('configu […]*

```diff
@@ -63,27 +63,44 @@
         }
     },
     {
         "action": "rewrite",
         "comment": "If Volto is available, this is important for full text search, do not remove unless in Classic UI only environments",
         "configuration": {
             "enforce": false,
-            "source": "@components/collectiveelastic/blocks_plaintext",
+            "source": "@components/blocks_plaintext",
             "target": "blocks_plaintext"
         }
     },
     {
         "action": "additional_schema",
         "comment": "If Volto is available, this is important for full text search, do not remove unless in Classic UI only environments",
         "configuration": {
             "field": "zope.schema._bootstrapfields.Text",
             "name": "blocks_plaintext"
         }
     },
     {
+        "action": "rewrite",
+        "comment": "... needs this information, essential rewrite, do not remove",
+        "configuration": {
+            "enforce": true,
+            "source": "@components/collectiveelastic/section_id",
+            "target": "section"
+        }
+    },
+    {
+        "action": "additional_schema",
+        "comment": "Schema for above section_id, do not remove",
+        "configuration": {
+            "field": "zope.schema._field.ASCIILine",
+            "name": "section"
+        }
+    },
+    {
         "action": "full_remove",
         "comment": "If volto.blocks is available, remove all its fields.",
         "configuration": {
             "name": "volto.blocks",
             "section": "behaviors"
         }
     },
@@ -207,9 +224,17 @@
         "action": "field_remove",
         "comment": "No need for plone.layoutaware (Mosaic) layout related.",
         "configuration": {
             "field": "sectionSiteLayout",
             "name": "plone.layoutaware",
             "section": "behaviors"
         }
+    },
+    {
+        "action": "additional_schema",
+        "comment": "Fix field type of review_state to keyword",
+        "configuration": {
+            "field": "zope.schema._field.ASCIILine",
+            "name": "review_state"
+        }
     }
 ]
```

### Comparing `collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/PKG-INFO` & `collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: collective.elastic.ingest
-Version: 2.0.1
+Version: 2.1.0
 Summary: Ingestion service queue runner between Plone RestAPI and ElasticSearch or OpenSearch.
 Author: Katja Süss, Peter Holzer
 Author-email: Jens Klein <jk@kleinundpartner.at>
 Maintainer-email: Jens Klein <jk@kleinundpartner.at>
 License: GPL 2.0
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.ingest
 Project-URL: Changelog, https://github.com/collective/collective.elastic.ingest/blob/main/CHANGES.rst
 Project-URL: Source, https://github.com/collective/collective.elastic.ingest
 Project-URL: Issues, https://github.com/collective/collective.elastic.ingest/issues
 Keywords: elasticsearch,opensearch,plone,celery,search,indexer
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: Addon
-Classifier: Framework :: Plone :: 5.2
-Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
@@ -310,15 +307,15 @@
 ``rewrite``
     Moves content data from one position in the field-tree to another.
     The configuration must be a mapping with ``source`` and ``target`` keys.
     The value of ``source`` is the path to the data to move.
     The value of ``target`` is the path to the new location of the data (missing containers are created).
     The value of ``enforce`` is a boolean value (default: False). If True, the source must exist, otherwise an error is raised.
 
-    Example: ``"configuration": {"source": "@components/collectiveelastic/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
+    Example: ``"configuration": {"source": "@components/blocks_plaintext",  "target": "blocks_plaintext", "enforce": false}``
 
 ``remove``
     Deletes a field or sub-field from the content data.
     The value of ``target`` is the path to the data to delete.
 
 ``field_remove``
     Deletes a field from the full schema and its field value from the content.
```

### Comparing `collective.elastic.ingest-2.0.1/src/collective.elastic.ingest.egg-info/SOURCES.txt` & `collective_elastic_ingest-2.1.0/src/collective.elastic.ingest.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CONTRIBUTORS.rst
 LICENSE.GPL
 LICENSE.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 examples/analysis/analysis-german.json
+examples/analysis/elasticsearch-keywords-german.txt
 examples/analysis/elasticsearch-lexicon-german.txt
 examples/analysis/mappings-german-analysis.json
 examples/docker-es/.env
 examples/docker-es/docker-compose.yml
 examples/docker-es/configuration/mappings.json
 examples/docker-os/.env
 examples/docker-os/Dockerfile
@@ -24,14 +25,15 @@
 src/collective.elastic.ingest.egg-info/dependency_links.txt
 src/collective.elastic.ingest.egg-info/requires.txt
 src/collective.elastic.ingest.egg-info/top_level.txt
 src/collective/elastic/ingest/__init__.py
 src/collective/elastic/ingest/analysis.py
 src/collective/elastic/ingest/celery.py
 src/collective/elastic/ingest/client.py
+src/collective/elastic/ingest/deleteindex.py
 src/collective/elastic/ingest/elastic.py
 src/collective/elastic/ingest/ingestion.py
 src/collective/elastic/ingest/logging.py
 src/collective/elastic/ingest/mapping.py
 src/collective/elastic/ingest/plone.py
 src/collective/elastic/ingest/plone_test.py
 src/collective/elastic/ingest/postprocessing.py
```

