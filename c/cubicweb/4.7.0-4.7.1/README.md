# Comparing `tmp/cubicweb-4.7.0.tar.gz` & `tmp/cubicweb-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-4.7.0.tar", last modified: Wed Apr  3 11:58:52 2024, max compression
+gzip compressed data, was "cubicweb-4.7.1.tar", last modified: Fri Apr 19 09:51:48 2024, max compression
```

## Comparing `cubicweb-4.7.0.tar` & `cubicweb-4.7.1.tar`

### file list

```diff
@@ -1,1370 +1,1320 @@
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.138896 cubicweb-4.7.0/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2002 2024-04-03 11:58:45.000000 cubicweb-4.7.0/CONTRIBUTING.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17987 2021-04-20 14:56:24.000000 cubicweb-4.7.0/COPYING
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26527 2021-04-20 14:56:24.000000 cubicweb-4.7.0/COPYING.LESSER
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4977 2024-04-03 11:58:45.000000 cubicweb-4.7.0/MANIFEST.in
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4250 2024-04-03 11:58:52.138896 cubicweb-4.7.0/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/README.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__init__.py
--rwxr-xr-x   0 schabot   (1000) schabot   (1000)       69 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__main__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1665 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6885 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/_exceptions.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3860 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/_gcdebug.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5211 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/appobject.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1671 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/crypto.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    66337 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwconfig.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32638 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4899 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwgettext.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    25982 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwvreg.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/dataimport/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1987 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3274 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/csv.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    21081 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/importer.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26515 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/massive_store.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/pgstore.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    18127 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/stores.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/dataimport/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/dataimport/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)   474710 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/geonames.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)      113 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/people.csv
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1231 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12362 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/timeZones.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1987 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2513 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_csv.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16176 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_massive_store.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4179 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_pgstore.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8221 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_stores.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10720 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/unittest_importer.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2669 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/debug.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    27112 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5449 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/apptest_config.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      266 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/cwmock.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5146 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/qunit.css
--rw-r--r--   0 schabot   (1000) schabot   (1000)   115758 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/qunit.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)    39808 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/devctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3702 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/fake.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    24531 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/fill.py
--rwxr-xr-x   0 schabot   (1000) schabot   (1000)     1011 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/fix_po_encoding
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10982 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/htmlparser.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5298 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/httptest.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9195 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/instrument.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2354 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/realdbtest.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10873 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/repotest.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6796 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/stresstester.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/bootstrap_cubes
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11311 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/firstnames.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:51.998895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      460 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2657 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1720 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1679 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:51.998895 cubicweb-4.7.0/cubicweb/devtools/test/data/static/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)       10 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      353 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      321 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      136 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      136 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      719 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/utils.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4354 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_dbfill.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6402 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_devctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2475 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_fill.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3225 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_i18n.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4687 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_testlib.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/testlib.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5324 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    24563 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/adapters.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6476 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/authobjs.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4193 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/lib.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5944 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/schemaobjs.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4095 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/sources.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/data/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/test/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1307 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/test/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9992 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/test/unittest_base.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    36719 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/test/unittest_wfobjs.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22858 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/wfobjs.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    59384 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entity.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/ext/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5821 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/ext/html4zope.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1839 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/markdown.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/ext/test/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2013 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/test/unittest_markdown.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/hooks/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4593 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1544 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/bookmark.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3089 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/email.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13217 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/integrity.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5680 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/metadata.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9725 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/notification.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8157 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/security.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10630 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/synccomputed.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    60802 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/syncschema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4913 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/syncsession.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2952 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/syncsources.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      291 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data/hooks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2728 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/data-computed/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1700 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data-computed/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1729 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_bookmarks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13062 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_hooks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8490 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_integrity.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1513 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_notificationhooks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2308 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_security.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_synccomputed.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    24424 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncschema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4778 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsession.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2667 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsources.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15886 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/workflow.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/i18n/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    93082 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/de.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)    61668 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/en.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)   112148 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/es.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)   106920 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/fr.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3749 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5624 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/mail.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3352 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/md5crypt.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22356 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/migration.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      688 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      395 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.1_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.3_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3186 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.23.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      913 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.24.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1410 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.24.4_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      117 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.27.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      217 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.30.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.31.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      423 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.32.3_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       25 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.38.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20108 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/bootstrapmigration_repository.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3368 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/postcreate.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/scripts/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1446 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/chpasswd.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      393 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/detect_cycle.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5710 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/fast_drop_entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      799 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/scripts/ldap_change_base_dn.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3466 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/migration_helper.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1097 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/source_highlight.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3270 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/mttransforms.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17397 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/multipart.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    50906 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/predicates.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9523 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11835 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/auth.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4474 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/config.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7548 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/core.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1483 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/csrf.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7077 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_source_code.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1927 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1505 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3912 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1592 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4852 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2980 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8484 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/debugtoolbar_panels.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1489 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/default_session.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1837 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/development.ini.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3767 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/predicates.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1843 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/pyramid.ini.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/pyramidctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5309 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/resources.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7395 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/rest_api.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9651 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/session.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2447 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        5 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      416 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1327 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3624 2024-02-23 08:55:59.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_auth.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3652 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_config.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6447 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_content_negociation.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      782 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_core.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      986 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_tools.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2065 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/tools.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1929 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pytestconf.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1802 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/rdf.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2170 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/repoapi.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17494 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/req.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    41745 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rqlrewrite.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rqlsuggestions.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    27291 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rset.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11656 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rtags.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    57848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6149 2024-02-23 08:55:59.000000 cubicweb-4.7.0/cubicweb/schema_exporters.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/schemas/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2279 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/Bookmark.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1696 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1662 2022-08-09 14:03:17.000000 cubicweb-4.7.0/cubicweb/schemas/_regproc.postgres.sql
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13898 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/base.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15024 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/bootstrap.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11853 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/workflow.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.038895 cubicweb-4.7.0/cubicweb/server/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3275 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/check_unused_index.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    23043 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/checkintegrity.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6110 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/edition.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    38571 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/hook.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    77833 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/migractions.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    35925 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/querier.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    47931 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/repository.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    19156 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/rqlannotation.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13785 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/schema2sql.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    28692 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/schemaserial.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3168 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/serverconfig.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    56184 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/serverctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32564 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/session.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.038895 cubicweb-4.7.0/cubicweb/server/sources/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13281 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    18181 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/datafeed.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16896 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/ldapfeed.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    78080 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/native.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    71034 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/rql2sql.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11149 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/storages.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22712 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sqlutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22485 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/ssplanner.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1087 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/hooks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1503 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/ldap_test.ldif
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/site_cubicweb.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1565 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data/slapd.conf.in
--rw-r--r--   0 schabot   (1000) schabot   (1000)       77 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/sources_extern
--rw-r--r--   0 schabot   (1000) schabot   (1000)       97 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/sources_multi
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-cwep002/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1299 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-cwep002/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2510 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Company.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1242 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3298 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/State.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      980 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3778 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/toignore
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1345 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/datacomputed/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/datacomputed/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8829 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_datafeed.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2192 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_edition.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4875 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_hook.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26126 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_ldapsource.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    96689 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_querier.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)   101040 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_rql2sql.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    23306 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_rqlannotation.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11087 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_schema2sql.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    28561 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_schemaserial.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    38100 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_server_security.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5431 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_server_utils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3908 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_serverctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2296 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_session.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1609 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_sources_native.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2449 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_sqlutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_ssplanner.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17465 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_storage.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1139 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_tools.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    21764 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_undo.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2619 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_utils.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3596 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_migractions/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    47791 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/unittest_migractions.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9724 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/unittest_migractions.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1972 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/unittest_migractions.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/postcreate.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/site_cubicweb.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10298 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/unittest_postgres.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/hooks.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1345 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    38041 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_repository/unittest_repository.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5178 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/utils.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1112 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      262 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/.hgignore.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      109 2022-08-09 14:03:17.000000 cubicweb-4.7.0/cubicweb/skeleton/.yamllint.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      249 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/Dockerfile.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      367 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/MANIFEST.in.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1484 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/README.rst.tmpl
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       97 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      593 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       24 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
--rw-r--r--   0 schabot   (1000) schabot   (1000)      190 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      203 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
--rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      425 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      378 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      180 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      221 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      747 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)      215 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/setup.py.tmpl
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2001 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      377 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1351 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/tox.ini.tmpl
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/smoke_test/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1504 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1455 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1364 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12938 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/ldapparser.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14419 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/notification.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5861 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/services.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8236 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/supervising.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1154 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1079 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4020 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_email.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3059 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_notification.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5404 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_register_user.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5051 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_supervising.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1994 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/tags.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/test/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/test/data/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       31 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/data/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1109 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1128 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/hooks.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/views/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/views/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1024 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/entities/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/hooks/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      845 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      875 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       51 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      857 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      887 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      157 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1565 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1555 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/erqlexpr_on_ertype.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       77 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/lowered_etype.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.0.3_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.0.4_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      855 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_common.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      847 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_repository.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.2_Any.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      402 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_computedrel.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1555 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1401 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_attr.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1182 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_eetype.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4319 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/scripts/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      164 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script1.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      168 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script2.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      187 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script3.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/server_migration/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
--rw-r--r--   0 schabot   (1000) schabot   (1000)      882 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      131 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/uppered_rtype.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       16 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/bootstrap_cubes
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/
--rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3723 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/schema.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data_schemareader/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      732 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data_schemareader/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2304 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_binary.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      404 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_crypto.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17592 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_cwconfig.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7457 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_cwctl.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    48020 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_entity.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4855 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_fast_drop_entities.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8357 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_mail.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7471 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_migration.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15441 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_predicates.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_repoapi.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5850 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_req.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    46300 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rqlrewrite.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rqlsuggestions.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    32589 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rset.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6543 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_rtags.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    34435 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4047 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_toolsutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9658 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_uilib.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_vregistry.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3998 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_wfutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16545 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/toolsutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3836 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/transaction.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    19530 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/uilib.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12356 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/utils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5113 2024-03-26 15:31:00.000000 cubicweb-4.7.0/cubicweb/wfutils.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1578 2024-02-05 14:10:08.000000 cubicweb-4.7.0/cubicweb/xy.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb.egg-info/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4250 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/PKG-INFO
--rw-r--r--   0 schabot   (1000) schabot   (1000)    53563 2024-04-03 11:58:51.000000 cubicweb-4.7.0/cubicweb.egg-info/SOURCES.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/dependency_links.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      117 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/entry_points.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2021-11-04 14:45:29.000000 cubicweb-4.7.0/cubicweb.egg-info/not-zip-safe
--rw-r--r--   0 schabot   (1000) schabot   (1000)      500 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/requires.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        9 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/top_level.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7511 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/4.0.0_how_to_migrate.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2811 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/Makefile
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/_static/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    34494 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/_static/favicon.ico
--rw-r--r--   0 schabot   (1000) schabot   (1000)    34494 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/_static/favicon.ico.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/_static/logo-cubicweb.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9202 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/_static/logo-cubicweb.svg.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1681 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/announce.en.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1982 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/announce.fr.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/api/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2251 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/__init__.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      181 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/appobject.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      830 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/cwvreg.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      491 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/dataimport.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)       87 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/api/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2540 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/predicates.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/api/pyramid/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      249 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/auth.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      358 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/pyramid/bwcompat.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      613 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/pyramid/core.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      296 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/login.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      259 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/profile.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      200 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/session.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      289 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/url_redirection.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      234 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      144 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/req.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      140 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/rset.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      781 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/urlpublishing.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      393 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/urlrewrite.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      520 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/web.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14655 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-app.en.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7806 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/_maybe_to_integrate/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      225 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1286 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/rss-xml.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      751 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/template.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/additionnal_services/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      369 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/additionnal_services/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13562 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/additionnal_services/undo.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/admin/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2253 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/book/admin/backups.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5658 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/admin/config.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/create-instance.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/create-instance.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3396 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3396 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4034 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/deploy.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4034 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/deploy.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      409 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      409 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/index.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5265 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/instance-config.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5265 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/instance-config.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4825 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/admin/ldap.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      130 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/multisources.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      366 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/rql-logs.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2064 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/setup.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2064 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/setup.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3596 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/site-config.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/annexes/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/depends.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3257 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/docstrings-conventions.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/annexes/faq.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16153 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/annexes/faq.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      234 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3481 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/mercurial.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/annexes/rql/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2115 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/Graph-ex.gif
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1167 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/rql/debugging.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4697 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/implementation.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      267 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/rql/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5570 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/intro.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    27490 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/rql/language.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2703 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2703 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2147 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/connections_pooler.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/cubes/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2645 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/available-cubes.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      932 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/cc-newcube.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      208 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6827 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6827 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1967 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/what-is-a-cube.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4021 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/dataimport.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/datamodel/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1389 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/baseschema.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6178 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/define-workflows.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    34880 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/definition.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1043 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/metadata.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2940 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/debug_channels.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/devcore/
--rw-r--r--   0 schabot   (1000) schabot   (1000)       67 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/devcore/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1129 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/devcore/reqbase.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devrepo/entityclasses/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5159 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/adapters.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7268 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/application-logic.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5285 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/data-as-objects.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      303 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1719 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/load-sort.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4399 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/fti.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      504 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9469 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/migration.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2668 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/profiling.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devrepo/repo/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9731 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/repo/hooks.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      155 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/repo/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1087 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/book/devrepo/repo/notifications.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11467 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/repo/sessions.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)       75 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/repo/tasks.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    21316 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/testing.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    18289 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devrepo/vreg.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    18289 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devrepo/vreg.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devweb/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      915 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/ajax.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      915 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/ajax.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3473 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/controllers.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3473 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/controllers.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      890 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/css.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      890 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/css.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/devweb/edition/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11979 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11979 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3955 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3955 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9905 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/examples.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9905 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/examples.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15506 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/form.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15506 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/form.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      286 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      286 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/index.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      698 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/facets.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      698 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/facets.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/httpcaching.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/httpcaching.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      392 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      392 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/index.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10057 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/internationalization.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10057 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/internationalization.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/js.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/js.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      265 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/property.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      265 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/property.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2017 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/publisher.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2017 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/publisher.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5119 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/request.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5119 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/request.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      709 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/resource.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      709 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/resource.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      454 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/rtags.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      454 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/rtags.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1418 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/searchbar.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1418 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/searchbar.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/devweb/views/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5889 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5889 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      701 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      701 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1291 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/boxes.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1291 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/boxes.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2320 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2320 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      476 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      476 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/index.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10179 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/primary.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10179 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/primary.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5991 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/reledit.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5991 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/reledit.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      521 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/startup.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      521 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/startup.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5919 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/table.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5919 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/table.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5506 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5506 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4192 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/views.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4192 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/views.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      347 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/wdoc.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      347 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/wdoc.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1703 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1703 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      947 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/warning.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/intro/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    10427 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/concepts.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1369 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/history.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      385 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/index.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/pyramid/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1371 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/auth.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1371 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/auth.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1314 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/pyramid/ctl.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3771 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3771 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)      844 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/pyramid/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1795 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/quickstart.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1795 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/quickstart.rst.orig
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5411 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/settings.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5411 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/settings.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/security/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8041 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/security/csrf.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8041 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/security/csrf.rst.orig
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/src/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2930 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/src/archi_globale.dia
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1735 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/src/main_template_layout.dia
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.118896 cubicweb-4.7.0/doc/changes/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6619 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.14.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3904 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.15.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3647 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.16.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1815 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.17.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3632 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.18.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6757 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.19.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3165 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.20.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2991 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.21.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3689 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.22.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2799 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.23.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4033 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.24.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4655 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.25.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      434 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.26.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6870 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.27.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2656 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.28.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1249 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.29.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5588 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.30.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3683 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.31.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7979 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.32.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1728 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.32_reledit.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5635 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.33.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4524 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.34.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4849 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.35.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     4507 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.36.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.37.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8870 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.38.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6425 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.0.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      914 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.1.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      233 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.2.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2656 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.3.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      264 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.4.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.5.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1949 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.6.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      126 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.7.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      746 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/changelog.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)       99 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7654 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/conf.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/images/
--rw-r--r--   0 schabot   (1000) schabot   (1000)    98393 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/03-transitions-view_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12650 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/breadcrumbs_header.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    85073 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_general_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   124385 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_registry_content_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   111325 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_registry_decisions_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   134505 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_rql_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   192629 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_rql_traceback_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   107766 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_show_source.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    55625 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_show_source_link.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   126845 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_sql_panel.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    97343 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_traceback_source_link.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    57300 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/example-card-with-rql-directive.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    55168 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/example-card-with-rql-table-directive.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2277 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_date_range.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6013 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_has_image.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22016 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_overview.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1873 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_range.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    21685 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_00-login_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    30326 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_01-start_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    35859 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_02-cookie-values_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    33922 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_02-create-blog_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    28123 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-list-one-blog_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    82897 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-site-config-panel_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   119813 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-state-submitted_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    98393 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-transitions-view_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    34771 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_04-detail-one-blog_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    28345 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_05-list-two-blog_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    49230 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_06-add-relation-entryof_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    96838 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_06-main-template-logo_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    40383 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_07-detail-one-blogentry_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    30591 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_08-schema_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    33091 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_09-new-view-blogentry_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    42230 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_10-blog-with-two-entries_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17757 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8674 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13842 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template_layout.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    46411 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/primaryview_template.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14758 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/primaryview_template.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22773 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/request_session.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7211 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/request_session.svg
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12030 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/server-class-diagram.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    62022 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-form_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   105173 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    58500 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-primary_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    42013 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blogs-list_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   109769 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_form-generic-relations_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    65646 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    13605 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_gettext_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    88970 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_logged_in_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    11548 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_login-form_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   100347 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    63097 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    62431 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-default-primary_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    74856 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    79709 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-custom-footer_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   128406 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-schema_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    71500 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-siteinfo_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   104834 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_schema_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    22098 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_schema_graphviz_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   150520 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_siteconfig_en.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    60672 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_admin.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    61388 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_city_created.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    50694 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_city_creation.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    71561 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_data_model_schema.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    48896 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_empty_instance.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    55671 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_finished_import.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    57063 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_list_view.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    70893 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_created.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    61656 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_creation.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    74005 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_with_city_name.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   225824 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_react_map.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    53544 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_with_schema.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   354637 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_background-image.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    30437 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_boxes.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    54643 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_breadcrumbs.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   324086 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_facets.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    40520 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_grey-box.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    16843 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_index-after.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26875 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_index-before.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17580 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_login-box.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    57814 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_prevnext.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    81362 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui1.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    93291 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui2.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)   290338 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui3.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    43051 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_history-view_w600.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    26036 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_mesage_w600.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    39625 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_startup-link_w600.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17558 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-filter-shadow.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    14013 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-filter.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)    12375 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-shadow.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9676 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table.png
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7344 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2011 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/plan_formation_python_cubicweb.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      139 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/stdlib.txt
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tools/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1462 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tools/generate_modules.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1624 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tools/mode_plan.py
--rwxr-xr-x   0 schabot   (1000) schabot   (1000)     4944 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tools/pyjsrest.py
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/advanced/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      604 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/advanced/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5486 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part01_create-cube.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    17016 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part02_security.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5614 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/advanced/part03_bfss.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15384 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part04_ui-base.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    15114 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part05_ui-advanced.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/base/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3867 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/base/blog-in-five-minutes.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/conclusion.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)    20435 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/base/customizing-the-application.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7821 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/discovering-the-ui.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1340 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/index.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/dataimport/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9014 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_import.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3336 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_parser.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)    29917 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/tutorials/dataimport/index.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6576 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/schema.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)      568 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/index.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/museum/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     5961 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/data-management.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     6403 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/develop-app.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3860 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/develop-ui.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     8840 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/enhance-views.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     2702 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/getting-started.rst
--rw-r--r--   0 schabot   (1000) schabot   (1000)     1595 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/index.rst
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/extras/
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3545 2021-09-01 09:36:34.000000 cubicweb-4.7.0/extras/cubicweb-ctl.bash_completion
--rw-r--r--   0 schabot   (1000) schabot   (1000)     7414 2021-04-20 14:56:24.000000 cubicweb-4.7.0/jshintrc
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/man/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      651 2024-01-16 10:36:25.000000 cubicweb-4.7.0/man/cubicweb-ctl.1
--rw-r--r--   0 schabot   (1000) schabot   (1000)       56 2024-01-16 10:36:25.000000 cubicweb-4.7.0/mypy.ini
--rw-r--r--   0 schabot   (1000) schabot   (1000)      536 2021-09-01 09:36:34.000000 cubicweb-4.7.0/pylintrc
-drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.138896 cubicweb-4.7.0/requirements/
--rw-r--r--   0 schabot   (1000) schabot   (1000)      174 2024-04-03 11:58:45.000000 cubicweb-4.7.0/requirements/dev.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      310 2024-04-03 11:58:45.000000 cubicweb-4.7.0/requirements/doc.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      377 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/from-forge.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      380 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-base.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       16 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-dataimport.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       15 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-devtools.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)        9 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-ext.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-hooks.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      128 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-pyramid.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)       35 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-server.txt
--rw-r--r--   0 schabot   (1000) schabot   (1000)      115 2024-04-03 11:58:52.138896 cubicweb-4.7.0/setup.cfg
--rw-r--r--   0 schabot   (1000) schabot   (1000)     3279 2024-04-03 11:58:45.000000 cubicweb-4.7.0/setup.py
--rw-r--r--   0 schabot   (1000) schabot   (1000)     9036 2024-04-03 11:58:45.000000 cubicweb-4.7.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.820646 cubicweb-4.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-19 09:51:16.000000 cubicweb-4.7.1/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2024-04-19 09:51:16.000000 cubicweb-4.7.1/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)     4977 2024-04-19 09:51:16.000000 cubicweb-4.7.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5161 2024-04-19 09:51:48.820646 cubicweb-4.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.320640 cubicweb-4.7.1/cubicweb/
+-rw-rw-rw-   0 root         (0) root         (0)     7503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       69 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6885 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/_gcdebug.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/appobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    66337 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    32638 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwgettext.py
+-rw-rw-rw-   0 root         (0) root         (0)    25982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/cwvreg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.328640 cubicweb-4.7.1/cubicweb/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    21081 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    26515 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    15503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)    18127 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/stores.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.332640 cubicweb-4.7.1/cubicweb/dataimport/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.332640 cubicweb-4.7.1/cubicweb/dataimport/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)   474710 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/geonames.csv
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/people.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data/timeZones.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.336640 cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    16176 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     4179 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8221 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/dataimport/test/unittest_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2669 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.340640 cubicweb-4.7.1/cubicweb/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)    27112 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5449 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/apptest_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.340640 cubicweb-4.7.1/cubicweb/devtools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/cwmock.js
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/qunit.css
+-rw-rw-rw-   0 root         (0) root         (0)   115758 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/data/qunit.js
+-rw-rw-rw-   0 root         (0) root         (0)    39808 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fake.py
+-rw-rw-rw-   0 root         (0) root         (0)    24531 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fill.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/fix_po_encoding
+-rw-rw-rw-   0 root         (0) root         (0)    10982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/htmlparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9195 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/realdbtest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10873 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/repotest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6796 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/stresstester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.344640 cubicweb-4.7.1/cubicweb/devtools/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.344640 cubicweb-4.7.1/cubicweb/devtools/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/firstnames.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.240639 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.348640 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.244639 cubicweb-4.7.1/cubicweb/devtools/test/data/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.352640 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/dep_1.js
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/deps_2.js
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
+-rw-rw-rw-   0 root         (0) root         (0)      321 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_dbfill.py
+-rw-rw-rw-   0 root         (0) root         (0)     6402 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_fill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/test/unittest_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    20848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.352640 cubicweb-4.7.1/cubicweb/entities/
+-rw-rw-rw-   0 root         (0) root         (0)     5324 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24563 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/authobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     5944 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/schemaobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4095 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/entities/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9992 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/unittest_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    36719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/test/unittest_wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    22858 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entities/wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    59384 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/ext/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5821 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/html4zope.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.356640 cubicweb-4.7.1/cubicweb/ext/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/ext/test/unittest_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.364640 cubicweb-4.7.1/cubicweb/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/email.py
+-rw-rw-rw-   0 root         (0) root         (0)    13217 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5680 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     9725 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8157 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/security.py
+-rw-rw-rw-   0 root         (0) root         (0)    10630 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    60802 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/syncsources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.368641 cubicweb-4.7.1/cubicweb/hooks/test/data-computed/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/data-computed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_bookmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)    13062 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_notificationhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24424 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/hooks/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.372640 cubicweb-4.7.1/cubicweb/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    93082 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    61668 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)   112148 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)   106920 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     5624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/md5crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)    22356 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.372640 cubicweb-4.7.1/cubicweb/misc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.376641 cubicweb-4.7.1/cubicweb/misc/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.22.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3186 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.23.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.24.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1410 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.24.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.27.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.30.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.31.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.32.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/3.38.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)    20108 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3368 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.380641 cubicweb-4.7.1/cubicweb/misc/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/chpasswd.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/detect_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     5710 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/ldap_change_base_dn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3466 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/scripts/migration_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/misc/source_highlight.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/mttransforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17397 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)    50906 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/predicates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.388641 cubicweb-4.7.1/cubicweb/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     9523 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4474 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7077 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_source_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.388641 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/debugtoolbar_panels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/default_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/development.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     3767 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/pyramid.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)    13622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/pyramidctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5309 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     7395 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9651 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.392641 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6447 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_content_negociation.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/test/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pyramid/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    17494 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/req.py
+-rw-rw-rw-   0 root         (0) root         (0)    41745 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    11503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rset.py
+-rw-rw-rw-   0 root         (0) root         (0)    11656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    57848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     6149 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schema_exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.396641 cubicweb-4.7.1/cubicweb/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/Bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/_regproc.postgres.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13898 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15024 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    11853 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/schemas/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.404641 cubicweb-4.7.1/cubicweb/server/
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/check_unused_index.py
+-rw-rw-rw-   0 root         (0) root         (0)    23043 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/checkintegrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/edition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38571 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    77833 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/migractions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35925 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/querier.py
+-rw-rw-rw-   0 root         (0) root         (0)    47931 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)    19156 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13785 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28692 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)     3168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/serverconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    56204 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    32564 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.408641 cubicweb-4.7.1/cubicweb/server/sources/
+-rw-rw-rw-   0 root         (0) root         (0)    13281 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18181 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    16896 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/ldapfeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    78080 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/native.py
+-rw-rw-rw-   0 root         (0) root         (0)    71034 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11149 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sources/storages.py
+-rw-rw-rw-   0 root         (0) root         (0)    22712 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22485 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/ssplanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.416641 cubicweb-4.7.1/cubicweb/server/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.420641 cubicweb-4.7.1/cubicweb/server/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.452642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/ldap_test.ldif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/slapd.conf.in
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/sources_extern
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data/sources_multi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-cwep002/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-cwep002/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.424641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.428641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.428641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.432641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.436641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.440641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.444641 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/toignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.448641 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_edition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    26126 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_ldapsource.py
+-rw-rw-rw-   0 root         (0) root         (0)    96689 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_querier.py
+-rw-rw-rw-   0 root         (0) root         (0)   101040 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    23306 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28561 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)    38100 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_server_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_sources_native.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_ssplanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    17465 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21764 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_undo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.456642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.460642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.464642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.468642 cubicweb-4.7.1/cubicweb/server/test_migractions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.496642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.472642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.476642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.480642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.484642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.488642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.492642 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    47791 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.500642 cubicweb-4.7.1/cubicweb/server/test_migractions2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.528643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.504642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.508642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.508642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.512642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.516642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.520642 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.524643 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.532643 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9724 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions2/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.560643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.536643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.540643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.544643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.548643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.552643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.556643 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.564643 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_migractions3/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_postgres/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.568643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.572643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.576643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_postgres/unittest_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.580643 cubicweb-4.7.1/cubicweb/server/test_repository/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.588643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.588643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.592643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.592643 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.584643 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    38041 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/test_repository/unittest_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     5178 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/server/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.596644 cubicweb-4.7.1/cubicweb/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.gitlab-ci.yml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.hgignore.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/.yamllint.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/Dockerfile.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/MANIFEST.in.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/README.rst.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.600643 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.600643 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.604644 cubicweb-4.7.1/cubicweb/skeleton/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/realdb_test_CUBENAME.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/skeleton/tox.ini.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.608644 cubicweb-4.7.1/cubicweb/smoke_test/
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.608644 cubicweb-4.7.1/cubicweb/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/ldapparser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14419 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5861 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     8236 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/supervising.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.612644 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.616644 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.616644 cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     3059 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_register_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/sobjects/test/unittest_supervising.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.624644 cubicweb-4.7.1/cubicweb/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.628644 cubicweb-4.7.1/cubicweb/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.636644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.636644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/views/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/entities/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.640644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.644644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.648644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.648644 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/erqlexpr_on_ertype.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/lowered_etype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.652644 cubicweb-4.7.1/cubicweb/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.0.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.0.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_common.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/migration/0.1.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_computedrel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_ertype_read.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_eetype.py
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.652644 cubicweb-4.7.1/cubicweb/test/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script1.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script2.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/scripts/script3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.656644 cubicweb-4.7.1/cubicweb/test/data/server_migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.10.2_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.5.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/2.6.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)      882 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data/uppered_rtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.632644 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data-rewrite/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.656644 cubicweb-4.7.1/cubicweb/test/data_schemareader/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/data_schemareader/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    17592 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     7457 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    48020 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8357 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)    15441 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_req.py
+-rw-rw-rw-   0 root         (0) root         (0)    46300 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6503 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    32589 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     6543 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    34435 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9658 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/test/unittest_wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    16545 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3836 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    19530 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12356 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2024-04-19 09:51:16.000000 cubicweb-4.7.1/cubicweb/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.816646 cubicweb-4.7.1/cubicweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5161 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51739 2024-04-19 09:51:48.000000 cubicweb-4.7.1/cubicweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-19 09:51:47.000000 cubicweb-4.7.1/cubicweb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.660644 cubicweb-4.7.1/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     7511 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/4.0.0_how_to_migrate.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.660644 cubicweb-4.7.1/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/_static/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/announce.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/announce.fr.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.668645 cubicweb-4.7.1/doc/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/__init__.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/appobject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/cwvreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      491 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/dataimport.rst
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/predicates.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.668645 cubicweb-4.7.1/doc/api/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/bwcompat.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/login.rst
+-rw-rw-rw-   0 root         (0) root         (0)      259 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/profile.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/session.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid/url_redirection.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/pyramid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/req.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/rset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      781 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/urlpublishing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/urlrewrite.rst
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/api/web.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/
+-rw-rw-rw-   0 root         (0) root         (0)    14655 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-app.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7806 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-gae-app.en.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/_maybe_to_integrate/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/D050-architecture.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/rss-xml.rst
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/_maybe_to_integrate/template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.672644 cubicweb-4.7.1/doc/book/additionnal_services/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/additionnal_services/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/additionnal_services/undo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.680645 cubicweb-4.7.1/doc/book/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/backups.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/create-instance.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/cubicweb-ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4034 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/deploy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5265 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/instance-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/ldap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/multisources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      366 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/rql-logs.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/admin/site-config.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.680645 cubicweb-4.7.1/doc/book/annexes/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/depends.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/docstrings-conventions.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/mercurial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.684645 cubicweb-4.7.1/doc/book/annexes/rql/
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/Graph-ex.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/implementation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5570 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)    27490 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/language.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2703 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/annexes/rql/usecases.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.688645 cubicweb-4.7.1/doc/book/devrepo/
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/connections_pooler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.692645 cubicweb-4.7.1/doc/book/devrepo/cubes/
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/available-cubes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/cc-newcube.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6827 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/cubes/what-is-a-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/dataimport.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.692645 cubicweb-4.7.1/doc/book/devrepo/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/baseschema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6178 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/define-workflows.rst
+-rw-rw-rw-   0 root         (0) root         (0)    34880 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/definition.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/datamodel/metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/debug_channels.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.696645 cubicweb-4.7.1/doc/book/devrepo/devcore/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/devcore/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/devcore/reqbase.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.696645 cubicweb-4.7.1/doc/book/devrepo/entityclasses/
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/adapters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7268 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/application-logic.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/data-as-objects.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/entityclasses/load-sort.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4399 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/fti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      504 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9469 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/profiling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.700645 cubicweb-4.7.1/doc/book/devrepo/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/hooks.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11467 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/sessions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/repo/tasks.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21316 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18289 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devrepo/vreg.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.704645 cubicweb-4.7.1/doc/book/devweb/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/controllers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/css.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.708645 cubicweb-4.7.1/doc/book/devweb/edition/
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/dissection.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/editcontroller.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9905 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15506 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/edition/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      698 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/facets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/httpcaching.rst
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10057 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/internationalization.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/js.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/property.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/publisher.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/request.rst
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/resource.rst
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/rtags.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/searchbar.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.716645 cubicweb-4.7.1/doc/book/devweb/views/
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/basetemplates.rst
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/baseviews.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/boxes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/breadcrumbs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/idownloadable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10179 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/startup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/urlpublish.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/views.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/wdoc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/views/xmlrss.rst
+-rw-rw-rw-   0 root         (0) root         (0)      947 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/devweb/warning.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.716645 cubicweb-4.7.1/doc/book/intro/
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/concepts.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      385 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/intro/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/debug_toolbar.rst
+-rw-rw-rw-   0 root         (0) root         (0)      844 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/pyramid/settings.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/security/
+-rw-rw-rw-   0 root         (0) root         (0)     8041 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/security/csrf.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.720645 cubicweb-4.7.1/doc/book/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/src/archi_globale.dia
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/book/src/main_template_layout.dia
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.736645 cubicweb-4.7.1/doc/changes/
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.14.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.15.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.16.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.17.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.18.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.19.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.20.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.21.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.22.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.23.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.24.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.25.rst
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.26.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6870 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.27.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.28.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.29.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.30.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.31.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.32.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.32_reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5635 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.33.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.34.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4849 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.35.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.36.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.37.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8870 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/3.38.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6425 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      914 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.3.rst
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.4.rst
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.5.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.6.rst
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/4.7.rst
+-rw-rw-rw-   0 root         (0) root         (0)      746 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/changes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7654 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.796646 cubicweb-4.7.1/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    12650 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/breadcrumbs_header.png
+-rw-rw-rw-   0 root         (0) root         (0)    85073 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_general_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   124385 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_registry_content_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   111325 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_registry_decisions_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   134505 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_rql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   192629 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_rql_traceback_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   107766 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_show_source.png
+-rw-rw-rw-   0 root         (0) root         (0)    55625 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_show_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)   126845 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_sql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)    97343 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/debugtoolbar_traceback_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)    57300 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/example-card-with-rql-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)    55168 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/example-card-with-rql-table-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_date_range.png
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_has_image.png
+-rw-rw-rw-   0 root         (0) root         (0)    22016 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_overview.png
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/facet_range.png
+-rw-rw-rw-   0 root         (0) root         (0)    21685 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_00-login_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30326 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_01-start_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    35859 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_02-cookie-values_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33922 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_02-create-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28123 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-list-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    82897 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-site-config-panel_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   119813 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-state-submitted_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    34771 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_04-detail-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28345 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_05-list-two-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    49230 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_06-add-relation-entryof_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    96838 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_06-main-template-logo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    40383 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_07-detail-one-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30591 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_08-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33091 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_09-new-view-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42230 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/lax-book_10-blog-with-two-entries_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    17757 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template.png
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13842 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/main_template_layout.png
+-rw-rw-rw-   0 root         (0) root         (0)    46411 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/primaryview_template.png
+-rw-rw-rw-   0 root         (0) root         (0)    14758 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/primaryview_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22773 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/request_session.png
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/request_session.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12030 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/server-class-diagram.png
+-rw-rw-rw-   0 root         (0) root         (0)    62022 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   105173 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-primary-after-post-creation_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    58500 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blog-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_blogs-list_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   109769 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_form-generic-relations_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    65646 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    13605 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_gettext_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    88970 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_index_logged_in_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_login-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   100347 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    63097 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-custom-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    62431 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-default-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    74856 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-community-taggable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    79709 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-custom-footer_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   128406 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    71500 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_myblog-siteinfo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   104834 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    22098 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_schema_graphviz_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   150520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-base_siteconfig_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    60672 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_admin.png
+-rw-rw-rw-   0 root         (0) root         (0)    61388 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_city_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    50694 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_city_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    71561 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_data_model_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)    48896 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_empty_instance.png
+-rw-rw-rw-   0 root         (0) root         (0)    55671 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_finished_import.png
+-rw-rw-rw-   0 root         (0) root         (0)    57063 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_list_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    70893 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    61656 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    74005 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_museum_with_city_name.png
+-rw-rw-rw-   0 root         (0) root         (0)   225824 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_react_map.png
+-rw-rw-rw-   0 root         (0) root         (0)    53544 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-museum_with_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)   354637 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_background-image.png
+-rw-rw-rw-   0 root         (0) root         (0)    30437 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_boxes.png
+-rw-rw-rw-   0 root         (0) root         (0)    54643 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_breadcrumbs.png
+-rw-rw-rw-   0 root         (0) root         (0)   324086 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_facets.png
+-rw-rw-rw-   0 root         (0) root         (0)    40520 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_grey-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    16843 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_index-after.png
+-rw-rw-rw-   0 root         (0) root         (0)    26875 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_index-before.png
+-rw-rw-rw-   0 root         (0) root         (0)    17580 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_login-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    57814 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_prevnext.png
+-rw-rw-rw-   0 root         (0) root         (0)    81362 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui1.png
+-rw-rw-rw-   0 root         (0) root         (0)    93291 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui2.png
+-rw-rw-rw-   0 root         (0) root         (0)   290338 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/tutos-photowebsite_ui3.png
+-rw-rw-rw-   0 root         (0) root         (0)    43051 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_history-view_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    26036 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_mesage_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    39625 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/undo_startup-link_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    17558 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-filter-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-filter.png
+-rw-rw-rw-   0 root         (0) root         (0)    12375 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/images/views-table.png
+-rw-rw-rw-   0 root         (0) root         (0)     7344 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/plan_formation_python_cubicweb.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/stdlib.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/generate_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/mode_plan.py
+-rwxrwxrwx   0 root         (0) root         (0)     4944 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tools/pyjsrest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tutorials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.800646 cubicweb-4.7.1/doc/tutorials/advanced/
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5486 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part01_create-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part02_security.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5614 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part03_bfss.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15384 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part04_ui-base.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15114 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/advanced/part05_ui-advanced.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.804646 cubicweb-4.7.1/doc/tutorials/base/
+-rw-rw-rw-   0 root         (0) root         (0)     3867 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/blog-in-five-minutes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/conclusion.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20435 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/customizing-the-application.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/discovering-the-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/base/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.804646 cubicweb-4.7.1/doc/tutorials/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     9014 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    29917 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6576 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/dataimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.808646 cubicweb-4.7.1/doc/tutorials/museum/
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/data-management.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/develop-app.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/develop-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8840 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/enhance-views.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-04-19 09:51:16.000000 cubicweb-4.7.1/doc/tutorials/museum/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.808646 cubicweb-4.7.1/extras/
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2024-04-19 09:51:16.000000 cubicweb-4.7.1/extras/cubicweb-ctl.bash_completion
+-rw-rw-rw-   0 root         (0) root         (0)     7414 2024-04-19 09:51:16.000000 cubicweb-4.7.1/jshintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.812646 cubicweb-4.7.1/man/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-19 09:51:16.000000 cubicweb-4.7.1/man/cubicweb-ctl.1
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-19 09:51:16.000000 cubicweb-4.7.1/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-19 09:51:16.000000 cubicweb-4.7.1/pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 09:51:48.816646 cubicweb-4.7.1/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/from-forge.txt
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-base.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-dataimport.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-devtools.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-ext.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-hooks.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-pyramid.txt
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-04-19 09:51:16.000000 cubicweb-4.7.1/requirements/test-server.txt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-19 09:51:48.820646 cubicweb-4.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-04-19 09:51:16.000000 cubicweb-4.7.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     9036 2024-04-19 09:51:16.000000 cubicweb-4.7.1/tox.ini
```

### Comparing `cubicweb-4.7.0/CONTRIBUTING.rst` & `cubicweb-4.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/COPYING` & `cubicweb-4.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/COPYING.LESSER` & `cubicweb-4.7.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/MANIFEST.in` & `cubicweb-4.7.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/PKG-INFO` & `cubicweb-4.7.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: cubicweb
-Version: 4.7.0
-Summary: a repository of entities / relations for knowledge management
-Home-page: https://www.cubicweb.org
-Author: Logilab
-Author-email: contact@logilab.fr
-License: LGPL
-Requires-Python: >=3.7
-Provides-Extra: captcha
-Provides-Extra: crypto
-Provides-Extra: ext
-Provides-Extra: ical
-Provides-Extra: postgresql
-Provides-Extra: s3
-License-File: COPYING
-License-File: COPYING.LESSER
-
 CubicWeb semantic web framework
 ===============================
 
 CubicWeb is a entities / relations based knowledge management system
 developped at Logilab.
 
 This package contains:
