# Comparing `tmp/os-collect-config-9.2.0.tar.gz` & `tmp/os-collect-config-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/os-collect-config-9.2.0.tar", last modified: Fri Aug 24 14:53:15 2018, max compression
+gzip compressed data, was "dist/os-collect-config-9.2.1.tar", last modified: Thu Mar 14 10:43:37 2019, max compression
```

## Comparing `os-collect-config-9.2.0.tar` & `os-collect-config-9.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      798 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/setup.cfg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2282 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/AUTHORS
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/os_collect_config/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       40 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/common.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3944 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/heat.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/local.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6463 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/zaqar.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2862 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/ec2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/os_collect_config/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5853 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_ec2.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10447 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_zaqar.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3429 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5536 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_local.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7555 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_request.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3339 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_heat_local.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3727 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_cache.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7585 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_heat.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3085 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_merger.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5443 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_config_drive.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24609 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_collect.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10611 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/tests/test_cfn.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5885 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/cfn.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1713 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/merger.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      719 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4760 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/keystone.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1909 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/heat_local.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3184 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/request.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2635 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/cache.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5467 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/config_drive.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2075 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/exc.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12326 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os_collect_config/collect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      610 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12843 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os-collect-config-and-friends.odg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/os_collect_config.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/os_collect_config.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/os_collect_config.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-08-24 14:52:59.000000 os-collect-config-9.2.0/os_collect_config.egg-info/not-zip-safe
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       94 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/MANIFEST.in
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      962 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-08-24 14:53:15.000000 os-collect-config-9.2.0/zuul.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      115 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/zuul.d/layout.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/LICENSE
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/.coveragerc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22264 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/os-collect-config-and-friends.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11254 2018-08-24 14:53:14.000000 os-collect-config-9.2.0/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2018-08-24 14:50:03.000000 os-collect-config-9.2.0/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      610 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2282 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      798 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1707 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/AUTHORS
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/setup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       94 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/MANIFEST.in
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config.egg-info/requires.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/test-requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      977 2019-03-14 10:40:57.000000 os-collect-config-9.2.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/os_collect_config/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5536 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_local.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5443 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_config_drive.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7585 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_heat.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5853 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_ec2.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    24609 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_collect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3085 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_merger.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3727 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_cache.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7555 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_request.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10611 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_cfn.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10447 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_zaqar.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3339 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_heat_local.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3429 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/tests/test_keystone.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4760 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/keystone.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/local.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6463 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/zaqar.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1713 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/merger.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2635 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/cache.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3944 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/heat.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2075 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/exc.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5885 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/cfn.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2862 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/ec2.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12486 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/collect.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1909 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/heat_local.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       40 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/common.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3184 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/request.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5467 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/config_drive.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      719 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os_collect_config/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11426 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/ChangeLog
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/LICENSE
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12843 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os-collect-config-and-friends.odg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/zuul.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      284 2019-03-14 10:40:57.000000 os-collect-config-9.2.1/zuul.d/layout.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    22264 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/os-collect-config-and-friends.svg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       58 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2019-03-14 10:43:37.000000 os-collect-config-9.2.1/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      141 2019-03-14 10:40:53.000000 os-collect-config-9.2.1/.coveragerc
```

### Comparing `os-collect-config-9.2.0/setup.cfg` & `os-collect-config-9.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/README.rst` & `os-collect-config-9.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/AUTHORS` & `os-collect-config-9.2.1/AUTHORS`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 Jeremy Stanley <fungi@yuggoth.org>
 John Trowbridge <trown@redhat.com>
 Lukas Bezdicka <lbezdick@redhat.com>
 Mark McLoughlin <markmc@redhat.com>
 Monty Taylor <mordred@inaugust.com>
 Motohiro OTSUKA <ootsuka@mxs.nes.nec.co.jp>
 Ondřej Nový <ondrej.novy@firma.seznam.cz>
+OpenStack Release Bot <infra-root@openstack.org>
 Robert Collins <rbtcollins@hp.com>
 Roman Podoliaka <rpodolyaka@mirantis.com>
 Sagi Shnaidman <sshnaidm@redhat.com>
 Sascha Peilicke <speilicke@suse.com>
 Steve Baker <sbaker@redhat.com>
 Steve Kowalik <steven@wedontsleep.org>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Thomas Herve <therve@redhat.com>
 Thomas Herve <thomas.herve@enovance.com>
 Tim Miller <tim.miller.0@gmail.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 Yanyan Hu <yanyanhu@cn.ibm.com>
-Zuul <zuul@review.openstack.org>
 gecong1973 <ge.cong@zte.com.cn>
 huang.zhiping <huang.zhiping@99cloud.net>
 melissaml <ma.lei@99cloud.net>
 rbtcollins <robertc@robertcollins.net>
 ricolin <rico.lin@easystack.cn>
```

