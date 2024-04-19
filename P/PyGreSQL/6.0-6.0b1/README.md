# Comparing `tmp/PyGreSQL-6.0.tar.gz` & `tmp/PyGreSQL-6.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGreSQL-6.0.tar", last modified: Tue Oct  3 19:45:36 2023, max compression
+gzip compressed data, was "PyGreSQL-6.0b1.tar", last modified: Wed Sep  6 17:34:07 2023, max compression
```

## Comparing `PyGreSQL-6.0.tar` & `PyGreSQL-6.0b1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:36.343708 PyGreSQL-6.0/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1402 2023-08-28 16:13:38.000000 PyGreSQL-6.0/LICENSE.txt
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      521 2023-09-04 21:53:28.000000 PyGreSQL-6.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-10-03 19:45:36.328192 PyGreSQL-6.0/PKG-INFO
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:32.951676 PyGreSQL-6.0/PyGreSQL.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4822 2023-10-03 19:45:29.000000 PyGreSQL-6.0/PyGreSQL.egg-info/PKG-INFO
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2240 2023-10-03 19:45:32.000000 PyGreSQL-6.0/PyGreSQL.egg-info/SOURCES.txt
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)        1 2023-10-03 19:45:29.000000 PyGreSQL-6.0/PyGreSQL.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-09-04 10:47:40.000000 PyGreSQL-6.0/PyGreSQL.egg-info/not-zip-safe
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)        8 2023-10-03 19:45:29.000000 PyGreSQL-6.0/PyGreSQL.egg-info/top_level.txt
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1463 2023-09-06 14:54:53.000000 PyGreSQL-6.0/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:33.116517 PyGreSQL-6.0/docs/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      634 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/Makefile
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:33.175893 PyGreSQL-6.0/docs/_static/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9326 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/_static/favicon.ico
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9719 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/_static/pygresql.png
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2330 2023-09-06 14:51:34.000000 PyGreSQL-6.0/docs/about.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:33.405117 PyGreSQL-6.0/docs/community/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      160 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/homes.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      473 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      148 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/issues.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      369 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/mailinglist.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      797 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/source.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      783 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/community/support.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3201 2023-10-03 18:50:22.000000 PyGreSQL-6.0/docs/conf.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:33.595322 PyGreSQL-6.0/docs/contents/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    37573 2023-10-03 19:10:42.000000 PyGreSQL-6.0/docs/contents/changelog.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      650 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/contents/examples.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1983 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/contents/general.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      555 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/contents/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     7970 2023-09-06 14:51:44.000000 PyGreSQL-6.0/docs/contents/install.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:33.991743 PyGreSQL-6.0/docs/contents/pg/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    17126 2023-09-01 11:41:02.000000 PyGreSQL-6.0/docs/contents/pg/adaptation.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    27211 2023-09-04 16:15:48.000000 PyGreSQL-6.0/docs/contents/pg/connection.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3959 2023-08-28 16:13:38.000000 PyGreSQL-6.0/docs/contents/pg/db_types.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    40007 2023-09-04 06:28:30.000000 PyGreSQL-6.0/docs/contents/pg/db_wrapper.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      315 2023-08-28 16:13:39.000000 PyGreSQL-6.0/docs/contents/pg/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      852 2023-08-28 16:13:39.000000 PyGreSQL-6.0/docs/contents/pg/introduction.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6468 2023-09-04 16:15:34.000000 PyGreSQL-6.0/docs/contents/pg/large_objects.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    28899 2023-09-04 19:56:19.000000 PyGreSQL-6.0/docs/contents/pg/module.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4541 2023-08-28 16:13:39.000000 PyGreSQL-6.0/docs/contents/pg/notification.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14763 2023-09-02 20:43:05.000000 PyGreSQL-6.0/docs/contents/pg/query.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:34.328462 PyGreSQL-6.0/docs/contents/pgdb/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14996 2023-09-01 11:51:59.000000 PyGreSQL-6.0/docs/contents/pgdb/adaptation.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3850 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/pgdb/connection.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    15775 2023-09-04 06:29:10.000000 PyGreSQL-6.0/docs/contents/pgdb/cursor.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      285 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/pgdb/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      761 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/pgdb/introduction.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     7120 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/pgdb/module.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3496 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/pgdb/typecache.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     5712 2023-09-01 22:45:36.000000 PyGreSQL-6.0/docs/contents/pgdb/types.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:34.594294 PyGreSQL-6.0/docs/contents/postgres/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4735 2023-09-01 11:46:24.000000 PyGreSQL-6.0/docs/contents/postgres/advanced.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    12413 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/postgres/basic.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4939 2023-09-01 12:01:32.000000 PyGreSQL-6.0/docs/contents/postgres/func.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      413 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/postgres/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4667 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/contents/postgres/syscat.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9475 2023-09-04 06:25:29.000000 PyGreSQL-6.0/docs/contents/tutorial.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1325 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/copyright.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:34.740245 PyGreSQL-6.0/docs/download/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1336 2023-08-28 16:13:40.000000 PyGreSQL-6.0/docs/download/download.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      807 2023-09-06 09:59:15.000000 PyGreSQL-6.0/docs/download/files.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      530 2023-09-01 18:08:07.000000 PyGreSQL-6.0/docs/download/index.rst
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      800 2023-08-28 16:13:41.000000 PyGreSQL-6.0/docs/make.bat
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)       13 2023-08-28 16:13:41.000000 PyGreSQL-6.0/docs/requirements.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:35.065032 PyGreSQL-6.0/ext/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    56478 2023-09-06 15:43:28.000000 PyGreSQL-6.0/ext/pgconn.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)    45947 2023-09-02 10:59:22.000000 PyGreSQL-6.0/ext/pginternal.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)    13433 2023-09-02 11:32:51.000000 PyGreSQL-6.0/ext/pglarge.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)    41577 2023-09-06 13:26:38.000000 PyGreSQL-6.0/ext/pgmodule.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3944 2023-09-02 11:32:51.000000 PyGreSQL-6.0/ext/pgnotice.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)    30767 2023-09-02 11:32:51.000000 PyGreSQL-6.0/ext/pgquery.c
--rw-r--r--   0 vscode    (1000) vscode    (1000)    24127 2023-09-04 19:22:46.000000 PyGreSQL-6.0/ext/pgsource.c
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4558 2023-08-28 16:13:41.000000 PyGreSQL-6.0/ext/pgtypes.h
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:35.492342 PyGreSQL-6.0/pg/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3594 2023-09-05 20:34:56.000000 PyGreSQL-6.0/pg/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16678 2023-09-06 14:11:28.000000 PyGreSQL-6.0/pg/_pg.pyi
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23710 2023-09-05 13:41:48.000000 PyGreSQL-6.0/pg/adapt.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1094 2023-09-05 10:09:37.000000 PyGreSQL-6.0/pg/attrs.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15133 2023-09-05 10:14:12.000000 PyGreSQL-6.0/pg/cast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-09-06 13:32:57.000000 PyGreSQL-6.0/pg/core.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    62761 2023-09-06 14:11:51.000000 PyGreSQL-6.0/pg/db.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1163 2023-09-05 13:15:58.000000 PyGreSQL-6.0/pg/error.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3728 2023-09-05 21:18:39.000000 PyGreSQL-6.0/pg/helpers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5717 2023-09-05 10:10:53.000000 PyGreSQL-6.0/pg/notify.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      125 2023-09-04 16:35:39.000000 PyGreSQL-6.0/pg/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      615 2023-09-05 11:10:41.000000 PyGreSQL-6.0/pg/tz.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:35.760492 PyGreSQL-6.0/pgdb/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3819 2023-09-05 15:08:04.000000 PyGreSQL-6.0/pgdb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7369 2023-09-05 14:02:12.000000 PyGreSQL-6.0/pgdb/adapt.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    20617 2023-09-05 14:12:44.000000 PyGreSQL-6.0/pgdb/cast.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2140 2023-09-05 22:35:11.000000 PyGreSQL-6.0/pgdb/connect.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5077 2023-09-05 21:19:05.000000 PyGreSQL-6.0/pgdb/connection.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      353 2023-09-05 14:14:32.000000 PyGreSQL-6.0/pgdb/constants.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    25696 2023-09-05 20:42:19.000000 PyGreSQL-6.0/pgdb/cursor.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       63 2023-09-04 16:33:49.000000 PyGreSQL-6.0/pgdb/py.typed
--rw-r--r--   0 vscode    (1000) vscode    (1000)      844 2023-09-05 13:46:09.000000 PyGreSQL-6.0/pgdb/typecode.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2621 2023-10-03 18:45:46.000000 PyGreSQL-6.0/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-10-03 19:45:36.344998 PyGreSQL-6.0/setup.cfg
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6850 2023-10-03 19:00:39.000000 PyGreSQL-6.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-10-03 19:45:36.276747 PyGreSQL-6.0/tests/
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)      476 2023-08-28 16:13:41.000000 PyGreSQL-6.0/tests/__init__.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1093 2023-09-04 19:47:08.000000 PyGreSQL-6.0/tests/config.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    31764 2023-09-05 22:15:42.000000 PyGreSQL-6.0/tests/dbapi20.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    10955 2023-09-05 22:11:45.000000 PyGreSQL-6.0/tests/test_classic.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2716 2023-09-05 08:39:40.000000 PyGreSQL-6.0/tests/test_classic_attrdict.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)   101346 2023-10-03 18:13:48.000000 PyGreSQL-6.0/tests/test_classic_connection.py
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)   202523 2023-10-03 18:13:19.000000 PyGreSQL-6.0/tests/test_classic_dbwrapper.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    41819 2023-09-06 15:05:59.000000 PyGreSQL-6.0/tests/test_classic_functions.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14716 2023-09-03 11:10:03.000000 PyGreSQL-6.0/tests/test_classic_largeobj.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    13282 2023-09-02 08:16:55.000000 PyGreSQL-6.0/tests/test_classic_notification.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    57406 2023-09-05 22:34:23.000000 PyGreSQL-6.0/tests/test_dbapi20.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)    18863 2023-09-03 21:50:00.000000 PyGreSQL-6.0/tests/test_dbapi20_copy.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6406 2023-09-04 20:40:59.000000 PyGreSQL-6.0/tests/test_tutorial.py
--rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1094 2023-10-03 18:22:15.000000 PyGreSQL-6.0/tox.ini
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:07.931941 PyGreSQL-6.0b1/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1402 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/LICENSE.txt
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      521 2023-09-04 21:53:28.000000 PyGreSQL-6.0b1/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4821 2023-09-06 17:34:07.928937 PyGreSQL-6.0b1/PKG-INFO
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:05.172369 PyGreSQL-6.0b1/PyGreSQL.egg-info/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4821 2023-09-06 17:34:02.000000 PyGreSQL-6.0b1/PyGreSQL.egg-info/PKG-INFO
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2240 2023-09-06 17:34:04.000000 PyGreSQL-6.0b1/PyGreSQL.egg-info/SOURCES.txt
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        1 2023-09-06 17:34:02.000000 PyGreSQL-6.0b1/PyGreSQL.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-09-04 10:47:40.000000 PyGreSQL-6.0b1/PyGreSQL.egg-info/not-zip-safe
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)        8 2023-09-06 17:34:02.000000 PyGreSQL-6.0b1/PyGreSQL.egg-info/top_level.txt
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1463 2023-09-06 14:54:53.000000 PyGreSQL-6.0b1/README.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:05.316928 PyGreSQL-6.0b1/docs/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      634 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/Makefile
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:05.379385 PyGreSQL-6.0b1/docs/_static/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9326 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/_static/favicon.ico
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9719 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/_static/pygresql.png
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2330 2023-09-06 14:51:34.000000 PyGreSQL-6.0b1/docs/about.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:05.602876 PyGreSQL-6.0b1/docs/community/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      160 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/homes.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      473 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      148 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/issues.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      369 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/mailinglist.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      797 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/source.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      783 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/community/support.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2915 2023-09-06 14:56:25.000000 PyGreSQL-6.0b1/docs/conf.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:05.910211 PyGreSQL-6.0b1/docs/contents/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    37321 2023-09-06 15:08:48.000000 PyGreSQL-6.0b1/docs/contents/changelog.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      650 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/contents/examples.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1983 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/contents/general.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      555 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/contents/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     7970 2023-09-06 14:51:44.000000 PyGreSQL-6.0b1/docs/contents/install.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:06.352533 PyGreSQL-6.0b1/docs/contents/pg/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    17126 2023-09-01 11:41:02.000000 PyGreSQL-6.0b1/docs/contents/pg/adaptation.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    27211 2023-09-04 16:15:48.000000 PyGreSQL-6.0b1/docs/contents/pg/connection.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3959 2023-08-28 16:13:38.000000 PyGreSQL-6.0b1/docs/contents/pg/db_types.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    40007 2023-09-04 06:28:30.000000 PyGreSQL-6.0b1/docs/contents/pg/db_wrapper.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      315 2023-08-28 16:13:39.000000 PyGreSQL-6.0b1/docs/contents/pg/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      852 2023-08-28 16:13:39.000000 PyGreSQL-6.0b1/docs/contents/pg/introduction.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6468 2023-09-04 16:15:34.000000 PyGreSQL-6.0b1/docs/contents/pg/large_objects.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    28899 2023-09-04 19:56:19.000000 PyGreSQL-6.0b1/docs/contents/pg/module.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4541 2023-08-28 16:13:39.000000 PyGreSQL-6.0b1/docs/contents/pg/notification.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14763 2023-09-02 20:43:05.000000 PyGreSQL-6.0b1/docs/contents/pg/query.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:06.668341 PyGreSQL-6.0b1/docs/contents/pgdb/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14996 2023-09-01 11:51:59.000000 PyGreSQL-6.0b1/docs/contents/pgdb/adaptation.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3850 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/pgdb/connection.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    15775 2023-09-04 06:29:10.000000 PyGreSQL-6.0b1/docs/contents/pgdb/cursor.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      285 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/pgdb/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      761 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/pgdb/introduction.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     7120 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/pgdb/module.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3496 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/pgdb/typecache.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     5712 2023-09-01 22:45:36.000000 PyGreSQL-6.0b1/docs/contents/pgdb/types.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:06.852634 PyGreSQL-6.0b1/docs/contents/postgres/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4735 2023-09-01 11:46:24.000000 PyGreSQL-6.0b1/docs/contents/postgres/advanced.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    12413 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/postgres/basic.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4939 2023-09-01 12:01:32.000000 PyGreSQL-6.0b1/docs/contents/postgres/func.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      413 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/postgres/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4667 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/contents/postgres/syscat.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     9475 2023-09-04 06:25:29.000000 PyGreSQL-6.0b1/docs/contents/tutorial.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1325 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/copyright.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:06.938978 PyGreSQL-6.0b1/docs/download/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1336 2023-08-28 16:13:40.000000 PyGreSQL-6.0b1/docs/download/download.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      807 2023-09-06 09:59:15.000000 PyGreSQL-6.0b1/docs/download/files.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      530 2023-09-01 18:08:07.000000 PyGreSQL-6.0b1/docs/download/index.rst
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      800 2023-08-28 16:13:41.000000 PyGreSQL-6.0b1/docs/make.bat
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)       13 2023-08-28 16:13:41.000000 PyGreSQL-6.0b1/docs/requirements.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:07.132328 PyGreSQL-6.0b1/ext/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    56478 2023-09-06 15:43:28.000000 PyGreSQL-6.0b1/ext/pgconn.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    45947 2023-09-02 10:59:22.000000 PyGreSQL-6.0b1/ext/pginternal.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    13433 2023-09-02 11:32:51.000000 PyGreSQL-6.0b1/ext/pglarge.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    41577 2023-09-06 13:26:38.000000 PyGreSQL-6.0b1/ext/pgmodule.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3944 2023-09-02 11:32:51.000000 PyGreSQL-6.0b1/ext/pgnotice.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    30767 2023-09-02 11:32:51.000000 PyGreSQL-6.0b1/ext/pgquery.c
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    24127 2023-09-04 19:22:46.000000 PyGreSQL-6.0b1/ext/pgsource.c
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     4558 2023-08-28 16:13:41.000000 PyGreSQL-6.0b1/ext/pgtypes.h
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:07.400515 PyGreSQL-6.0b1/pg/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3594 2023-09-05 20:34:56.000000 PyGreSQL-6.0b1/pg/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    16678 2023-09-06 14:11:28.000000 PyGreSQL-6.0b1/pg/_pg.pyi
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23710 2023-09-05 13:41:48.000000 PyGreSQL-6.0b1/pg/adapt.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1094 2023-09-05 10:09:37.000000 PyGreSQL-6.0b1/pg/attrs.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    15133 2023-09-05 10:14:12.000000 PyGreSQL-6.0b1/pg/cast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3680 2023-09-06 13:32:57.000000 PyGreSQL-6.0b1/pg/core.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    62761 2023-09-06 14:11:51.000000 PyGreSQL-6.0b1/pg/db.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1163 2023-09-05 13:15:58.000000 PyGreSQL-6.0b1/pg/error.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3728 2023-09-05 21:18:39.000000 PyGreSQL-6.0b1/pg/helpers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5717 2023-09-05 10:10:53.000000 PyGreSQL-6.0b1/pg/notify.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      125 2023-09-04 16:35:39.000000 PyGreSQL-6.0b1/pg/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      615 2023-09-05 11:10:41.000000 PyGreSQL-6.0b1/pg/tz.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:07.608913 PyGreSQL-6.0b1/pgdb/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     3819 2023-09-05 15:08:04.000000 PyGreSQL-6.0b1/pgdb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7369 2023-09-05 14:02:12.000000 PyGreSQL-6.0b1/pgdb/adapt.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20617 2023-09-05 14:12:44.000000 PyGreSQL-6.0b1/pgdb/cast.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2140 2023-09-05 22:35:11.000000 PyGreSQL-6.0b1/pgdb/connect.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5077 2023-09-05 21:19:05.000000 PyGreSQL-6.0b1/pgdb/connection.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      353 2023-09-05 14:14:32.000000 PyGreSQL-6.0b1/pgdb/constants.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    25696 2023-09-05 20:42:19.000000 PyGreSQL-6.0b1/pgdb/cursor.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       63 2023-09-04 16:33:49.000000 PyGreSQL-6.0b1/pgdb/py.typed
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      844 2023-09-05 13:46:09.000000 PyGreSQL-6.0b1/pgdb/typecode.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2607 2023-09-06 14:56:15.000000 PyGreSQL-6.0b1/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-09-06 17:34:07.932941 PyGreSQL-6.0b1/setup.cfg
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6405 2023-09-06 14:56:20.000000 PyGreSQL-6.0b1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-09-06 17:34:07.905615 PyGreSQL-6.0b1/tests/
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)      476 2023-08-28 16:13:41.000000 PyGreSQL-6.0b1/tests/__init__.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1093 2023-09-04 19:47:08.000000 PyGreSQL-6.0b1/tests/config.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    31764 2023-09-05 22:15:42.000000 PyGreSQL-6.0b1/tests/dbapi20.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    10955 2023-09-05 22:11:45.000000 PyGreSQL-6.0b1/tests/test_classic.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     2716 2023-09-05 08:39:40.000000 PyGreSQL-6.0b1/tests/test_classic_attrdict.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)   101307 2023-09-06 15:44:11.000000 PyGreSQL-6.0b1/tests/test_classic_connection.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)   202484 2023-09-06 15:49:02.000000 PyGreSQL-6.0b1/tests/test_classic_dbwrapper.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    41819 2023-09-06 15:05:59.000000 PyGreSQL-6.0b1/tests/test_classic_functions.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    14716 2023-09-03 11:10:03.000000 PyGreSQL-6.0b1/tests/test_classic_largeobj.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    13282 2023-09-02 08:16:55.000000 PyGreSQL-6.0b1/tests/test_classic_notification.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    57406 2023-09-05 22:34:23.000000 PyGreSQL-6.0b1/tests/test_dbapi20.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)    18863 2023-09-03 21:50:00.000000 PyGreSQL-6.0b1/tests/test_dbapi20_copy.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     6406 2023-09-04 20:40:59.000000 PyGreSQL-6.0b1/tests/test_tutorial.py
+-rwxrwxrwx   0 vscode    (1000) vscode    (1000)     1065 2023-09-06 17:29:06.000000 PyGreSQL-6.0b1/tox.ini
```

### Comparing `PyGreSQL-6.0/LICENSE.txt` & `PyGreSQL-6.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/MANIFEST.in` & `PyGreSQL-6.0b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/PKG-INFO` & `PyGreSQL-6.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyGreSQL
-Version: 6.0
+Version: 6.0b1
 Summary: Python PostgreSQL interfaces
 Home-page: https://pygresql.github.io/