```

### Comparing `cubicweb-4.7.0/cubicweb/__init__.py` & `cubicweb-4.7.1/cubicweb/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb global packaging information for the cubicweb knowledge management
 software
 """
 
 modname = distname = "cubicweb"
 
-numversion = (4, 7, 0)
+numversion = (4, 7, 1)
 version = ".".join(str(num) for num in numversion)
 
 description = "a repository of entities / relations for knowledge management"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = "https://www.cubicweb.org"
 license = "LGPL"
```

### Comparing `cubicweb-4.7.0/cubicweb/_exceptions.py` & `cubicweb-4.7.1/cubicweb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/_gcdebug.py` & `cubicweb-4.7.1/cubicweb/_gcdebug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/appobject.py` & `cubicweb-4.7.1/cubicweb/appobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/crypto.py` & `cubicweb-4.7.1/cubicweb/crypto.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/cwconfig.py` & `cubicweb-4.7.1/cubicweb/cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/cwctl.py` & `cubicweb-4.7.1/cubicweb/cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/cwgettext.py` & `cubicweb-4.7.1/cubicweb/cwgettext.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/cwvreg.py` & `cubicweb-4.7.1/cubicweb/cwvreg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/__init__.py` & `cubicweb-4.7.1/cubicweb/dataimport/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/csv.py` & `cubicweb-4.7.1/cubicweb/dataimport/csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/importer.py` & `cubicweb-4.7.1/cubicweb/dataimport/importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/massive_store.py` & `cubicweb-4.7.1/cubicweb/dataimport/massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/pgstore.py` & `cubicweb-4.7.1/cubicweb/dataimport/pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/stores.py` & `cubicweb-4.7.1/cubicweb/dataimport/stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/data/geonames.csv` & `cubicweb-4.7.1/cubicweb/dataimport/test/data/geonames.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/data/timeZones.txt` & `cubicweb-4.7.1/cubicweb/dataimport/test/data/timeZones.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/schema.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/data-massimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/test_csv.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/test_massive_store.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/test_massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/test_pgstore.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/test_pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/test_stores.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/test_stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/dataimport/test/unittest_importer.py` & `cubicweb-4.7.1/cubicweb/dataimport/test/unittest_importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/debug.py` & `cubicweb-4.7.1/cubicweb/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/__init__.py` & `cubicweb-4.7.1/cubicweb/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/apptest_config.py` & `cubicweb-4.7.1/cubicweb/devtools/apptest_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/data/qunit.css` & `cubicweb-4.7.1/cubicweb/devtools/data/qunit.css`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/data/qunit.js` & `cubicweb-4.7.1/cubicweb/devtools/data/qunit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/devctl.py` & `cubicweb-4.7.1/cubicweb/devtools/devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/fake.py` & `cubicweb-4.7.1/cubicweb/devtools/fake.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/fill.py` & `cubicweb-4.7.1/cubicweb/devtools/fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/fix_po_encoding` & `cubicweb-4.7.1/cubicweb/devtools/fix_po_encoding`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/htmlparser.py` & `cubicweb-4.7.1/cubicweb/devtools/htmlparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/httptest.py` & `cubicweb-4.7.1/cubicweb/devtools/httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/instrument.py` & `cubicweb-4.7.1/cubicweb/devtools/instrument.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/realdbtest.py` & `cubicweb-4.7.1/cubicweb/devtools/realdbtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/repotest.py` & `cubicweb-4.7.1/cubicweb/devtools/repotest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/stresstester.py` & `cubicweb-4.7.1/cubicweb/devtools/stresstester.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/data/firstnames.txt` & `cubicweb-4.7.1/cubicweb/devtools/test/data/firstnames.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-4.7.1/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/devtools/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/utils.js` & `cubicweb-4.7.1/cubicweb/devtools/test/data/static/js_examples/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/unittest_dbfill.py` & `cubicweb-4.7.1/cubicweb/devtools/test/unittest_dbfill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/unittest_devctl.py` & `cubicweb-4.7.1/cubicweb/devtools/test/unittest_devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/unittest_fill.py` & `cubicweb-4.7.1/cubicweb/devtools/test/unittest_fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/unittest_i18n.py` & `cubicweb-4.7.1/cubicweb/devtools/test/unittest_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/test/unittest_testlib.py` & `cubicweb-4.7.1/cubicweb/devtools/test/unittest_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/devtools/testlib.py` & `cubicweb-4.7.1/cubicweb/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/__init__.py` & `cubicweb-4.7.1/cubicweb/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/adapters.py` & `cubicweb-4.7.1/cubicweb/entities/adapters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/authobjs.py` & `cubicweb-4.7.1/cubicweb/entities/authobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/lib.py` & `cubicweb-4.7.1/cubicweb/entities/lib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/schemaobjs.py` & `cubicweb-4.7.1/cubicweb/entities/schemaobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/sources.py` & `cubicweb-4.7.1/cubicweb/entities/sources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/test/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/entities/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/entities/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/test/unittest_base.py` & `cubicweb-4.7.1/cubicweb/entities/test/unittest_base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/test/unittest_wfobjs.py` & `cubicweb-4.7.1/cubicweb/entities/test/unittest_wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entities/wfobjs.py` & `cubicweb-4.7.1/cubicweb/entities/wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/entity.py` & `cubicweb-4.7.1/cubicweb/entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/ext/__init__.py` & `cubicweb-4.7.1/cubicweb/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/ext/html4zope.py` & `cubicweb-4.7.1/cubicweb/ext/html4zope.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/ext/markdown.py` & `cubicweb-4.7.1/cubicweb/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/ext/test/unittest_markdown.py` & `cubicweb-4.7.1/cubicweb/ext/test/unittest_markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/__init__.py` & `cubicweb-4.7.1/cubicweb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/bookmark.py` & `cubicweb-4.7.1/cubicweb/hooks/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/email.py` & `cubicweb-4.7.1/cubicweb/hooks/email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/integrity.py` & `cubicweb-4.7.1/cubicweb/hooks/integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/metadata.py` & `cubicweb-4.7.1/cubicweb/hooks/metadata.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/notification.py` & `cubicweb-4.7.1/cubicweb/hooks/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/security.py` & `cubicweb-4.7.1/cubicweb/hooks/security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/synccomputed.py` & `cubicweb-4.7.1/cubicweb/hooks/synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/syncschema.py` & `cubicweb-4.7.1/cubicweb/hooks/syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/syncsession.py` & `cubicweb-4.7.1/cubicweb/hooks/syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/syncsources.py` & `cubicweb-4.7.1/cubicweb/hooks/syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/hooks/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/data-computed/schema.py` & `cubicweb-4.7.1/cubicweb/hooks/test/data-computed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_bookmarks.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_hooks.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_integrity.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_notificationhooks.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_notificationhooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_security.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_synccomputed.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncschema.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsession.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsources.py` & `cubicweb-4.7.1/cubicweb/hooks/test/unittest_syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/hooks/workflow.py` & `cubicweb-4.7.1/cubicweb/hooks/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/i18n/de.po` & `cubicweb-4.7.1/cubicweb/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/i18n/en.po` & `cubicweb-4.7.1/cubicweb/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/i18n/es.po` & `cubicweb-4.7.1/cubicweb/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/i18n/fr.po` & `cubicweb-4.7.1/cubicweb/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/i18n.py` & `cubicweb-4.7.1/cubicweb/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/mail.py` & `cubicweb-4.7.1/cubicweb/mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/md5crypt.py` & `cubicweb-4.7.1/cubicweb/md5crypt.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/migration.py` & `cubicweb-4.7.1/cubicweb/migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/3.22.0_Any.py` & `cubicweb-4.7.1/cubicweb/misc/migration/3.22.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/3.23.0_Any.py` & `cubicweb-4.7.1/cubicweb/misc/migration/3.23.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/3.24.0_Any.py` & `cubicweb-4.7.1/cubicweb/misc/migration/3.24.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/3.24.4_Any.py` & `cubicweb-4.7.1/cubicweb/misc/migration/3.24.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/bootstrapmigration_repository.py` & `cubicweb-4.7.1/cubicweb/misc/migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/misc/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/scripts/chpasswd.py` & `cubicweb-4.7.1/cubicweb/misc/scripts/chpasswd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/scripts/fast_drop_entities.py` & `cubicweb-4.7.1/cubicweb/misc/scripts/fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/scripts/ldap_change_base_dn.py` & `cubicweb-4.7.1/cubicweb/misc/scripts/ldap_change_base_dn.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/scripts/migration_helper.py` & `cubicweb-4.7.1/cubicweb/misc/scripts/migration_helper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/misc/source_highlight.py` & `cubicweb-4.7.1/cubicweb/misc/source_highlight.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/mttransforms.py` & `cubicweb-4.7.1/cubicweb/mttransforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/multipart.py` & `cubicweb-4.7.1/cubicweb/multipart.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/predicates.py` & `cubicweb-4.7.1/cubicweb/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/__init__.py` & `cubicweb-4.7.1/cubicweb/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/auth.py` & `cubicweb-4.7.1/cubicweb/pyramid/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/config.py` & `cubicweb-4.7.1/cubicweb/pyramid/config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/core.py` & `cubicweb-4.7.1/cubicweb/pyramid/core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/csrf.py` & `cubicweb-4.7.1/cubicweb/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_source_code.py` & `cubicweb-4.7.1/cubicweb/pyramid/debug_source_code.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako` & `cubicweb-4.7.1/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/debugtoolbar_panels.py` & `cubicweb-4.7.1/cubicweb/pyramid/debugtoolbar_panels.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/default_session.py` & `cubicweb-4.7.1/cubicweb/pyramid/default_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/development.ini.tmpl` & `cubicweb-4.7.1/cubicweb/pyramid/development.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/predicates.py` & `cubicweb-4.7.1/cubicweb/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/pyramid.ini.tmpl` & `cubicweb-4.7.1/cubicweb/pyramid/pyramid.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/pyramidctl.py` & `cubicweb-4.7.1/cubicweb/pyramid/pyramidctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/resources.py` & `cubicweb-4.7.1/cubicweb/pyramid/resources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/rest_api.py` & `cubicweb-4.7.1/cubicweb/pyramid/rest_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/session.py` & `cubicweb-4.7.1/cubicweb/pyramid/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/__init__.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/test_auth.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/test_config.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/test_content_negociation.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/test_content_negociation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/test_core.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/test/test_tools.py` & `cubicweb-4.7.1/cubicweb/pyramid/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pyramid/tools.py` & `cubicweb-4.7.1/cubicweb/pyramid/tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/pytestconf.py` & `cubicweb-4.7.1/cubicweb/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/rdf.py` & `cubicweb-4.7.1/cubicweb/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/repoapi.py` & `cubicweb-4.7.1/cubicweb/repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/req.py` & `cubicweb-4.7.1/cubicweb/req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/rqlrewrite.py` & `cubicweb-4.7.1/cubicweb/rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/rqlsuggestions.py` & `cubicweb-4.7.1/cubicweb/rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/rset.py` & `cubicweb-4.7.1/cubicweb/rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/rtags.py` & `cubicweb-4.7.1/cubicweb/rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schema.py` & `cubicweb-4.7.1/cubicweb/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schema_exporters.py` & `cubicweb-4.7.1/cubicweb/schema_exporters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/Bookmark.py` & `cubicweb-4.7.1/cubicweb/schemas/Bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/__init__.py` & `cubicweb-4.7.1/cubicweb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/_regproc.postgres.sql` & `cubicweb-4.7.1/cubicweb/schemas/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/base.py` & `cubicweb-4.7.1/cubicweb/schemas/base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/bootstrap.py` & `cubicweb-4.7.1/cubicweb/schemas/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/schemas/workflow.py` & `cubicweb-4.7.1/cubicweb/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/__init__.py` & `cubicweb-4.7.1/cubicweb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/check_unused_index.py` & `cubicweb-4.7.1/cubicweb/server/check_unused_index.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/checkintegrity.py` & `cubicweb-4.7.1/cubicweb/server/checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/edition.py` & `cubicweb-4.7.1/cubicweb/server/edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/hook.py` & `cubicweb-4.7.1/cubicweb/server/hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/migractions.py` & `cubicweb-4.7.1/cubicweb/server/migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/querier.py` & `cubicweb-4.7.1/cubicweb/server/querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/repository.py` & `cubicweb-4.7.1/cubicweb/server/repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/rqlannotation.py` & `cubicweb-4.7.1/cubicweb/server/rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/schema2sql.py` & `cubicweb-4.7.1/cubicweb/server/schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/schemaserial.py` & `cubicweb-4.7.1/cubicweb/server/schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/serverconfig.py` & `cubicweb-4.7.1/cubicweb/server/serverconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/serverctl.py` & `cubicweb-4.7.1/cubicweb/server/serverctl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1147,21 +1147,21 @@
             },
         ),
     )
 
     def _get_dump_from_s3(self, appid, filepath):
         # fget_object(bucket_name, object_name, file_path, request_headers=None, ssec=None, version_id=None, extra_query_params=None, tmp_file_path=None)
         config = CubicWebConfiguration.config_for(appid)
-        s3_bucket_name = config.get("s3-bucket-name")
+        s3_bucket_name = config.get("dump-s3-bucket-name")
 
         # open s3 connection
         client = _get_s3_client(
-            config.get("s3-endpoint-url"),
-            config.get("s3-access-key"),
-            config.get("s3-secret-key"),
+            config.get("dump-s3-endpoint-url"),
+            config.get("dump-s3-access-key"),
+            config.get("dump-s3-secret-key"),
             s3_bucket_name,
         )
 
         tmpfile = NamedTemporaryFile(suffix=f".{filepath.split('.', maxsplit=1)[-1]}")
 
         # download file to tmp file
         client.fget_object(s3_bucket_name, filepath, tmpfile.name)
```

### Comparing `cubicweb-4.7.0/cubicweb/server/session.py` & `cubicweb-4.7.1/cubicweb/server/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/__init__.py` & `cubicweb-4.7.1/cubicweb/server/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/datafeed.py` & `cubicweb-4.7.1/cubicweb/server/sources/datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/ldapfeed.py` & `cubicweb-4.7.1/cubicweb/server/sources/ldapfeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/native.py` & `cubicweb-4.7.1/cubicweb/server/sources/native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/rql2sql.py` & `cubicweb-4.7.1/cubicweb/server/sources/rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sources/storages.py` & `cubicweb-4.7.1/cubicweb/server/sources/storages.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/sqlutils.py` & `cubicweb-4.7.1/cubicweb/server/sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/ssplanner.py` & `cubicweb-4.7.1/cubicweb/server/ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/ldap_test.ldif` & `cubicweb-4.7.1/cubicweb/server/test/data/ldap_test.ldif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data/slapd.conf.in` & `cubicweb-4.7.1/cubicweb/server/test/data/slapd.conf.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-cwep002/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-cwep002/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-migractions/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Company.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Company.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Dates.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/State.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/State.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/__init__.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schema2sql/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/datacomputed/schema.py` & `cubicweb-4.7.1/cubicweb/server/test/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_datafeed.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_edition.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_hook.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_ldapsource.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_ldapsource.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_querier.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_rql2sql.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_rqlannotation.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_schema2sql.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_schemaserial.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_server_security.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_server_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_server_utils.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_server_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_serverctl.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_session.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_sources_native.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_sources_native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_sqlutils.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_ssplanner.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_storage.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_storage.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_tools.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_undo.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_undo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test/unittest_utils.py` & `cubicweb-4.7.1/cubicweb/server/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py` & `cubicweb-4.7.1/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions/unittest_migractions.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions2/unittest_migractions.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions2/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_migractions3/unittest_migractions.py` & `cubicweb-4.7.1/cubicweb/server/test_migractions3/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/postcreate.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_postgres/unittest_postgres.py` & `cubicweb-4.7.1/cubicweb/server/test_postgres/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/entities.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/hooks.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/schema.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/test_repository/unittest_repository.py` & `cubicweb-4.7.1/cubicweb/server/test_repository/unittest_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/server/utils.py` & `cubicweb-4.7.1/cubicweb/server/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/.gitlab-ci.yml.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/README.rst.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/README.rst.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/setup.py.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py` & `cubicweb-4.7.1/cubicweb/skeleton/test/realdb_test_CUBENAME.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/skeleton/tox.ini.tmpl` & `cubicweb-4.7.1/cubicweb/skeleton/tox.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py` & `cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py` & `cubicweb-4.7.1/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/__init__.py` & `cubicweb-4.7.1/cubicweb/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/ldapparser.py` & `cubicweb-4.7.1/cubicweb/sobjects/ldapparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/notification.py` & `cubicweb-4.7.1/cubicweb/sobjects/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/services.py` & `cubicweb-4.7.1/cubicweb/sobjects/services.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/supervising.py` & `cubicweb-4.7.1/cubicweb/sobjects/supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/__init__.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/data/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_email.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_notification.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_register_user.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_register_user.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_supervising.py` & `cubicweb-4.7.1/cubicweb/sobjects/test/unittest_supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/tags.py` & `cubicweb-4.7.1/cubicweb/tags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_email/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_file/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_forge/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__init__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/schema.py` & `cubicweb-4.7.1/cubicweb/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/entities.py` & `cubicweb-4.7.1/cubicweb/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/erqlexpr_on_ertype.py` & `cubicweb-4.7.1/cubicweb/test/data/erqlexpr_on_ertype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.0.3_Any.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.0.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.0.4_Any.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.0.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_Any.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_common.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_common.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_repository.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.0_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.2_Any.py` & `cubicweb-4.7.1/cubicweb/test/data/migration/0.1.2_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_ertype_read.py` & `cubicweb-4.7.1/cubicweb/test/data/rqlexpr_on_ertype_read.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_attr.py` & `cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_attr.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_eetype.py` & `cubicweb-4.7.1/cubicweb/test/data/rrqlexpr_on_eetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/schema.py` & `cubicweb-4.7.1/cubicweb/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py` & `cubicweb-4.7.1/cubicweb/test/data/server_migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py` & `cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py` & `cubicweb-4.7.1/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data-rewrite/schema.py` & `cubicweb-4.7.1/cubicweb/test/data-rewrite/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/data_schemareader/schema.py` & `cubicweb-4.7.1/cubicweb/test/data_schemareader/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_binary.py` & `cubicweb-4.7.1/cubicweb/test/unittest_binary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_cwconfig.py` & `cubicweb-4.7.1/cubicweb/test/unittest_cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_cwctl.py` & `cubicweb-4.7.1/cubicweb/test/unittest_cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_entity.py` & `cubicweb-4.7.1/cubicweb/test/unittest_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_fast_drop_entities.py` & `cubicweb-4.7.1/cubicweb/test/unittest_fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_mail.py` & `cubicweb-4.7.1/cubicweb/test/unittest_mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_migration.py` & `cubicweb-4.7.1/cubicweb/test/unittest_migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_predicates.py` & `cubicweb-4.7.1/cubicweb/test/unittest_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_repoapi.py` & `cubicweb-4.7.1/cubicweb/test/unittest_repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_req.py` & `cubicweb-4.7.1/cubicweb/test/unittest_req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_rqlrewrite.py` & `cubicweb-4.7.1/cubicweb/test/unittest_rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_rqlsuggestions.py` & `cubicweb-4.7.1/cubicweb/test/unittest_rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_rset.py` & `cubicweb-4.7.1/cubicweb/test/unittest_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_rtags.py` & `cubicweb-4.7.1/cubicweb/test/unittest_rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_schema.py` & `cubicweb-4.7.1/cubicweb/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_toolsutils.py` & `cubicweb-4.7.1/cubicweb/test/unittest_toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_uilib.py` & `cubicweb-4.7.1/cubicweb/test/unittest_uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_vregistry.py` & `cubicweb-4.7.1/cubicweb/test/unittest_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/test/unittest_wfutils.py` & `cubicweb-4.7.1/cubicweb/test/unittest_wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/toolsutils.py` & `cubicweb-4.7.1/cubicweb/toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/transaction.py` & `cubicweb-4.7.1/cubicweb/transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/uilib.py` & `cubicweb-4.7.1/cubicweb/uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/utils.py` & `cubicweb-4.7.1/cubicweb/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/wfutils.py` & `cubicweb-4.7.1/cubicweb/wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb/xy.py` & `cubicweb-4.7.1/cubicweb/xy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/cubicweb.egg-info/SOURCES.txt` & `cubicweb-4.7.1/cubicweb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -773,17 +773,15 @@
 doc/announce.en.txt
 doc/announce.fr.txt
 doc/conf.py
 doc/index.rst
 doc/plan_formation_python_cubicweb.txt
 doc/stdlib.txt
 doc/_static/favicon.ico
-doc/_static/favicon.ico.orig
 doc/_static/logo-cubicweb.svg
-doc/_static/logo-cubicweb.svg.orig
 doc/api/__init__.rst
 doc/api/appobject.rst
 doc/api/cwvreg.rst
 doc/api/dataimport.rst
 doc/api/index.rst
 doc/api/predicates.rst
 doc/api/pyramid.rst
@@ -805,58 +803,48 @@
 doc/book/_maybe_to_integrate/rss-xml.rst
 doc/book/_maybe_to_integrate/template.rst
 doc/book/additionnal_services/index.rst
 doc/book/additionnal_services/undo.rst
 doc/book/admin/backups.rst
 doc/book/admin/config.rst
 doc/book/admin/create-instance.rst
-doc/book/admin/create-instance.rst.orig
 doc/book/admin/cubicweb-ctl.rst
-doc/book/admin/cubicweb-ctl.rst.orig
 doc/book/admin/deploy.rst
-doc/book/admin/deploy.rst.orig
 doc/book/admin/index.rst
-doc/book/admin/index.rst.orig
 doc/book/admin/instance-config.rst
-doc/book/admin/instance-config.rst.orig
 doc/book/admin/ldap.rst
 doc/book/admin/multisources.rst
 doc/book/admin/rql-logs.rst
 doc/book/admin/setup.rst
-doc/book/admin/setup.rst.orig
 doc/book/admin/site-config.rst
 doc/book/annexes/depends.rst
 doc/book/annexes/docstrings-conventions.rst
 doc/book/annexes/faq.rst
-doc/book/annexes/faq.rst.orig
 doc/book/annexes/index.rst
 doc/book/annexes/mercurial.rst
 doc/book/annexes/rql/Graph-ex.gif
 doc/book/annexes/rql/debugging.rst
 doc/book/annexes/rql/implementation.rst
 doc/book/annexes/rql/index.rst
 doc/book/annexes/rql/intro.rst
 doc/book/annexes/rql/language.rst
 doc/book/annexes/rql/usecases.rst
-doc/book/annexes/rql/usecases.rst.orig
 doc/book/devrepo/connections_pooler.rst
 doc/book/devrepo/dataimport.rst
 doc/book/devrepo/debug_channels.rst
 doc/book/devrepo/fti.rst
 doc/book/devrepo/index.rst
 doc/book/devrepo/migration.rst
 doc/book/devrepo/profiling.rst
 doc/book/devrepo/testing.rst
 doc/book/devrepo/vreg.rst
-doc/book/devrepo/vreg.rst.orig
 doc/book/devrepo/cubes/available-cubes.rst
 doc/book/devrepo/cubes/cc-newcube.rst
 doc/book/devrepo/cubes/index.rst
 doc/book/devrepo/cubes/layout.rst
-doc/book/devrepo/cubes/layout.rst.orig
 doc/book/devrepo/cubes/what-is-a-cube.rst
 doc/book/devrepo/datamodel/baseschema.rst
 doc/book/devrepo/datamodel/define-workflows.rst
 doc/book/devrepo/datamodel/definition.rst
 doc/book/devrepo/datamodel/index.rst
 doc/book/devrepo/datamodel/metadata.rst
 doc/book/devrepo/devcore/index.rst
@@ -868,95 +856,57 @@
 doc/book/devrepo/entityclasses/load-sort.rst
 doc/book/devrepo/repo/hooks.rst
 doc/book/devrepo/repo/index.rst
 doc/book/devrepo/repo/notifications.rst
 doc/book/devrepo/repo/sessions.rst
 doc/book/devrepo/repo/tasks.rst
 doc/book/devweb/ajax.rst
-doc/book/devweb/ajax.rst.orig
 doc/book/devweb/controllers.rst
-doc/book/devweb/controllers.rst.orig
 doc/book/devweb/css.rst
-doc/book/devweb/css.rst.orig
 doc/book/devweb/facets.rst
-doc/book/devweb/facets.rst.orig
 doc/book/devweb/httpcaching.rst
-doc/book/devweb/httpcaching.rst.orig
 doc/book/devweb/index.rst
-doc/book/devweb/index.rst.orig
 doc/book/devweb/internationalization.rst
-doc/book/devweb/internationalization.rst.orig
 doc/book/devweb/js.rst
-doc/book/devweb/js.rst.orig
 doc/book/devweb/property.rst
-doc/book/devweb/property.rst.orig
 doc/book/devweb/publisher.rst
-doc/book/devweb/publisher.rst.orig
 doc/book/devweb/request.rst
-doc/book/devweb/request.rst.orig
 doc/book/devweb/resource.rst
-doc/book/devweb/resource.rst.orig
 doc/book/devweb/rtags.rst
-doc/book/devweb/rtags.rst.orig
 doc/book/devweb/searchbar.rst
-doc/book/devweb/searchbar.rst.orig
 doc/book/devweb/warning.rst
 doc/book/devweb/edition/dissection.rst
-doc/book/devweb/edition/dissection.rst.orig
 doc/book/devweb/edition/editcontroller.rst
-doc/book/devweb/edition/editcontroller.rst.orig
 doc/book/devweb/edition/examples.rst
-doc/book/devweb/edition/examples.rst.orig
 doc/book/devweb/edition/form.rst
-doc/book/devweb/edition/form.rst.orig
 doc/book/devweb/edition/index.rst
-doc/book/devweb/edition/index.rst.orig
 doc/book/devweb/views/basetemplates.rst
-doc/book/devweb/views/basetemplates.rst.orig
 doc/book/devweb/views/baseviews.rst
-doc/book/devweb/views/baseviews.rst.orig
 doc/book/devweb/views/boxes.rst
-doc/book/devweb/views/boxes.rst.orig
 doc/book/devweb/views/breadcrumbs.rst
-doc/book/devweb/views/breadcrumbs.rst.orig
 doc/book/devweb/views/idownloadable.rst
-doc/book/devweb/views/idownloadable.rst.orig
 doc/book/devweb/views/index.rst
-doc/book/devweb/views/index.rst.orig
 doc/book/devweb/views/primary.rst
-doc/book/devweb/views/primary.rst.orig
 doc/book/devweb/views/reledit.rst
-doc/book/devweb/views/reledit.rst.orig
 doc/book/devweb/views/startup.rst
-doc/book/devweb/views/startup.rst.orig
 doc/book/devweb/views/table.rst
-doc/book/devweb/views/table.rst.orig
 doc/book/devweb/views/urlpublish.rst
-doc/book/devweb/views/urlpublish.rst.orig
 doc/book/devweb/views/views.rst
-doc/book/devweb/views/views.rst.orig
 doc/book/devweb/views/wdoc.rst
-doc/book/devweb/views/wdoc.rst.orig
 doc/book/devweb/views/xmlrss.rst
-doc/book/devweb/views/xmlrss.rst.orig
 doc/book/intro/concepts.rst
 doc/book/intro/history.rst
 doc/book/intro/index.rst
 doc/book/pyramid/auth.rst
-doc/book/pyramid/auth.rst.orig
 doc/book/pyramid/ctl.rst
 doc/book/pyramid/debug_toolbar.rst
-doc/book/pyramid/debug_toolbar.rst.orig
 doc/book/pyramid/index.rst
 doc/book/pyramid/quickstart.rst
-doc/book/pyramid/quickstart.rst.orig
 doc/book/pyramid/settings.rst
-doc/book/pyramid/settings.rst.orig
 doc/book/security/csrf.rst
-doc/book/security/csrf.rst.orig
 doc/book/src/archi_globale.dia
 doc/book/src/main_template_layout.dia
 doc/changes/3.14.rst
 doc/changes/3.15.rst
 doc/changes/3.16.rst
 doc/changes/3.17.rst
 doc/changes/3.18.rst
```

### Comparing `cubicweb-4.7.0/doc/4.0.0_how_to_migrate.rst` & `cubicweb-4.7.1/doc/4.0.0_how_to_migrate.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/Makefile` & `cubicweb-4.7.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/_static/favicon.ico` & `cubicweb-4.7.1/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/_static/logo-cubicweb.svg` & `cubicweb-4.7.1/doc/_static/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/announce.en.txt` & `cubicweb-4.7.1/doc/announce.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/announce.fr.txt` & `cubicweb-4.7.1/doc/announce.fr.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/__init__.rst` & `cubicweb-4.7.1/doc/api/__init__.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/cwvreg.rst` & `cubicweb-4.7.1/doc/api/cwvreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/predicates.rst` & `cubicweb-4.7.1/doc/api/predicates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/pyramid/core.rst` & `cubicweb-4.7.1/doc/api/pyramid/core.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/urlpublishing.rst` & `cubicweb-4.7.1/doc/api/urlpublishing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/api/web.rst` & `cubicweb-4.7.1/doc/api/web.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-app.en.txt` & `cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt` & `cubicweb-4.7.1/doc/book/MERGE_ME-tut-create-gae-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/_maybe_to_integrate/rss-xml.rst` & `cubicweb-4.7.1/doc/book/_maybe_to_integrate/rss-xml.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/_maybe_to_integrate/template.rst` & `cubicweb-4.7.1/doc/book/_maybe_to_integrate/template.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/additionnal_services/undo.rst` & `cubicweb-4.7.1/doc/book/additionnal_services/undo.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/backups.rst` & `cubicweb-4.7.1/doc/book/admin/backups.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/config.rst` & `cubicweb-4.7.1/doc/book/admin/config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/create-instance.rst` & `cubicweb-4.7.1/doc/book/admin/create-instance.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst` & `cubicweb-4.7.1/doc/book/admin/cubicweb-ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/deploy.rst` & `cubicweb-4.7.1/doc/book/admin/deploy.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/instance-config.rst` & `cubicweb-4.7.1/doc/book/admin/instance-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/ldap.rst` & `cubicweb-4.7.1/doc/book/admin/ldap.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/setup.rst` & `cubicweb-4.7.1/doc/book/admin/setup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/admin/site-config.rst` & `cubicweb-4.7.1/doc/book/admin/site-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/depends.rst` & `cubicweb-4.7.1/doc/book/annexes/depends.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/docstrings-conventions.rst` & `cubicweb-4.7.1/doc/book/annexes/docstrings-conventions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/faq.rst` & `cubicweb-4.7.1/doc/book/annexes/faq.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/faq.rst.orig` & `cubicweb-4.7.1/doc/book/devweb/edition/form.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,434 +1,378 @@
-.. -*- coding: utf-8 -*-
+.. include:: ../warning.rst
 
-Frequently Asked Questions (FAQ)
-================================
+.. _webform:
 
+HTML form construction
+----------------------
 
-Generalities
-````````````
+CubicWeb provides the somewhat usual form / field / widget / renderer abstraction
+to provide generic building blocks which will greatly help you in building forms
+properly integrated with CubicWeb (coherent display, error handling, etc...),
+while keeping things as flexible as possible.
+
+A ``form`` basically only holds a set of ``fields``, and has te be bound to a
+``renderer`` which is responsible to layout them. Each field is bound to a
+``widget`` that will be used to fill in value(s) for that field (at form
+generation time) and 'decode' (fetch and give a proper Python type to) values
+sent back by the browser.
+
+The ``field`` should be used according to the type of what you want to edit.
+E.g. if you want to edit some date, you'll have to use the
+:class:`cubicweb_web.formfields.DateField`. Then you can choose among multiple
+widgets to edit it, for instance :class:`cubicweb_web.formwidgets.TextInput` (a
+bare text field), :class:`~cubicweb_web.formwidgets.DateTimePicker` (a simple
+calendar) or even :class:`~cubicweb_web.formwidgets.JQueryDatePicker` (the JQuery
+calendar).  You can of course also write your own widget.
 
-Why do you use the LGPL license to prevent me from doing X ?
-------------------------------------------------------------
+Exploring the available forms
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-LGPL means that *if* you redistribute your application, you need to
-redistribute the changes you made to CubicWeb under the LGPL licence.
-
-Publishing a web site has nothing to do with redistributing source
-code according to the terms of the LGPL. A fair amount of companies
-use modified LGPL code for internal use. And someone could publish a
-*CubicWeb* component under a BSD licence for others to plug into a
-LGPL framework without any problem. The only thing we are trying to
-prevent here is someone taking the framework and packaging it as
-closed source to his own clients.
-
-Why does not CubicWeb have a template language ?
-------------------------------------------------
-
-There are enough template languages out there. You can use your
-preferred template language if you want.
-
-.. TODO explain how to use a template language
-
-*CubicWeb* does not define its own templating language as this was
-not our goal. Based on our experience, we realized that
-we could gain productivity by letting designers use design tools
-and developpers develop without the use of the templating language
-as an intermediary that could not be anyway efficient for both parties.
-Python is the templating language that we use in *CubicWeb*, but again,
-it does not prevent you from using a templating language.
-
-Moreover, CubicWeb currently supports `simpletal`_ out of the box and
-it is also possible to use the `cwtags`_ library to build html trees
-using the `with statement`_ with more comfort than raw strings.
-
-.. _`simpletal`: http://www.owlfish.com/software/simpleTAL/
-.. _`cwtags`: https://forge.extranet.logilab.fr/cubicweb/cubes/tag
-.. _`with statement`: http://www.python.org/dev/peps/pep-0343/
-
-Why do you think using pure python is better than using a template language ?
------------------------------------------------------------------------------
-
-Python is an Object Oriented Programming language and as such it
-already provides a consistent and strong architecture and syntax
-a templating language would not reach.
-
-Using Python instead of a template langage for describing the user interface
-makes it to maintain with real functions/classes/contexts without the need of
-learning a new dialect. By using Python, we use standard OOP techniques and
-this is a key factor in a robust application.
-
-CubicWeb looks pretty recent. Is it stable ?
---------------------------------------------
-
-It is constantly evolving, piece by piece.  The framework has evolved since
-2001 and data has been migrated from one schema to the other ever since. There
-is a well-defined way to handle data and schema migration.
-
-You can see the roadmap there:
-https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/boards.
-
-
-Why is the RQL query language looking similar to X ?
-----------------------------------------------------
-
-It may remind you of SQL but it is higher level than SQL, more like
-SPARQL. Except that SPARQL did not exist when we started the project.
-With version 3.4, CubicWeb has support for SPARQL.
-
-The RQL language is what is going to make a difference with django-
-like frameworks for several reasons.
-
-1. accessing data is *much* easier with it. One can write complex
-   queries with RQL that would be tedious to define and hard to maintain
-   using an object/filter suite of method calls.
-
-2. it offers an abstraction layer allowing your applications to run
-   on multiple back-ends. That means not only various SQL backends
-   (postgresql, sqlite, sqlserver, mysql), but also non-SQL data stores like
-   LDAP directories and subversion/mercurial repositories (see the `vcsfile`
-   component).
-
-Which ajax library is CubicWeb using ?
---------------------------------------
-
-CubicWeb uses jQuery_ and provides a few helpers on top of that. Additionally,
-some jQuery plugins are provided (some are provided in specific cubes).
-
-.. _jQuery: http://jquery.com
-
-
-Development
-```````````
-
-How to change the instance logo ?
----------------------------------
-
-The logo is managed by css. You must provide a custom css that will contain
-the code below:
-
-::
-
-     #logo {
-        background-image: url("logo.jpg");
-     }
-
-
-``logo.jpg`` is in ``mycube/data`` directory.
-
-How to create an anonymous user ?
----------------------------------
-
-This allows to browse the site without being authenticated. In the
-``all-in-one.conf`` file of your instance, define the anonymous user
-as follows ::
-
-  # login of the CubicWeb user account to use for anonymous user (if you want to
-  # allow anonymous)
-  anonymous-user=anon
-
-  # password of the CubicWeb user account matching login
-  anonymous-password=anon
-
-You also must ensure that this `anon` user is a registered user of
-the DB backend. If not, you can create through the administation
-interface of your instance by adding a user with in the group `guests`.
-
-.. note::
-    While creating a new instance, you can decide to allow access
-    to anonymous user, which will automatically execute what is
-    decribed above.
-
-
-How to format an entity date attribute ?
-----------------------------------------
-
-If your schema has an attribute of type `Date` or `Datetime`, you usually want to
-format it when displaying it. First, you should define your preferred format
-using the site configuration panel
-``http://appurl/view?vid=systempropertiesform`` and then set ``ui.date`` and/or
-``ui.datetime``.  Then in the view code, use:
+A small excursion into a |cubicweb| shell is the quickest way to
+discover available forms (or application objects in general).
 
 .. sourcecode:: python
 
-    entity.printable_value(date_attribute)
-
-which will always return a string whatever the attribute's type (so it's
-recommended also for other attribute types). By default it expects to generate
-HTML, so it deals with rich text formating, xml escaping...
-
-How to update a database after a schema modification ?
-------------------------------------------------------
-
-It depends on what has been modified in the schema.
+ >>> from pprint import pprint
+ >>> pprint( session.vreg['forms'] )
+ {'base': [<class 'cubicweb_web.views.forms.FieldsForm'>,
+           <class 'cubicweb_web.views.forms.EntityFieldsForm'>],
+  'changestate': [<class 'cubicweb_web.views.workflow.ChangeStateForm'>,
+                  <class 'cubicweb_tracker.views.forms.VersionChangeStateForm'>],
+  'composite': [<class 'cubicweb_web.views.forms.CompositeForm'>,
+                <class 'cubicweb_web.views.forms.CompositeEntityForm'>],
+  'deleteconf': [<class 'cubicweb_web.views.editforms.DeleteConfForm'>],
+  'edition': [<class 'cubicweb_web.views.autoform.AutomaticEntityForm'>,
+              <class 'cubicweb_web.views.workflow.TransitionEditionForm'>,
+              <class 'cubicweb_web.views.workflow.StateEditionForm'>],
+  'logform': [<class 'cubicweb_web.views.basetemplates.LogForm'>],
+  'massmailing': [<class 'cubicweb_web.views.massmailing.MassMailingForm'>],
+  'muledit': [<class 'cubicweb_web.views.editforms.TableEditForm'>]}
+
+
+The two most important form families here (for all practical purposes) are `base`
+and `edition`. Most of the time one wants alterations of the
+:class:`AutomaticEntityForm` to generate custom forms to handle edition of an
+entity.
+
+The Automatic Entity Form
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. automodule:: cubicweb_web.views.autoform
+
+Anatomy of a choices function
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Let's have a look at the `ticket_done_in_choices` function given to
+the `choices` parameter of the relation tag that is applied to the
+('Ticket', 'done_in', '*') relation definition, as it is both typical
+and sophisticated enough. This is a code snippet from the `tracker`_
+cube.
+
+.. _`tracker`: https://forge.extranet.logilab.fr/cubicweb/cubes/tracker
+
+The ``Ticket`` entity type can be related to a ``Project`` and a
+``Version``, respectively through the ``concerns`` and ``done_in``
+relations. When a user is about to edit a ticket, we want to fill the
+combo box for the ``done_in`` relation with values pertinent with
+respect to the context. The important context here is:
 
-* update the permissions and properties of an entity or a relation:
-  ``sync_schema_props_perms('MyEntityOrRelation')``.
+* creation or modification (we cannot fetch values the same way in
+  either case)
 
-* add an attribute: ``add_attribute('MyEntityType', 'myattr')``.
-
-* add a relation: ``add_relation_definition('SubjRelation', 'MyRelation', 'ObjRelation')``.
-
-I get `NoSelectableObject` exceptions, how do I debug selectors ?
------------------------------------------------------------------
-
-You just need to put the appropriate context manager around view/component
-selection. One standard place for components is in cubicweb/vregistry.py:
+* ``__linkto`` url parameter given in a creation context
 
 .. sourcecode:: python
 
-    def possible_objects(self, *args, **kwargs):
-        """return an iterator on possible objects in this registry for the given
-        context
-        """
-        from logilab.common.registry import traced_selection
-        with traced_selection():
-            for appobjects in self.itervalues():
-                try:
-                    yield self._select_best(appobjects, *args, **kwargs)
-                except NoSelectableObject:
-                    continue
-
-This will yield additional WARNINGs, like this::
-
-    2009-01-09 16:43:52 - (cubicweb.selectors) WARNING: selector one_line_rset returned 0 for <class 'cubicweb_web.views.basecomponents.WFHistoryVComponent'>
+    from cubicweb_web import formfields
 
-For views, you can put this context in `cubicweb/web/views/basecontrollers.py` in
-the `ViewController`:
+    def ticket_done_in_choices(form, field):
+        entity = form.edited_entity
+        # first see if its specified by __linkto form parameters
+        linkedto = form.linked_to[('done_in', 'subject')]
+        if linkedto:
+            return linkedto
+        # it isn't, get initial values
+        vocab = field.relvoc_init(form)
+        veid = None
+        # try to fetch the (already or pending) related version and project
+        if not entity.has_eid():
+            peids = form.linked_to[('concerns', 'subject')]
+            peid = peids and peids[0]
+        else:
+            peid = entity.project.eid
+            veid = entity.done_in and entity.done_in[0].eid
+        if peid:
+            # we can complete the vocabulary with relevant values
+            rschema = form._cw.vreg.schema['done_in'].rdef('Ticket', 'Version')
+            rset = form._cw.execute(
+                'Any V, VN ORDERBY version_sort_value(VN) '
+                'WHERE V version_of P, P eid %(p)s, V num VN, '
+                'V in_state ST, NOT ST name "published"', {'p': peid}, 'p')
+            vocab += [(v.view('combobox'), v.eid) for v in rset.entities()
+                      if rschema.has_perm(form._cw, 'add', toeid=v.eid)
+                      and v.eid != veid]
+        return vocab
+
+The first thing we have to do is fetch potential values from the ``__linkto`` url
+parameter that is often found in entity creation contexts (the creation action
+provides such a parameter with a predetermined value; for instance in this case,
+ticket creation could occur in the context of a `Version` entity). The
+:class:`~cubicweb_web.formfields.RelationField` field class provides a
+:meth:`~cubicweb_web.formfields.RelationField.relvoc_linkedto` method that gets a
+list suitably filled with vocabulary values.
 
 .. sourcecode:: python
 
-    def _select_view_and_rset(self, rset):
-        ...
-        try:
-            from logilab.common.registry import traced_selection
-            with traced_selection():
-                view = self._cw.vreg['views'].select(vid, req, rset=rset)
-        except ObjectNotFound:
-            self.warning("the view %s could not be found", vid)
-            req.set_message(req._("The view %s could not be found") % vid)
-            vid = vid_from_rset(req, rset, self._cw.vreg.schema)
-            view = self._cw.vreg['views'].select(vid, req, rset=rset)
-        ...
-
-I get "database is locked" when executing tests
------------------------------------------------
+        linkedto = field.relvoc_linkedto(form)
+        if linkedto:
+            return linkedto
+
+Then, if no ``__linkto`` argument was given, we must prepare the vocabulary with
+an initial empty value (because `done_in` is not mandatory, we must allow the
+user to not select a verson) and already linked values. This is done with the
+:meth:`~cubicweb_web.formfields.RelationField.relvoc_init` method.
 
-If you have "database is locked" as error when you are executing security tests,
-it is usually because commit or rollback are missing before login() calls.
+.. sourcecode:: python
 
-You can also use a context manager, to avoid such errors, as described
-here: :ref:`securitytest`.
+        vocab = field.relvoc_init(form)
 
+But then, we have to give more: if the ticket is related to a project,
+we should provide all the non published versions of this project
+(`Version` and `Project` can be related through the `version_of`
+relation). Conversely, if we do not know yet the project, it would not
+make sense to propose all existing versions as it could potentially
+lead to incoherences. Even if these will be caught by some
+RQLConstraint, it is wise not to tempt the user with error-inducing
+candidate values.
+
+The "ticket is related to a project" part must be decomposed as:
+
+* this is a new ticket which is created is the context of a project
+
+* this is an already existing ticket, linked to a project (through the
+  `concerns` relation)
+
+* there is no related project (quite unlikely given the cardinality of
+  the `concerns` relation, so it can only mean that we are creating a
+  new ticket, and a project is about to be selected but there is no
+  ``__linkto`` argument)
 
-What are hooks used for ?
--------------------------
+.. note::
 
-Hooks are executed around (actually before or after) events.  The most common
-events are data creation, update and deletion.  They permit additional constraint
-checking (those not expressible at the schema level), pre and post computations
-depending on data movements.
+   the last situation could happen in several ways, but of course in a
+   polished application, the paths to ticket creation should be
+   controlled so as to avoid a suboptimal end-user experience
 
-As such, they are a vital part of the framework.
+Hence, we try to fetch the related project.
 
-Other kinds of hooks, called Operations, are available
-for execution just before commit.
+.. sourcecode:: python
 
-For more information, read :ref:`hooks` section.
+        veid = None
+        if not entity.has_eid():
+            peids = form.linked_to[('concerns', 'subject')]
+            peid = peids and peids[0]
+        else:
+            peid = entity.project.eid
+            veid = entity.done_in and entity.done_in[0].eid
+
+We distinguish between entity creation and entity modification using
+the ``Entity.has_eid()`` method, which returns `False` on creation. At
+creation time the only way to get a project is through the
+``__linkto`` parameter. Notice that we fetch the version in which the
+ticket is `done_in` if any, for later.
 
+.. note::
 
-Configuration
-`````````````
+  the implementation above assumes that if there is a ``__linkto``
+  parameter, it is only about a project. While it makes sense most of
+  the time, it is not an absolute. Depending on how an entity creation
+  action action url is built, several outcomes could be possible
+  there
 
-How to configure a LDAP source ?
---------------------------------
+If the ticket is already linked to a project, fetching it is
+trivial. Then we add the relevant version to the initial vocabulary.
 
-See :ref:`LDAP`.
+.. sourcecode:: python
 
-How to import LDAP users in |cubicweb| ?
-----------------------------------------
+        if peid:
+            rschema = form._cw.vreg.schema['done_in'].rdef('Ticket', 'Version')
+            rset = form._cw.execute(
+                'Any V, VN ORDERBY version_sort_value(VN) '
+                'WHERE V version_of P, P eid %(p)s, V num VN, '
+                'V in_state ST, NOT ST name "published"', {'p': peid})
+            vocab += [(v.view('combobox'), v.eid) for v in rset.entities()
+                      if rschema.has_perm(form._cw, 'add', toeid=v.eid)
+                      and v.eid != veid]
+
+.. warning::
+
+   we have to defend ourselves against lack of a project eid. Given
+   the cardinality of the `concerns` relation, there *must* be a
+   project, but this rule can only be enforced at validation time,
+   which will happen of course only after form subsmission
+
+Here, given a project eid, we complete the vocabulary with all
+unpublished versions defined in the project (sorted by number) for
+which the current user is allowed to establish the relation.
+
+
+Building self-posted form with custom fields/widgets
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Sometimes you want a form that is not related to entity edition. For those,
+you'll have to handle form posting by yourself. Here is a complete example on how
+to achieve this (and more).
 
-  Here is a useful script which enables you to import LDAP users
-  into your *CubicWeb* instance by running the following:
+Imagine you want a form that selects a month period. There are no proper
+field/widget to handle this in CubicWeb, so let's start by defining them:
 
 .. sourcecode:: python
 
-    import os
-    import pwd
-    import sys
-
-    from logilab.database import get_connection
-
-    def getlogin():
-        """avoid using os.getlogin() because of strange tty/stdin problems
-        (man 3 getlogin)
-        Another solution would be to use $LOGNAME, $USER or $USERNAME
+    # let's have the whole import list at the beginning, even those necessary for
+    # subsequent snippets
+    from logilab.common import date
+    from logilab.mtconverter import xml_escape
+    from cubicweb.predicates import match_kwargs
+    from cubicweb_web.view import View
+    from cubicweb_web import RequestError, ProcessFormError
+    from cubicweb_web import formfields as fields, formwidgets as wdgs
+    from cubicweb_web.views import forms, calendar
+
+    class MonthSelect(wdgs.Select):
+        """Custom widget to display month and year. Expect value to be given as a
+        date instance.
         """