### Comparing `os-collect-config-9.2.0/os_collect_config/heat.py` & `os-collect-config-9.2.1/os_collect_config/heat.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/local.py` & `os-collect-config-9.2.1/os_collect_config/local.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/zaqar.py` & `os-collect-config-9.2.1/os_collect_config/zaqar.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/ec2.py` & `os-collect-config-9.2.1/os_collect_config/ec2.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_ec2.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_ec2.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_zaqar.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_zaqar.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_keystone.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_keystone.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_local.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_request.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_heat_local.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_heat_local.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_cache.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_heat.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_heat.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_merger.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_config_drive.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_config_drive.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_collect.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/tests/test_cfn.py` & `os-collect-config-9.2.1/os_collect_config/tests/test_cfn.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/cfn.py` & `os-collect-config-9.2.1/os_collect_config/cfn.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/merger.py` & `os-collect-config-9.2.1/os_collect_config/merger.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/version.py` & `os-collect-config-9.2.1/os_collect_config/version.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/keystone.py` & `os-collect-config-9.2.1/os_collect_config/keystone.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/heat_local.py` & `os-collect-config-9.2.1/os_collect_config/heat_local.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/request.py` & `os-collect-config-9.2.1/os_collect_config/request.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/cache.py` & `os-collect-config-9.2.1/os_collect_config/cache.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/config_drive.py` & `os-collect-config-9.2.1/os_collect_config/config_drive.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/exc.py` & `os-collect-config-9.2.1/os_collect_config/exc.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config/collect.py` & `os-collect-config-9.2.1/os_collect_config/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -237,14 +237,17 @@
         except IOError:
             pass
     return m.hexdigest()
 
 
 def __main__(args=sys.argv, collector_kwargs_map=None):
     signal.signal(signal.SIGHUP, reexec_self)
+    # NOTE(bnemec): We need to exit on SIGPIPEs so systemd can restart us.
+    #               See lp 1795030
+    signal.signal(signal.SIGPIPE, signal.SIG_DFL)
     setup_conf()
     CONF(args=args[1:], prog="os-collect-config",
          version=version.version_info.version_string())
 
     # This resets the logging infrastructure which prevents capturing log
     # output in tests cleanly, so should only be called if there isn't already
     # handlers defined i.e. not in unit tests
```

### Comparing `os-collect-config-9.2.0/PKG-INFO` & `os-collect-config-9.2.1/os_collect_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-collect-config
-Version: 9.2.0
+Version: 9.2.1
 Summary: Collect and cache metadata, run hooks on changes.
 Home-page: http://git.openstack.org/cgit/openstack/os-collect-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os-collect-config-9.2.0/requirements.txt` & `os-collect-config-9.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os-collect-config-and-friends.odg` & `os-collect-config-9.2.1/os-collect-config-and-friends.odg`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os_collect_config.egg-info/PKG-INFO` & `os-collect-config-9.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-collect-config
-Version: 9.2.0
+Version: 9.2.1
 Summary: Collect and cache metadata, run hooks on changes.
 Home-page: http://git.openstack.org/cgit/openstack/os-collect-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `os-collect-config-9.2.0/os_collect_config.egg-info/SOURCES.txt` & `os-collect-config-9.2.1/os_collect_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/setup.py` & `os-collect-config-9.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/tox.ini` & `os-collect-config-9.2.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 skipsdist = True
 envlist = py35,py27,pep8
 
 [testenv]
 usedevelop = True
 install_command = pip install {opts} {packages}
 deps =
-       -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt}
+       -c{env:UPPER_CONSTRAINTS_FILE:https://git.openstack.org/cgit/openstack/requirements/plain/upper-constraints.txt?h=stable/rocky}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 commands =
   stestr run --slowest {posargs}
 
 [tox:jenkins]
 sitepackages = True
```

### Comparing `os-collect-config-9.2.0/LICENSE` & `os-collect-config-9.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/os-collect-config-and-friends.svg` & `os-collect-config-9.2.1/os-collect-config-and-friends.svg`

 * *Files identical despite different names*

### Comparing `os-collect-config-9.2.0/ChangeLog` & `os-collect-config-9.2.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+9.2.1
+-----
+
+* Don't ignore SIGPIPE
+* import zuul job settings from project-config
+* Update UPPER\_CONSTRAINTS\_FILE for stable/rocky
+* Update .gitreview for stable/rocky
+
 9.2.0
 -----
 
 
 9.1.0
 -----
```

