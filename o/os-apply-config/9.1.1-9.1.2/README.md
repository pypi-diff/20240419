# Comparing `tmp/os-apply-config-9.1.1.tar.gz` & `tmp/os-apply-config-9.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/os-apply-config-9.1.1.tar", last modified: Thu Mar 14 10:46:04 2019, max compression
+gzip compressed data, was "dist/os-apply-config-9.1.2.tar", last modified: Fri Jun 21 13:51:10 2019, max compression
```

## Comparing `os-apply-config-9.1.1.tar` & `os-apply-config-9.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      323 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4789 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      780 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6633 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1469 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/AUTHORS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/setup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      112 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/MANIFEST.in
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/test-requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      957 2019-03-14 10:44:15.000000 os-apply-config-9.1.1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1377 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/test_json_renderer.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17248 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/test_apply_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/glance/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      192 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/glance/script.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/keystone/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       34 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/keystone/keystone.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/allow_empty
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/mode
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        4 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/empty
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       19 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/allow_empty.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/empty.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/templates/etc/control/mode.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2920 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/test_oac_file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6275 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/test_value_type.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/owner.uid
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/group.gid
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/group.name
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/group.name.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        9 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/owner.uid.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        9 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/group.gid.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/owner.name.oac
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/chown_templates/owner.name
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5161 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/tests/test_collect_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1517 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/renderers.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1604 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/value_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/__init__.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    14298 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/apply_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2464 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/collect_config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4314 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/oac_file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      655 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/config_exception.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      717 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/os_apply_config/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      551 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7310 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/zuul.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      390 2019-03-14 10:44:15.000000 os-apply-config-9.1.1/zuul.d/layout.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6633 2019-03-14 10:46:04.000000 os-apply-config-9.1.1/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      135 2019-03-14 10:44:12.000000 os-apply-config-9.1.1/.coveragerc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/zuul.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      390 2019-06-21 13:48:01.000000 os-apply-config-9.1.2/zuul.d/layout.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/setup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      112 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/MANIFEST.in
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      135 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/.coveragerc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1604 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/value_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      717 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/version.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)    14298 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/apply_config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      655 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/config_exception.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1564 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/renderers.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4314 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/oac_file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2464 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/collect_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17467 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/test_apply_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/keystone/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       34 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/keystone/keystone.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/glance/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      192 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/glance/script.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        4 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/empty
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/empty.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/mode
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/allow_empty
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/mode.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       19 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/templates/etc/control/allow_empty.oac
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/group.gid
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/owner.name
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        9 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/group.gid.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/owner.name.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       12 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/group.name.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       11 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/owner.uid
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        9 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/owner.uid.oac
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       10 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/chown_templates/group.name
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5161 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/test_collect_config.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6275 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/test_value_type.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1377 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/test_json_renderer.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2920 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/os_apply_config/tests/test_oac_file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       56 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/AUTHORS
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/LICENSE
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      957 2019-06-21 13:48:01.000000 os-apply-config-9.1.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       16 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/os_apply_config.egg-info/top_level.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      500 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/test-requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      323 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4793 2019-06-21 13:48:01.000000 os-apply-config-9.1.2/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7430 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/ChangeLog
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      551 2019-06-21 13:47:52.000000 os-apply-config-9.1.2/lower-constraints.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      780 2019-06-21 13:51:10.000000 os-apply-config-9.1.2/setup.cfg
```

### Comparing `os-apply-config-9.1.1/README.rst` & `os-apply-config-9.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,14 @@
 
 
 Quick Start
 ===========
 ::
 
    # install it
-   sudo pip install -U git+git://git.openstack.org/openstack/os-apply-config.git
+   sudo pip install -U git+https://git.openstack.org/openstack/os-apply-config.git
 
    # grab example templates
-   git clone git://git.openstack.org/openstack/tripleo-image-elements /tmp/config
+   git clone https://git.openstack.org/openstack/tripleo-image-elements /tmp/config
 
    # run it
    os-apply-config -t /tmp/config/elements/nova/os-apply-config/ -m /tmp/config/elements/seed-stack-config/config.json -o /tmp/config_output
```

### Comparing `os-apply-config-9.1.1/setup.cfg` & `os-apply-config-9.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config.egg-info/SOURCES.txt` & `os-apply-config-9.1.2/os_apply_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config.egg-info/PKG-INFO` & `os-apply-config-9.1.2/os_apply_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-apply-config
-Version: 9.1.1
+Version: 9.1.2
 Summary: Config files from cloud metadata
 Home-page: http://git.openstack.org/cgit/openstack/os-apply-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -143,18 +143,18 @@
         
         
         Quick Start
         ===========
         ::
         
            # install it
-           sudo pip install -U git+git://git.openstack.org/openstack/os-apply-config.git
+           sudo pip install -U git+https://git.openstack.org/openstack/os-apply-config.git
         
            # grab example templates