-        return pwd.getpwuid(os.getuid())[0]
-
 
-    try:
-        database = sys.argv[1]
-    except IndexError:
-        print 'USAGE: python ldap2system.py <database>'
-        sys.exit(1)
+        def format_value(self, form, field, value):
+            return u'%s/%s' % (value.year, value.month)
 
-    if input('update %s db ? [y/n]: ' % database).strip().lower().startswith('y'):
-        cnx = get_connection(user=getlogin(), database=database)
-        cursor = cnx.cursor()
+        def process_field_data(self, form, field):
+            val = super(MonthSelect, self).process_field_data(form, field)
+            try:
+                year, month = val.split('/')
+                year = int(year)
+                month = int(month)
+                return date.date(year, month, 1)
+            except ValueError:
+                raise ProcessFormError(
+                    form._cw._('badly formated date string %s') % val)
 
-        insert = ('INSERT INTO euser (creation_date, eid, modification_date, login, '
-                  ' firstname, surname, last_login_time, upassword) '
-                  "VALUES (%(mtime)s, %(eid)s, %(mtime)s, %(login)s, %(firstname)s, "
-                  "%(surname)s, %(mtime)s, './fqEz5LeZnT6');")
-        update = "UPDATE entities SET source='system' WHERE eid=%(eid)s;"
-        cursor.execute("SELECT eid,type,source,extid,mtime FROM entities WHERE source!='system'")
-        for eid, type, source, extid, mtime in cursor.fetchall():
-            if type != 'CWUser':
-                print "don't know what to do with entity type", type
-                continue
-            if source != 'ldapuser':
-                print "don't know what to do with source type", source
-                continue
-            ldapinfos = dict(x.strip().split('=') for x in extid.split(','))
-            login = ldapinfos['uid']
-            firstname = ldapinfos['uid'][0].upper()
-            surname = ldapinfos['uid'][1:].capitalize()
-            if login != 'jcuissinat':
-                args = dict(eid=eid, type=type, source=source, login=login,
-                            firstname=firstname, surname=surname, mtime=mtime)
-                print args
-                cursor.execute(insert, args)
-                cursor.execute(update, args)
 