-Download-URL: https://pygresql.github.io/download/
+Download-URL: https://pygresql.github.io/contents/download/
 Author: D'Arcy J. M. Cain
 Author-email: "D'Arcy J. M. Cain" <darcy@pygresql.org>, Christoph Zwerschke <cito@online.de>
 License: Written by D'Arcy J.M. Cain (darcy@PyGreSQL.org)
         
         Based heavily on code written by Pascal Andre (andre@chimay.via.ecp.fr)
         
         Copyright (c) 1995, Pascal Andre
@@ -33,21 +33,21 @@
         
         THE AUTHORS SPECIFICALLY DISCLAIM ANY WARRANTIES, INCLUDING, BUT NOT LIMITED
         TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
         PURPOSE.  THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS, AND THE
         AUTHORS HAVE NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES,
         ENHANCEMENTS, OR MODIFICATIONS.
         
-Project-URL: Homepage, https://pygresql.github.io/
-Project-URL: Documentation, https://pygresql.github.io/contents/
-Project-URL: Source Code, https://github.com/PyGreSQL/PyGreSQL
-Project-URL: Issue Tracker, https://github.com/PyGreSQL/PyGreSQL/issues/
-Project-URL: Changelog, https://pygresql.github.io/contents/changelog.html
-Project-URL: Download, https://pygresql.github.io/download/
-Project-URL: Mailing List, https://mail.vex.net/mailman/listinfo/pygresql
+Project-URL: homepage, https://pygresql.github.io/
+Project-URL: documentation, https://pygresql.github.io/contents/
+Project-URL: source, https://github.com/PyGreSQL/PyGreSQL
+Project-URL: issues, https://github.com/PyGreSQL/PyGreSQL/issues/
+Project-URL: changelog, https://pygresql.github.io/contents/changelog.html
+Project-URL: download, https://pygresql.github.io/download/
+Project-URL: mailing list, https://mail.vex.net/mailman/listinfo/pygresql
 Keywords: pygresql,postgresql,database,api,dbapi
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
```

### Comparing `PyGreSQL-6.0/PyGreSQL.egg-info/PKG-INFO` & `PyGreSQL-6.0b1/PyGreSQL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PyGreSQL
-Version: 6.0
+Version: 6.0b1
 Summary: Python PostgreSQL interfaces
 Home-page: https://pygresql.github.io/
