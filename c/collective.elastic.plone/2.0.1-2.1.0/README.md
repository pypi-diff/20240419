# Comparing `tmp/collective.elastic.plone-2.0.1.tar.gz` & `tmp/collective_elastic_plone-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.elastic.plone-2.0.1.tar", last modified: Tue Mar  5 10:46:39 2024, max compression
+gzip compressed data, was "collective_elastic_plone-2.1.0.tar", last modified: Fri Apr 19 10:09:41 2024, max compression
```

## Comparing `collective.elastic.plone-2.0.1.tar` & `collective_elastic_plone-2.1.0.tar`

### file list

```diff
@@ -1,74 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/DEVELOP.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/LICENSE.GPL
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.820033 collective.elastic.plone-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.820033 collective.elastic.plone-2.0.1/src/collective/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.820033 collective.elastic.plone-2.0.1/src/collective/elastic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/configure.zcml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/browser/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/configure.zcml
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/eslib.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/collective.es.plone.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.820033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/en/LC_MESSAGES/collective.es.plone.po
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/update.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/update.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.820033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/default/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/default/browserlayer.xml
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/default/catalog.xml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/default/metadata.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.828033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/uninstall/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/uninstall/browserlayer.xml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/uninstall/catalog.xml
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/proxyindex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/queueprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/configure.zcml
--rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/expansions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/configure.zcml
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/post.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/request_example.json
--rw-r--r--   0 runner    (1001) docker     (127)    31883 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/response_example.json
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/setuphandlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/upgrades.zcml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/addIndex.zpt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/index.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/manageIndex.zpt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10259 2024-03-05 10:46:39.000000 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-03-05 10:46:39.000000 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 10:46:39.000000 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-05 10:46:39.000000 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-05 10:46:39.000000 collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 10:46:39.832033 collective.elastic.plone-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/tests/test_proxyindex.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/tests/test_restapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-05 10:46:36.000000 collective.elastic.plone-2.0.1/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/DEVELOP.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/LICENSE.GPL
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.057964 collective_elastic_plone-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.057964 collective_elastic_plone-2.1.0/src/collective/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.057964 collective_elastic_plone-2.1.0/src/collective/elastic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.061964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/configure.zcml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/browser/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/configure.zcml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/collective.es.plone.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.057964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/en/LC_MESSAGES/collective.es.plone.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/update.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      494 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/update.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.057964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/default/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/default/browserlayer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/default/catalog.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/default/metadata.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/monolingual/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/monolingual/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/monolingual/registry.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/multilingual/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/multilingual/metadata.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/multilingual/registry.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/uninstall/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/uninstall/catalog.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/proxyindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/queueprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.065964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/configure.zcml
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/expansions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/configure.zcml
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/request_example.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31883 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/response_example.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/setuphandlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/upgrades.zcml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/addIndex.zpt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/index.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/manageIndex.zpt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-19 10:09:41.000000 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-19 10:09:41.000000 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:09:41.000000 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 10:09:41.000000 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 10:09:41.000000 collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:09:41.069964 collective_elastic_plone-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/tests/test_proxyindex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/tests/test_restapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-19 10:09:37.000000 collective_elastic_plone-2.1.0/tests/test_setup.py
```

### Comparing `collective.elastic.plone-2.0.1/CHANGES.rst` & `collective_elastic_plone-2.1.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+2.1.0 (2024-04-19)
+------------------
+
+- Add profiles for testing monolingual and multilingual. [ksuess]
+- Add @@clear-and-update-index-server-index. [ksuess]
+- Fix error handling in REST API service @kitsearch [ksuess]
+
+
 2.0.1 (2024-02-05)
 ------------------
 
 - Dev/CI/CD: Update Makefile and configuration.
   [thet, jensens]
 - Documentation: Clarify procedure to update/initialize the Open-/ElasticSearch with data. [jensens]
 - Fix: Kitsearch security check AttributeError [jensens]