-        cnx.commit()
-        cnx.close()
+    class MonthPeriodField(fields.CompoundField):
+        """custom field composed of two subfields, 'begin_month' and 'end_month'.
 
+        It expects to be used on form that has 'mindate' and 'maxdate' in its
+        extra arguments, telling the range of month to display.
+        """
 
-Security
-````````
-
-How to reset the password for user joe ?
-----------------------------------------
-
-If you want to reset the admin password for ``myinstance``, do::
-
-    $ cubicweb-ctl reset-admin-pwd myinstance
-
-You need to generate a new encrypted password::
-
-    $ python
-    >>> from cubicweb.server.utils import crypt_password
-    >>> crypt_password('joepass')
-    'qHO8282QN5Utg'
-    >>>
-
-and paste it in the database::
-
-    $ psql mydb
-    mydb=> update cw_cwuser set cw_upassword='qHO8282QN5Utg' where cw_login='joe';
-    UPDATE 1
-
-if you're running over SQL Server, you need to use the CONVERT
-function to convert the string to varbinary(255). The SQL query is
-therefore::
-
-    update cw_cwuser set cw_upassword=CONVERT(varbinary(255), 'qHO8282QN5Utg') where cw_login='joe';
-
-Be careful, the encryption algorithm is different on Windows and on
-Unix. You cannot therefore use a hash generated on Unix to fill in a
-Windows database, nor the other way round.
-
-
-You can prefer use a migration script similar to this shell invocation instead::
-
-    $ cubicweb-ctl shell <instance>
-    >>> from cubicweb import Binary
-    >>> from cubicweb.server.utils import crypt_password
-    >>> crypted = crypt_password('joepass')
-    >>> rset = rql('Any U WHERE U is CWUser, U login "joe"')
-    >>> joe = rset.get_entity(0,0)
-    >>> joe.cw_set(upassword=Binary(crypted))
-
-Please, refer to the script example is provided in the `misc/examples/chpasswd.py` file.
+        def __init__(self, *args, **kwargs):
+            kwargs.setdefault('widget', wdgs.IntervalWidget())
+            super(MonthPeriodField, self).__init__(
+                [fields.StringField(name='begin_month',
+                                    choices=self.get_range, sort=False,
+                                    value=self.get_mindate,
+                                    widget=MonthSelect()),
+                 fields.StringField(name='end_month',
+                                    choices=self.get_range, sort=False,
+                                    value=self.get_maxdate,
+                                    widget=MonthSelect())], *args, **kwargs)
+
+        @staticmethod
+        def get_range(form, field):
+            mindate = date.todate(form.cw_extra_kwargs['mindate'])
+            maxdate = date.todate(form.cw_extra_kwargs['maxdate'])
+            assert mindate <= maxdate
+            _ = form._cw._
+            months = []
+            while mindate <= maxdate:
+                label = '%s %s' % (_(calendar.MONTHNAMES[mindate.month - 1]),
+                                   mindate.year)
+                value = field.widget.format_value(form, field, mindate)
+                months.append( (label, value) )
+                mindate = date.next_month(mindate)
+            return months
+
+        @staticmethod
+        def get_mindate(form, field):
+            return form.cw_extra_kwargs['mindate']
+
+        @staticmethod
+        def get_maxdate(form, field):
+            return form.cw_extra_kwargs['maxdate']
+
+        def process_posted(self, form):
+            for field, value in super(MonthPeriodField, self).process_posted(form):
+                if field.name == 'end_month':
+                    value = date.last_day(value)
+                yield field, value
+
+
+Here we first define a widget that will be used to select the beginning and the
+end of the period, displaying months like '<month> YYYY' but using 'YYYY/mm' as
+actual value.
+
+We then define a field that will actually hold two fields, one for the beginning
+and another for the end of the period. Each subfield uses the widget we defined
+earlier, and the outer field itself uses the standard
+:class:`IntervalWidget`. The field adds some logic:
+
+* a vocabulary generation function `get_range`, used to populate each sub-field
 