-Download-URL: https://pygresql.github.io/download/
+Download-URL: https://pygresql.github.io/contents/download/
 Author: D'Arcy J. M. Cain
 Author-email: "D'Arcy J. M. Cain" <darcy@pygresql.org>, Christoph Zwerschke <cito@online.de>
 License: Written by D'Arcy J.M. Cain (darcy@PyGreSQL.org)
         
         Based heavily on code written by Pascal Andre (andre@chimay.via.ecp.fr)
         
         Copyright (c) 1995, Pascal Andre
@@ -33,21 +33,21 @@
         
         THE AUTHORS SPECIFICALLY DISCLAIM ANY WARRANTIES, INCLUDING, BUT NOT LIMITED
         TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
         PURPOSE.  THE SOFTWARE PROVIDED HEREUNDER IS ON AN "AS IS" BASIS, AND THE
         AUTHORS HAVE NO OBLIGATIONS TO PROVIDE MAINTENANCE, SUPPORT, UPDATES,
         ENHANCEMENTS, OR MODIFICATIONS.
         
-Project-URL: Homepage, https://pygresql.github.io/
-Project-URL: Documentation, https://pygresql.github.io/contents/
-Project-URL: Source Code, https://github.com/PyGreSQL/PyGreSQL
-Project-URL: Issue Tracker, https://github.com/PyGreSQL/PyGreSQL/issues/
-Project-URL: Changelog, https://pygresql.github.io/contents/changelog.html
-Project-URL: Download, https://pygresql.github.io/download/
-Project-URL: Mailing List, https://mail.vex.net/mailman/listinfo/pygresql
+Project-URL: homepage, https://pygresql.github.io/
+Project-URL: documentation, https://pygresql.github.io/contents/
+Project-URL: source, https://github.com/PyGreSQL/PyGreSQL
+Project-URL: issues, https://github.com/PyGreSQL/PyGreSQL/issues/
+Project-URL: changelog, https://pygresql.github.io/contents/changelog.html
+Project-URL: download, https://pygresql.github.io/download/
+Project-URL: mailing list, https://mail.vex.net/mailman/listinfo/pygresql
 Keywords: pygresql,postgresql,database,api,dbapi
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
```

### Comparing `PyGreSQL-6.0/PyGreSQL.egg-info/SOURCES.txt` & `PyGreSQL-6.0b1/PyGreSQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/README.rst` & `PyGreSQL-6.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/Makefile` & `PyGreSQL-6.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/_static/favicon.ico` & `PyGreSQL-6.0b1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/_static/pygresql.png` & `PyGreSQL-6.0b1/docs/_static/pygresql.png`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/about.rst` & `PyGreSQL-6.0b1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/community/source.rst` & `PyGreSQL-6.0b1/docs/community/source.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/community/support.rst` & `PyGreSQL-6.0b1/docs/community/support.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/conf.py` & `PyGreSQL-6.0b1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,15 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'PyGreSQL'
 author = 'The PyGreSQL team'
 copyright = '2023, ' + author
 
-def project_version():
-    with open('../pyproject.toml') as f:
-        for d in f:
-            if d.startswith("version ="):
-                version = d.split("=")[1].strip().strip('"')
-                return version
-    raise Exception("Cannot determine PyGreSQL version")
-
-version = release = project_version()
+version = release = '6.0b1'
 
 language = 'en'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['sphinx.ext.autodoc']
```