-           git clone git://git.openstack.org/openstack/tripleo-image-elements /tmp/config
+           git clone https://git.openstack.org/openstack/tripleo-image-elements /tmp/config
         
            # run it
            os-apply-config -t /tmp/config/elements/nova/os-apply-config/ -m /tmp/config/elements/seed-stack-config/config.json -o /tmp/config_output
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `os-apply-config-9.1.1/AUTHORS` & `os-apply-config-9.1.2/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Coleman Corrigan <coleman.corrigan@hp.com>
 Dan Prince <dprince@redhat.com>
 Derek Higgins <derekh@redhat.com>
 Doug Hellmann <doug@doughellmann.com>
 Emilien Macchi <emilien@redhat.com>
 Flavio Percoco <flaper87@gmail.com>
 Ghe Rivero <ghe.rivero@hp.com>
+Ian Wienand <iwienand@redhat.com>
 JUN JIE NAN <nanjj@cn.ibm.com>
 James E. Blair <jeblair@openstack.org>
 James E. Blair <jeblair@redhat.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Jonathan Brownell <brownell@hp.com>
 Matthew Flusche <mflusche@redhat.com>
 Monty Taylor <mordred@inaugust.com>
@@ -31,10 +32,11 @@
 Steve Kowalik <steven@wedontsleep.org>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
 Tim Miller <tim.miller.0@gmail.com>
 Tomas Sedovic <tsedovic@redhat.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
 XiaojueGuan <guanalbertjone@gmail.com>
+Zane Bitter <zbitter@redhat.com>
 gecong1973 <ge.cong@zte.com.cn>
 rbtcollins <robertc@robertcollins.net>
 ricolin <rico.lin@easystack.cn>
```

### Comparing `os-apply-config-9.1.1/setup.py` & `os-apply-config-9.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/tox.ini` & `os-apply-config-9.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/tests/test_json_renderer.py` & `os-apply-config-9.1.2/os_apply_config/tests/test_json_renderer.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/tests/test_apply_config.py` & `os-apply-config-9.1.2/os_apply_config/tests/test_apply_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,19 @@
         self.assertEqual(
             "ab123cd",
             apply_config.render_moustache("ab{{x.a}}cd", {"x": {"a": "123"}}))
 
     def test_render_moustache_bad_key(self):
         self.assertEqual(u'', apply_config.render_moustache("{{badkey}}", {}))
 
+    def test_render_moustache_none(self):
+        self.assertEqual('foo: ',
+                         apply_config.render_moustache("foo: {{foo}}",
+                                                       {'foo': None}))
+
     def test_render_executable(self):
         params = {"x": "foo"}
         self.assertEqual("foo\n", apply_config.render_executable(
             template("/etc/glance/script.conf"), params))
 
     def test_render_executable_failure(self):
         self.assertRaises(
```

### Comparing `os-apply-config-9.1.1/os_apply_config/tests/test_oac_file.py` & `os-apply-config-9.1.2/os_apply_config/tests/test_oac_file.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/tests/test_value_type.py` & `os-apply-config-9.1.2/os_apply_config/tests/test_value_type.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/tests/test_collect_config.py` & `os-apply-config-9.1.2/os_apply_config/tests/test_collect_config.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/renderers.py` & `os-apply-config-9.1.2/os_apply_config/renderers.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,8 +34,10 @@
         return super(JsonRenderer, self).__init__(file_encoding,
                                                   string_encoding,
                                                   decode_errors, search_dirs,
                                                   file_extension, escape,
                                                   partials, missing_tags)
 
     def str_coerce(self, val):
+        if val is None:
+            return b''
         return json.dumps(val)
```

### Comparing `os-apply-config-9.1.1/os_apply_config/value_types.py` & `os-apply-config-9.1.2/os_apply_config/value_types.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/apply_config.py` & `os-apply-config-9.1.2/os_apply_config/apply_config.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/collect_config.py` & `os-apply-config-9.1.2/os_apply_config/collect_config.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/oac_file.py` & `os-apply-config-9.1.2/os_apply_config/oac_file.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/config_exception.py` & `os-apply-config-9.1.2/os_apply_config/config_exception.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/os_apply_config/version.py` & `os-apply-config-9.1.2/os_apply_config/version.py`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/lower-constraints.txt` & `os-apply-config-9.1.2/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/ChangeLog` & `os-apply-config-9.1.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+9.1.2
+-----
+
+* Don't render None as "null"
+* OpenDev Migration Patch
+* Replace openstack.org git:// URLs with https://
+
 9.1.1
 -----
 
 * import zuul job settings from project-config
 * Update UPPER\_CONSTRAINTS\_FILE for stable/rocky
 * Update .gitreview for stable/rocky
```

### Comparing `os-apply-config-9.1.1/LICENSE` & `os-apply-config-9.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os-apply-config-9.1.1/PKG-INFO` & `os-apply-config-9.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: os-apply-config
-Version: 9.1.1
+Version: 9.1.2
 Summary: Config files from cloud metadata
 Home-page: http://git.openstack.org/cgit/openstack/os-apply-config
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -143,18 +143,18 @@
         
         
         Quick Start
         ===========
         ::
         
            # install it
-           sudo pip install -U git+git://git.openstack.org/openstack/os-apply-config.git
+           sudo pip install -U git+https://git.openstack.org/openstack/os-apply-config.git
         
            # grab example templates
-           git clone git://git.openstack.org/openstack/tripleo-image-elements /tmp/config
+           git clone https://git.openstack.org/openstack/tripleo-image-elements /tmp/config
         
            # run it
            os-apply-config -t /tmp/config/elements/nova/os-apply-config/ -m /tmp/config/elements/seed-stack-config/config.json -o /tmp/config_output
         
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