-The more experimented people would use RQL request directly::
+* two 'value' functions `get_mindate` and `get_maxdate`, used to tell to
+  subfields which value they should consider on form initialization
 
-    >>> rql('SET X upassword %(a)s WHERE X is CWUser, X login "joe"',
-    ...     {'a': crypted})
+* overriding of `process_posted`, called when the form is being posted, so that
+  the end of the period is properly set to the last day of the month.
 
-I've just created a user in a group and it doesn't work !
----------------------------------------------------------
+Now, we can define a very simple form:
 
-You are probably getting errors such as ::
+.. sourcecode:: python
 
-  remove {'PR': 'Project', 'C': 'CWUser'} from solutions since your_user has no read access to cost
+    class MonthPeriodSelectorForm(forms.FieldsForm):
+        __regid__ = 'myform'
+        __select__ = match_kwargs('mindate', 'maxdate')
 
-This is because you have to put your user in the "users" group. The user has to
-be in both groups.
+        form_buttons = [wdgs.SubmitButton()]
+        form_renderer_id = 'onerowtable'
+        period = MonthPeriodField()
 
-How is security implemented ?
-------------------------------
 
-The basis for security is a mapping from operations to groups or
-arbitrary RQL expressions. These mappings are scoped to entities and
-relations.
+where we simply add our field, set a submit button and use a very simple renderer
+(try others!). Also we specify a selector that ensures form will have arguments
+necessary to our field.
 
-This is an example for an Entity Type definition:
+Now, we need a view that will wrap the form and handle post when it occurs,
+simply displaying posted values in the page:
 
 .. sourcecode:: python
 
-    class Version(EntityType):
-        """a version is defining the content of a particular project's
-        release"""
-        # definition of attributes is voluntarily missing
-        __permissions__ = {'read': ('managers', 'users', 'guests',),
-                           'update': ('managers', 'logilab', 'owners'),
-                           'delete': ('managers',),
-                           'add': ('managers', 'logilab',
-                                   ERQLExpression('X version_of PROJ, U in_group G, '
-                                                  'PROJ require_permission P, '
-                                                  'P name "add_version", P require_group G'),)}
-
-The above means that permission to read a Version is granted to any
-user that is part of one of the groups 'managers', 'users', 'guests'.
-The 'add' permission is granted to users in group 'managers' or
-'logilab' or to users in group G, if G is linked by a permission
-entity named "add_version" to the version's project.
-
-An example for a Relation Definition (RelationType both defines a
-relation type and implicitly one relation definition, on which the
-permissions actually apply):
-
-.. sourcecode:: python
+    class SelfPostingForm(View):
+        __regid__ = 'myformview'
 
-    class version_of(RelationType):
-        """link a version to its project. A version is necessarily linked
-        to one and only one project. """
-        # some lines voluntarily missing
-        __permissions__ = {'read': ('managers', 'users', 'guests',),
-                           'delete': ('managers', ),
-                           'add': ('managers', 'logilab',
-                                   RRQLExpression('O require_permission P, P name "add_version", '
-                                                  'U in_group G, P require_group G'),) }
-
-The main difference lies in the basic available operations (there is
-no 'update' operation) and the usage of an RRQLExpression (rql
-expression for a relation) instead of an ERQLExpression (rql
-expression for an entity).
-
-You can find additional information in the section :ref:`securitymodel`.
-
-Is it possible to bypass security from the UI (web front) part ?
-----------------------------------------------------------------
-
-No. Only Hooks/Operations can do that.
-
-Can PostgreSQL and CubicWeb authentication work with kerberos ?
-----------------------------------------------------------------
-
-If you have PostgreSQL set up to accept kerberos authentication, you can set
-the db-host, db-name and db-user parameters in the `sources` configuration
-file while leaving the password blank. It should be enough for your
-instance to connect to postgresql with a kerberos ticket.
+        def call(self):
+            mindate, maxdate = date.date(2010, 1, 1), date.date(2012, 1, 1)
+            form = self._cw.vreg['forms'].select(
+                'myform', self._cw, mindate=mindate, maxdate=maxdate, action='')
+            try:
+                posted = form.process_posted()
+                self.w(u'<p>posted values %s</p>' % xml_escape(repr(posted)))
+            except RequestError: # no specified period asked
+                pass
+            form.render(w=self.w, formvalues=self._cw.form)
+
+
+Notice usage of the :meth:`process_posted` method, that will return a dictionary
+of typed values (because they have been processed by the field). In our case, when
+the form is posted you should see a dictionary with 'begin_month' and 'end_month'
+as keys with the selected dates as value (as a python `date` object).
+
+
+APIs
+~~~~
+
+.. automodule:: cubicweb_web.formfields
+.. automodule:: cubicweb_web.formwidgets
+.. automodule:: cubicweb_web.views.forms
+.. automodule:: cubicweb_web.views.formrenderers
```

### Comparing `cubicweb-4.7.0/doc/book/annexes/mercurial.rst` & `cubicweb-4.7.1/doc/book/annexes/mercurial.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/Graph-ex.gif` & `cubicweb-4.7.1/doc/book/annexes/rql/Graph-ex.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/debugging.rst` & `cubicweb-4.7.1/doc/book/annexes/rql/debugging.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/implementation.rst` & `cubicweb-4.7.1/doc/book/annexes/rql/implementation.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/intro.rst` & `cubicweb-4.7.1/doc/book/annexes/rql/intro.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/language.rst` & `cubicweb-4.7.1/doc/book/annexes/rql/language.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst` & `cubicweb-4.7.1/doc/book/annexes/rql/usecases.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/connections_pooler.rst` & `cubicweb-4.7.1/doc/book/devrepo/connections_pooler.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/cubes/available-cubes.rst` & `cubicweb-4.7.1/doc/book/devrepo/cubes/available-cubes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/cubes/cc-newcube.rst` & `cubicweb-4.7.1/doc/book/devrepo/cubes/cc-newcube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst` & `cubicweb-4.7.1/doc/book/devrepo/cubes/layout.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/cubes/what-is-a-cube.rst` & `cubicweb-4.7.1/doc/book/devrepo/cubes/what-is-a-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/dataimport.rst` & `cubicweb-4.7.1/doc/book/devrepo/dataimport.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/datamodel/baseschema.rst` & `cubicweb-4.7.1/doc/book/devrepo/datamodel/baseschema.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/datamodel/define-workflows.rst` & `cubicweb-4.7.1/doc/book/devrepo/datamodel/define-workflows.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/datamodel/definition.rst` & `cubicweb-4.7.1/doc/book/devrepo/datamodel/definition.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/datamodel/metadata.rst` & `cubicweb-4.7.1/doc/book/devrepo/datamodel/metadata.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/debug_channels.rst` & `cubicweb-4.7.1/doc/book/devrepo/debug_channels.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/devcore/reqbase.rst` & `cubicweb-4.7.1/doc/book/devrepo/devcore/reqbase.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/entityclasses/adapters.rst` & `cubicweb-4.7.1/doc/book/devrepo/entityclasses/adapters.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/entityclasses/application-logic.rst` & `cubicweb-4.7.1/doc/book/devrepo/entityclasses/application-logic.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/entityclasses/data-as-objects.rst` & `cubicweb-4.7.1/doc/book/devrepo/entityclasses/data-as-objects.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/entityclasses/load-sort.rst` & `cubicweb-4.7.1/doc/book/devrepo/entityclasses/load-sort.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/fti.rst` & `cubicweb-4.7.1/doc/book/devrepo/fti.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/migration.rst` & `cubicweb-4.7.1/doc/book/devrepo/migration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/profiling.rst` & `cubicweb-4.7.1/doc/book/devrepo/profiling.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/repo/hooks.rst` & `cubicweb-4.7.1/doc/book/devrepo/repo/hooks.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/repo/notifications.rst` & `cubicweb-4.7.1/doc/book/devrepo/repo/notifications.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/repo/sessions.rst` & `cubicweb-4.7.1/doc/book/devrepo/repo/sessions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/testing.rst` & `cubicweb-4.7.1/doc/book/devrepo/testing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devrepo/vreg.rst` & `cubicweb-4.7.1/doc/book/devrepo/vreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/ajax.rst` & `cubicweb-4.7.1/doc/book/devweb/ajax.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/controllers.rst` & `cubicweb-4.7.1/doc/book/devweb/controllers.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/css.rst` & `cubicweb-4.7.1/doc/book/devweb/css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst` & `cubicweb-4.7.1/doc/book/devweb/edition/dissection.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst` & `cubicweb-4.7.1/doc/book/devweb/edition/editcontroller.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/edition/examples.rst` & `cubicweb-4.7.1/doc/book/devweb/edition/examples.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/edition/form.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/part05_ui-advanced.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,378 +1,389 @@
-.. include:: ../warning.rst
+.. -*- coding: utf-8 -*-
 