```

### Comparing `collective.elastic.plone-2.0.1/DEVELOP.rst` & `collective_elastic_plone-2.1.0/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/LICENSE.GPL` & `collective_elastic_plone-2.1.0/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/LICENSE.rst` & `collective_elastic_plone-2.1.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/PKG-INFO` & `collective_elastic_plone-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: collective.elastic.plone
-Version: 2.0.1
+Version: 2.1.0
 Summary: Plone Search Integration: Addon to index content in Open-/ElasticSearch
 Author: Jens Klein, Katja Süss, Peter Holzer
 Maintainer-email: Jens Klein <jk@kleinundpartner.at>
 License: GPL 2.0
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.plone
 Project-URL: Changelog, https://github.com/collective/collective.elastic.plone/blob/main/CHANGES.rst
 Project-URL: Source, https://github.com/collective/collective.elastic.plone
 Project-URL: Issues, https://github.com/collective/collective.elastic.plone/issues
 Keywords: elasticsearch,opensearch,plone,celery,search,indexer
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 Requires-Dist: plone.restapi
-Requires-Dist: collective.elastic.ingest>=2.0.0rc9
+Requires-Dist: collective.elastic.ingest>=2.1.0
 Requires-Dist: jinja2
 Requires-Dist: deepmerge
 Provides-Extra: redis
 Requires-Dist: collective.elastic.ingest[redis]; extra == "redis"
 Provides-Extra: rabbitmq
 Requires-Dist: collective.elastic.ingest[rabbitmq]; extra == "rabbitmq"
 Provides-Extra: opensearch
@@ -143,15 +144,15 @@
 After Startup
 -------------
 
 After startup you need to install the addon in Plone via the Addons control panel.
 This replaces the SearchableText index with the proxy index and a minimal configuration.
 Best is to alter the configuration to the projects needs.
 
-To index all content in the catalog, append ``/@@update-elasticsearch`` to the URL of your Plone site.
+To index all content in the catalog, append ``/@@update-index-server-index`` to the URL of your Plone site.
 This queues all content for indexing in ElasticSearch (but not in the ZCatalog).
 Alternatively a reindex catalog (in ZMI under advanced tab) works too.
 
 New or modified content is queued for indexing automatically.
 
 
 --------------
@@ -159,15 +160,15 @@
 --------------
 
 The proxy index works out of the box in Volto.
 
 However, in Volto a direct (and much faster) search is possible by using the ``@kitsearch`` endpoint, bypassing the catalog.
 The endpoint takes a native Open-/ ElasticSearch query and returns the results with Plone permission check.
 
-The Volto add-on `volto-searchkit-block <https://github.com/rohberg/volto-searchkit-block/>`_ (based on `react-searchkit <https://www.npmjs.com/package/react-searchkit>`_) provides a configurable block using this endpoint.
+The Volto add-on `volto-searchkit-block <https://www.npmjs.com/package/@rohberg/volto-searchkit-block>`_ provides a configurable block using this endpoint.
 
 Remark:
 For security reasons, in collective.elastic.plone 2.0.0 the ``@kitsearch`` endpoint always overrides any "API URL" and "API index" settings with the configured values from the environment.
 
 Configuration
 =============
```

### Comparing `collective.elastic.plone-2.0.1/README.rst` & `collective_elastic_plone-2.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 After Startup
 -------------
 
 After startup you need to install the addon in Plone via the Addons control panel.
 This replaces the SearchableText index with the proxy index and a minimal configuration.
 Best is to alter the configuration to the projects needs.
 
-To index all content in the catalog, append ``/@@update-elasticsearch`` to the URL of your Plone site.
+To index all content in the catalog, append ``/@@update-index-server-index`` to the URL of your Plone site.
 This queues all content for indexing in ElasticSearch (but not in the ZCatalog).
 Alternatively a reindex catalog (in ZMI under advanced tab) works too.
 
 New or modified content is queued for indexing automatically.
 
 
 --------------
@@ -112,15 +112,15 @@
 --------------
 
 The proxy index works out of the box in Volto.
 
 However, in Volto a direct (and much faster) search is possible by using the ``@kitsearch`` endpoint, bypassing the catalog.
 The endpoint takes a native Open-/ ElasticSearch query and returns the results with Plone permission check.
 
-The Volto add-on `volto-searchkit-block <https://github.com/rohberg/volto-searchkit-block/>`_ (based on `react-searchkit <https://www.npmjs.com/package/react-searchkit>`_) provides a configurable block using this endpoint.
+The Volto add-on `volto-searchkit-block <https://www.npmjs.com/package/@rohberg/volto-searchkit-block>`_ provides a configurable block using this endpoint.
 
 Remark:
 For security reasons, in collective.elastic.plone 2.0.0 the ``@kitsearch`` endpoint always overrides any "API URL" and "API index" settings with the configured values from the environment.
 
 Configuration
 =============