### Comparing `PyGreSQL-6.0/docs/contents/changelog.rst` & `PyGreSQL-6.0b1/docs/contents/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 ChangeLog
 =========
 
-Version 6.0 (2023-10-03)
-------------------------
-- Tested with the recent releases of Python 3.12 and PostgreSQL 16.
-- Make pyproject.toml the only source of truth for the version number.
-- Please also note the changes already made in version 6.0b1.
-
 Version 6.0b1 (2023-09-06)
 --------------------------
 - Officially support Python 3.12 and PostgreSQL 16 (tested with rc versions).
 - Removed support for Python versions older than 3.7 (released June 2017)
   and PostgreSQL older than version 10 (released October 2017).
 - Converted the standalone modules `pg` and `pgdb` to packages with
   several submodules each. The C extension module is now part of the
```

### Comparing `PyGreSQL-6.0/docs/contents/examples.rst` & `PyGreSQL-6.0b1/docs/contents/examples.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/general.rst` & `PyGreSQL-6.0b1/docs/contents/general.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/index.rst` & `PyGreSQL-6.0b1/docs/contents/index.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/install.rst` & `PyGreSQL-6.0b1/docs/contents/install.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/adaptation.rst` & `PyGreSQL-6.0b1/docs/contents/pg/adaptation.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/connection.rst` & `PyGreSQL-6.0b1/docs/contents/pg/connection.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/db_types.rst` & `PyGreSQL-6.0b1/docs/contents/pg/db_types.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/db_wrapper.rst` & `PyGreSQL-6.0b1/docs/contents/pg/db_wrapper.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/introduction.rst` & `PyGreSQL-6.0b1/docs/contents/pg/introduction.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/large_objects.rst` & `PyGreSQL-6.0b1/docs/contents/pg/large_objects.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/module.rst` & `PyGreSQL-6.0b1/docs/contents/pg/module.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/notification.rst` & `PyGreSQL-6.0b1/docs/contents/pg/notification.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pg/query.rst` & `PyGreSQL-6.0b1/docs/contents/pg/query.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/adaptation.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/adaptation.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/connection.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/connection.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/cursor.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/cursor.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/introduction.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/introduction.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/module.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/module.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/typecache.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/typecache.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/pgdb/types.rst` & `PyGreSQL-6.0b1/docs/contents/pgdb/types.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/postgres/advanced.rst` & `PyGreSQL-6.0b1/docs/contents/postgres/advanced.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/postgres/basic.rst` & `PyGreSQL-6.0b1/docs/contents/postgres/basic.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/postgres/func.rst` & `PyGreSQL-6.0b1/docs/contents/postgres/func.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/postgres/syscat.rst` & `PyGreSQL-6.0b1/docs/contents/postgres/syscat.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/contents/tutorial.rst` & `PyGreSQL-6.0b1/docs/contents/tutorial.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/copyright.rst` & `PyGreSQL-6.0b1/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/download/download.rst` & `PyGreSQL-6.0b1/docs/download/download.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/download/files.rst` & `PyGreSQL-6.0b1/docs/download/files.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/download/index.rst` & `PyGreSQL-6.0b1/docs/download/index.rst`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/docs/make.bat` & `PyGreSQL-6.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgconn.c` & `PyGreSQL-6.0b1/ext/pgconn.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pginternal.c` & `PyGreSQL-6.0b1/ext/pginternal.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pglarge.c` & `PyGreSQL-6.0b1/ext/pglarge.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgmodule.c` & `PyGreSQL-6.0b1/ext/pgmodule.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgnotice.c` & `PyGreSQL-6.0b1/ext/pgnotice.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgquery.c` & `PyGreSQL-6.0b1/ext/pgquery.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgsource.c` & `PyGreSQL-6.0b1/ext/pgsource.c`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/ext/pgtypes.h` & `PyGreSQL-6.0b1/ext/pgtypes.h`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/__init__.py` & `PyGreSQL-6.0b1/pg/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/_pg.pyi` & `PyGreSQL-6.0b1/pg/_pg.pyi`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/adapt.py` & `PyGreSQL-6.0b1/pg/adapt.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/attrs.py` & `PyGreSQL-6.0b1/pg/attrs.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/cast.py` & `PyGreSQL-6.0b1/pg/cast.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/core.py` & `PyGreSQL-6.0b1/pg/core.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/db.py` & `PyGreSQL-6.0b1/pg/db.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/error.py` & `PyGreSQL-6.0b1/pg/error.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/helpers.py` & `PyGreSQL-6.0b1/pg/helpers.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/notify.py` & `PyGreSQL-6.0b1/pg/notify.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pg/tz.py` & `PyGreSQL-6.0b1/pg/tz.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/__init__.py` & `PyGreSQL-6.0b1/pgdb/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/adapt.py` & `PyGreSQL-6.0b1/pgdb/adapt.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/cast.py` & `PyGreSQL-6.0b1/pgdb/cast.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/connect.py` & `PyGreSQL-6.0b1/pgdb/connect.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/connection.py` & `PyGreSQL-6.0b1/pgdb/connection.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/cursor.py` & `PyGreSQL-6.0b1/pgdb/cursor.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pgdb/typecode.py` & `PyGreSQL-6.0b1/pgdb/typecode.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/pyproject.toml` & `PyGreSQL-6.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyGreSQL"
-version = "6.0"
+version = "6.0b1"
 requires-python = ">=3.7"
 authors = [
   {name = "D'Arcy J. M. Cain", email = "darcy@pygresql.org"},
   {name = "Christoph Zwerschke", email = "cito@online.de"},
 ]
 description = "Python PostgreSQL interfaces"
 readme = "README.rst"