-.. _webform:
+Building my photos web site with |cubicweb| part V: let's make it even more user friendly
+=========================================================================================
 
-HTML form construction
-----------------------
+.. _uiprops:
 
-CubicWeb provides the somewhat usual form / field / widget / renderer abstraction
-to provide generic building blocks which will greatly help you in building forms
-properly integrated with CubicWeb (coherent display, error handling, etc...),
-while keeping things as flexible as possible.
-
-A ``form`` basically only holds a set of ``fields``, and has te be bound to a
-``renderer`` which is responsible to layout them. Each field is bound to a
-``widget`` that will be used to fill in value(s) for that field (at form
-generation time) and 'decode' (fetch and give a proper Python type to) values
-sent back by the browser.
-
-The ``field`` should be used according to the type of what you want to edit.
-E.g. if you want to edit some date, you'll have to use the
-:class:`cubicweb_web.formfields.DateField`. Then you can choose among multiple
-widgets to edit it, for instance :class:`cubicweb_web.formwidgets.TextInput` (a
-bare text field), :class:`~cubicweb_web.formwidgets.DateTimePicker` (a simple
-calendar) or even :class:`~cubicweb_web.formwidgets.JQueryDatePicker` (the JQuery
-calendar).  You can of course also write your own widget.
+Step 1: tired of the default look?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-Exploring the available forms
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+OK... Now our site has its most desired features. But... I would like to make it look
+somewhat like *my* website. It is not www.cubicweb.org after all. Let's tackle this
+first!
 
-A small excursion into a |cubicweb| shell is the quickest way to
-discover available forms (or application objects in general).
+The first thing we can to is to change the logo. There are various way to achieve
+this. The easiest way is to put a :file:`logo.png` file into the cube's :file:`data`
+directory. As data files are looked at according to cubes order (CubicWeb
+resources coming last), that file will be selected instead of CubicWeb's one.
+
+.. Note::
+   As the location for static resources are cached, you'll have to restart
+   your instance for this to be taken into account.
+
+Though there are some cases where you don't want to use a :file:`logo.png` file.
+For instance if it's a JPEG file. You can still change the logo by defining in
+the cube's :file:`uiprops.py` file:
 
 .. sourcecode:: python
 
- >>> from pprint import pprint
- >>> pprint( session.vreg['forms'] )
- {'base': [<class 'cubicweb_web.views.forms.FieldsForm'>,
-           <class 'cubicweb_web.views.forms.EntityFieldsForm'>],
-  'changestate': [<class 'cubicweb_web.views.workflow.ChangeStateForm'>,
-                  <class 'cubicweb_tracker.views.forms.VersionChangeStateForm'>],
-  'composite': [<class 'cubicweb_web.views.forms.CompositeForm'>,
-                <class 'cubicweb_web.views.forms.CompositeEntityForm'>],
-  'deleteconf': [<class 'cubicweb_web.views.editforms.DeleteConfForm'>],
-  'edition': [<class 'cubicweb_web.views.autoform.AutomaticEntityForm'>,
-              <class 'cubicweb_web.views.workflow.TransitionEditionForm'>,
-              <class 'cubicweb_web.views.workflow.StateEditionForm'>],
-  'logform': [<class 'cubicweb_web.views.basetemplates.LogForm'>],
-  'massmailing': [<class 'cubicweb_web.views.massmailing.MassMailingForm'>],
-  'muledit': [<class 'cubicweb_web.views.editforms.TableEditForm'>]}
-
-
-The two most important form families here (for all practical purposes) are `base`
-and `edition`. Most of the time one wants alterations of the
-:class:`AutomaticEntityForm` to generate custom forms to handle edition of an
-entity.
+   LOGO = data('logo.jpg')
 
-The Automatic Entity Form
-~~~~~~~~~~~~~~~~~~~~~~~~~
+.. Note::
+   If the file :file:`uiprops.py` doesn't exist in your cube, simply create it.
+
+The uiprops machinery is used to define some static file resources,
+such as the logo, default Javascript / CSS files, as well as CSS
+properties (we'll see that later).
+
+.. Note::
+   This file is imported specifically by |cubicweb|, with a predefined name space,
+   containing for instance the `data` function, telling the file is somewhere
+   in a cube or CubicWeb's data directory.
+
+   One side effect of this is that it can't be imported as a regular python
+   module.
+
+The nice thing is that in debug mode, change to a :file:`uiprops.py` file are detected
+and then automatically reloaded.
+
+Now, as it's a photos web-site, I would like to have a photo of mine as background...
+After some trials I won't detail here, I've found a working recipe explained `here`_.
+All I've to do is to override some stuff of the default CubicWeb user interface to
+apply it as explained.
+
+The first thing to to get the ``<img/>`` tag as first element after the
+``<body>`` tag.  If you know a way to avoid this by simply specifying the image
+in the CSS, tell me!  The easiest way to do so is to override the
+:class:`HTMLPageHeader` view, since that's the one that is directly called once
+the ``<body>`` has been written. How did I find this?  By looking in the
+:mod:`cubiweb.web.views.basetemplates` module, since I know that global page
+layouts sits there. I could also have grep the "body" tag in
+:mod:`cubicweb_web.views`... Finding this was the hardest part. Now all I need is
+to customize it to write that ``img`` tag, as below in :file:`views.py`:
 
-.. automodule:: cubicweb_web.views.autoform
+.. sourcecode:: python
 
-Anatomy of a choices function
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    from cubicweb_web.views import basetemplates
 
-Let's have a look at the `ticket_done_in_choices` function given to
-the `choices` parameter of the relation tag that is applied to the
-('Ticket', 'done_in', '*') relation definition, as it is both typical
-and sophisticated enough. This is a code snippet from the `tracker`_
-cube.
 
-.. _`tracker`: https://forge.extranet.logilab.fr/cubicweb/cubes/tracker
+    class HTMLPageHeader(basetemplates.HTMLPageHeader):
+        # override this since it's the easier way to have our bg image
+        # as the first element following <body>
+        def call(self, **kwargs):
+            self.w(u'<img id="bg-image" src="%sbackground.jpg" alt="background image"/>'
+                   % self._cw.datadir_url)
+            super(HTMLPageHeader, self).call(**kwargs)
 
-The ``Ticket`` entity type can be related to a ``Project`` and a
-``Version``, respectively through the ``concerns`` and ``done_in``
-relations. When a user is about to edit a ticket, we want to fill the
-combo box for the ``done_in`` relation with values pertinent with
-respect to the context. The important context here is:
 
-* creation or modification (we cannot fetch values the same way in
-  either case)
+    def registration_callback(vreg):
+        vreg.register_all(globals().values(), __name__, (HTMLPageHeader))
+        vreg.register_and_replace(HTMLPageHeader, basetemplates.HTMLPageHeader)
 
-* ``__linkto`` url parameter given in a creation context
 
-.. sourcecode:: python
+As you may have guessed, my background image is in a :file:`background.jpg` file
+in the cube's :file:`data` directory, but there are still some things to explain
+to newcomers here:
 
-    from cubicweb_web import formfields
+* The :meth:`call` method is there the main access point of the view. It's called by
+  the view's :meth:`render` method. It is not the only access point for a view, but
+  this will be detailed later.
 
-    def ticket_done_in_choices(form, field):
-        entity = form.edited_entity
-        # first see if its specified by __linkto form parameters
-        linkedto = form.linked_to[('done_in', 'subject')]
-        if linkedto:
-            return linkedto
-        # it isn't, get initial values
-        vocab = field.relvoc_init(form)
-        veid = None
-        # try to fetch the (already or pending) related version and project
-        if not entity.has_eid():
-            peids = form.linked_to[('concerns', 'subject')]
-            peid = peids and peids[0]
-        else:
-            peid = entity.project.eid
-            veid = entity.done_in and entity.done_in[0].eid
-        if peid:
-            # we can complete the vocabulary with relevant values
-            rschema = form._cw.vreg.schema['done_in'].rdef('Ticket', 'Version')
-            rset = form._cw.execute(
-                'Any V, VN ORDERBY version_sort_value(VN) '
-                'WHERE V version_of P, P eid %(p)s, V num VN, '
-                'V in_state ST, NOT ST name "published"', {'p': peid}, 'p')
-            vocab += [(v.view('combobox'), v.eid) for v in rset.entities()
-                      if rschema.has_perm(form._cw, 'add', toeid=v.eid)
-                      and v.eid != veid]
-        return vocab
-
-The first thing we have to do is fetch potential values from the ``__linkto`` url
-parameter that is often found in entity creation contexts (the creation action
-provides such a parameter with a predetermined value; for instance in this case,
-ticket creation could occur in the context of a `Version` entity). The
-:class:`~cubicweb_web.formfields.RelationField` field class provides a
-:meth:`~cubicweb_web.formfields.RelationField.relvoc_linkedto` method that gets a
-list suitably filled with vocabulary values.
+* Calling `self.w` writes something to the output stream. Except for binary views
+  (which do not generate text), it *must* be passed an Unicode string.
 
-.. sourcecode:: python
+* The proper way to get a file in :file:`data` directory is to use the `datadir_url`
+  attribute of the incoming request (e.g. `self._cw`).
 
-        linkedto = field.relvoc_linkedto(form)
-        if linkedto:
-            return linkedto
-
-Then, if no ``__linkto`` argument was given, we must prepare the vocabulary with
-an initial empty value (because `done_in` is not mandatory, we must allow the
-user to not select a verson) and already linked values. This is done with the
-:meth:`~cubicweb_web.formfields.RelationField.relvoc_init` method.
+I won't explain again the :func:`registration_callback` stuff, you should understand it
+now!  If not, go back to `previous post in the series`_ :)
 
-.. sourcecode:: python
+Fine. Now all I've to do is to add a bit of CSS to get it to behave nicely (which
+is not the case at all for now). I'll put all this in a :file:`cubes.sytweb.css`
+file, stored as usual in our :file:`data` directory:
 
-        vocab = field.relvoc_init(form)
+.. sourcecode:: css
 
-But then, we have to give more: if the ticket is related to a project,
-we should provide all the non published versions of this project
-(`Version` and `Project` can be related through the `version_of`
-relation). Conversely, if we do not know yet the project, it would not
-make sense to propose all existing versions as it could potentially
-lead to incoherences. Even if these will be caught by some
-RQLConstraint, it is wise not to tempt the user with error-inducing
-candidate values.
 
-The "ticket is related to a project" part must be decomposed as:
+    /* fixed full screen background image
+     * as explained on http://webdesign.about.com/od/css3/f/blfaqbgsize.htm
+     *
+     * syt update: set z-index=0 on the img instead of z-index=1 on div#page & co to
+     * avoid pb with the user actions menu
+     */
+    img#bg-image {
+        position: fixed;
+        top: 0;
+        left: 0;
+        width: 100%;
+        height: 100%;
+        z-index: 0;
+    }
 
-* this is a new ticket which is created is the context of a project
+    div#page, table#header, div#footer {
+        background: transparent;
+        position: relative;
+    }
 
-* this is an already existing ticket, linked to a project (through the
-  `concerns` relation)
+    /* add some space around the logo
+     */
+    img#logo {
+        padding: 5px 15px 0px 15px;
+    }
 
-* there is no related project (quite unlikely given the cardinality of
-  the `concerns` relation, so it can only mean that we are creating a
-  new ticket, and a project is about to be selected but there is no
-  ``__linkto`` argument)
+    /* more dark font for metadata to have a chance to see them with the background
+     *  image
+     */
+    div.metadata {
+        color: black;
+    }
 
-.. note::
+You can see here stuff explained in the cited page, with only a slight modification
+explained in the comments, plus some additional rules to make things somewhat cleaner:
 
-   the last situation could happen in several ways, but of course in a
-   polished application, the paths to ticket creation should be
-   controlled so as to avoid a suboptimal end-user experience
+* a bit of padding around the logo
 
-Hence, we try to fetch the related project.
+* darker metadata which appears by default below the content (the white frame in the page)
+
+To get this CSS file used everywhere in the site, I have to modify the :file:`uiprops.py` file
+introduced above:
 
 .. sourcecode:: python
 
-        veid = None
-        if not entity.has_eid():
-            peids = form.linked_to[('concerns', 'subject')]
-            peid = peids and peids[0]
-        else:
-            peid = entity.project.eid
-            veid = entity.done_in and entity.done_in[0].eid
-
-We distinguish between entity creation and entity modification using
-the ``Entity.has_eid()`` method, which returns `False` on creation. At
-creation time the only way to get a project is through the
-``__linkto`` parameter. Notice that we fetch the version in which the
-ticket is `done_in` if any, for later.
-
-.. note::
-
-  the implementation above assumes that if there is a ``__linkto``
-  parameter, it is only about a project. While it makes sense most of
-  the time, it is not an absolute. Depending on how an entity creation
-  action action url is built, several outcomes could be possible
-  there
+   STYLESHEETS = sheet['STYLESHEETS'] + [data('cubes.sytweb.css')]
 
-If the ticket is already linked to a project, fetching it is
-trivial. Then we add the relevant version to the initial vocabulary.
+.. Note::
+   `sheet` is another predefined variable containing values defined by
+   already process `:file:`uiprops.py`` file, notably the CubicWeb's one.
+
+Here we simply want our CSS in addition to CubicWeb's base CSS files, so we
+redefine the `STYLESHEETS` variable to existing CSS (accessed through the `sheet`
+variable) with our one added. I could also have done:
 
 .. sourcecode:: python
 
-        if peid:
-            rschema = form._cw.vreg.schema['done_in'].rdef('Ticket', 'Version')
-            rset = form._cw.execute(
-                'Any V, VN ORDERBY version_sort_value(VN) '
-                'WHERE V version_of P, P eid %(p)s, V num VN, '
-                'V in_state ST, NOT ST name "published"', {'p': peid})
-            vocab += [(v.view('combobox'), v.eid) for v in rset.entities()
-                      if rschema.has_perm(form._cw, 'add', toeid=v.eid)
-                      and v.eid != veid]
-
-.. warning::
-
-   we have to defend ourselves against lack of a project eid. Given
-   the cardinality of the `concerns` relation, there *must* be a
-   project, but this rule can only be enforced at validation time,
-   which will happen of course only after form subsmission
-
-Here, given a project eid, we complete the vocabulary with all
-unpublished versions defined in the project (sorted by number) for
-which the current user is allowed to establish the relation.
-
-
-Building self-posted form with custom fields/widgets
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Sometimes you want a form that is not related to entity edition. For those,
-you'll have to handle form posting by yourself. Here is a complete example on how
-to achieve this (and more).
+   sheet['STYLESHEETS'].append(data('cubes.sytweb.css'))
+
+But this is less interesting since we don't see the overriding mechanism...
+
+At this point, the site should start looking good, the background image being
+resized to fit the screen.
+
+.. image:: ../../images/tutos-photowebsite_background-image.png
 
-Imagine you want a form that selects a month period. There are no proper
-field/widget to handle this in CubicWeb, so let's start by defining them:
+The final touch: let's customize CubicWeb's CSS to get less orange... By simply adding
 
 .. sourcecode:: python
 
-    # let's have the whole import list at the beginning, even those necessary for
-    # subsequent snippets
-    from logilab.common import date
-    from logilab.mtconverter import xml_escape
-    from cubicweb.predicates import match_kwargs
-    from cubicweb_web.view import View
-    from cubicweb_web import RequestError, ProcessFormError
-    from cubicweb_web import formfields as fields, formwidgets as wdgs
-    from cubicweb_web.views import forms, calendar
-
-    class MonthSelect(wdgs.Select):
-        """Custom widget to display month and year. Expect value to be given as a
-        date instance.
-        """
+  contextualBoxTitleBg = incontextBoxTitleBg = '#AAAAAA'
 
-        def format_value(self, form, field, value):
-            return u'%s/%s' % (value.year, value.month)
+and reloading the page we've just seen, we know have a nice greyed box instead of
+the orange one:
+
+.. image:: ../../images/tutos-photowebsite_grey-box.png
+
+This is because CubicWeb's CSS include some variables which are
+expanded by values defined in :file:`uiprops.py` file. In our case we controlled the
+properties of the CSS `background` property of boxes with CSS class
+`contextualBoxTitleBg` and `incontextBoxTitleBg`.
 
-        def process_field_data(self, form, field):
-            val = super(MonthSelect, self).process_field_data(form, field)
-            try:
-                year, month = val.split('/')
-                year = int(year)
-                month = int(month)
-                return date.date(year, month, 1)
-            except ValueError:
-                raise ProcessFormError(
-                    form._cw._('badly formated date string %s') % val)
-
-
-    class MonthPeriodField(fields.CompoundField):
-        """custom field composed of two subfields, 'begin_month' and 'end_month'.
-
-        It expects to be used on form that has 'mindate' and 'maxdate' in its
-        extra arguments, telling the range of month to display.
-        """
-
-        def __init__(self, *args, **kwargs):
-            kwargs.setdefault('widget', wdgs.IntervalWidget())
-            super(MonthPeriodField, self).__init__(
-                [fields.StringField(name='begin_month',
-                                    choices=self.get_range, sort=False,
-                                    value=self.get_mindate,
-                                    widget=MonthSelect()),
-                 fields.StringField(name='end_month',
-                                    choices=self.get_range, sort=False,
-                                    value=self.get_maxdate,
-                                    widget=MonthSelect())], *args, **kwargs)
-
-        @staticmethod
-        def get_range(form, field):
-            mindate = date.todate(form.cw_extra_kwargs['mindate'])
-            maxdate = date.todate(form.cw_extra_kwargs['maxdate'])
-            assert mindate <= maxdate
-            _ = form._cw._
-            months = []
-            while mindate <= maxdate:
-                label = '%s %s' % (_(calendar.MONTHNAMES[mindate.month - 1]),
-                                   mindate.year)
-                value = field.widget.format_value(form, field, mindate)
-                months.append( (label, value) )
-                mindate = date.next_month(mindate)
-            return months
-
-        @staticmethod
-        def get_mindate(form, field):
-            return form.cw_extra_kwargs['mindate']
-
-        @staticmethod
-        def get_maxdate(form, field):
-            return form.cw_extra_kwargs['maxdate']
-
-        def process_posted(self, form):
-            for field, value in super(MonthPeriodField, self).process_posted(form):
-                if field.name == 'end_month':
-                    value = date.last_day(value)
-                yield field, value
-
-
-Here we first define a widget that will be used to select the beginning and the
-end of the period, displaying months like '<month> YYYY' but using 'YYYY/mm' as
-actual value.
-
-We then define a field that will actually hold two fields, one for the beginning
-and another for the end of the period. Each subfield uses the widget we defined
-earlier, and the outer field itself uses the standard
-:class:`IntervalWidget`. The field adds some logic:
-
-* a vocabulary generation function `get_range`, used to populate each sub-field
 
-* two 'value' functions `get_mindate` and `get_maxdate`, used to tell to
-  subfields which value they should consider on form initialization
+Step 2: configuring boxes
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Boxes present to the user some ways to use the application. Let's first do a few
+user interface tweaks in our :file:`views.py` file:
 
-* overriding of `process_posted`, called when the form is being posted, so that
-  the end of the period is properly set to the last day of the month.
+.. sourcecode:: python
 
-Now, we can define a very simple form:
+  from cubicweb.predicates import none_rset
+  from cubicweb_web.views import bookmark
+  from cubicweb_zone import views as zone
+  from cubicweb_tag import views as tag
+
+
+  # change bookmarks box selector so it's only displayed on startup views
+  bookmark.BookmarksBox.__select__ = bookmark.BookmarksBox.__select__ & none_rset()
+  # move zone box to the left instead of in the context frame and tweak its order
+  zone.ZoneBox.context = 'left'
+  zone.ZoneBox.order = 100
+  # move tags box to the left instead of in the context frame and tweak its order
+  tag.TagsBox.context = 'left'
+  tag.TagsBox.order = 102
+  # hide similarity box, not interested
+  tag.SimilarityBox.visible = False
+
+The idea is to move all boxes in the left column, so we get more space for the
+photos.  Now, serious things: I want a box similar to the tags box but to handle
+the `Person displayed_on File` relation. We can do this simply by adding a
+:class:`AjaxEditRelationCtxComponent` subclass to our views, as below:
 
 .. sourcecode:: python
 