```

### Comparing `collective.elastic.plone-2.0.1/pyproject.toml` & `collective_elastic_plone-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "collective.elastic.plone"
-version = "2.0.1"
+version = "2.1.0"
 description = "Plone Search Integration: Addon to index content in Open-/ElasticSearch"
 keywords = ["elasticsearch", "opensearch", "plone", "celery", "search", "indexer"]
 readme = "README.rst"
 maintainers = [
     {name = "Jens Klein", email = "jk@kleinundpartner.at"},
 ]
 authors = [
@@ -15,26 +15,27 @@
 requires-python = ">=3.9"
 license = { text = "GPL 2.0" }
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Plone",
     "Framework :: Plone :: Addon",
     "Framework :: Plone :: 6.0",
+    "Framework :: Plone :: 6.1",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Development Status :: 5 - Production/Stable",
 ]
 dependencies = [
     "plone.restapi",  # pulls in whole Products.CMFPlone too
-    "collective.elastic.ingest>=2.0.0rc9",
+    "collective.elastic.ingest>=2.1.0",
     "jinja2",
     "deepmerge",
 ]
 
 [project.urls]
 PyPI = "https://pypi.python.org/pypi/collective.elastic.plone"
 Changelog = "https://github.com/collective/collective.elastic.plone/blob/main/CHANGES.rst"
```

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/__init__.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/__init__.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/configure.zcml` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/configure.zcml`

 * *Files 17% similar despite different names*

```diff
@@ -31,14 +31,32 @@
       title="OpenSearch/ Elasticsearch indexer and index (uninstall)"
       directory="profiles/uninstall"
       description="Uninstalls the collective.elastic.plone add-on."
       provides="Products.GenericSetup.interfaces.EXTENSION"
       post_handler=".setuphandlers.uninstall"
       />
 
+  <genericsetup:registerProfile
+      name="singlelingual"
+      title="Testing profile monolingual"
+      directory="profiles/monolingual"
+      description="Sets language to german"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      post_handler=".setuphandlers.post_install"
+      />
+
+  <genericsetup:registerProfile
+      name="multilingual"
+      title="Testing profile multilingual en/de"
+      directory="profiles/multilingual"
+      description="Makes site multilingual with languages english/german"
+      provides="Products.GenericSetup.interfaces.EXTENSION"
+      post_handler=".setuphandlers.post_install"
+      />
+
   <utility
       factory=".setuphandlers.HiddenProfiles"
       name="collective.elastic.plone-hiddenprofiles"
       />
 
   <!-- -*- extra stuff goes here -*- -->
```

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/README.rst` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/README.rst`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/locales/update.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/locales/update.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/profiles/default/catalog.xml` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/profiles/default/catalog.xml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/proxyindex.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/proxyindex.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/queueprocessor.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/queueprocessor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 from . import INDEX_NAME
 from .interfaces import IElasticSearchIndexQueueProcessor
 from collective.elastic.ingest.celery import index
 from collective.elastic.ingest.celery import unindex
 from kombu.exceptions import OperationalError
 from plone import api
+from plone.api.exc import CannotGetPortalError
 from plone.dexterity.interfaces import IDexterityContent
+from Products.CMFCore.utils import getToolByName
 from Products.GenericSetup.tool import UNKNOWN
 from zope.annotation import IAnnotations
 from zope.interface import implementer
 
 import logging
 import time
 
 
-logger = logging.getLogger("collective.elastic.index")
+logger = logging.getLogger("collective.elastic.plone")
 
 
 @implementer(IElasticSearchIndexQueueProcessor)
 class ElasticSearchIndexQueueProcessor:
     """a queue processor for Open-/ElasticSearch"""
 
-    def _active(self):
-        portal_setup = api.portal.get_tool("portal_setup")
+    def _active(self, obj=None):
+        try:
+            portal_setup = api.portal.get_tool("portal_setup")
+        except CannotGetPortalError:
+            """Applying profile "plone.volto:multilingual" during set up
+            of robot server fails on creating/indexing language
+            infrastructure content.
+            """
+            portal_setup = getToolByName(obj, "portal_setup")
+
         return (
-            portal_setup.getLastVersionForProfile("collective.elastic.plone:default")
+            portal_setup.getLastVersionForProfile(
+                "collective.elastic.plone:default")
             != UNKNOWN
         )
 
     def index(self, obj, attributes=None):
-        if not self._active() or not IDexterityContent.providedBy(obj):
+        if not self._active(obj) or not IDexterityContent.providedBy(obj):
             return
         # get transaction id
         ts = time.time()
         annotations = IAnnotations(obj)
         annotations["ELASTIC_LAST_INDEXING_QUEUED_TIMESTAMP"] = ts
         index.delay("/".join(obj.getPhysicalPath()), ts, INDEX_NAME)
 
     def reindex(self, obj, attributes=None, update_metadata=1):
