# Comparing `tmp/dsms_sdk-1.4.0rc4.tar.gz` & `tmp/dsms_sdk-1.4.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsms_sdk-1.4.0rc4.tar", last modified: Fri Apr 19 00:02:49 2024, max compression
+gzip compressed data, was "dsms_sdk-1.4.0rc5.tar", last modified: Fri Apr 19 00:21:48 2024, max compression
```

## Comparing `dsms_sdk-1.4.0rc4.tar` & `dsms_sdk-1.4.0rc5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.883701 dsms_sdk-1.4.0rc4/
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 00:02:49.883701 dsms_sdk-1.4.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.875701 dsms_sdk-1.4.0rc4/dsms/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.875701 dsms_sdk-1.4.0rc4/dsms/apps/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/apps/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.875701 dsms_sdk-1.4.0rc4/dsms/core/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/core/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/core/dsms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.875701 dsms_sdk-1.4.0rc4/dsms/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16352 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/ktype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/affiliations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/authors.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/contacts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/custom_datatype/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/custom_datatype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/custom_datatype/numerical.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/external_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/linked_kitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/properties/user_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/queries/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.879701 dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/sparql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16912 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/dsms/knowledge/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.883701 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 00:02:49.000000 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-19 00:02:49.000000 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:02:49.000000 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 00:02:49.000000 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 00:02:49.000000 dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 00:02:49.883701 dsms_sdk-1.4.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:49.883701 dsms_sdk-1.4.0rc4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/tests/test_kitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 00:02:39.000000 dsms_sdk-1.4.0rc4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.721469 dsms_sdk-1.4.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 00:21:48.721469 dsms_sdk-1.4.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.709469 dsms_sdk-1.4.0rc5/dsms/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.713469 dsms_sdk-1.4.0rc5/dsms/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/apps/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.713469 dsms_sdk-1.4.0rc5/dsms/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/core/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7701 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/core/dsms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.713469 dsms_sdk-1.4.0rc5/dsms/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16352 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/ktype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.713469 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/affiliations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/authors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/contacts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/custom_datatype/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/custom_datatype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/custom_datatype/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/external_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/linked_kitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/properties/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/sparql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/dsms/knowledge/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-19 00:21:48.000000 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-19 00:21:48.000000 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:21:48.000000 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-19 00:21:48.000000 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 00:21:48.000000 dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-19 00:21:48.721469 dsms_sdk-1.4.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:48.717469 dsms_sdk-1.4.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/tests/test_kitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-19 00:21:41.000000 dsms_sdk-1.4.0rc5/tests/test_utils.py
```

### Comparing `dsms_sdk-1.4.0rc4/LICENSE` & `dsms_sdk-1.4.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/PKG-INFO` & `dsms_sdk-1.4.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc4
+Version: 1.4.0rc5
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc4/README.md` & `dsms_sdk-1.4.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/apps/apps.py` & `dsms_sdk-1.4.0rc5/dsms/apps/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/apps/utils.py` & `dsms_sdk-1.4.0rc5/dsms/apps/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/core/configuration.py` & `dsms_sdk-1.4.0rc5/dsms/core/configuration.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/core/context.py` & `dsms_sdk-1.4.0rc5/dsms/core/context.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/core/dsms.py` & `dsms_sdk-1.4.0rc5/dsms/core/dsms.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/core/utils.py` & `dsms_sdk-1.4.0rc5/dsms/core/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/kitem.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/ktype.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/ktype.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/__init__.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/affiliations.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/affiliations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/annotations.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/annotations.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/apps.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/apps.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/attachments.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/attachments.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/authors.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/authors.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/base.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/contacts.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/contacts.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/custom_datatype/numerical.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/custom_datatype/numerical.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/external_links.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/external_links.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/hdf5.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/hdf5.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/linked_kitems.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/linked_kitems.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/summary.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/summary.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/properties/user_groups.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/properties/user_groups.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/queries/base.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/queries/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/base.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/base.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/conversion.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/conversion.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/sparql.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/sparql.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/semantics/units/utils.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/semantics/units/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/sparql_interface.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/sparql_interface.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/subgraph.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/subgraph.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/sparql_interface/utils.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/sparql_interface/utils.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/dsms/knowledge/utils.py` & `dsms_sdk-1.4.0rc5/dsms/knowledge/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,21 +265,20 @@
         },
         exclude_none=True,
     )
     payload = json.loads(dumped)
     payload.update(
         external_links={
             link.label: str(link.url) for link in kitem.external_links
-        }
+        },
+        **differences,
     )
     if kitem.custom_properties:
         custom_properties = kitem.custom_properties.model_dump()
-        payload.update(
-            custom_properties={"content": custom_properties}, **differences
-        )
+        payload.update(custom_properties={"content": custom_properties})
     response = _perform_request(
         f"api/knowledge/kitems/{kitem.id}", "put", json=payload
     )
     if not response.ok:
         raise ValueError(
             f"KItem with uuid `{kitem.id}` could not be updated in DSMS: {response.text}`"
         )
```

### Comparing `dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/PKG-INFO` & `dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsms_sdk
-Version: 1.4.0rc4
+Version: 1.4.0rc5
 Summary: Python SDK core-package for working with the Dataspace Management System (DSMS).
 Home-page: https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 Author: Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 Author-email: matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 License: BSD-3-Clause
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `dsms_sdk-1.4.0rc4/dsms_sdk.egg-info/SOURCES.txt` & `dsms_sdk-1.4.0rc5/dsms_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/setup.cfg` & `dsms_sdk-1.4.0rc5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dsms_sdk
-version = v1.4.0rc4
+version = v1.4.0rc5
 description = Python SDK core-package for working with the Dataspace Management System (DSMS).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MI-FraunhoferIWM/dsms-python-sdk
 author = Matthias Büschelberger, Yoav Nahshon, Pablo De Andres
 author_email = matthias.bueschelberger@iwm.fraunhofer.de, yoav.nahshon@iwm.fraunhofer.de, pablo.de.andres@iwm.fraunhofer.de
 license = BSD-3-Clause
```

### Comparing `dsms_sdk-1.4.0rc4/tests/conftest.py` & `dsms_sdk-1.4.0rc5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/tests/test_kitem.py` & `dsms_sdk-1.4.0rc5/tests/test_kitem.py`

 * *Files identical despite different names*

### Comparing `dsms_sdk-1.4.0rc4/tests/test_utils.py` & `dsms_sdk-1.4.0rc5/tests/test_utils.py`

 * *Files identical despite different names*