-    class MonthPeriodSelectorForm(forms.FieldsForm):
-        __regid__ = 'myform'
-        __select__ = match_kwargs('mindate', 'maxdate')
+    from cubicweb import _
+    from logilab.common.decorators import monkeypatch
+    from cubicweb import ValidationError
+    from cubicweb_web.views import uicfg, component
+    from cubicweb_web.views import basecontrollers
+
+
+    # hide displayed_on relation using uicfg since it will be displayed by the box below
+    uicfg.primaryview_section.tag_object_of(('*', 'displayed_on', '*'), 'hidden')
+
+
+    class PersonBox(component.AjaxEditRelationCtxComponent):
+        __regid__ = 'sytweb.displayed-on-box'
+        # box position
+        order = 101
+        context = 'left'
+        # define relation to be handled
+        rtype = 'displayed_on'
+        role = 'object'
+        target_etype = 'Person'
+        # messages
+        added_msg = _('person has been added')
+        removed_msg = _('person has been removed')
+        # bind to js_* methods of the json controller
+        fname_vocabulary = 'unrelated_persons'
+        fname_validate = 'link_to_person'
+        fname_remove = 'unlink_person'
+
+
+    @monkeypatch(basecontrollers.JSonController)
+    @basecontrollers.jsonize
+    def js_unrelated_persons(self, eid):
+        """return tag unrelated to an entity"""
+        rql = "Any F + ' ' + S WHERE P surname S, P firstname F, X eid %(x)s, NOT P displayed_on X"
+        return [name for (name,) in self._cw.execute(rql, {'x' : eid})]
+
+
+    @monkeypatch(basecontrollers.JSonController)
+    def js_link_to_person(self, eid, people):
+        req = self._cw
+        for name in people:
+            name = name.strip().title()
+            if not name:
+                continue
+            try:
+                firstname, surname = name.split(None, 1)
+            except:
+                raise ValidationError(eid, {('displayed_on', 'object'): 'provide <first name> <surname>'})
+            rset = req.execute('Person P WHERE '
+                               'P firstname %(firstname)s, P surname %(surname)s',
+                               locals())
+            if rset:
+                person = rset.get_entity(0, 0)
+            else:
+                person = req.create_entity('Person', firstname=firstname,
+                                                surname=surname)
+            req.execute('SET P displayed_on X WHERE '
+                        'P eid %(p)s, X eid %(x)s, NOT P displayed_on X',
+                        {'p': person.eid, 'x' : eid})
+
+
+    @monkeypatch(basecontrollers.JSonController)
+    def js_unlink_person(self, eid, personeid):
+        self._cw.execute('DELETE P displayed_on X WHERE P eid %(p)s, X eid %(x)s',
+                         {'p': personeid, 'x': eid})
+
+
+You basically subclass to configure with some class attributes. The `fname_*`
+attributes give the name of methods that should be defined on the json control to
+make the AJAX part of the widget work: one to get the vocabulary, one to add a
+relation and another to delete a relation. These methods must start by a `js_`
+prefix and are added to the controller using the `@monkeypatch` decorator. In my
+case, the most complicated method is the one which adds a relation, since it
+tries to see if the person already exists, and else automatically create it,
+assuming the user entered "firstname surname".
+
+Let's see how it looks like on a file primary view:
+
+.. image:: ../../images/tutos-photowebsite_boxes.png
+
+Great, it's now as easy for me to link my pictures to people than to tag them.
+Also, visitors get a consistent display of these two pieces of information.
+
+.. Note::
+  The ui component system has been refactored in `CubicWeb 3.10`_, which also
+  introduced the :class:`AjaxEditRelationCtxComponent` class.
+
+
+Step 3: configuring facets
+~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The last feature we'll add today is facet configuration. If you access to the
+'/file' url, you'll see a set of 'facets' appearing in the left column. Facets
+provide an intuitive way to build a query incrementally, by proposing to the user
+various way to restrict the result set. For instance CubicWeb proposes a facet to
+restrict based on who created an entity; the tag cube proposes a facet to
+restrict based on tags; the zoe cube a facet to restrict based on geographical
+location, and so on. In that gist, I want to propose a facet to restrict based on
+the people displayed on the picture. To do so, there are various classes in the
+:mod:`cubicweb_web.facet` module which simply have to be configured using class
+attributes as we've done for the box. In our case, we'll define a subclass of
+:class:`RelationFacet`.
+
+.. Note::
+
+   Since that's ui stuff, we'll continue to add code below to our
+   :file:`views.py` file. Though we begin to have a lot of various code their, so
+   it's may be a good time to split our views module into submodules of a `view`
+   package. In our case of a simple application (glue) cube, we could start using
+   for instance the layout below: ::
+
+     views/__init__.py   # uicfg configuration, facets
+     views/layout.py     # header/footer/background stuff
+     views/components.py # boxes, adapters
+     views/pages.py      # index view, 404 view
+
+.. sourcecode:: python
 
-        form_buttons = [wdgs.SubmitButton()]
-        form_renderer_id = 'onerowtable'
-        period = MonthPeriodField()
+    from cubicweb_web import facet
 
 
-where we simply add our field, set a submit button and use a very simple renderer
-(try others!). Also we specify a selector that ensures form will have arguments
-necessary to our field.
+    class DisplayedOnFacet(facet.RelationFacet):
+        __regid__ = 'displayed_on-facet'
+        # relation to be displayed
+        rtype = 'displayed_on'
+        role = 'object'
+        # view to use to display persons
+        label_vid = 'combobox'
 
-Now, we need a view that will wrap the form and handle post when it occurs,
-simply displaying posted values in the page:
+Let's say we also want to filter according to the `visibility` attribute. This is
+even simpler as we just have to derive from the :class:`AttributeFacet` class:
 
 .. sourcecode:: python
 
-    class SelfPostingForm(View):
-        __regid__ = 'myformview'
+    class VisibilityFacet(facet.AttributeFacet):
+        __regid__ = 'visibility-facet'
+        rtype = 'visibility'
+
+Now if I search for some pictures on my site, I get the following facets available:
+
+.. image:: ../../images/tutos-photowebsite_facets.png
+
+.. Note::
+
+  By default a facet must be applyable to every entity in the result set and
+  provide at leat two elements of vocabulary to be displayed (for instance you
+  won't see the `created_by` facet if the same user has created all
+  entities). This may explain why you don't see yours...
+
+
+Conclusion
+~~~~~~~~~~
+
+We started to see the power behind the infrastructure provided by the
+framework, both on the pure ui (CSS, Javascript) side and on the Python side
+(high level generic classes for components, including boxes and facets). We now
+have, with a few lines of code, a full-featured web site with a personalized look.
+
+Of course we'll probably want more as time goes, but we can now
+concentrate on making good pictures, publishing albums and sharing them with
+friends...
 
-        def call(self):
-            mindate, maxdate = date.date(2010, 1, 1), date.date(2012, 1, 1)
-            form = self._cw.vreg['forms'].select(
-                'myform', self._cw, mindate=mindate, maxdate=maxdate, action='')
-            try:
-                posted = form.process_posted()
-                self.w(u'<p>posted values %s</p>' % xml_escape(repr(posted)))
-            except RequestError: # no specified period asked
-                pass
-            form.render(w=self.w, formvalues=self._cw.form)
-
-
-Notice usage of the :meth:`process_posted` method, that will return a dictionary
-of typed values (because they have been processed by the field). In our case, when
-the form is posted you should see a dictionary with 'begin_month' and 'end_month'
-as keys with the selected dates as value (as a python `date` object).
-
-
-APIs
-~~~~
-
-.. automodule:: cubicweb_web.formfields
-.. automodule:: cubicweb_web.formwidgets
-.. automodule:: cubicweb_web.views.forms
-.. automodule:: cubicweb_web.views.formrenderers
 
 
+.. _`CubicWeb 3.10`: http://www.cubicweb.org/blogentry/1330518
+.. _`here`: http://webdesign.about.com/od/css3/f/blfaqbgsize.htm
+.. _`previous post in the series`: part04_ui-base.rst
```

### Comparing `cubicweb-4.7.0/doc/book/devweb/facets.rst` & `cubicweb-4.7.1/doc/book/devweb/facets.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/httpcaching.rst` & `cubicweb-4.7.1/doc/book/devweb/httpcaching.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/internationalization.rst` & `cubicweb-4.7.1/doc/book/devweb/internationalization.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/internationalization.rst.orig` & `cubicweb-4.7.1/doc/book/devweb/views/primary.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,314 +1,278 @@
-.. include:: warning.rst
+.. include:: ../warning.rst
 
-.. -*- coding: utf-8 -*-
+.. _primary_view:
 
-.. _internationalization:
+The Primary View
+-----------------
 
-Internationalization
----------------------
+By default, *CubicWeb* provides a view that fits every available
+entity type. This is the first view you might be interested in
+modifying. It is also one of the richest and most complex.
 
-Cubicweb fully supports the internalization of its content and interface.
+It is automatically selected on a one line result set containing an
+entity.
 
-Cubicweb's interface internationalization is based on the translation project `GNU gettext`_.
+It lives in the :mod:`cubicweb_web.views.primary` module.
 
-.. _`GNU gettext`: https://www.gnu.org/software/gettext/
+The *primary* view is supposed to render a maximum of informations about the
+entity.
 
-Cubicweb' internalization involves two steps:
+.. _primary_view_layout:
 
-* in your Python code and cubicweb-tal templates : mark translatable strings
+Layout
+``````
 
-* in your instance : handle the translation catalog, edit translations
+The primary view has the following layout.
 
-String internationalization
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
+.. image:: ../../../images/primaryview_template.png
 