-        if not self._active():
+        if not self._active(obj):
+            logger.error(f"Reindexing of {obj} failed.'")
             return
         try:
             self.index(obj, attributes)
         except OperationalError as e:
             logger.exception(
                 f"ElasticSearchIndexQueueProcessor. Reindexing failed: {str(e)}. "
                 "Check Open-/ ElasticSearch configuration."
             )
 
     def unindex(self, obj):
-        if not self._active():
+        if not self._active(obj):
             return
         uid = api.content.get_uuid(obj)
         unindex.delay(uid, INDEX_NAME)
 
     def begin(self):
         pass
```

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/blocks.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/blocks.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/configure.zcml` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/expansions.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/expansions.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/post.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/post.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,53 +24,41 @@
 logger = logging.getLogger(__name__)
 
 
 class Kitsearch(Service):
     """Request to Open-/ElasticSearch
 
     Args:
-        query (dict): elasticsearch_url, INDEX_NAME, elasticsearch_payload (query)
+        (dict): elasticsearch_payload (query. See request_example.json)
     """
 
     def reply(self):
         data = json_body(self.request)
 
         if not data:
             return {}
 
         return self.search(self._extend_es_query(data))
 
     def search(self, data):
         """Fetch with Python elasticsearch module."""
-        # for security reasons we do not allow to pass the index name and the elasticsearch_url
-        # in the request body. Instead we use the values from the config.
+        # For security reasons we do not allow to pass the
+        # index name and the elasticsearch_url in the request body.
+        # Instead we use the values from the config.
 
         query_body = data.get("elasticsearch_payload", {})
 
-        es_kwargs = dict(
+        search_kwargs = dict(
             index=INDEX_NAME,
             body=query_body,
         )
         if not query_body.get("size", None):
-            es_kwargs["size"] = 10
-        es = get_client()
-        try:
-            result = es.search(**es_kwargs)
-        except RequestError as e:
-            self.request.response.setStatus(500)
-            return dict(error=dict(message=e.message))
-        except TransportError as e:
-            self.request.response.setStatus(503)
-            return dict(error=dict(message=e.message))
-        except NotFoundError as e:
-            self.request.response.setStatus(404)
-            return dict(error=dict(message=e.body["error"]["reason"]))
-        except Exception as e:
-            self.request.response.setStatus(500)
-            return dict(error=dict(message=e.message))
+            search_kwargs["size"] = 10
+        indexer_client = get_client()
+        result = indexer_client.search(**search_kwargs)
         # result is of type ObjectApiResponse
         return dict(result)
 
     def _extend_es_query(self, esquery):
         """Extend query with roles, user and groups."""
         if getSecurityManager().checkPermission("Manage portal", self.context):
             # god-mode: query without allowedRolesAndUsers
```

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/request_example.json` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/request_example.json`

 * *Files 5% similar despite different names*

```diff
@@ -170,11 +170,9 @@
                             }
                         },
                     }
                 },
                 "filter": {"match_all": {}},
             },
         },
-    },
-    "elasticsearch_url": "http://localhost:9200",
-    "elasticsearch_index": "plone2020",
+    }
 }