@@ -29,21 +29,21 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.urls]
-Homepage = "https://pygresql.github.io/"
-Documentation = "https://pygresql.github.io/contents/"
-"Source Code" = "https://github.com/PyGreSQL/PyGreSQL"
-"Issue Tracker" = "https://github.com/PyGreSQL/PyGreSQL/issues/"
-Changelog = "https://pygresql.github.io/contents/changelog.html"
-Download = "https://pygresql.github.io/download/"
-"Mailing List" = "https://mail.vex.net/mailman/listinfo/pygresql"
+homepage = "https://pygresql.github.io/"
+documentation = "https://pygresql.github.io/contents/"
+source = "https://github.com/PyGreSQL/PyGreSQL"
+issues = "https://github.com/PyGreSQL/PyGreSQL/issues/"
+changelog = "https://pygresql.github.io/contents/changelog.html"
+download = "https://pygresql.github.io/download/"
+"mailing list" = "https://mail.vex.net/mailman/listinfo/pygresql"
 
 [tool.ruff]
 target-version = "py37"
 line-length = 79
 select = [
   "E",   # pycodestyle
   "F",   # pyflakes
```

### Comparing `PyGreSQL-6.0/setup.py` & `PyGreSQL-6.0b1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,39 +15,22 @@
 import warnings
 from distutils.ccompiler import get_default_compiler
 from distutils.sysconfig import get_python_inc, get_python_lib
 
 from setuptools import Extension, setup
 from setuptools.command.build_ext import build_ext
 
-
-def project_version():
-    """Read the PyGreSQL version from the pyproject.toml file."""
-    with open('pyproject.toml') as f:
-        for d in f:
-            if d.startswith("version ="):
-                version = d.split("=")[1].strip().strip('"')
-                return version
-    raise Exception("Cannot determine PyGreSQL version")
-
-
-def project_readme():
-    """Get the content of the README file."""
-    with open('README.rst') as f:
-        return f.read()
-
-
-version = project_version()
+version = '6.0b1'
 
 if not (3, 7) <= sys.version_info[:2] < (4, 0):
     raise Exception(
         f"Sorry, PyGreSQL {version} does not support this Python version")
 
-long_description = project_readme()
-
+with open('README.rst') as f:
+    long_description = f.read()
 
 # For historical reasons, PyGreSQL does not install itself as a single
 # "pygresql" package, but as two top-level modules "pg", providing the
 # classic interface, and "pgdb" for the modern DB-API 2.0 interface.
 # These two top-level Python modules share the same C extension "_pg".
 
 def pg_config(s):
@@ -146,15 +129,15 @@
     description='Python PostgreSQL Interfaces',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     keywords='pygresql postgresql database api dbapi',
     author="D'Arcy J. M. Cain",
     author_email="darcy@PyGreSQL.org",
     url='https://pygresql.github.io/',
-    download_url='https://pygresql.github.io/download/',
+    download_url='https://pygresql.github.io/contents/download/',
     project_urls={
         'Documentation': 'https://pygresql.github.io/contents/',
         'Issue Tracker': 'https://github.com/PyGreSQL/PyGreSQL/issues/',
         'Mailing List': 'https://mail.vex.net/mailman/listinfo/pygresql',
         'Source Code': 'https://github.com/PyGreSQL/PyGreSQL'},
     classifiers=[
         'Development Status :: 6 - Mature',
```

### Comparing `PyGreSQL-6.0/tests/config.py` & `PyGreSQL-6.0b1/tests/config.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/dbapi20.py` & `PyGreSQL-6.0b1/tests/dbapi20.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_classic.py` & `PyGreSQL-6.0b1/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_classic_attrdict.py` & `PyGreSQL-6.0b1/tests/test_classic_attrdict.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_classic_connection.py` & `PyGreSQL-6.0b1/tests/test_classic_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,18 +191,17 @@
         ssl_in_use = self.connection.ssl_in_use
         self.assertIsInstance(ssl_in_use, bool)
         self.assertFalse(ssl_in_use)
 
     def test_attribute_ssl_attributes(self):
         ssl_attributes = self.connection.ssl_attributes
         self.assertIsInstance(ssl_attributes, dict)
-        if ssl_attributes:
-            self.assertEqual(ssl_attributes, {
-                'cipher': None, 'compression': None, 'key_bits': None,
-                'library': None, 'protocol': None})
+        self.assertEqual(ssl_attributes, {
+            'cipher': None, 'compression': None, 'key_bits': None,
+            'library': None, 'protocol': None})
 
     def test_attribute_status(self):
         status_ok = 1
         self.assertIsInstance(self.connection.status, int)
         self.assertEqual(self.connection.status, status_ok)
 
     def test_attribute_user(self):
```

### Comparing `PyGreSQL-6.0/tests/test_classic_dbwrapper.py` & `PyGreSQL-6.0b1/tests/test_classic_dbwrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,18 +186,17 @@
         ssl_in_use = self.db.ssl_in_use
         self.assertIsInstance(ssl_in_use, bool)
         self.assertFalse(ssl_in_use)
 
     def test_attribute_ssl_attributes(self):
         ssl_attributes = self.db.ssl_attributes
         self.assertIsInstance(ssl_attributes, dict)
-        if ssl_attributes:
-            self.assertEqual(ssl_attributes, {
-                'cipher': None, 'compression': None, 'key_bits': None,
-                'library': None, 'protocol': None})
+        self.assertEqual(ssl_attributes, {
+            'cipher': None, 'compression': None, 'key_bits': None,
+            'library': None, 'protocol': None})
 
     def test_attribute_status(self):
         status_ok = 1
         status = self.db.status
         self.assertIsInstance(status, int)
         self.assertEqual(status, status_ok)
         self.assertEqual(status, self.db.db.status)
```

### Comparing `PyGreSQL-6.0/tests/test_classic_functions.py` & `PyGreSQL-6.0b1/tests/test_classic_functions.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_classic_largeobj.py` & `PyGreSQL-6.0b1/tests/test_classic_largeobj.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_classic_notification.py` & `PyGreSQL-6.0b1/tests/test_classic_notification.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_dbapi20.py` & `PyGreSQL-6.0b1/tests/test_dbapi20.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_dbapi20_copy.py` & `PyGreSQL-6.0b1/tests/test_dbapi20_copy.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tests/test_tutorial.py` & `PyGreSQL-6.0b1/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `PyGreSQL-6.0/tox.ini` & `PyGreSQL-6.0b1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # config file for tox
 
 [tox]
 envlist = py3{7,8,9,10,11,12},ruff,mypy,cformat,docs
 
 [testenv:ruff]
 basepython = python3.11
-deps = ruff>=0.0.292
+deps = ruff>=0.0.287
 commands =
     ruff setup.py pg pgdb tests
 
 [testenv:mypy]
 basepython = python3.11
 deps = mypy>=1.5.1
 commands =
@@ -29,16 +29,16 @@
 commands =
     sphinx-build -b html -nEW docs docs/_build/html
 
 [testenv:build]
 basepython = python3.11
 deps =
     setuptools>=68
-    wheel>=0.41,<1
-    build>=1,<2
+    wheel>=0.41
+    build>=0.10
 commands =
     python -m build -s -n -C strict -C memory-size
 
 [testenv:coverage]
 basepython = python3.11
 deps =
     coverage>=7,<8
@@ -46,12 +46,10 @@
     coverage run -m unittest discover
     coverage html
 
 [testenv]
 passenv =
     PG*
     PYGRESQL_*
-deps =
-    setuptools>=68
 commands =
     python setup.py clean --all build_ext --force --inplace --strict --memory-size
     python -m unittest {posargs:discover}
```