-User defined string
-```````````````````
+.. _primary_view_configuration:
 
-In the Python code and cubicweb-tal templates translatable strings can be
-marked in one of the following ways :
+Primary view configuration
+``````````````````````````
 
- * by using the *built-in* function `_`:
+If you want to customize the primary view of an entity, overriding the primary
+view class may not be necessary. For simple adjustments (attributes or relations
+display locations and styles), a much simpler way is to use uicfg.
 
-   .. sourcecode:: python
+Attributes/relations display location
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-     class PrimaryView(EntityView):
-         """the full view of an non final entity"""
-         __regid__ = 'primary'
-         title = _('primary')
+In the primary view, there are three sections where attributes and
+relations can be displayed (represented in pink in the image above):
 
-  OR
+* 'attributes'
+* 'relations'
+* 'sideboxes'
 
- * by using the equivalent request's method:
+**Attributes** can only be displayed in the attributes section (default
+  behavior). They can also be hidden. By default, attributes of type `Password`
+  and `Bytes` are hidden.
 
-   .. sourcecode:: python
-
-     class NoResultView(View):
-         """default view when no result has been found"""
-         __regid__ = 'noresult'
-
-         def call(self, **kwargs):
-             self.w(u'<div class="searchMessage"><strong>%s</strong></div>\n'
-                 % self._cw._('No result matching query'))
-
-The goal of the *built-in* function `_` is only **to mark the
-translatable strings**, it will only return the string to translate
-itself, but not its translation (it's actually another name for the
-`unicode` builtin).
-
-In the other hand the request's method `self._cw._` is also meant to
-retrieve the proper translation of translation strings in the
-requested language.
-
-Finally you can also use the `__` (two underscores) attribute of request object to get a
-translation for a string *which should not itself added to the catalog*,
-usually in case where the actual msgid is created by string interpolation ::
-
-  self._cw.__('This %s' % etype)
-
-In this example `._cw.__` is used instead of `._cw._` so we don't have 'This %s' in
-messages catalogs.
-
-Translations in cubicweb-tal template can also be done with TAL tags
-`i18n:content` and `i18n:replace`.
-
-If you need to mark other messages as translatable,
-you can create a file named `i18n/static-messages.pot`, see for example :ref:`translate-application-cube`.
-
-You could put there messages not found in the python sources or
-overrides some messages that are in cubes used in the dependencies.
-
-Generated string
-````````````````
-
-We do not need to mark the translation strings of entities/relations used by a
-particular instance's schema as they are generated automatically. String for
-various actions are also generated.
-
-For exemple the following schema:
+For instance, to hide the ``title`` attribute of the ``Blog`` entity:
 
 .. sourcecode:: python
 
+   from cubicweb_web.views import uicfg
+   uicfg.primaryview_section.tag_attribute(('Blog', 'title'), 'hidden')
 
-  class EntityA(EntityType):
-      relation_a2b = SubjectRelation('EntityB')
-
-  class EntityB(EntityType):
-      pass
-
-May generate the following message ::
-
-  add EntityA relation_a2b EntityB subject
-
-This message will be used in views of ``EntityA`` for creation of a new
-``EntityB`` with a preset relation ``relation_a2b`` between the current
-``EntityA`` and the new ``EntityB``. The opposite message ::
-
-  add EntityA relation_a2b EntityB object
-
-Is used for similar creation of an ``EntityA`` from a view of ``EntityB``. The
-title of they respective creation form will be ::
-
-  creating EntityB (EntityA %(linkto)s relation_a2b EntityB)
-
-  creating EntityA (EntityA relation_a2b %(linkto)s EntityA)
-
-In the translated string you can use ``%(linkto)s`` for reference to the source
-``entity``.
+**Relations** can be either displayed in one of the three sections or hidden.
 
-Handling the translation catalog
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+For relations, there are two methods:
 
-Once the internationalization is done in your code, you need to populate and
-update the translation catalog. Cubicweb provides the following commands for this
-purpose:
+* ``tag_object_of`` for modifying the primary view of the object
+* ``tag_subject_of`` for modifying the primary view of the subject
 
+These two methods take two arguments:
 
-* `i18ncubicweb` updates Cubicweb framework's translation
-  catalogs. Unless you actually work on the framework itself, you
-  don't need to use this command.
+* a triplet ``(subject, relation_name, object)``, where subject or object can be replaced with ``'*'``
+* the section name or ``hidden``
 
-* `i18ncube` updates the translation catalogs of *one particular cube*
-  (or of all cubes). After this command is executed you must update
-  the translation files *.po* in the "i18n" directory of your
-  cube. This command will of course not remove existing translations
-  still in use. It will mark unused translation but not remove them.
-
-* `i18ninstance` recompiles the translation catalogs of *one particular
-  instance* (or of all instances) after the translation catalogs of
-  its cubes have been updated. This command is automatically
-  called every time you create or update your instance. The compiled
-  catalogs (*.mo*) are stored in the i18n/<lang>/LC_MESSAGES of
-  instance where `lang` is the language identifier ('en' or 'fr'
-  for exemple).
-
-
-Example
-```````
-
-You have added and/or modified some translation strings in your cube
-(after creating a new view or modifying the cube's schema for exemple).
-To update the translation catalogs you need to do:
-
-1. `cubicweb-ctl i18ncube <cube>`
-2. Edit the `<cube>/i18n/xxx.po` files and add missing translations (those with an empty `msgstr`)
-3. `hg ci -m "updated i18n catalogs"`
-4. `cubicweb-ctl i18ninstance <myinstance>`
-
-
-Customizing the messages extraction process
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-The messages extraction performed by the ``i18ncommand`` collects messages
-from a few different sources:
-
-- the schema and application definition (entity names, docstrings,
-  help messages, uicfg),
-
-- the source files:
-
-  - ``i18n:content`` or ``i18n:replace`` directives from TAL files (with ``.pt`` extension),
-  - strings prefixed by an underscore (``_``) in python files,
-  - strings with double quotes prefixed by an underscore in javascript files.
-
-The source files are collected by walking through the cube directory,
-but ignoring a few directories like ``.hg``, ``.tox``, ``test`` or
-``node_modules``.
-
-If you need to customize this behaviour in your cube, you have to
-extend the ``cubicweb.devtools.devctl.I18nCubeMessageExtractor``. The
-example below will collect strings from ``jinja2`` files and ignore
-the ``static`` directory during the messages collection phase::
-
-  # mymodule.py
-  from cubicweb.devtools import devctl
-
-  class MyMessageExtractor(devctl.I18nCubeMessageExtractor):
-
-      blacklist = devctl.I18nCubeMessageExtractor | {'static'}
-      formats = devctl.I18nCubeMessageExtractor.formats + ['jinja2']
-
-      def collect_jinja2(self):
-          return self.find('.jinja2')
+.. sourcecode:: python
 
-      def extract_jinja2(self, files):
-          return self._xgettext(files, output='jinja.pot',
-                                extraopts='-L python --from-code=utf-8')
+   pv_section = uicfg.primaryview_section
+   # hide every relation `entry_of` in the `Blog` primary view
+   pv_section.tag_object_of(('*', 'entry_of', 'Blog'), 'hidden')
 
-Then, you'll have to register it with a ``cubicweb.i18ncube`` entry point
-in your cube's setup.py::
+   # display `entry_of` relations in the `relations`
+   # section in the `BlogEntry` primary view
+   pv_section.tag_subject_of(('BlogEntry', 'entry_of', '*'), 'relations')
 
-  setup(
-      # ...
-      entry_points={
-          # ...
-          'cubicweb.i18ncube': [
-              'mycube=cubicweb_mycube.mymodule:MyMessageExtractor',
-          ],
-      },
-      # ...
-  )
 
+Display content
+^^^^^^^^^^^^^^^
 
-Editing po files
-~~~~~~~~~~~~~~~~
+You can use ``primaryview_display_ctrl`` to customize the display of attributes
+or relations. Values of ``primaryview_display_ctrl`` are dictionaries.
 
-Using a PO aware editor
-````````````````````````
 
-Many tools exist to help maintain .po (PO) files. Common editors or
-development environment provides modes for these. One can also find
-dedicated PO files editor, such as `poedit`_.
+Common keys for attributes and relations are:
 
-.. _`poedit`:  http://www.poedit.net/
+* ``vid``: specifies the regid of the view for displaying the attribute or the relation.
 
-While usage of such a tool is commendable, PO files are perfectly
-editable with a (unicode aware) plain text editor. It is also useful
-to know their structure for troubleshooting purposes.
+  If ``vid`` is not specified, the default value depends on the section:
+    * ``attributes`` section: 'reledit' view
+    * ``relations`` section: 'autolimited' view
+    * ``sideboxes`` section: 'sidebox' view
 
-Structure of a PO file
-``````````````````````
+* ``order``: int used to control order within a section. When not specified,
+  automatically set according to order in which tags are added.
 
-In this section, we selectively quote passages of the `GNU gettext`_
-manual chapter on PO files, available there::
+* ``label``: label for the relations section or side box
 
- https://www.gnu.org/software/hello/manual/gettext/PO-Files.html
+* ``showlabel``: boolean telling whether the label is displayed
 
-One PO file entry has the following schematic structure::
+.. sourcecode:: python
 
-     white-space
-     #  translator-comments
-     #. extracted-comments
-     #: reference...
-     #, flag...
-     #| msgid previous-untranslated-string
-     msgid untranslated-string
-     msgstr translated-string
+   # let us remind the schema of a blog entry
+   class BlogEntry(EntityType):
+       title = String(required=True, fulltextindexed=True, maxsize=256)
+       publish_date = Date(default='TODAY')
+       content = String(required=True, fulltextindexed=True)
+       entry_of = SubjectRelation('Blog', cardinality='?*')
+
+   # now, we want to show attributes
+   # with an order different from that in the schema definition
+   view_ctrl = uicfg.primaryview_display_ctrl
+   for index, attr in enumerate('title', 'content', 'publish_date'):
+       view_ctrl.tag_attribute(('BlogEntry', attr), {'order': index})
+
+By default, relations displayed in the 'relations' section are being displayed by
+the 'autolimited' view. This view will use comma separated values, or list view
+and/or limit your rset if there is too much items in it (and generate the "view
+all" link in this case).
+
+You can control this view by setting the following values in the
+`primaryview_display_ctrl` relation tag:
+
+* `limit`, maximum number of entities to display. The value of the
+  'navigation.related-limit'  cwproperty is used by default (which is 8 by default).
+  If None, no limit.
+
+* `use_list_limit`, number of entities until which they should be display as a list
+  (eg using the 'list' view). Below that limit, the 'csv' view is used. If None,
+  display using 'csv' anyway.
+
+* `subvid`, the subview identifier (eg view that should be used of each item in the
+  list)
+
+Notice you can also use the `filter` key to set up a callback taking the related
+result set as argument and returning it filtered, to do some arbitrary filtering
+that can't be done using rql for instance.
 
 
-A simple entry can look like this::
+.. sourcecode:: python
 
-     #: lib/error.c:116
-     msgid "Unknown system error"
-     msgstr "Error desconegut del sistema"
+   pv_section = uicfg.primaryview_section
+   # in `CWUser` primary view, display `created_by`
+   # relations in relations section
+   pv_section.tag_object_of(('*', 'created_by', 'CWUser'), 'relations')
+
+   # display this relation as a list, sets the label,
+   # limit the number of results and filters on comments
+   def filter_comment(rset):
+       return rset.filtered_rset(lambda x: x.e_schema == 'Comment')
+   pv_ctrl = uicfg.primaryview_display_ctrl
+   pv_ctrl.tag_object_of(('*', 'created_by', 'CWUser'),
+                         {'vid': 'list', 'label': _('latest comment(s):'),
+                          'limit': True,
+                          'filter': filter_comment})
+
+.. warning:: with the ``primaryview_display_ctrl`` rtag, the subject or the
+   object of the relation is ignored for respectively ``tag_object_of`` or
+   ``tag_subject_of``. To avoid warnings during execution, they should be set to
+   ``'*'``.
+
+
+.. automodule:: cubicweb_web.views.primary
+
+
+Example of customization and creation
+`````````````````````````````````````
+
+We'll show you now an example of a ``primary`` view and how to customize it.
+
+If you want to change the way a ``BlogEntry`` is displayed, just
+override the method ``cell_call()`` of the view ``primary`` in
+``BlogDemo/views.py``.
 
-It is also possible to have entries with a context specifier. They
-look like this::
+.. sourcecode:: python
 
-     white-space
-     #  translator-comments
-     #. extracted-comments
-     #: reference...
-     #, flag...
-     #| msgctxt previous-context
-     #| msgid previous-untranslated-string
-     msgctxt context
-     msgid untranslated-string
-     msgstr translated-string
+   from cubicweb.predicates import is_instance
+   from cubicweb_web.views.primary import Primaryview
 
+   class BlogEntryPrimaryView(PrimaryView):
+       __select__ = PrimaryView.__select__ & is_instance('BlogEntry')
 
-The context serves to disambiguate messages with the same
-untranslated-string. It is possible to have several entries with the
-same untranslated-string in a PO file, provided that they each have a
-different context. Note that an empty context string and an absent
-msgctxt line do not mean the same thing.
+       def render_entity_attributes(self, entity):
+           self.w(u'<p>published on %s</p>' %
+                  entity.publish_date.strftime('%Y-%m-%d'))
+           super(BlogEntryPrimaryView, self).render_entity_attributes(entity)
 
-Contexts and CubicWeb
-`````````````````````
 
-CubicWeb PO files have both non-contextual and contextual msgids.
+The above source code defines a new primary view for
+``BlogEntry``. The `__reid__` class attribute is not repeated there since it
+is inherited through the `primary.PrimaryView` class.
 
-Contextual entries are automatically used in some cases. For instance,
-entity.dc_type(), eschema.display_name(req) or display_name(etype,
-req, form, context) methods/function calls will use them.
+The selector for this view chains the selector of the inherited class
+with its own specific criterion.
 
-It is also possible to explicitly use a context with `_cw.pgettext(context,
-msgid)`.
+The view method ``self.w()`` is used to output data. Here `lines
+08-09` output HTML for the publication date of the entry.
 
+.. image:: ../../../images/lax-book_09-new-view-blogentry_en.png
+   :alt: blog entries now look much nicer
 
-.. _translate-application-cube:
+Let us now improve the primary view of a blog
 
-Specialize translation for an application cube
-``````````````````````````````````````````````
+.. sourcecode:: python
 
-Every cube has its own translation files. For a specific application cube
-it can be useful to specialize translations of other cubes. You can either mark
-those strings for translation using `_` in the python code, or add a
-`static-messages.pot` file into the `i18n` directory. This file
-looks like: ::
+ from logilab.mtconverter import xml_escape
+ from cubicweb.predicates import is_instance, one_line_rset
+ from cubicweb_web.views.primary import Primaryview
+
+ class BlogPrimaryView(PrimaryView):
+     __regid__ = 'primary'
+     __select__ = PrimaryView.__select__ & is_instance('Blog')
+     rql = 'Any BE ORDERBY D DESC WHERE BE entry_of B, BE publish_date D, B eid %(b)s'
+
+     def render_entity_relations(self, entity):
+         rset = self._cw.execute(self.rql, {'b' : entity.eid})
+         for entry in rset.entities():
+             self.w(u'<p>%s</p>' % entry.view('inblogcontext'))
+
+ class BlogEntryInBlogView(EntityView):
+     __regid__ = 'inblogcontext'
+     __select__ = is_instance('BlogEntry')
+
+     def cell_call(self, row, col):
+         entity = self.cw_rset.get_entity(row, col)
+         self.w(u'<a href="%s" title="%s">%s</a>' %
+                entity.absolute_url(),
+                xml_escape(entity.content[:50]),
+                xml_escape(entity.description))
+
+This happens in two places. First we override the
+render_entity_relations method of a Blog's primary view. Here we want
+to display our blog entries in a custom way.
+
+At `line 10`, a simple request is made to build a result set with all
+the entities linked to the current ``Blog`` entity by the relationship
+``entry_of``. The part of the framework handling the request knows
+about the schema and infers that such entities have to be of the
+``BlogEntry`` kind and retrieves them (in the prescribed publish_date
+order).
+
+The request returns a selection of data called a result set. Result
+set objects have an .entities() method returning a generator on
+requested entities (going transparently through the `ORM` layer).
+
+At `line 13` the view 'inblogcontext' is applied to each blog entry to
+output HTML. (Note that the 'inblogcontext' view is not defined
+whatsoever in *CubicWeb*. You are absolutely free to define whole view
+families.) We juste arrange to wrap each blogentry output in a 'p'
+html element.
+
+Next, we define the 'inblogcontext' view. This is NOT a primary view,
+with its well-defined sections (title, metadata, attribtues,
+relations/boxes). All a basic view has to define is cell_call.
+
+Since views are applied to result sets which can be tables of data, we
+have to recover the entity from its (row,col)-coordinates (`line
+20`). Then we can spit some HTML.
+
+.. warning::
+
+  Be careful: all strings manipulated in *CubicWeb* are actually
+  unicode strings. While web browsers are usually tolerant to
+  incoherent encodings they are being served, we should not abuse
+  it. Hence we have to properly escape our data. The xml_escape()
+  function has to be used to safely fill (X)HTML elements from Python
+  unicode strings.
 
-    msgid ""
-    msgstr ""
-    "PO-Revision-Date: YEAR-MO-DA HO:MI +ZONE\n"
-    "MIME-Version: 1.0\n"
-    "Content-Type: text/plain; charset=UTF-8\n"
-    "Content-Transfer-Encoding: 8bit\n"
-    "Generated-By: pygettext.py 1.5\n"
-    "Plural-Forms: nplurals=2; plural=(n > 1);\n"
+Assuming we added entries to the blog titled `MyLife`, displaying it
+now allows to read its description and all its entries.
 
-    msgig "expression to be translated"
-    msgstr ""
+.. image:: ../../../images/lax-book_10-blog-with-two-entries_en.png
+   :alt: a blog and all its entries
 
-Doing this, ``expression to be translated`` will be taken into account by
-the ``i18ncube`` command and additional messages will then appear in `.po` files
-of the cube.
```

### Comparing `cubicweb-4.7.0/doc/book/devweb/js.rst` & `cubicweb-4.7.1/doc/book/devweb/js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/publisher.rst` & `cubicweb-4.7.1/doc/book/devweb/publisher.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/request.rst` & `cubicweb-4.7.1/doc/book/devweb/request.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/resource.rst` & `cubicweb-4.7.1/doc/book/devweb/resource.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/searchbar.rst` & `cubicweb-4.7.1/doc/book/devweb/searchbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst` & `cubicweb-4.7.1/doc/book/devweb/views/basetemplates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst` & `cubicweb-4.7.1/doc/book/devweb/views/baseviews.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/boxes.rst` & `cubicweb-4.7.1/doc/book/devweb/views/boxes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst` & `cubicweb-4.7.1/doc/book/devweb/views/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst` & `cubicweb-4.7.1/doc/book/devweb/views/idownloadable.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/reledit.rst` & `cubicweb-4.7.1/doc/book/devweb/views/reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/startup.rst` & `cubicweb-4.7.1/doc/book/devweb/views/startup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/table.rst` & `cubicweb-4.7.1/doc/book/devweb/views/table.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst` & `cubicweb-4.7.1/doc/book/devweb/views/urlpublish.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/views.rst` & `cubicweb-4.7.1/doc/book/devweb/views/views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst` & `cubicweb-4.7.1/doc/book/devweb/views/xmlrss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/devweb/warning.rst` & `cubicweb-4.7.1/doc/book/devweb/warning.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/intro/concepts.rst` & `cubicweb-4.7.1/doc/book/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/intro/history.rst` & `cubicweb-4.7.1/doc/book/intro/history.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/auth.rst` & `cubicweb-4.7.1/doc/book/pyramid/auth.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/ctl.rst` & `cubicweb-4.7.1/doc/book/pyramid/ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst` & `cubicweb-4.7.1/doc/book/pyramid/debug_toolbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/index.rst` & `cubicweb-4.7.1/doc/book/pyramid/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/quickstart.rst` & `cubicweb-4.7.1/doc/book/pyramid/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/pyramid/settings.rst` & `cubicweb-4.7.1/doc/book/pyramid/settings.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/security/csrf.rst` & `cubicweb-4.7.1/doc/book/security/csrf.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/src/archi_globale.dia` & `cubicweb-4.7.1/doc/book/src/archi_globale.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/book/src/main_template_layout.dia` & `cubicweb-4.7.1/doc/book/src/main_template_layout.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.14.rst` & `cubicweb-4.7.1/doc/changes/3.14.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.15.rst` & `cubicweb-4.7.1/doc/changes/3.15.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.16.rst` & `cubicweb-4.7.1/doc/changes/3.16.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.17.rst` & `cubicweb-4.7.1/doc/changes/3.17.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.18.rst` & `cubicweb-4.7.1/doc/changes/3.18.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.19.rst` & `cubicweb-4.7.1/doc/changes/3.19.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.20.rst` & `cubicweb-4.7.1/doc/changes/3.20.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.21.rst` & `cubicweb-4.7.1/doc/changes/3.21.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.22.rst` & `cubicweb-4.7.1/doc/changes/3.22.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.23.rst` & `cubicweb-4.7.1/doc/changes/3.23.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.24.rst` & `cubicweb-4.7.1/doc/changes/3.24.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.25.rst` & `cubicweb-4.7.1/doc/changes/3.25.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.27.rst` & `cubicweb-4.7.1/doc/changes/3.27.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.28.rst` & `cubicweb-4.7.1/doc/changes/3.28.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.29.rst` & `cubicweb-4.7.1/doc/changes/3.29.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.30.rst` & `cubicweb-4.7.1/doc/changes/3.30.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.31.rst` & `cubicweb-4.7.1/doc/changes/3.31.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.32.rst` & `cubicweb-4.7.1/doc/changes/3.32.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.32_reledit.rst` & `cubicweb-4.7.1/doc/changes/3.32_reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.33.rst` & `cubicweb-4.7.1/doc/changes/3.33.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.34.rst` & `cubicweb-4.7.1/doc/changes/3.34.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.35.rst` & `cubicweb-4.7.1/doc/changes/3.35.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.36.rst` & `cubicweb-4.7.1/doc/changes/3.36.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.37.rst` & `cubicweb-4.7.1/doc/changes/3.37.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/3.38.rst` & `cubicweb-4.7.1/doc/changes/3.38.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/4.0.rst` & `cubicweb-4.7.1/doc/changes/4.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/4.1.rst` & `cubicweb-4.7.1/doc/changes/4.1.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/4.3.rst` & `cubicweb-4.7.1/doc/changes/4.3.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/4.5.rst` & `cubicweb-4.7.1/doc/changes/4.5.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/4.6.rst` & `cubicweb-4.7.1/doc/changes/4.6.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/changes/changelog.rst` & `cubicweb-4.7.1/doc/changes/changelog.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/conf.py` & `cubicweb-4.7.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/03-transitions-view_en.png` & `cubicweb-4.7.1/doc/images/03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/breadcrumbs_header.png` & `cubicweb-4.7.1/doc/images/breadcrumbs_header.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_general_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_general_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_registry_content_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_registry_content_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_registry_decisions_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_registry_decisions_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_rql_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_rql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_rql_traceback_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_rql_traceback_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_show_source.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_show_source.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_show_source_link.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_show_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_sql_panel.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_sql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/debugtoolbar_traceback_source_link.png` & `cubicweb-4.7.1/doc/images/debugtoolbar_traceback_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/example-card-with-rql-directive.png` & `cubicweb-4.7.1/doc/images/example-card-with-rql-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/example-card-with-rql-table-directive.png` & `cubicweb-4.7.1/doc/images/example-card-with-rql-table-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/facet_date_range.png` & `cubicweb-4.7.1/doc/images/facet_date_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/facet_has_image.png` & `cubicweb-4.7.1/doc/images/facet_has_image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/facet_overview.png` & `cubicweb-4.7.1/doc/images/facet_overview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/facet_range.png` & `cubicweb-4.7.1/doc/images/facet_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_00-login_en.png` & `cubicweb-4.7.1/doc/images/lax-book_00-login_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_01-start_en.png` & `cubicweb-4.7.1/doc/images/lax-book_01-start_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_02-cookie-values_en.png` & `cubicweb-4.7.1/doc/images/lax-book_02-cookie-values_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_02-create-blog_en.png` & `cubicweb-4.7.1/doc/images/lax-book_02-create-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_03-list-one-blog_en.png` & `cubicweb-4.7.1/doc/images/lax-book_03-list-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_03-site-config-panel_en.png` & `cubicweb-4.7.1/doc/images/lax-book_03-site-config-panel_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_03-state-submitted_en.png` & `cubicweb-4.7.1/doc/images/lax-book_03-state-submitted_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_03-transitions-view_en.png` & `cubicweb-4.7.1/doc/images/lax-book_03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_04-detail-one-blog_en.png` & `cubicweb-4.7.1/doc/images/lax-book_04-detail-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_05-list-two-blog_en.png` & `cubicweb-4.7.1/doc/images/lax-book_05-list-two-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_06-add-relation-entryof_en.png` & `cubicweb-4.7.1/doc/images/lax-book_06-add-relation-entryof_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_06-main-template-logo_en.png` & `cubicweb-4.7.1/doc/images/lax-book_06-main-template-logo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_07-detail-one-blogentry_en.png` & `cubicweb-4.7.1/doc/images/lax-book_07-detail-one-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_08-schema_en.png` & `cubicweb-4.7.1/doc/images/lax-book_08-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_09-new-view-blogentry_en.png` & `cubicweb-4.7.1/doc/images/lax-book_09-new-view-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/lax-book_10-blog-with-two-entries_en.png` & `cubicweb-4.7.1/doc/images/lax-book_10-blog-with-two-entries_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/main_template.png` & `cubicweb-4.7.1/doc/images/main_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/main_template.svg` & `cubicweb-4.7.1/doc/images/main_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/main_template_layout.png` & `cubicweb-4.7.1/doc/images/main_template_layout.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/primaryview_template.png` & `cubicweb-4.7.1/doc/images/primaryview_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/primaryview_template.svg` & `cubicweb-4.7.1/doc/images/primaryview_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/request_session.png` & `cubicweb-4.7.1/doc/images/request_session.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/request_session.svg` & `cubicweb-4.7.1/doc/images/request_session.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/server-class-diagram.png` & `cubicweb-4.7.1/doc/images/server-class-diagram.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_blog-form_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_blog-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_blog-primary-after-post-creation_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_blog-primary_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_blog-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_blogs-list_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_blogs-list_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_form-generic-relations_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_form-generic-relations_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_index_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_index_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_index_gettext_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_index_gettext_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_index_logged_in_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_index_logged_in_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_login-form_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_login-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-custom-primary_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-custom-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-default-primary_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-default-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-community-taggable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-custom-footer_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-custom-footer_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-schema_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_myblog-siteinfo_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_myblog-siteinfo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_schema_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_schema_graphviz_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_schema_graphviz_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-base_siteconfig_en.png` & `cubicweb-4.7.1/doc/images/tutos-base_siteconfig_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_admin.png` & `cubicweb-4.7.1/doc/images/tutos-museum_admin.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_city_created.png` & `cubicweb-4.7.1/doc/images/tutos-museum_city_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_city_creation.png` & `cubicweb-4.7.1/doc/images/tutos-museum_city_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_data_model_schema.png` & `cubicweb-4.7.1/doc/images/tutos-museum_data_model_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_empty_instance.png` & `cubicweb-4.7.1/doc/images/tutos-museum_empty_instance.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_finished_import.png` & `cubicweb-4.7.1/doc/images/tutos-museum_finished_import.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_list_view.png` & `cubicweb-4.7.1/doc/images/tutos-museum_list_view.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_museum_created.png` & `cubicweb-4.7.1/doc/images/tutos-museum_museum_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_museum_creation.png` & `cubicweb-4.7.1/doc/images/tutos-museum_museum_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_museum_with_city_name.png` & `cubicweb-4.7.1/doc/images/tutos-museum_museum_with_city_name.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_react_map.png` & `cubicweb-4.7.1/doc/images/tutos-museum_react_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-museum_with_schema.png` & `cubicweb-4.7.1/doc/images/tutos-museum_with_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_background-image.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_background-image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_boxes.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_boxes.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_breadcrumbs.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_breadcrumbs.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_facets.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_facets.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_grey-box.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_grey-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_index-after.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_index-after.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_index-before.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_index-before.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_login-box.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_login-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_prevnext.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_prevnext.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui1.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui1.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui2.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui2.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui3.png` & `cubicweb-4.7.1/doc/images/tutos-photowebsite_ui3.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/undo_history-view_w600.png` & `cubicweb-4.7.1/doc/images/undo_history-view_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/undo_mesage_w600.png` & `cubicweb-4.7.1/doc/images/undo_mesage_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/undo_startup-link_w600.png` & `cubicweb-4.7.1/doc/images/undo_startup-link_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/views-table-filter-shadow.png` & `cubicweb-4.7.1/doc/images/views-table-filter-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/views-table-filter.png` & `cubicweb-4.7.1/doc/images/views-table-filter.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/views-table-shadow.png` & `cubicweb-4.7.1/doc/images/views-table-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/images/views-table.png` & `cubicweb-4.7.1/doc/images/views-table.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/index.rst` & `cubicweb-4.7.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/plan_formation_python_cubicweb.txt` & `cubicweb-4.7.1/doc/plan_formation_python_cubicweb.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tools/generate_modules.py` & `cubicweb-4.7.1/doc/tools/generate_modules.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tools/mode_plan.py` & `cubicweb-4.7.1/doc/tools/mode_plan.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tools/pyjsrest.py` & `cubicweb-4.7.1/doc/tools/pyjsrest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/advanced/index.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/advanced/part01_create-cube.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/part01_create-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/advanced/part02_security.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/part02_security.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/advanced/part03_bfss.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/part03_bfss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/advanced/part04_ui-base.rst` & `cubicweb-4.7.1/doc/tutorials/advanced/part04_ui-base.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/base/blog-in-five-minutes.rst` & `cubicweb-4.7.1/doc/tutorials/base/blog-in-five-minutes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/base/conclusion.rst` & `cubicweb-4.7.1/doc/tutorials/base/conclusion.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/base/customizing-the-application.rst` & `cubicweb-4.7.1/doc/tutorials/base/customizing-the-application.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/base/discovering-the-ui.rst` & `cubicweb-4.7.1/doc/tutorials/base/discovering-the-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/base/index.rst` & `cubicweb-4.7.1/doc/tutorials/base/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_import.py` & `cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_import.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_parser.py` & `cubicweb-4.7.1/doc/tutorials/dataimport/diseasome_parser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/dataimport/index.rst` & `cubicweb-4.7.1/doc/tutorials/dataimport/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/dataimport/schema.py` & `cubicweb-4.7.1/doc/tutorials/dataimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/index.rst` & `cubicweb-4.7.1/doc/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/data-management.rst` & `cubicweb-4.7.1/doc/tutorials/museum/data-management.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/develop-app.rst` & `cubicweb-4.7.1/doc/tutorials/museum/develop-app.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/develop-ui.rst` & `cubicweb-4.7.1/doc/tutorials/museum/develop-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/enhance-views.rst` & `cubicweb-4.7.1/doc/tutorials/museum/enhance-views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/getting-started.rst` & `cubicweb-4.7.1/doc/tutorials/museum/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/doc/tutorials/museum/index.rst` & `cubicweb-4.7.1/doc/tutorials/museum/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/extras/cubicweb-ctl.bash_completion` & `cubicweb-4.7.1/extras/cubicweb-ctl.bash_completion`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/jshintrc` & `cubicweb-4.7.1/jshintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/man/cubicweb-ctl.1` & `cubicweb-4.7.1/man/cubicweb-ctl.1`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/pylintrc` & `cubicweb-4.7.1/pylintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/setup.py` & `cubicweb-4.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.7.0/tox.ini` & `cubicweb-4.7.1/tox.ini`

 * *Files identical despite different names*