```

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/kitsearch/response_example.json` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/kitsearch/response_example.json`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/schema.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/schema.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/restapi/service.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/restapi/service.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/setuphandlers.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/testing.py` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/testing.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/addIndex.zpt` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/addIndex.zpt`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective/elastic/plone/www/manageIndex.zpt` & `collective_elastic_plone-2.1.0/src/collective/elastic/plone/www/manageIndex.zpt`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/PKG-INFO` & `collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: collective.elastic.plone
-Version: 2.0.1
+Version: 2.1.0
 Summary: Plone Search Integration: Addon to index content in Open-/ElasticSearch
 Author: Jens Klein, Katja Süss, Peter Holzer
 Maintainer-email: Jens Klein <jk@kleinundpartner.at>
 License: GPL 2.0
 Project-URL: PyPI, https://pypi.python.org/pypi/collective.elastic.plone
 Project-URL: Changelog, https://github.com/collective/collective.elastic.plone/blob/main/CHANGES.rst
 Project-URL: Source, https://github.com/collective/collective.elastic.plone
 Project-URL: Issues, https://github.com/collective/collective.elastic.plone/issues
 Keywords: elasticsearch,opensearch,plone,celery,search,indexer
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 6.0
+Classifier: Framework :: Plone :: 6.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.GPL
 License-File: LICENSE.rst
 Requires-Dist: plone.restapi
-Requires-Dist: collective.elastic.ingest>=2.0.0rc9
+Requires-Dist: collective.elastic.ingest>=2.1.0
 Requires-Dist: jinja2
 Requires-Dist: deepmerge
 Provides-Extra: redis
 Requires-Dist: collective.elastic.ingest[redis]; extra == "redis"
 Provides-Extra: rabbitmq
 Requires-Dist: collective.elastic.ingest[rabbitmq]; extra == "rabbitmq"
 Provides-Extra: opensearch
@@ -143,15 +144,15 @@
 After Startup
 -------------
 
 After startup you need to install the addon in Plone via the Addons control panel.
 This replaces the SearchableText index with the proxy index and a minimal configuration.
 Best is to alter the configuration to the projects needs.
 
-To index all content in the catalog, append ``/@@update-elasticsearch`` to the URL of your Plone site.
+To index all content in the catalog, append ``/@@update-index-server-index`` to the URL of your Plone site.
 This queues all content for indexing in ElasticSearch (but not in the ZCatalog).
 Alternatively a reindex catalog (in ZMI under advanced tab) works too.
 
 New or modified content is queued for indexing automatically.
 
 
 --------------
@@ -159,15 +160,15 @@
 --------------
 
 The proxy index works out of the box in Volto.
 
 However, in Volto a direct (and much faster) search is possible by using the ``@kitsearch`` endpoint, bypassing the catalog.
 The endpoint takes a native Open-/ ElasticSearch query and returns the results with Plone permission check.
 
-The Volto add-on `volto-searchkit-block <https://github.com/rohberg/volto-searchkit-block/>`_ (based on `react-searchkit <https://www.npmjs.com/package/react-searchkit>`_) provides a configurable block using this endpoint.
+The Volto add-on `volto-searchkit-block <https://www.npmjs.com/package/@rohberg/volto-searchkit-block>`_ provides a configurable block using this endpoint.
 
 Remark:
 For security reasons, in collective.elastic.plone 2.0.0 the ``@kitsearch`` endpoint always overrides any "API URL" and "API index" settings with the configured values from the environment.
 
 Configuration
 =============
```

### Comparing `collective.elastic.plone-2.0.1/src/collective.elastic.plone.egg-info/SOURCES.txt` & `collective_elastic_plone-2.1.0/src/collective.elastic.plone.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/collective.elastic.plone.egg-info/PKG-INFO
 src/collective.elastic.plone.egg-info/SOURCES.txt
 src/collective.elastic.plone.egg-info/dependency_links.txt
 src/collective.elastic.plone.egg-info/requires.txt
 src/collective.elastic.plone.egg-info/top_level.txt
 src/collective/elastic/plone/__init__.py
 src/collective/elastic/plone/configure.zcml
-src/collective/elastic/plone/eslib.py
 src/collective/elastic/plone/interfaces.py
 src/collective/elastic/plone/proxyindex.py
 src/collective/elastic/plone/queueprocessor.py
 src/collective/elastic/plone/setuphandlers.py
 src/collective/elastic/plone/testing.py
 src/collective/elastic/plone/upgrades.py
 src/collective/elastic/plone/upgrades.zcml
@@ -29,14 +28,18 @@
 src/collective/elastic/plone/locales/collective.es.plone.pot
 src/collective/elastic/plone/locales/update.py
 src/collective/elastic/plone/locales/update.sh
 src/collective/elastic/plone/locales/en/LC_MESSAGES/collective.es.plone.po
 src/collective/elastic/plone/profiles/default/browserlayer.xml
 src/collective/elastic/plone/profiles/default/catalog.xml
 src/collective/elastic/plone/profiles/default/metadata.xml
+src/collective/elastic/plone/profiles/monolingual/metadata.xml
+src/collective/elastic/plone/profiles/monolingual/registry.xml
+src/collective/elastic/plone/profiles/multilingual/metadata.xml
+src/collective/elastic/plone/profiles/multilingual/registry.xml
 src/collective/elastic/plone/profiles/uninstall/browserlayer.xml
 src/collective/elastic/plone/profiles/uninstall/catalog.xml
 src/collective/elastic/plone/restapi/__init__.py
 src/collective/elastic/plone/restapi/blocks.py
 src/collective/elastic/plone/restapi/configure.zcml
 src/collective/elastic/plone/restapi/expansions.py
 src/collective/elastic/plone/restapi/schema.py
```

### Comparing `collective.elastic.plone-2.0.1/tests/test_proxyindex.py` & `collective_elastic_plone-2.1.0/tests/test_proxyindex.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/tests/test_restapi.py` & `collective_elastic_plone-2.1.0/tests/test_restapi.py`

 * *Files identical despite different names*

### Comparing `collective.elastic.plone-2.0.1/tests/test_setup.py` & `collective_elastic_plone-2.1.0/tests/test_setup.py`

 * *Files identical despite different names*

