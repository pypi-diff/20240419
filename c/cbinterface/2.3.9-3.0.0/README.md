# Comparing `tmp/cbinterface-2.3.9.tar.gz` & `tmp/cbinterface-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cbinterface-2.3.9.tar", last modified: Mon Apr 19 14:54:10 2021, max compression
+gzip compressed data, was "cbinterface-3.0.0.tar", last modified: Fri Apr 19 19:09:25 2024, max compression
```

## Comparing `cbinterface-2.3.9.tar` & `cbinterface-3.0.0.tar`

### file list

```diff
@@ -1,78 +1,39 @@
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/bin/
--rwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)      242 2021-03-14 18:50:56.000000 cbinterface-2.3.9/bin/cbinterface
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/tests/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)        0 2021-01-24 04:43:50.000000 cbinterface-2.3.9/tests/__init__.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     3941 2021-03-02 22:08:16.000000 cbinterface-2.3.9/tests/test_cbinterface_psc.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2947 2021-04-19 14:53:05.000000 cbinterface-2.3.9/tests/test_cbinterface.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    12950 2021-04-11 12:53:56.000000 cbinterface-2.3.9/tests/test_cbinterface_response.py
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/tests/test_data/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      594 2021-03-12 00:35:52.000000 cbinterface-2.3.9/tests/test_data/playbooking.around.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      556 2021-02-16 20:50:39.000000 cbinterface-2.3.9/tests/test_data/netconns.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     4048 2021-02-16 20:52:57.000000 cbinterface-2.3.9/tests/test_data/regmods.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      323 2021-02-16 21:19:19.000000 cbinterface-2.3.9/tests/test_data/ancestry_str.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     4254 2021-02-13 22:19:29.000000 cbinterface-2.3.9/tests/test_data/cb_response_server_info.json
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    43531 2021-02-16 17:02:44.000000 cbinterface-2.3.9/tests/test_data/00007c6f-0000-0a28-01d6-ffde20451832.json
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      654 2021-02-16 20:54:31.000000 cbinterface-2.3.9/tests/test_data/crossprocs.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2037 2021-02-14 00:25:15.000000 cbinterface-2.3.9/tests/test_data/facet_data.json
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1100 2021-02-16 20:49:05.000000 cbinterface-2.3.9/tests/test_data/filemods.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     7513 2021-02-16 20:53:48.000000 cbinterface-2.3.9/tests/test_data/modloads.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      356 2021-03-12 00:41:34.000000 cbinterface-2.3.9/tests/test_data/remediating.around.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      149 2021-02-16 17:04:33.000000 cbinterface-2.3.9/tests/test_data/process_tree_str.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      708 2021-02-16 21:18:07.000000 cbinterface-2.3.9/tests/test_data/printed_process_info.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      189 2021-02-22 19:11:06.000000 cbinterface-2.3.9/tests/test_data/children.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    50790 2021-03-02 22:03:51.000000 cbinterface-2.3.9/tests/test_data/H8NDJUE1-02361dc7-000009d4-00000000-1d70b8a6f55bfa7.json
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2918 2021-02-14 00:25:15.000000 cbinterface-2.3.9/tests/test_data/facet_data_output.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    40931 2021-03-24 19:48:07.000000 cbinterface-2.3.9/README.md
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     4796 2021-04-02 20:47:02.000000 cbinterface-2.3.9/cbinterface/helpers.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       22 2021-04-19 14:52:57.000000 cbinterface-2.3.9/cbinterface/__init__.py
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/playbook_configs/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1154 2021-03-14 18:55:55.000000 cbinterface-2.3.9/cbinterface/playbook_configs/collect_browsing_history.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1297 2021-04-06 20:44:25.000000 cbinterface-2.3.9/cbinterface/playbook_configs/force_restart.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      723 2021-03-14 20:13:51.000000 cbinterface-2.3.9/cbinterface/playbook_configs/delete_directory.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      410 2021-03-10 23:39:38.000000 cbinterface-2.3.9/cbinterface/playbook_configs/collect_scheduled_tasks.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      620 2021-03-14 20:14:08.000000 cbinterface-2.3.9/cbinterface/playbook_configs/delete_scheduled_task.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      674 2021-03-14 20:14:30.000000 cbinterface-2.3.9/cbinterface/playbook_configs/delete_service.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     4422 2021-04-16 13:43:36.000000 cbinterface-2.3.9/cbinterface/config.py
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/psc/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     8574 2021-04-04 03:03:53.000000 cbinterface-2.3.9/cbinterface/psc/ubs.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)        0 2021-03-02 21:38:51.000000 cbinterface-2.3.9/cbinterface/psc/__init__.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     9537 2021-04-08 16:27:07.000000 cbinterface-2.3.9/cbinterface/psc/query.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    18448 2021-04-15 21:04:25.000000 cbinterface-2.3.9/cbinterface/psc/process.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    27468 2021-04-16 01:56:16.000000 cbinterface-2.3.9/cbinterface/psc/intel.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    12431 2021-03-24 19:48:07.000000 cbinterface-2.3.9/cbinterface/psc/sessions.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     3959 2021-03-09 05:55:47.000000 cbinterface-2.3.9/cbinterface/psc/device.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    37412 2021-04-15 21:04:25.000000 cbinterface-2.3.9/cbinterface/psc/cli.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2055 2021-04-02 20:47:02.000000 cbinterface-2.3.9/cbinterface/psc/enumerations.py
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/response/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2344 2021-04-02 19:45:49.000000 cbinterface-2.3.9/cbinterface/response/query.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    13876 2021-04-12 18:53:34.000000 cbinterface-2.3.9/cbinterface/response/process.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     3328 2021-03-10 19:19:22.000000 cbinterface-2.3.9/cbinterface/response/sensor.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    11939 2021-03-24 19:48:07.000000 cbinterface-2.3.9/cbinterface/response/sessions.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    20363 2021-04-11 12:30:43.000000 cbinterface-2.3.9/cbinterface/response/cli.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1605 2021-03-10 20:11:43.000000 cbinterface-2.3.9/cbinterface/response/enumerations.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1472 2021-04-02 20:47:02.000000 cbinterface-2.3.9/cbinterface/response/watchlists.py
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/templates/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2647 2021-03-14 19:54:30.000000 cbinterface-2.3.9/cbinterface/templates/playbook.ini
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1566 2021-03-13 23:54:29.000000 cbinterface-2.3.9/cbinterface/templates/remediate.ini
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface/tools/
--rwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)     2521 2021-04-02 20:47:02.000000 cbinterface-2.3.9/cbinterface/tools/chromium_history_parser.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)      952 2021-03-09 04:04:27.000000 cbinterface-2.3.9/cbinterface/tools/get_chromium_browsing_data.bat
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    15204 2021-04-02 20:47:03.000000 cbinterface-2.3.9/cbinterface/scripted_live_response.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    17531 2021-04-11 12:29:21.000000 cbinterface-2.3.9/cbinterface/cli.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    24030 2021-04-08 23:31:56.000000 cbinterface-2.3.9/cbinterface/commands.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       38 2021-04-19 14:54:10.000000 cbinterface-2.3.9/setup.cfg
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    49842 2021-04-19 14:54:10.000000 cbinterface-2.3.9/PKG-INFO
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1663 2021-04-03 21:43:08.000000 cbinterface-2.3.9/setup.py
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       92 2021-03-02 23:04:23.000000 cbinterface-2.3.9/.gitignore
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       51 2021-03-02 22:45:40.000000 cbinterface-2.3.9/requirements.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    11342 2021-02-10 12:20:43.000000 cbinterface-2.3.9/LICENSE
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     1090 2021-04-19 14:53:33.000000 cbinterface-2.3.9/pyproject.toml
-drwxr-xr-x   0 smcfeely (10010) cybersecurity  (7000)        0 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       51 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/requires.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)    49842 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/PKG-INFO
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       18 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/top_level.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)        1 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/dependency_links.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)     2083 2021-04-19 14:54:10.000000 cbinterface-2.3.9/cbinterface.egg-info/SOURCES.txt
--rw-r--r--   0 smcfeely (10010) cybersecurity  (7000)       43 2021-03-02 22:57:29.000000 cbinterface-2.3.9/MANIFEST.in
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.304456 cbinterface-3.0.0/
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    11342 2024-03-28 15:59:31.000000 cbinterface-3.0.0/LICENSE
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       43 2024-03-28 15:59:31.000000 cbinterface-3.0.0/MANIFEST.in
+-rw-r--r--   0 cybersecurity  (7000) cybersecurity  (7000)     2219 2024-04-19 19:09:25.304456 cbinterface-3.0.0/PKG-INFO
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     1244 2024-04-19 19:02:56.000000 cbinterface-3.0.0/README.md
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.288456 cbinterface-3.0.0/bin/
+-rwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)      242 2024-03-28 15:59:31.000000 cbinterface-3.0.0/bin/cbinterface
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.292456 cbinterface-3.0.0/cbinterface/
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       22 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/__init__.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    18846 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/cli.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    24118 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/commands.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     7131 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/config.py
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.300456 cbinterface-3.0.0/cbinterface/enterprise_edr/
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/__init__.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    47526 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/cli.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     7902 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/device.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     2065 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/enumerations.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    34177 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/intel.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    21507 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/process.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    15949 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/query.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    12445 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/sessions.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    12242 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/enterprise_edr/ubs.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     5119 2024-04-19 19:02:56.000000 cbinterface-3.0.0/cbinterface/helpers.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    15204 2024-03-28 15:59:31.000000 cbinterface-3.0.0/cbinterface/scripted_live_response.py
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.300456 cbinterface-3.0.0/cbinterface.egg-info/
+-rw-r--r--   0 cybersecurity  (7000) cybersecurity  (7000)     2219 2024-04-19 19:09:25.000000 cbinterface-3.0.0/cbinterface.egg-info/PKG-INFO
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)      855 2024-04-19 19:09:25.000000 cbinterface-3.0.0/cbinterface.egg-info/SOURCES.txt
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)        1 2024-04-19 19:09:25.000000 cbinterface-3.0.0/cbinterface.egg-info/dependency_links.txt
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       74 2024-04-19 19:09:25.000000 cbinterface-3.0.0/cbinterface.egg-info/requires.txt
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       18 2024-04-19 19:09:25.000000 cbinterface-3.0.0/cbinterface.egg-info/top_level.txt
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     1127 2024-04-19 19:02:56.000000 cbinterface-3.0.0/pyproject.toml
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       74 2024-04-19 19:02:56.000000 cbinterface-3.0.0/requirements.txt
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)       38 2024-04-19 19:09:25.304456 cbinterface-3.0.0/setup.cfg
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     1675 2024-04-19 19:02:56.000000 cbinterface-3.0.0/setup.py
+drwxrwxr-x   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-04-19 19:09:25.300456 cbinterface-3.0.0/tests/
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)        0 2024-03-28 15:59:31.000000 cbinterface-3.0.0/tests/__init__.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     2947 2024-03-28 15:59:31.000000 cbinterface-3.0.0/tests/test_cbinterface.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)     3905 2024-04-19 19:02:56.000000 cbinterface-3.0.0/tests/test_cbinterface_psc.py
+-rw-rw-r--   0 cybersecurity  (7000) cybersecurity  (7000)    13023 2024-03-28 15:59:31.000000 cbinterface-3.0.0/tests/test_cbinterface_response.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cbinterface-2.3.9/tests/test_cbinterface_psc.py` & `cbinterface-3.0.0/tests/test_cbinterface_psc.py`

 * *Files 13% similar despite different names*

```diff
@@ -49,69 +49,66 @@
 
 def test_dummy_process(monkeypatch):
     assert isinstance(load_dummy_process(monkeypatch), Process)
 
 
 def test_make_device_query(monkeypatch):
     from cbapi.psc.devices_query import DeviceSearchQuery
-    from cbinterface.psc.device import make_device_query
+    from cbinterface.enterprise_edr.device import make_device_query
 
     def _count(self):
         return 0
 
     cb = fake_cb_api(monkeypatch)
     monkeypatch.setattr(DeviceSearchQuery, "_count", _count)
     assert isinstance(make_device_query(cb, "name:test"), DeviceSearchQuery)
 
 
 def test_make_process_query(monkeypatch):
     from cbapi.psc.threathunter.models import AsyncProcessQuery
-    from cbinterface.psc.query import make_process_query
+    from cbinterface.enterprise_edr.query import make_process_query
 
     cb = fake_cb_api(monkeypatch)
-    assert isinstance(make_process_query(cb, "process_name:loop.exe"), AsyncProcessQuery)
+    assert isinstance(make_process_query(cb, "process_name:loop.exe", raise_exceptions=False), AsyncProcessQuery)
 
 
 def test_is_valid_process_query(monkeypatch):
     from cbapi.psc.threathunter.models import AsyncProcessQuery
-    from cbinterface.psc.query import make_process_query
-    from cbinterface.psc.query import is_valid_process_query
+    from cbinterface.enterprise_edr.query import make_process_query
+    from cbinterface.enterprise_edr.query import is_valid_process_query
 
     def _get_object(url, query_parameters):
         assert url == "/api/investigate/v1/orgs/ork_gey/processes/search_validation"
         assert query_parameters["q"] == "process_name:loop.exe"
         return {"valid": True}
 
     cb = fake_cb_api(monkeypatch)
     monkeypatch.setattr(cb, "get_object", _get_object)
-    query = make_process_query(cb, "process_name:loop.exe")
+    query = make_process_query(cb, "process_name:loop.exe", raise_exceptions=False)
     assert is_valid_process_query(query) is True
 
 
 def test_is_process_loaded(monkeypatch):
-    from cbinterface.psc.process import is_process_loaded
+    from cbinterface.enterprise_edr.process import is_process_loaded
 
     p = load_dummy_process(monkeypatch)
     assert is_process_loaded(p) is True
 
 
 def test_process_to_dict(monkeypatch, mocker):
     from cbapi.psc.threathunter.models import Event
-    from cbinterface.psc.process import process_to_dict
+    from cbinterface.enterprise_edr.process import process_to_dict
 
     data = get_dummy_process_data()
     p = load_dummy_process(monkeypatch)
 
-    def _events(self):
-        all_events = []
-        # NOTE, could use this same events HACK to allow users to parse events from json as-if from the Cb PSC.
-        for etype in p._events.keys():
-            all_events.extend(data["events"][etype])
-        return [Event(p._cb, initial_data=e) for e in all_events]
-
-    monkeypatch.setattr(Process, "events", _events)
-    mocker.patch("cbinterface.psc.process.print_ancestry", return_value=data["process_ancestry"])
-    mocker.patch("cbinterface.psc.process.print_process_tree", return_value=data["process_tree"])
+    all_events = []
+    for etype in p._events.keys():
+        all_events.extend(data["events"][etype])
+
+    mocker.patch("cbinterface.enterprise_edr.process.yield_events", return_value=all_events)
+    mocker.patch("cbinterface.enterprise_edr.process.print_ancestry", return_value=data["process_ancestry"])
+    mocker.patch("cbinterface.enterprise_edr.process.print_process_tree", return_value=data["process_tree"])
     process_dict = process_to_dict(p)
     assert isinstance(process_dict, dict)
     assert process_dict.keys() == data.keys()
     assert process_dict["events"] == data["events"]
```

### Comparing `cbinterface-2.3.9/tests/test_cbinterface.py` & `cbinterface-3.0.0/tests/test_cbinterface.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import os
 
 HOME_PATH = os.path.dirname(os.path.abspath(__file__))
 
 
 def test_version():
     from cbinterface import __version__
-    assert __version__ == "2.3.9"
+
+    assert __version__ == "2.3.33"
+
 
 def test_timezone_settings():
     from dateutil import tz
     from cbinterface.config import set_timezone, get_timezone
 
     set_timezone("GMT")
     assert "GMT" == os.environ["CBINTERFACE_TIMEZONE"]
@@ -28,41 +30,52 @@
 
     set_default_cbapi_product("buckets")
     assert get_default_cbapi_product() == "buckets"
     set_default_cbapi_product("more_buckets")
     set_default_cbapi_profile("stacks")
     assert f"{get_default_cbapi_product()}:{get_default_cbapi_profile()}" == "more_buckets:stacks"
 
+
 def test_playbook_map():
     from cbinterface.config import get_playbook_map
+
     playbook_map = get_playbook_map()
     assert isinstance(playbook_map, dict)
     playbook = list(playbook_map.values())[0]
-    assert list(playbook.keys()) == ['path', 'name', 'description']
+    assert list(playbook.keys()) == ["path", "name", "description"]
+
 
 def test_playbook_build():
     from cbinterface.scripted_live_response import build_playbook_commands
     from cbinterface.commands import GetFile, PutFile, ExecuteCommand
 
     commands = build_playbook_commands(f"{HOME_PATH}/test_data/playbooking.around.ini")
     # order matters
     assert len(commands) == 3
     assert isinstance(commands[0], PutFile)
     assert isinstance(commands[1], ExecuteCommand)
     assert isinstance(commands[2], GetFile)
 
+
 def test_remediation_script():
     from cbinterface.scripted_live_response import build_remediation_commands
-    from cbinterface.commands import ( GetFile, PutFile, ExecuteCommand, DeleteFile,
-                                       KillProcessByID, KillProcessByName,
-                                       DeleteRegistryKeyValue, DeleteRegistryKey)
+    from cbinterface.commands import (
+        GetFile,
+        PutFile,
+        ExecuteCommand,
+        DeleteFile,
+        KillProcessByID,
+        KillProcessByName,
+        DeleteRegistryKeyValue,
+        DeleteRegistryKey,
+    )
 
     cmds = build_remediation_commands(f"{HOME_PATH}/test_data/remediating.around.ini")
     assert isinstance(cmds, list)
-    #for cmd in cmds:
+    # for cmd in cmds:
     #    print(type(cmd))
     assert len(cmds) == 16
     assert isinstance(cmds[0], KillProcessByID)
     assert isinstance(cmds[1], KillProcessByName)
     assert isinstance(cmds[2], ExecuteCommand)
     assert isinstance(cmds[3], GetFile)
     assert isinstance(cmds[4], ExecuteCommand)
```

### Comparing `cbinterface-2.3.9/tests/test_cbinterface_response.py` & `cbinterface-3.0.0/tests/test_cbinterface_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,19 +173,19 @@
 
     def _get_query_results(url, query_parameters=None, default=None):
         assert url == "/api/v1/process"
         assert query_parameters == [("cb.urlver", 1), ("q", "hostname:hippo"), ("start", 0), ("rows", 0)]
         return {}
 
     cb = fake_cb_response_api(monkeypatch)
-    result = make_process_query(cb, "hostname:hippo")
+    result = make_process_query(cb, "hostname:hippo", raise_exceptions=False)
     assert isinstance(result, ProcessQuery)
-    result = make_process_query(cb, "hostname:hippo", datetime.now())
+    result = make_process_query(cb, "hostname:hippo", datetime.now(), raise_exceptions=False)
     assert isinstance(result, ProcessQuery)
-    result = make_process_query(cb, "hostname:hippo", datetime.now(), datetime.now())
+    result = make_process_query(cb, "hostname:hippo", datetime.now(), datetime.now(), raise_exceptions=False)
     assert isinstance(result, ProcessQuery)
     monkeypatch.setattr(cb, "get_object", _get_query_results)
     assert len(result) == 0
 
 
 def test_print_facet_histogram():
     from io import StringIO
@@ -362,14 +362,15 @@
 
     proc = get_process(monkeypatch)
     set_timezone("GMT")
     assert "2021-02-10 18:54:14.323000+0000" == as_configured_timezone(proc.start)
     set_timezone("US/Eastern")
     assert "2021-02-10 13:54:14.323000-0500" == as_configured_timezone(proc.start)
 
+
 """time zones change time zones
 def test_utc_offset_to_potential_tz_names():
     from datetime import timedelta
     from cbinterface.helpers import utc_offset_to_potential_tz_names
 
     zones = utc_offset_to_potential_tz_names(timedelta(hours=5, minutes=30))
     assert len(zones) == 3
```

### Comparing `cbinterface-2.3.9/cbinterface/helpers.py` & `cbinterface-3.0.0/cbinterface/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-"""Helper functions for common actions.
-"""
+"""Helper functions for common actions."""
 
-import os
 import re
 import sys
 import signal
 import logging
 import datetime
 
 from pathlib import PureWindowsPath, PurePosixPath
@@ -14,29 +12,29 @@
 from dateutil import tz
 from dateutil.parser import isoparse
 from dateutil.zoneinfo import get_zonefile_instance
 
 LOGGER = logging.getLogger("cbinterface.helpers")
 
 UUID_REGEX = re.compile(r"[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}", re.I)
-PSC_GUID_REGEX = re.compile(r"[0-9A-Z]{8}-[0-9a-f]{8}-[0-9a-f]{8}-[0-9a-f]{8}-[0-9a-f]{15}", re.I)
+EEDR_GUID_REGEX = re.compile(r"[0-9A-Z]{8}-[0-9a-f]{8}-[0-9a-f]{8}-[0-9a-f]{8}-[0-9a-f]{15}", re.I)
 
 
 def is_uuid(uuid: str):
     """Returns True if the given string matches the UUID pattern."""
     return UUID_REGEX.match(uuid)
 
 
-def is_psc_guid(guid: str):
-    """Returns True if the given string matches the format of a PSC GUID."""
-    return PSC_GUID_REGEX.match(guid)
+def is_eedr_guid(guid: str):
+    """Returns True if the given string matches the format of a EEDR GUID."""
+    return EEDR_GUID_REGEX.match(guid)
 
 
 def input_with_timeout(prompt, default=None, timeout=30, stderr=True):
-    """Wait up to timeout for user input"""
+    """Wait up to timeout for user input."""
 
     def _log_and_exit(signum, frame):
         if stderr:
             sys.stderr.write("\n")
         else:
             sys.stdout.write("\n")
         LOGGER.error("Timeout reached waiting for input.")
@@ -51,15 +49,15 @@
     answer = input() or default
     signal.alarm(0)
     return answer
 
 
 def clean_exit(signal, frame):
     print()
-    LOGGER.info(f"caught KeyboardInterrupt. exiting.")
+    LOGGER.info("caught KeyboardInterrupt. exiting.")
     sys.exit(0)
 
 
 def get_os_independent_filepath(unknown_os_file_path: str) -> Union[PureWindowsPath, PurePosixPath]:
     """Return a proper os filepath object."""
     filepath = PureWindowsPath(unknown_os_file_path)
     nixfilepath = PurePosixPath(unknown_os_file_path)
@@ -72,15 +70,15 @@
     """Convert timestamp to the configured time zone."""
     from cbinterface.config import get_timezone
 
     if not timestamp:
         return timestamp
 
     if isinstance(timestamp, str):
-        # psc
+        # enterprise edr
         try:
             timestamp = isoparse(timestamp)
         except ValueError:
             return ""
 
     if isinstance(timestamp, str):
         # legacy format
@@ -104,20 +102,21 @@
             potential_zones.append(zone)
 
     return list(sorted(potential_zones))
 
 
 def create_histogram_string(data: dict) -> str:
     """A convenience function that creates a graph in the form of a string.
+
     Args:
         data: A dictionary, where the values are integers representing a count of the keys.
+
     Returns:
         A graph in string form, pre-formatted for raw printing.
     """
-
     assert isinstance(data, dict)
     for key in data.keys():
         assert isinstance(data[key], int)
 
     total_results = sum([value for value in data.values()])
     txt = ""
 
@@ -143,7 +142,18 @@
             int(longest_key - len(r[0])) * " ",
             r[0],
             r[1],
             str(r[2])[:4],
             "\u25A0" * (int(r[2] / 2)),
         )
     return txt
+
+
+def convert_csv_data_to_dictionary(csv_data: str):
+    """Convert CSV content to a dictionary representation."""
+    import csv
+    from io import StringIO
+
+    csv_data_stream = StringIO(csv_data)
+    csvReader = csv.DictReader(csv_data_stream)
+    json_data = [dict(row) for row in csvReader]
+    return json_data
```

### Comparing `cbinterface-2.3.9/cbinterface/psc/query.py` & `cbinterface-3.0.0/cbinterface/enterprise_edr/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,196 @@
-"""Functions that work with query related Carbon Black APIs.
-"""
+"""Functions that work with query related Carbon Black APIs."""
 
+import time
 import datetime
 import logging
-from dateutil import tz
 
-from typing import Union
+from typing import Union, Dict, List
 
-# NOTE: boil everything down to CbPSCBaseAPI where possible
-# so "enterprise standard" will work wherever possible?
-# from cbapi.psc.rest_api import CbPSCBaseAPI
-from cbapi.psc.threathunter import CbThreatHunterAPI, Process
-from cbapi.psc.threathunter.models import AsyncProcessQuery
+from cbc_sdk import CBCloudAPI
+from cbc_sdk.platform.processes import AsyncProcessQuery, Process
+from cbc_sdk.errors import ServerError, ClientError, ObjectNotFoundError
+
+LOGGER = logging.getLogger("cbinterface.enterprise_edr.query")
+
+# NOTE: To receive all events, you must resubmit the search request until processed_segments is equal to total_segments.
+# https://developer.carbonblack.com/reference/carbon-black-cloud/platform/latest/platform-search-api-processes/#get-events-associated-with-a-given-process-v2
+MAX_EVENT_SEARCH_SEGMENT_EXTENSION = 10
+
+
+def create_event_search(
+    p: Union[Process, Dict],
+    search_data: Dict = {},
+    criteria: Dict = {},
+    fields: List = ["*"],
+    query: str = None,
+    time_range: Dict = {},
+    rows=1000,
+    start: int = 0,
+    sort: Dict = [{"field": "event_timestamp", "order": "asc"}],
+) -> Dict:
+    """Perform an event search.
 
-LOGGER = logging.getLogger("cbinterface.psc.query")
+    NOTE: If p is a dictionary, an instance of CBC API must be passed as "_cb".
+
+    Without anything specified, the default is to return ALL events for the process.
+    """
+    # NOTE that this one is not job based search.
+
+    cb = p.get("_cb")
+    url = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/events/{p.get('process_guid')}/_search"
+
+    if not search_data:
+        if not query:
+            query = f"process_guid:{p.get('process_guid')}"
+        search_data = {
+            "criteria": criteria,
+            "fields": fields,
+            "query": query,
+            "rows": rows,
+            "start": start,
+            "sort": sort,
+        }
+        if time_range:
+            # "time_range" = { "end": "2020-01-27T18:34:04Z", "start": "2020-01-18T18:34:04Z"}
+            search_data["time_range"] = time_range
+
+    try:
+        result = cb.post_object(url, search_data)
+        return result.json()
+    except ServerError as e:
+        LOGGER.error(f"Caught ServerError searching events: {e}")
+        return False
+    except ClientError as e:
+        LOGGER.warning(f"got ClientError searching events: {e}")
+        return False
+    except ValueError:
+        LOGGER.warning(f"got unexpected {result}")
+        return False
+
+
+def event_search_complete(cb: CBCloudAPI, job_id):
+    """Return true when a search is complete."""
+    url = f"/api/investigate/v1/orgs/{cb.credentials.org_key}/enriched_events/search_jobs/{job_id}"
+    result = cb.get_object(url)
+    if result["completed"] == result["contacted"]:
+        return True
+    return False
+
+
+def get_event_search_results(cb: CBCloudAPI, job_id) -> Dict:
+    """Return any results of an event search."""
+    url = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/enriched_events/search_jobs/{job_id}/results"
+    try:
+        while not event_search_complete(cb, job_id):
+            time.sleep(0.1)
+    except Exception as e:
+        LOGGER.error(f"got exception waiting for event search to complete: {e}")
+        return None
+    try:
+        return cb.get_object(url)
+    except Exception:
+        LOGGER.error("could not get results: {e}")
+        return None
+
+
+def yield_events(
+    p: Process,
+    search_data: Dict = {},
+    criteria: Dict = {},
+    query: str = None,
+    rows=1000,
+    start: int = 0,
+    max_results: int = None,  # limit results returned
+    start_time: datetime.datetime = None,
+    end_time: datetime.datetime = None,
+) -> Dict:
+    """Yield Process Events resulting from Event search."""
+    time_range = {}
+    if start_time:
+        time_range["start"] = start_time.isoformat()
+    if end_time:
+        time_range["end"] = end_time.isoformat()
+
+    position = start
+    still_querying = True
+    search_extension_count = 0
+    while still_querying:
+        result = create_event_search(
+            p,
+            search_data=search_data,
+            criteria=criteria,
+            query=query,
+            time_range=time_range,
+            rows=rows,
+            start=position,
+        )
+        if not result:
+            return result
+        LOGGER.debug(
+            f"got result (minus events): {[f'{key}={result[key]}' for key in result.keys() if key !='results']}"
+        )
+        if max_results and position + rows > max_results:
+            # get however many rows that may result in max_results
+            rows = max_results - position
+
+        total_results = result["num_available"]
+        if total_results != result["num_found"]:
+            LOGGER.debug("not all events are available.")
+        results = result.get("results", [])
+
+        LOGGER.debug(f"got {len(results)+position} out of {total_results} total events.")
+        for item in results:
+            yield item
+            position += 1
+            if max_results and position >= max_results:
+                still_querying = False
+                break
+        if position >= total_results:
+            if result.get("processed_segments") != result.get("total_segments"):
+                # NOTE: This can happen when CBC is bogged down, however, it also may be the process hasn't terminated.
+                # Usually this will complete on the first extension/second try.
+
+                if search_extension_count >= MAX_EVENT_SEARCH_SEGMENT_EXTENSION:
+                    still_querying = False
+                    break
+                search_extension_count += 1
+                remaining = MAX_EVENT_SEARCH_SEGMENT_EXTENSION - search_extension_count
+                LOGGER.info(
+                    f"CBC hasn't processed all segments. There could be more events. Extending search up to {remaining} more times ... "
+                )
+            else:
+                still_querying = False
+
+
+def get_process_search_jobs(cb):
+    url = f"/api/investigate/v1/orgs/{cb.credentials.org_key}/processes/search_jobs"
+    return cb.get_object(url)
+
+
+def get_process_search_status(cb, job_id):
+    url = f"/api/investigate/v1/orgs/{cb.credentials.org_key}/processes/search_jobs/{job_id}"
+    return cb.get_object(url)
+
+
+def get_process_search_results(cb, job_id):
+    url = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/processes/search_jobs/{job_id}/results"
+    return cb.get_object(url)
+
+
+def cancel_process_search(cb, job_id):
+    url = f"/api/investigate/v1/orgs/{cb.credentials.org_key}/processes/search_jobs/{job_id}"
+    return cb.delete_object(url)
 
 
 def is_valid_process_query(query: AsyncProcessQuery) -> bool:
     """Custom query validation.
 
     Args:
-        query: Cb threathunter query
+        query: CBCloudAPI query
     Returns:
         True if a valid query, else False.
     """
     if not query._doc_class.validation_url:
         LOGGER.debug("Unexpectedly, class has no validation url. hmm...")
         return True
 
@@ -35,103 +201,120 @@
         args["q"] = args["query"]
     # v2 search sort key does not work with v1 validation
     args.pop("sort", None)
     LOGGER.debug(f"attempting to validate query with args: {args}")
 
     validated = query._cb.get_object(url, query_parameters=args)
     if not validated.get("valid"):
-        LOGGER.error(f'Invalud query {validated["invalid_message"]}')
+        LOGGER.error(f'Invalid query {validated["invalid_message"]}')
         return False
     return True
 
 
-def is_valid_process_query_string(cb: CbThreatHunterAPI, query: str) -> bool:
-    """
-    Validates a process query string is valid for PSC.
+def is_valid_process_query_string(cb: CBCloudAPI, query: str) -> bool:
+    """Validates a process query string is valid for Enterprise EDR.
 
     Args:
-        cb: Cb PSC connection object
+        cb: CBCloudAPI connection object
         query (str): The query.
+
     Returns:
         True or False
     """
-    args = {"q": query}
-    url = f"/api/investigate/v1/orgs/{cb.credentials.org_key}/processes/search_validation"
-    validated = cb.get_object(url, query_parameters=args)
+    args = {"query": query}
+    url = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/processes/search_validation"
+    validated = cb.post_object(url, args).json()
     if not validated.get("valid"):
         return False
     return True
 
 
-def convert_from_legacy_query(cb: CbThreatHunterAPI, query: str) -> str:
-    """
-    Converts a legacy CB Response query to a ThreatHunter query.
+def convert_from_legacy_query(cb: CBCloudAPI, query: str) -> str:
+    """Converts a legacy CB Response (EDR) query to a Enterprise EDR query.
 
     Args:
-        cb: Cb PSC connection object
+        cb: CBCloudAPI connection object
         query (str): The query to convert.
+
     Returns:
         str: The converted query.
     """
     args = {"query": query}
-    resp = cb.post_object("/threathunter/feedmgr/v2/query/translate", args)
-    if resp.status_code != 200:
-        LOGGER.error(f"got {resp.status_code} attempting query conversion")
+    try:
+        resp = cb.post_object("/threathunter/feedmgr/v2/query/translate", args)
+    except ClientError as e:
+        LOGGER.error(f"got error attempting query conversion: {e}")
         return False
     resp = resp.json()
     return resp.get("query")
 
 
 def make_process_query(
-    cb: CbThreatHunterAPI, query: str, start_time: datetime.datetime = None, last_time: datetime.datetime = None
+    cb: CBCloudAPI,
+    query: str,
+    fields: List = ["*", "process_start_time"],
+    start_time: datetime.datetime = None,
+    last_time: datetime.datetime = None,
+    raise_exceptions=True,
+    validate_query=False,
+    silent=False,
 ) -> AsyncProcessQuery:
-    """Query the CbThreatHunterAPI environment and interface results.
+    """Query the CBCloudAPI environment and interface results.
 
     Args:
-        cb: A CbThreatHunterAPI object to use
+        cb: A CBCloudAPI object to use
         query: The process query
+        fields: fields to be included from the query.
         start_time: Set the process start time (UTC).
-        last_time: Set the process last time (UTC). Only processes with a start
-        time that falls before this last_time.
+        last_time: Set the process last time (UTC). Only processes with
+        a start time that falls before this last_time.
+        raise_exceptions: Let any exceptions raise up (library use)
+        validate_query: If True, validate the query before attempting to
+        use it.
+        silent: if True, suppress some printing from this function.
     Returns: AsyncProcessQuery or empty list.
     """
-
-    LOGGER.debug(f"buiding query: {query} between '{start_time}' and '{last_time}'")
+    LOGGER.debug(f"building query: {query} between '{start_time}' and '{last_time}'")
     processes = []
     try:
-        processes = cb.select(Process).where(query)
-        if not is_valid_process_query(processes):
+        processes = cb.select(Process).where(query).set_fields(fields)
+        if validate_query and not is_valid_process_query(processes):
             LOGGER.info(f"For help, refer to {cb.url}/#userGuideLocation=search-guide/investigate-th&fullscreen")
-            LOGGER.info(f"Is this a legacy query? ... Attempting to convert to PSC query ...")
+            LOGGER.info("Is this a legacy query? ... Attempting to convert to Enterprise EDR query ...")
             converted_query = convert_from_legacy_query(cb, query)
             if not converted_query:
-                LOGGER.info(f"failed to convert to PSC query... 🤡 your query is jacked up.")
+                LOGGER.info("failed to convert to Enterprise EDR query... 🤡 your query is jacked up.")
                 return []
             if is_valid_process_query_string(cb, converted_query):
-                LOGGER.info("successfully converted and validated the query you supplied to a PSC query 👍, see below.")
-                LOGGER.info(f"👇👇 try again with the following query 👇👇 - also, hint, single quotes are your friend. ")
+                LOGGER.info(
+                    "successfully converted and validated the query you supplied to a Enterprise EDR query 👍, see below."
+                )
+                LOGGER.info(
+                    "👇👇 try again with the following query 👇👇 - also, hint, single quotes are your friend. "
+                )
                 LOGGER.info(f"query: '{converted_query}'")
             return []
         if start_time or last_time:
             start_time = start_time.isoformat() if start_time else "*"
             end_time = last_time.isoformat() if last_time else "*"
             processes = processes.where(f"process_start_time:[{start_time} TO {end_time}]")
-        LOGGER.info(f"got {len(processes)} process results.")
+        if not silent:
+            LOGGER.info(f"got {len(processes)} process results.")
     except Exception as e:
+        if raise_exceptions:
+            raise (e)
         LOGGER.error(f"unexpected exception: {e}")
 
     return processes
 
 
 def print_facet_histogram(processes: AsyncProcessQuery):
-    """Print facets"""
-    # NOTE, this is a custom implementations. TODO, look at using the built in
-    # API methods: https://developer.carbonblack.com/reference/carbon-black-cloud/cb-threathunter/latest/process-search-v2/#start-a-process-facet-job
-    # Also, NOTE that this table lists fields that support faceting via the built in method, children is not one of them:
-    # https://developer.carbonblack.com/reference/cb-threathunter/latest/process-search-fields/
+    """Print facets."""
+    # NOTE, this is a custom implementations used before the v2
+    # Will probably be deprecated in favor of v2 using API facet job
     from cbinterface.helpers import create_histogram_string, get_os_independent_filepath
 
     fields = [
         "parent_name",
         "process_name",
         "process_reputation",
         "process_username",
@@ -150,50 +333,50 @@
                 if len(value) > 1:
                     LOGGER.info(f"condensing {value} to {value[0]}")
                 value = value[0]
             elif field_name in path_fields:
                 file_path = get_os_independent_filepath(value)
                 file_name = file_path.name
                 value = file_name
-            if value not in facet_dict[field_name]:
-                facet_dict[field_name][value] = 1
-            else:
-                facet_dict[field_name][value] += 1
+            facet_dict[field_name][value] = facet_dict[field_name].get(value, 0) + 1
 
     # special case for "children"
     try:
         facet_dict["childproc_name"] = {}
-        depth = 0
         for proc in processes:
             if proc.childproc_count < 1:
                 continue
             children = proc.summary.children or []
             for cp in children:
                 process_path = get_os_independent_filepath(cp.get("process_name"))
                 process_name = process_path.name
                 if process_name not in facet_dict["childproc_name"]:
                     facet_dict["childproc_name"][process_name] = 1
                 else:
                     facet_dict["childproc_name"][process_name] += 1
     except Exception as e:
         LOGGER.warning(f"problem enumerating child process names: {e}")
+        raise e
 
     print("\n------------------------- FACET HISTOGRAMS -------------------------")
     for field_name, facets in facet_dict.items():
         print(f"\n\t{field_name} results: {len(facets.keys())}")
         print("\t--------------------------------")
         print(create_histogram_string(facets))
     return
 
 
 def print_facet_histogram_v2(
-    cb: CbThreatHunterAPI, query: str, start_time: datetime.datetime = None, end_time: datetime.datetime = None
+    cb: CBCloudAPI,
+    query: str,
+    start_time: datetime.datetime = None,
+    end_time: datetime.datetime = None,
+    return_string=False,
 ):
-    """Get query facet results from the CbAPI enriched events facets."""
-
+    """Get query facet results from the CBCloudAPI enriched events facets."""
     # NOTE: no support for childproc facets with this built-in
 
     from cbinterface.helpers import get_os_independent_filepath
 
     post_data = {}
     post_data["query"] = query
     fields = [
@@ -205,44 +388,50 @@
         "device_name",
         "device_os",
     ]
     path_fields = ["parent_name", "process_name"]
     post_data["terms"] = {"fields": fields}
     post_data["time_range"] = {}
     if start_time:
-        post_data["time_range"]["start"] = start_time.isoformat()
+        post_data["time_range"]["start"] = start_time.isoformat() + "Z"
     if end_time:
-        post_data["time_range"]["end"] = end_time.isoformat()
-
-    # TODO handle status_code!=200 and response is not json for both requests
-
+        post_data["time_range"]["end"] = end_time.isoformat() + "Z"
     uri = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/processes/facet_jobs"
     job_id = cb.post_object(uri, post_data).json().get("job_id", None)
     if not job_id:
-        LOGGER.error(f"failed to get facet job.")
+        LOGGER.error("failed to get facet job.")
         return False
 
     uri = f"/api/investigate/v2/orgs/{cb.credentials.org_key}/processes/facet_jobs/{job_id}/results"
+    time.sleep(1)
     facet_data = cb.get_object(uri)
-
-    print("\n------------------------- FACET HISTOGRAMS -------------------------")
+    while facet_data["contacted"] != facet_data["completed"]:
+        facet_data = cb.get_object(uri)
+    txt = "\n------------------------- FACET HISTOGRAMS -------------------------\n"
     total = facet_data["num_found"]
     for facets in facet_data["terms"]:
         field_name = facets["field"]
-        print(f"\n\t{field_name} results: {len(facets['values'])}")
-        print("\t--------------------------------")
+        txt += f"\n\t{field_name} results: {len(facets['values'])}\n"
+        txt += "\t--------------------------------\n"
         for entry in facets["values"]:
             entry_name = entry["name"]
-            if field_name in path_fields and len(entry_name) > 55:
-                file_path = get_os_independent_filepath(entry_name)
-                file_name = file_path.name
-                file_path = entry_name[: len(entry_name) - len(file_name)]
-                file_path = file_path[: 40 - len(file_name)]
-                entry_name = f"{file_path}...{file_name}"
+            entry_length = 55 if field_name in path_fields else 20
+            if field_name in path_fields:
+                if len(entry_name) > 55:
+                    file_path = get_os_independent_filepath(entry_name)
+                    file_name = file_path.name
+                    file_path = entry_name[: len(entry_name) - len(file_name)]
+                    file_path = file_path[: 40 - len(file_name)]
+                    entry_name = f"{file_path}...{file_name}"
             bar_value = int(((entry["total"] / total) * 100) / 2)
-            print(
-                "%30s: %5s %5s%% %s"
-                % (entry_name, entry["total"], int(entry["total"] / total * 100), "\u25A0" * bar_value)
+            txt += f"%-{entry_length}s %5s %5s%% %s\n" % (
+                entry_name,
+                entry["total"],
+                int(entry["total"] / total * 100),
+                "\u25A0" * bar_value,
             )
 
-    print()
+    txt += "\n"
+    if return_string:
+        return txt
+    print(txt)
     return
```

### Comparing `cbinterface-2.3.9/cbinterface/psc/intel.py` & `cbinterface-3.0.0/cbinterface/enterprise_edr/intel.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,67 @@
 """All things intel & alerts.
 
 IOCs, Reports, Watchlists, Feeds, Alerts.
 
-NOTE on Response Watchlist to PSC EDR Intel Migrations:
+NOTE on Response Watchlist to Enterprise EDR Intel Migrations:
 
-  There are three different ways that I built to migrate Response 
-  Watchlists to PSC EDR Watchlists:
+  There are three different ways that I built to migrate Response
+  Watchlists to Enterprise EDR Watchlists:
    1. One-to-One
    2. Many-to-One
    3. Many-to-Two (Not connected to CLI)
 
  All of the above use the `yield_reports_created_from_response_watchlists` to convert
- Response Watchlists into PSC EDR Reports. That function converts the Response queries to
- valid PSC EDR queries. If a query doesn't validate/convert, a log is generated and it's 
+ Response Watchlists into Enterprise EDR Reports. That function converts the Response queries to
+ valid Enterprise EDR queries. If a query doesn't validate/convert, a log is generated and it's
  skipped. If it does validate, a Report is generated. If the Watchlist, in Response, was really slow or
- had errors the resulting PSC EDR Report will be set to "ignore" automatically. Additionally, I passed
+ had errors the resulting Enterprise EDR Report will be set to "ignore" automatically. Additionally, I passed
  all the available context about the Response Watchlist into the description of the resulting Reports.
 
  We had over 300 custom Response Watchlists, here is what I did for our use case:
-  1. I seperated the watchlists with true positive detections and low FP rates 
+  1. I seperated the watchlists with true positive detections and low FP rates
      using our ACE Alert metrics. I put the names of these Watchlists into a txt file
      and then exported them from response using the following command:
        `cat ~smcfeely/working/cbmigration/uniq.high_fidelity.watchlists.txt | cbinterface response_watchlist --watchlist-names-from-stdin -json > high_fid.response_watchlists.json`
 
   2. Next, I used the command below to import these Response Watchlists into a single
-     PSC EDR Watchlist I called "ACE Higher Fidelity Response Watchlists":
+     Enterprise EDR Watchlist I called "ACE Higher Fidelity Response Watchlists":
        `cbinterface intel migrate ~smcfeely/working/cbmigration/high_fid.response_watchlists.json --many-to-one`
 
   3. After that, I exported the remaining custom Response Watchlists into another json file and called the
-     `convert_response_watchlists_to_grouped_psc_edr_watchlists` function from a python terminal to organize 
-     the Response Watchlists into *two* PSC EDR Watchlists, one for Response Watchlists that have never
-     had a hit and then the ones remaining are lower fidelity and went into a "Low Fidelity" PSC EDR Watchlist.
-        
+     `convert_response_watchlists_to_grouped_enterprise_edr_watchlists` function from a python terminal to organize
+     the Response Watchlists into *two* Enterprise EDR Watchlists, one for Response Watchlists that have never
+     had a hit and then the ones remaining are lower fidelity and went into a "Low Fidelity" Enterprise EDR Watchlist.
+
 """
+
+import os
 import json
 import time
 import logging
 
 from dateutil import tz
 from dateutil.parser import parse as parse_timestamp
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Dict, List, Literal
 
-from cbapi.psc.threathunter import CbThreatHunterAPI
-from cbapi.errors import ServerError, ClientError, ObjectNotFoundError
+from cbc_sdk import CBCloudAPI
+from cbc_sdk.platform import Alert
+from cbc_sdk.errors import ServerError, ClientError, ObjectNotFoundError
 
-LOGGER = logging.getLogger("cbinterface.psc.intel")
+LOGGER = logging.getLogger("cbinterface.enterprise_edr.intel")
 
 
 ## Alerts ##
-def alert_search(
-    cb: CbThreatHunterAPI,
-    search_data: Dict = {},
-    criteria: Dict = {},
-    query: str = None,
-    rows=40,
-    sort: List[Dict] = [{"field": "first_event_time", "order": "DESC"}],
-    start: int = 0,
-    workflow_state=["OPEN", "DISMISSED"],
-) -> Dict:
-    """Perform an Alert search
+def alert_search(cb: CBCloudAPI, search_data: Dict) -> Dict:
+    """Perform an Alert search.
 
     One request and return the result.
     """
-    url = f"/appservices/v6/orgs/{cb.credentials.org_key}/alerts/watchlist/_search"
-    if not search_data:
-        if "workflow" not in criteria:
-            criteria["workflow"] = workflow_state
-        search_data = {"criteria": criteria, "query": query, "rows": rows, "start": start, "sort": sort}
+    url = f"/api/alerts/v7/orgs/{cb.credentials.org_key}/alerts/_search"
     try:
         result = cb.post_object(url, search_data)
         return result.json()
 
     except ServerError as e:
         LOGGER.error(f"Caught ServerError searching alerts: {e}")
         return False
@@ -80,214 +70,200 @@
         return False
     except ValueError:
         LOGGER.warning(f"got unexpected {result}")
         return False
 
 
 def yield_alerts(
-    cb: CbThreatHunterAPI,
-    search_data: Dict = {},
-    criteria: Dict = {},
+    cb: CBCloudAPI,
     query: str = None,
-    rows=40,
-    sort: List[Dict] = [{"field": "last_update_time", "order": "ASC"}],
-    start: int = 0,
-    workflow_state=["OPEN", "DISMISSED"],
-    max_results: int = None,  # limit results returned
+    time_range: Dict = None,
+    criteria: Dict = None,
+    exclusions: Dict = None,
+    sort: List[Dict] = [{"field": "backend_update_timestamp", "order": "ASC"}],
+    start: int = 1,
+    rows: int = 100,
+    max_results: int = 500,  # limit results returned
 ) -> Dict:
     """Yield Alerts resulting from alert search."""
-    position = start
+    data = {k: v for k, v in locals().items() if v is not None and k not in ["max_results", "cb"]}
     still_querying = True
     while still_querying:
-        if max_results and position + rows > max_results:
+        if max_results and data["start"] + rows > max_results:
             # get however many rows that may result in max_results
-            rows = max_results - position
-        result = alert_search(
-            cb,
-            search_data=search_data,
-            criteria=criteria,
-            query=query,
-            rows=rows,
-            sort=sort,
-            start=position,
-            workflow_state=workflow_state,
-        )
+            rows = max_results - data["start"]
+        result = alert_search(cb, data)
 
         if not result:
             return result
-
         total_results = result["num_found"]
         results = result.get("results", [])
-        LOGGER.debug(f"got {len(results)+position} out of {total_results} total alerts.")
+        LOGGER.debug(f"got {len(results)+data['start']-1} out of {total_results} total alerts.")
         for item in results:
             yield item
-            position += 1
-            if max_results and position >= max_results:
+            data["start"] += 1
+            if max_results and data["start"] >= max_results:
                 still_querying = False
                 break
 
-        if position >= total_results:
+        if data["start"] >= total_results:
             still_querying = False
             break
 
 
-def get_all_alerts(
-    cb: CbThreatHunterAPI,
-    search_data: Dict = {},
-    criteria: Dict = {},
-    query: str = None,
-    rows=40,
-    sort: List[Dict] = [{"field": "last_update_time", "order": "ASC"}],
-    start: int = 0,
-    workflow_state=["OPEN", "DISMISSED"],
-    max_results: int = None,  # limit results returned
-) -> Dict:
-    """Return list of Alerts resulting from alert search."""
-    return list(
-        yield_alerts(
-            cb,
-            search_data=search_data,
-            criteria=criteria,
-            query=query,
-            rows=rows,
-            sort=sort,
-            start=start,
-            workflow_state=workflow_state,
-            max_results=max_results,
-        )
-    )
-
-
-def get_alert(cb: CbThreatHunterAPI, alert_id) -> Dict:
+def get_alert(cb: CBCloudAPI, alert_id) -> Dict:
     """Get alert by ID."""
-    url = f"/appservices/v6/orgs/{cb.credentials.org_key}/alerts/{alert_id}"
+    url = f"/api/alerts/v7/orgs/{cb.credentials.org_key}/alerts/{alert_id}"
     try:
         return cb.get_object(url)
-    except ServerError:
-        LOGGER.error(f"Caught ServerError getting report {report_id}: {e}")
+    except ServerError as e:
+        LOGGER.error(f"Caught ServerError getting report {alert_id}: {e}")
 
 
-def update_alert_state(
-    cb: CbThreatHunterAPI,
-    alert_id,
-    state: Union["DISMISSED", "OPEN"],
-    remediation_state: str = None,
-    comment: str = None,
+def update_alert_status(
+    cb: CBCloudAPI,
+    alert_ids: List[str],
+    status: Literal["OPEN", "IN_PROGRESS", "CLOSED"],
+    determination: Literal["TRUE_POSITIVE", "FALSE_POSITIVE", "NONE"],
+    closure_reason: Literal["NO_REASON", "RESOLVED", "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"],
+    note: str = None,
 ) -> Dict:
-    """Update alert remediation state by ID."""
-    url = f"/appservices/v6/orgs/{cb.credentials.org_key}/alerts/{alert_id}/workflow"
-    remediation = {"state": state, "remediation_state": remediation_state, "comment": comment}
-    try:
-        return cb.post_object(url, remediation).json()
+    """Update alerts state."""
+    data = {k: v for k, v in locals().items() if v is not None and k not in ["cb", "alert_ids"]}
+    alert_query = cb.select(Alert).add_criteria("id", alert_ids)
+    job = alert_query.update(**data)
+    try:
+        alert_query = cb.select(Alert).add_criteria("id", alert_ids)
+        job = alert_query.update(**data)
+        job.await_completion().result()
+        return job.to_json()
     except ServerError as e:
         LOGGER.error(f"Caught ServerError: {e}")
         return False
     except ClientError as e:
         LOGGER.warning(f"got ClientError:: {e}")
         return False
 
 
 def interactively_update_alert_state(
-    cb: CbThreatHunterAPI,
+    cb: CBCloudAPI,
     alert_id,
-    state: Union["DISMISSED", "OPEN"] = None,
-    remediation_state: str = None,
-    comment: str = None,
+    status: Literal["OPEN", "IN_PROGRESS", "CLOSED"] = None,
+    determination: Literal["TRUE_POSITIVE", "FALSE_POSITIVE", "NONE"] = None,
+    closure_reason: Literal["NO_REASON", "RESOLVED", "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"] = None,
+    note: str = None,
 ) -> Dict:
     """Update alert remediation state by ID."""
     from cbinterface.helpers import input_with_timeout
 
-    if not state:
-        state = input_with_timeout("Alert state to set, DISMISSED or OPEN? [DISMISSED]: ") or "DISMISSED"
-        if state not in ["DISMISSED", "OPEN"]:
-            LOGGER.error(f"state must be one of [DISMISSED, OPEN], not {state}")
+    if not status:
+        status = input_with_timeout("Alert status to set, OPEN, IN_PROGRESS or CLOSED? [CLOSED]: ") or "CLOSED"
+        if status not in ["OPEN", "IN_PROGRESS", "CLOSED"]:
+            LOGGER.error(f"status must be one of [OPEN, IN_PROGRESS, CLOSED], not {status}")
+            return False
+    if not determination:
+        determination = input_with_timeout("Determination: ") or None
+        if determination not in ["TRUE_POSITIVE", "FALSE_POSITIVE", "NONE", None]:
+            LOGGER.error(f"determination must be one of [TRUE_POSITIVE, FALSE_POSITIVE, NONE], not {determination}")
             return False
-    if not remediation_state:
-        remediation_state = input_with_timeout("State of Remediation: ") or ""
-    if not comment:
-        comment = input_with_timeout("Comment: ") or ""
-    return update_alert_state(cb, alert_id, state, remediation_state, comment)
+    if not closure_reason:
+        closure_reason = input_with_timeout("Closure reason: ") or None
+        if closure_reason not in [
+            "NO_REASON",
+            "RESOLVED",
+            "RESOLVED_BENIGN_KNOWN_GOOD",
+            "DUPLICATE_CLEANUP",
+            "OTHER",
+            None,
+        ]:
+            LOGGER.error(
+                f"closure reason must be one of [NO_REASON, RESOLVED, RESOLVED_BENIGN_KNOWN_GOOD, DUPLICATE_CLEANUP, OTHER], not {closure_reason}"
+            )
+            return False
+    if not note:
+        note = input_with_timeout("Note: ") or None
+    return update_alert_status(cb, alert_id, status, determination, closure_reason, note)
 
 
 ## Reports ##
-def create_report(cb: CbThreatHunterAPI, report_data) -> Dict:
+def create_report(cb: CBCloudAPI, report_data) -> Dict:
     """Create an intel Report."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports"
     try:
         result = cb.post_object(url, report_data)
     except ServerError as e:
         LOGGER.error(f"Caught ServerError creating report: {e}")
         return False
     try:
         return result.json()
     except ValueError:
         return False
 
 
-def ignore_report(cb: CbThreatHunterAPI, report_id) -> Dict:
-    """Set this report to ignore status"""
+def ignore_report(cb: CBCloudAPI, report_id) -> Dict:
+    """Set this report to ignore status."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/ignore"
     try:
         return cb.put_object(url, {"ignore": True})
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting report {report_id}: {e}")
 
 
-def delete_report(cb: CbThreatHunterAPI, report_id) -> Dict:
-    """Set this report to ignore status"""
+def delete_report(cb: CBCloudAPI, report_id) -> Dict:
+    """Set this report to ignore status."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}"
     try:
         return cb.delete_object(url)
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError deleting report {report_id}: {e}")
 
 
-def get_report_status(cb: CbThreatHunterAPI, report_id) -> Dict:
-    """Get report to ignore status"""
+def get_report_status(cb: CBCloudAPI, report_id) -> Dict:
+    """Get report to ignore status."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/ignore"
     try:
         return cb.get_object(url)
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting report {report_id}: {e}")
 
 
-def activate_report(cb: CbThreatHunterAPI, report_id) -> Dict:
-    """Set this report to active status"""
+def activate_report(cb: CBCloudAPI, report_id) -> Dict:
+    """Set this report to active status."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/ignore"
     try:
         return cb.delete_object(url)
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting report {report_id}: {e}")
 
 
-def get_report(cb: CbThreatHunterAPI, report_id) -> Dict:
+def get_report(cb: CBCloudAPI, report_id) -> Dict:
     """Get report by report id."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}"
     try:
         report = cb.get_object(url)
         report["ignored"] = get_report_status(cb, report["id"])["ignored"]
         return report
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting report {report_id}: {e}")
     except ObjectNotFoundError:
         LOGGER.warning(f"report {report_id} does not exist")
 
 
-def get_report_with_IOC_status(cb: CbThreatHunterAPI, report_id) -> Dict:
+def get_report_with_IOC_status(cb: CBCloudAPI, report_id) -> Dict:
     """Get report and include status of every report IOC."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/iocs"
     report = get_report(cb, report_id)
     if not report:
         return None
     for ioc in report["iocs_v2"]:
         ioc["ignored"] = cb.get_object(f"{url}/{ioc['id']}/ignore")["ignored"]
     return report
 
 
-def update_report(cb: CbThreatHunterAPI, report_id, report_data) -> Dict:
+def update_report(cb: CBCloudAPI, report_id, report_data) -> Dict:
     """Update an existing report."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}"
 
     # clean up any ignored fields or Cb will bark back
     if "ignored" in report_data:
         del report_data["ignored"]
     for ioc in report_data["iocs_v2"]:
@@ -305,141 +281,208 @@
     except ClientError as e:
         LOGGER.warning(f"got ClientError updating report: {e}")
         return False
 
     return result.json()
 
 
-def update_report_ioc_query(cb: CbThreatHunterAPI, report_id, ioc_id, ioc_query_string) -> Dict:
+def write_basic_report_template() -> bool:
+    """Print a basic report template.
+
+    The template can be filled out to create a new threat report.
+    """
+    ioc2_template = {"id": 1, "match_type": "query", "values": ["query_string_here"]}
+    report_template = {
+        "title": None,
+        "description": None,  # required
+        "severity": None,
+        "link": None,
+        "tags": [],
+        "iocs_v2": [ioc2_template],  # required
+    }
+    template_name = "basic.threat_report.single_ioc_query.template.json"
+    with open(template_name, "w") as fp:
+        fp.write(json.dumps(report_template, indent=2))
+    if os.path.exists(template_name):
+        return template_name
+    return False
+
+
+def update_report_ioc_query(cb: CBCloudAPI, report_id, ioc_id, ioc_query_string) -> Dict:
     """Update IOC query value with ioc_query_string.
 
-    A cbapi.errors.ClientError will be raised if the query is not valid.
+    A cbc_sdk.errors.ClientError will be raised if the query is not valid.
     """
     report_data = get_report_with_IOC_status(cb, report_id)
     for ioc in report_data["iocs_v2"]:
         if ioc["id"] == ioc_id:
             if ioc["match_type"] != "query":
                 LOGGER.error(f"not a query based IOC: {ioc}")
                 return False
             if ioc["ignored"]:
-                LOGGER.warning(f"you're updating an IOC that is set to ignored.")
+                LOGGER.warning("you're updating an IOC that is set to ignored.")
             if len(ioc["values"]) > 1:
                 LOGGER.warning(
                     f"This query IOC has a surprising number of values that are about to be over-written: {ioc['values']}"
                 )
             ioc["values"] = [ioc_query_string]
     return update_report(cb, report_id, report_data)
 
 
-def interactively_update_report_ioc_query(cb: CbThreatHunterAPI, report_id, ioc_id) -> Dict:
+def interactively_update_report_ioc_query(cb: CBCloudAPI, report_id, ioc_id) -> Dict:
     """Prompt user for new query and update the report IOC query."""
     from cbinterface.helpers import input_with_timeout
 
+    report = get_report(cb, report_id)
+    if not report:
+        return None
+
+    ioc = [ioc for ioc in report["iocs_v2"] if ioc_id == ioc["id"]][0]
+    if ioc["match_type"] != "query":
+        LOGGER.warning(f"IOC={ioc_id} is not a query based IOC: {ioc}")
+
+    print(f"Current IOC query: {ioc['values'][0]}")
     new_ioc_query = input_with_timeout("Enter new query: ", timeout=90)
     return update_report_ioc_query(cb, report_id, ioc_id, new_ioc_query)
 
 
 def print_report(report: Dict) -> None:
     """Special print formatting."""
     print("\n------------------------- INTEL REPORT -------------------------")
     for field, value in report.items():
         if "iocs_v2" == field:
             continue
         print(f"\t{field}: {value}")
-    print(f"\tiocs_v2: ")
+    print("\tiocs_v2: ")
     for ioc in report["iocs_v2"]:
         for field, value in ioc.items():
             if field == "values":
                 continue
             print(f"\t\t{field}: {value}")
         for ioc_value in ioc["values"]:
             print(f"\t\tioc_value: {ioc_value}")
+        print()
     print()
 
 
 ## IOCs ##
+def ioc_does_exist(cb: CBCloudAPI, report_id, ioc_id):
+    """Check if the given report contains the ioc_id."""
+    report = get_report(cb, report_id)
+    if not report:
+        return None
+    for ioc in report["iocs_v2"]:
+        if ioc["id"] == ioc_id:
+            return True
+    return False
+
+
 # get IOC status
+def is_ioc_ignored(cb: CBCloudAPI, report_id, ioc_id, check_existence=False):
+    """Return status of IOC."""
+    if check_existence:
+        if not ioc_does_exist(cb, report_id, ioc_id):
+            LOGGER.warning("IOC does not exist.")
+            return None
+    url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/iocs/{ioc_id}/ignore"
+    return cb.get_object(url)["ignored"]
+
 
 # ignore IOC
+def ignore_ioc(cb: CBCloudAPI, report_id, ioc_id):
+    """Ignore this IOC."""
+    url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/iocs/{ioc_id}/ignore"
+    return cb.put_object(url, {"ignore": True})
+
 
 # activate IOC
+def activate_ioc(cb: CBCloudAPI, report_id, ioc_id):
+    """Activate IOC."""
+    url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/reports/{report_id}/iocs/{ioc_id}/ignore"
+    resp = cb.delete_object(url)
+    if resp.status_code == 204:
+        return True
+    return False
+
 
 ## Watchlists ##
-def get_all_watchlists(cb: CbThreatHunterAPI):
+def get_all_watchlists(cb: CBCloudAPI):
     """Return a list of all watchlists."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists"
     result = cb.get_object(url)
     return result.get("results", [])
 
 
-def get_watchlist(cb: CbThreatHunterAPI, watchlist_id):
+def get_watchlist(cb: CBCloudAPI, watchlist_id):
     """Get a watchlist by ID."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists"
     try:
         return cb.get_object(f"{url}/{watchlist_id}")
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting watchlist {watchlist_id}: {e}")
     except ObjectNotFoundError:
         LOGGER.warning(f"No watchlist with ID {watchlist_id}")
 
 
-def get_watchlists_like_name(cb: CbThreatHunterAPI, watchlist_name):
+def get_watchlists_like_name(cb: CBCloudAPI, watchlist_name):
     """Return watchlists with watchlist_name in their name."""
     return [wl for wl in get_all_watchlists(cb) if watchlist_name in wl["name"]]
 
 
-def create_watchlist(cb: CbThreatHunterAPI, watchlist_data: Dict):
+def create_watchlist(cb: CBCloudAPI, watchlist_data: Dict):
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists"
     try:
         result = cb.post_object(url, watchlist_data)
     except ServerError as e:
         LOGGER.error(f"Caught ServerError creating watchlist: {e}")
         return False
     except ClientError as e:
         LOGGER.warning(f"got ClientError creating watchlist: {e}")
         return False
 
     return result.json()
 
 
-def delete_watchlist(cb: CbThreatHunterAPI, watchlist_id) -> Dict:
-    """Set this report to ignore status"""
+def delete_watchlist(cb: CBCloudAPI, watchlist_id) -> Dict:
+    """Set this report to ignore status."""
     url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists/{watchlist_id}"
     try:
         return cb.delete_object(url)
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError deleting watchlist {watchlist_id}: {e}")
 
 
-def update_watchlist(cb: CbThreatHunterAPI, watchlist_data: Dict):
-    url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists"
+def update_watchlist(cb: CBCloudAPI, watchlist_data: Dict):
+    watchlist_id = watchlist_data["id"]
+    url = f"/threathunter/watchlistmgr/v3/orgs/{cb.credentials.org_key}/watchlists/{watchlist_id}"
     try:
         result = cb.put_object(url, watchlist_data)
     except ServerError as e:
         LOGGER.error(f"Caught ServerError creating watchlist: {e}")
         return False
     except ClientError as e:
         LOGGER.warning(f"got ClientError creating watchlist: {e}")
         return False
 
     return result.json()
 
 
 def create_watchlist_from_report_list(
-    cb: CbThreatHunterAPI, watchlist_name: str, watchlist_description: str, reports: List[Dict]
+    cb: CBCloudAPI, watchlist_name: str, watchlist_description: str, reports: List[Dict]
 ) -> Dict:
     """Create a watchlist built on the supplied intel reports.
 
     Use this to create a single watchlist comprised of the intel reports.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
       watchlist_name: Name for the resulting watchlist
       watchlist_description: Description for the resulting watchlist
       reports: The Intel Reports.
+
     Returns:
       Dict representation of the new Watchlist.
     """
     assert isinstance(reports, list)
     assert isinstance(reports[0], dict)
     assert "id" in reports[0]
 
@@ -457,136 +500,261 @@
         LOGGER.error(f"problem creating watchlist for {watchlist_data}")
         return False
     LOGGER.info(f"created watchlist: {watchlist}")
 
     return watchlist
 
 
-def assign_reports_to_watchlist(cb: CbThreatHunterAPI, watchlist_id: str, reports: List[Dict]) -> Dict:
+def assign_reports_to_watchlist(cb: CBCloudAPI, watchlist_id: str, reports: List[Dict]) -> Dict:
     """Set a watchlist report IDs attribute to the passed reports.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
       watchlist_id: The Watchlist ID to update.
       reports: The Intel Reports.
+
     Returns:
       The Watchlist in dict form.
     """
     watchlist_data = get_watchlist(cb, watchlist_id)
     if not watchlist_data:
         return None
     watchlist_data["report_ids"] = [r["id"] for r in reports]
     watchlist_data = update_watchlist(cb, watchlist_data)
     if not watchlist_data:
-        LOGGER.error(f"unexpected problem updating watchlist with report IDs.")
+        LOGGER.error("unexpected problem updating watchlist with report IDs.")
         return False
 
     return watchlist_data
 
 
+def create_new_report_and_append_to_watchlist(cb: CBCloudAPI, watchlist_id: str, report_data: Dict) -> Dict:
+    """Create a new threat report from JSON and append to watchlist."""
+    watchlist_data = get_watchlist(cb, watchlist_id)
+    if not watchlist_data:
+        LOGGER.error(f"watchlist does not exist: {watchlist_id}")
+        return False
+    watchlist_threat_reports_before = len(watchlist_data["report_ids"])
+
+    if "report" in report_data:
+        report_data = report_data["report"]
+
+    # create intel report
+    report = {
+        "title": report_data["title"],  # required
+        "description": report_data["description"],  # required
+        "timestamp": time.time(),
+        "severity": report_data.get("severity", 5),
+        "link": report_data.get("link", None),
+        "tags": report_data.get("tags", []),
+        "iocs_v2": report_data["iocs_v2"],  # required
+    }
+    intel_report = create_report(cb, report)
+    if not isinstance(intel_report, dict):
+        LOGGER.error(f"problem creating report for {report_data}")
+        return False
+    LOGGER.info(f"created intel report: {intel_report}")
+
+    # append intel report to Watchlist.
+    watchlist_data["report_ids"].append(intel_report["id"])
+    watchlist_data = update_watchlist(cb, watchlist_data)
+    if watchlist_data and len(watchlist_data["report_ids"]) == (watchlist_threat_reports_before + 1):
+        LOGGER.info("successfully appended new threat report to watchlist.")
+        return True
+    return False
+
+
 # TODO enable watchlist alerting/taging?
 
 # TODO disable watchlist alerting/taging?
 
+
 ## Feeds ##
-def get_all_feeds(cb: CbThreatHunterAPI, include_public=True) -> Dict:
+def get_all_feeds(cb: CBCloudAPI, include_public=True) -> Dict:
     """Retrieve all feeds owned by the caller.
 
     Provide include_public=true parameter to also include public community feeds.
     """
     url = f"/threathunter/feedmgr/v2/orgs/{cb.credentials.org_key}/feeds"
     params = {"include_public": include_public}
     result = cb.get_object(url, query_parameters=params)
     return result.get("results", [])
 
 
-def get_feed(cb: CbThreatHunterAPI, feed_id: str) -> Dict:
+def get_feed(cb: CBCloudAPI, feed_id: str) -> Dict:
     """Get a specific feed by ID."""
     url = f"/threathunter/feedmgr/v2/orgs/{cb.credentials.org_key}/feeds"
     try:
         return cb.get_object(f"{url}/{feed_id}")
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting feed {feed_id}: {e}")
     except ObjectNotFoundError:
         LOGGER.warning(f"No feed by feed id {feed_id}")
 
 
-def search_feed_names(cb: CbThreatHunterAPI, name: str) -> List[Dict]:
+def search_feed_names(cb: CBCloudAPI, name: str) -> List[Dict]:
     """Search for feeds by name."""
     return [f for f in get_all_feeds(cb) if name in f["name"]]
 
 
-def get_feed_report(cb: CbThreatHunterAPI, feed_id: str, report_id: str) -> Dict:
+def get_feed_report(cb: CBCloudAPI, feed_id: str, report_id: str) -> Dict:
     """Get a specific report from a specific feed."""
     url = f"/threathunter/feedmgr/v2/orgs/{cb.credentials.org_key}/feeds/{feed_id}/reports/{report_id}"
     try:
         return cb.get_object(url)
-    except ServerError:
+    except ServerError as e:
         LOGGER.error(f"Caught ServerError getting feed report {feed_id}: {e}")
     except ObjectNotFoundError:
         LOGGER.warning(f"No feed {feed_id} or report {report_id} in the feed")
 
 
-## Begin Response to PSC EDR Watchlist Migrations ##
-def yield_reports_created_from_response_watchlists(
-    cb: CbThreatHunterAPI, response_watchlists: List[Dict]
-) -> List[Dict]:
-    """Convert a list of response watchlists to PSC EDR intel reports.
+"""
+Begin Intel backup routines.
+"""
+
+
+def _safe_filename(raw_string):
+    import string
+
+    raw_string = raw_string.replace(" ", "_")
+    valid_chars = ["_", "-"]
+    valid_chars.extend(list(string.digits))
+    valid_chars.extend(list(string.ascii_lowercase))
+    valid_chars.extend(list(string.ascii_uppercase))
+    safe_string = ""
+    for char in raw_string:
+        if char in valid_chars:
+            safe_string += char
+    return safe_string
+
+
+def backup_watchlist_threat_reports(cb: CBCloudAPI, watchlist_ids: List):
+    """Backup threat reports for safe keeping.
+
+    Write threat report json to local directory for each watchlist ID.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
+      watchlist_ids: List of CBC watchlist IDs to backup.
+
+    Returns:
+      True on success.
+    """
+    from pathlib import Path
+    from cbinterface.config import get_data_directory
+
+    data_dir = get_data_directory()
+    if not os.path.exists(data_dir) or data_dir == ".":
+        LOGGER.warning("ENV CBINTERFACE_DATA_DIR does not exist. Using current working directory.")
+
+    backup_dir = os.path.join(data_dir, "cbc_intel")
+    Path(backup_dir).mkdir(parents=True, exist_ok=True)
+
+    file_paths = []
+    for watchlist_id in watchlist_ids:
+        watchlist = get_watchlist(cb, watchlist_id)
+        if not watchlist:
+            continue
+
+        wl_dir = _safe_filename(watchlist["name"])
+        wl_dir += ".wl"
+        wl_dir = os.path.join(backup_dir, wl_dir)
+        Path(wl_dir).mkdir(parents=True, exist_ok=True)
+
+        watchlist_path = os.path.join(wl_dir, "watchlist.json")
+        with open(watchlist_path, "w") as fp:
+            fp.write(json.dumps(watchlist))
+            file_paths.append(watchlist_path)
+
+        report_ids = watchlist.get("report_ids")
+        if report_ids:
+            for report_id in report_ids:
+                report = get_report(cb, report_id)
+                report_filename = _safe_filename(report["title"]) + ".json"
+                report_filepath = os.path.join(wl_dir, report_filename)
+                with open(report_filepath, "w") as fp:
+                    fp.write(json.dumps(report))
+                    file_paths.append(report_filepath)
+
+        classifier = watchlist.get("classifier")
+        if classifier and classifier.get("key") == "feed_id":
+            feed_id = classifier["value"]
+            feed = get_feed(cb, feed_id)
+            if not feed or not feed.get("feedinfo"):
+                continue
+            feed_name = _safe_filename(feed["feedinfo"]["name"]) + ".feed.json"
+            feed_filepath = os.path.join(wl_dir, feed_name)
+            with open(feed_filepath, "w") as fp:
+                fp.write(json.dumps(feed))
+                file_paths.append(feed_filepath)
+
+    for fp in file_paths:
+        if os.path.exists(fp):
+            LOGGER.info(f"wrote {fp}")
+        else:
+            LOGGER.error(f"failed to write {fp}")
+
+    return file_paths
+
+
+## Begin Response to Enterprise EDR Watchlist Migrations ##
+def yield_reports_created_from_response_watchlists(cb: CBCloudAPI, response_watchlists: List[Dict]) -> List[Dict]:
+    """Convert a list of response watchlists to Enterprise EDR intel reports.
+
+    Args:
+      cb: CBCloudAPI object
       response_watchlists: List of Response Watchlist in dictionary form.
+
     Returns:
-      Yield PSC Intel Reports for each Response Watchlist.
+      Yield EEDR Intel Reports for each Response Watchlist.
     """
-    psc_watchlist_names = [wl["name"] for wl in get_all_watchlists(cb)]
     for wl_data in response_watchlists:
-        # attempt to convert and validate query syntax for PSC
+        # attempt to convert and validate query syntax for EEDR
         if "query" not in wl_data:
             LOGGER.error("how does a legacy watchlist not have a query? make sure to convert search_query to query.")
             continue
         query = wl_data["query"]
         try:
             query = cb.convert_query(query)
             LOGGER.info(f"converted query: {query}")
         except Exception as e:
             LOGGER.error(f"problem converting query for {wl_data['name']} : {e}")
             continue
         if not cb.validate_query(query):
-            LOGGER.error(f"query did not validate")
+            LOGGER.error("query did not validate")
             continue
 
         report_tags = ["response_migrated_watchlist"]
         report_description = f"Legacy Cb Response Watchlist Description: {wl_data.get('description')}"
 
         ignore_this_report = False
 
         # warn of disabled watchlists
         if not wl_data["enabled"]:
             LOGGER.warning(f"{wl_data['name']} is disabled... NOT creating report.")
             ignore_this_report = True
-            report_description += f"\nIgnored: disabled in Cb Response"
+            report_description += "\nIgnored: disabled in Cb Response"
             report_tags.append("disabled_in_response")
 
         # warn on slow watchlists
         if wl_data["last_execution_time_ms"] is None:
             LOGGER.error(
                 f"{wl_data['name']} last_execution_time time is null. This means an error occurred with it's execution. Setting report to ignore."
             )
             ignore_this_report = True
-            report_description += f"\nIgnored: last execution error'd in Cb Response"
+            report_description += "\nIgnored: last execution error'd in Cb Response"
             report_tags.append("execution_errors_in_response")
         elif int(wl_data["last_execution_time_ms"]) > 10000:
             seconds = int(wl_data["last_execution_time_ms"]) / 1000
             LOGGER.warning(f"{wl_data['name']} last_execution_time took {seconds} seconds")
             report_tags.append("slow_in_response")
             if seconds > 30:
                 LOGGER.warning(f"{wl_data['name']} has been 💩 slow in response. Setting report to ignore...")
                 ignore_this_report = True
-                report_description += f"\nIgnored: has been 💩 slow in Cb Response. Improve it!?"
+                report_description += "\nIgnored: has been 💩 slow in Cb Response. Improve it!?"
 
         # inform of hit count per day
         hit_count = int(wl_data["total_hits"])
         if hit_count == 0:
             report_tags.append("no_hits_in_response")
         created_date = parse_timestamp(wl_data["date_added"]).astimezone(tz.gettz("UTC"))
         days_since_creation = (datetime.utcnow().astimezone(tz.gettz("UTC")) - created_date).days
@@ -612,26 +780,27 @@
         if ignore_this_report:
             if ignore_report(cb, intel_report["id"]):
                 LOGGER.info(f"ignored report {intel_report['id']}")
 
         yield intel_report
 
 
-def convert_response_watchlists_to_psc_edr_watchlists(
-    cb: CbThreatHunterAPI, response_watchlists: List[Dict]
+def convert_response_watchlists_to_enterprise_edr_watchlists(
+    cb: CBCloudAPI, response_watchlists: List[Dict]
 ) -> List[Dict]:
-    """Convert a list of response watchlists to PSC EDR watchlists.
+    """Convert a list of response watchlists to Enterprise EDR watchlists.
 
     This is a one-for-one Watchlist migration. You probably don't want this.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
       response_watchlists: List of response watchlist in dictionary form.
+
     Returns:
-      List of PSC Watchlists.
+      List of EEDR Watchlists.
     """
     results = []
     for intel_report in yield_reports_created_from_response_watchlists(cb, response_watchlists):
         report_id = intel_report["id"]
         # get original description
         name = intel_report.get("title")
         description = [rwl.get("description", "") for rwl in response_watchlists if rwl["name"] == name][0]
@@ -650,65 +819,67 @@
             continue
         LOGGER.info(f"created watchlist: {watchlist}")
         results.append(watchlist)
 
     return results
 
 
-def convert_response_watchlists_to_single_psc_edr_watchlist(
-    cb: CbThreatHunterAPI,
+def convert_response_watchlists_to_single_enterprise_edr_watchlist(
+    cb: CBCloudAPI,
     response_watchlists: List[Dict],
     watchlist_name: str = None,
     watchlist_description="Consolidated Cb Respone Watchlists. Each report in this watchlist is based on a Cb Response Watchlist",
 ) -> List[Dict]:
-    """Convert a list of Response Watchlists to PSC EDR watchlists.
+    """Convert a list of Response Watchlists to Enterprise EDR watchlists.
 
     This is a many-to-one Watchlist migration.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
       response_watchlists: List of Response Ratchlist in dictionary form.
-      watchlist_name: The name to give the resulting Response consolidated PSC EDR Watchlist.
+      watchlist_name: The name to give the resulting Response consolidated Enterprise EDR Watchlist.
       watchlist_description: The description to give the resulting Watchlist.
+
     Returns:
-      PSC Watchlist containing all Response Watchlists as intel Reports.
+      EEDR Watchlist containing all Response Watchlists as intel Reports.
     """
     from cbinterface.helpers import input_with_timeout
 
     if watchlist_name is None:
-        watchlist_name = input_with_timeout("Enter a name for the resulting PSC EDR Watchlist: ", stderr=False)
+        watchlist_name = input_with_timeout("Enter a name for the resulting Enterprise EDR Watchlist: ", stderr=False)
         watchlist_description = (
             input_with_timeout(
                 f"Enter a description for the Watchlist [default description: {watchlist_description}] : ", stderr=False
             )
             or watchlist_description
         )
 
     reports = list(yield_reports_created_from_response_watchlists(cb, response_watchlists))
     if not reports:
         return None
 
     return create_watchlist_from_report_list(cb, watchlist_name, watchlist_description, reports)
 
 
-def convert_response_watchlists_to_grouped_psc_edr_watchlists(
-    cb: CbThreatHunterAPI,
+def convert_response_watchlists_to_grouped_enterprise_edr_watchlists(
+    cb: CBCloudAPI,
     response_watchlists: List[Dict],
     watchlist_names_start_with: str = "ACE ",
 ) -> List[Dict]:
-    """Convert a list of Response Watchlists to PSC EDR watchlists.
+    """Convert a list of Response Watchlists to Enterprise EDR watchlists.
 
     This is a many-to-two Watchlist migration based on metrics provided by Response.
 
     Args:
-      cb: Cb PSC object
+      cb: CBCloudAPI object
       response_watchlists: List of Response Ratchlist in dictionary form.
       watchlist_names_start_with: A key/identifer to start the watchlist names with.
+
     Returns:
-      List of PSC Watchlists.
+      List of Enterprise EDR Watchlists.
     """
     from cbinterface.helpers import input_with_timeout
 
     reports = list(yield_reports_created_from_response_watchlists(cb, response_watchlists))
     if not reports:
         return None
```

### Comparing `cbinterface-2.3.9/cbinterface/psc/sessions.py` & `cbinterface-3.0.0/cbinterface/enterprise_edr/sessions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 from cbapi.errors import ObjectNotFoundError, TimeoutError
 
 # from cbapi.live_response_api import CbLRManagerBase, WorkItem, poll_status
 
 from typing import List, Union
 
 from cbinterface.commands import BaseSessionCommand
-from cbinterface.psc.device import is_device_online
+from cbinterface.enterprise_edr.device import is_device_online
 
-LOGGER = logging.getLogger("cbinterface.psc.session")
+LOGGER = logging.getLogger("cbinterface.enterprise_edr.session")
 
 CBLR_BASE = "/integrationServices/v3/cblr"
 
 
 class CustomLiveResponseJobScheduler(LiveResponseJobScheduler):
     def __init__(self, cb, psc_cb, max_workers=10):
         self.psc_cb = psc_cb
@@ -98,20 +98,20 @@
             time.sleep(0.5)
 
         if session and is_session_active(session):
             LOGGER.info(f"got active session {session.session_id}.")
         return session
 
     def submit_command(self, command: BaseSessionCommand, device: Union[int, Device]):
-        """
-        Create a new job to be executed as a Live Response.
+        """Create a new job to be executed as a Live Response.
 
         Args:
             command (BaseSessionCommand): The job to be scheduled.
             device (Device): Device to execute job on.
+
         Returns:
             Future: A reference to the running job.
         """
         assert isinstance(command, BaseSessionCommand)
 
         device_id = device
         if isinstance(device, Device):
```

### Comparing `cbinterface-2.3.9/cbinterface/psc/cli.py` & `cbinterface-3.0.0/cbinterface/enterprise_edr/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,79 +1,85 @@
-"""PSC Threathunter CLI functions."""
+"""Enterprise EDR CLI functions."""
 
 import os
-import re
 import sys
 import argparse
 import datetime
 import logging
 import json
-import time
 import yaml
 
+from dateutil import tz
+
 from typing import List, Union
 
-from cbapi import __file__ as cbapi_file_path
-from cbapi.errors import ObjectNotFoundError, MoreThanOneResultError, ClientError
-from cbapi.psc import Device
-from cbapi.psc.devices_query import DeviceSearchQuery
-from cbapi.psc.threathunter import CbThreatHunterAPI, Process, Watchlist, Report, Feed
-from cbapi.psc.threathunter.query import Query
-
-from cbinterface.helpers import is_psc_guid, clean_exit, input_with_timeout
-from cbinterface.psc.query import make_process_query, print_facet_histogram
-from cbinterface.psc.ubs import (
+from cbc_sdk import __file__ as cbc_sdk_file_path
+from cbc_sdk.platform.devices import Device, DeviceSearchQuery
+from cbc_sdk.errors import ObjectNotFoundError, MoreThanOneResultError, ClientError
+from cbc_sdk.enterprise_edr import Watchlist, Feed
+from cbc_sdk import CBCloudAPI
+from cbc_sdk.platform import Process
+from cbinterface.helpers import is_eedr_guid, clean_exit, input_with_timeout
+from cbinterface.enterprise_edr.query import make_process_query, print_facet_histogram, yield_events
+from cbinterface.enterprise_edr.ubs import (
     request_and_get_files,
     get_file_metadata,
     get_device_summary,
     get_signature_summary,
     get_file_path_summary,
     consolidate_metadata_and_summaries,
 )
-from cbinterface.psc.intel import (
-    convert_response_watchlists_to_psc_edr_watchlists,
+from cbinterface.enterprise_edr.intel import (
+    convert_response_watchlists_to_enterprise_edr_watchlists,
     get_all_watchlists,
     get_watchlist,
     get_report,
     delete_report,
     get_report_with_IOC_status,
     print_report,
     interactively_update_report_ioc_query,
-    convert_response_watchlists_to_single_psc_edr_watchlist,
+    convert_response_watchlists_to_single_enterprise_edr_watchlist,
     get_all_feeds,
     get_feed,
     get_feed_report,
     get_alert,
-    get_all_alerts,
-    update_alert_state,
+    yield_alerts,
+    update_alert_status,
     interactively_update_alert_state,
     get_watchlists_like_name,
     search_feed_names,
+    is_ioc_ignored,
+    ignore_ioc,
+    activate_ioc,
+    create_new_report_and_append_to_watchlist,
+    write_basic_report_template,
+    backup_watchlist_threat_reports,
 )
-from cbinterface.psc.device import (
+from cbinterface.enterprise_edr.device import (
     make_device_query,
     device_info,
     time_since_checkin,
     find_device_by_hostname,
     is_device_online,
+    yield_devices,
 )
-from cbinterface.psc.process import (
-    select_process,
+from cbinterface.enterprise_edr.process import (
     print_process_info,
     print_ancestry,
     print_process_tree,
     print_modloads,
     print_filemods,
     inspect_process_tree,
     print_netconns,
     print_regmods,
     print_crossprocs,
     print_childprocs,
     print_scriptloads,
     process_to_dict,
+    format_event_data,
 )
 from cbinterface.commands import (
     PutFile,
     ProcessListing,
     GetFile,
     ListRegKeyValues,
     RegKeyValue,
@@ -86,69 +92,70 @@
     KillProcessByName,
     DeleteRegistryKeyValue,
     DeleteRegistryKey,
     SetRegKeyValue,
     CreateRegKey,
     GetSystemMemoryDump,
 )
-from cbinterface.psc.sessions import (
+from cbinterface.enterprise_edr.sessions import (
     CustomLiveResponseSessionManager,
     get_session_by_id,
     device_live_response_sessions_by_device_id,
     all_live_response_sessions,
     get_session_commands,
     get_command_result,
     get_file_content,
     close_session_by_id,
 )
-from cbinterface.psc.enumerations import logon_history
-from cbinterface.config import get_playbook_map
+from cbinterface.enterprise_edr.enumerations import logon_history
+from cbinterface.config import (
+    get_playbook_map,
+    add_watchlist_id_to_intel_backup_list,
+    remove_watchlist_id_from_intel_backup_list,
+    get_intel_backup_watchlist_list,
+)
 from cbinterface.scripted_live_response import build_playbook_commands, build_remediation_commands
 
-LOGGER = logging.getLogger("cbinterface.psc.cli")
+LOGGER = logging.getLogger("cbinterface.enterprise_edr.cli")
 
 
-def toggle_device_quarantine(
-    cb: CbThreatHunterAPI, devices: Union[DeviceSearchQuery, List[Device]], quarantine: bool
-) -> bool:
+def toggle_device_quarantine(cb: CBCloudAPI, devices: Union[DeviceSearchQuery, List[Device]], quarantine: bool) -> bool:
     """Toggle device quarantine state.
 
     Args:
         devices: DeviceSearchQuery
         quarantine: set quarantine if True, else set quarantine to off state.
     """
     if len(devices) > 0:
         if len(devices) > 10 and quarantine:
             LOGGER.error(
-                f"For now, not going to quarnantine {len(devices)} devices as a safe gaurd "
+                f"For now, not going to quarantine {len(devices)} devices as a safeguard "
                 f"to prevent mass device impact... use the GUI if you must."
             )
             return False
         verbiage = "quarantine" if quarantine else "NOT quarantine"
         emotion = "👀" if quarantine else "👏"
         LOGGER.info(f"setting {verbiage} on {len(devices)} devices... {emotion}")
 
-        device_ids = []
         for d in devices:
             if d.quarantined == quarantine:
                 LOGGER.warning(f"device {d.id}:{d.name} is already set to {verbiage}.")
                 continue
             if not is_device_online(d):
                 LOGGER.info(f"device {d.id}:{d.name} hasn't checked in for: {time_since_checkin(d, refresh=False)}")
                 LOGGER.warning(f"device {d.id}:{d.name} appears offline 💤")
                 LOGGER.info(f"device {d.id}:{d.name} will change quarantine state when it comes online 👌")
-            device_ids.append(d.id)
-            cb.device_quarantine(device_ids, quarantine)
+            cb.device_quarantine([d.id], quarantine)
         return True
 
 
-def add_psc_arguments_to_parser(subparsers: argparse.ArgumentParser) -> None:
-    """Given an argument parser subparser, build a psc specific parser."""
-    # device query (psc)
-    parser_sensor = subparsers.add_parser("device", aliases=["d"], help="Execute a device query (PSC).")
+def add_eedr_arguments_to_parser(subparsers: argparse.ArgumentParser) -> None:
+    """Given an argument parser subparser, build a EEDR specific parser."""
+    # device query
+    parser_sensor = subparsers.add_parser("device", aliases=["d"], help="Execute a device query.")
     parser_sensor.add_argument("device_query", help="the device query you'd like to execute. 'FIELDS' for help.")
     parser_sensor.add_argument(
         "-nw",
         "--no-warnings",
         action="store_true",
         default=False,
         help="Don't warn before printing large query results",
@@ -170,14 +177,20 @@
     parser_sensor.add_argument(
         "-uq",
         "--un_quarantine",
         action="store_true",
         default=False,
         help="UN-Quarantine the devices returned by the query.",
     )
+    parser_sensor.add_argument(
+        "--export",
+        action="store_true",
+        default=False,
+        help="Export devices by status. WARNING: dumps json to console! Example: `cbinterface d ALL --export` would export 'ALL' devices.",
+    )
 
     # UBS parser
     parser_ubs = subparsers.add_parser(
         "ubs", help="Interface with the Universal Binary Store (UBS) to download files and/or get information."
     )
     parser_ubs.add_argument(
         "--sha256",
@@ -231,38 +244,73 @@
         action="store_true",
         help="Combine metadata and summaries per SHA-256",
     )
 
     # intel parser
     parser_intel = subparsers.add_parser("intel", help="Intel Feeds, Watchlists, Reports, & IOCs")
     parser_intel.add_argument("--json", action="store_true", help="Return results as JSON.")
+    parser_intel.add_argument(
+        "--backup",
+        action="store_true",
+        dest="intel_backup",
+        help="Download a copy of this watchlist and its threat reports.",
+    )
+    parser_intel.add_argument(
+        "--track-watchlist-id", action="store", help="Track this watchlist via configuration for backups."
+    )
+    parser_intel.add_argument(
+        "--untrack-watchlist-id", action="store", help="Remove this watchlist from the tracking list for backups."
+    )
 
     intel_subparsers = parser_intel.add_subparsers(dest="intel_command")
 
     # intel watchlists
-    parser_intel_watchlists = intel_subparsers.add_parser("watchlists", help="Interface with PSC Watchlists.")
+    parser_intel_watchlists = intel_subparsers.add_parser(
+        "watchlists", help="Interface with Enterprise EDR Watchlists."
+    )
     parser_intel_watchlists.add_argument("-lw", "--list-watchlists", action="store_true", help="List all watchlists.")
     parser_intel_watchlists.add_argument("-w", "--get-watchlist", action="store", help="Get watchlist by ID.")
     parser_intel_watchlists.add_argument(
         "-wn", "--watchlist-name-search", action="store", help="Search for watchlists by name."
     )
     parser_intel_watchlists.add_argument(
         "-wr", "--get-watchlist-report", action="store", help="Get a watchlist report by report ID."
     )
     parser_intel_watchlists.add_argument(
         "-dr", "--delete-watchlist-report", action="store", help="Delete watchlist report by ID."
     )
     parser_intel_watchlists.add_argument(
+        "-wt",
+        "--write-basic-threat-report-template",
+        action="store_true",
+        help="Write a basic single query IOC threat report template.",
+    )
+    parser_intel_watchlists.add_argument(
         "--update-ioc-query",
         action="store",
         help="Update a query IOC for the given report ID/IOC id. format: report_id/ioc_id",
     )
+    parser_intel_watchlists.add_argument("--get-ioc-status", action="store", help="Get active/ignore status of an IOC.")
+    parser_intel_watchlists.add_argument("--ignore-ioc", action="store", help="Ignore IOC.")
+    parser_intel_watchlists.add_argument("--activate-ioc", action="store", help="Activate IOC.")
+
+    # create new threat reports for watchlists
+    parser_intel_watchlists_subparsers = parser_intel_watchlists.add_subparsers(dest="intel_watchlist_command")
+    parser_intel_watchlist_creation = parser_intel_watchlists_subparsers.add_parser(
+        "new", help="Create new Threat Report for a Watchlist."
+    )
+    parser_intel_watchlist_creation.add_argument(
+        "report_path", action="store", help="Path to JSON representation of new Threat Report."
+    )
+    parser_intel_watchlist_creation.add_argument(
+        "-w", "--watchlist-id", required=True, action="store", help="The ID of a watchlist to append to."
+    )
 
     # intel feeds
-    parser_intel_feeds = intel_subparsers.add_parser("feeds", help="Interface with PSC Feeds.")
+    parser_intel_feeds = intel_subparsers.add_parser("feeds", help="Interface with Enterprise EDR Feeds.")
     parser_intel_feeds.add_argument("-lf", "--list-feeds", action="store_true", help="List all Feeds, public included.")
     parser_intel_feeds.add_argument(
         "-f",
         "--get-feed",
         action="store",
         help="Get Feed by ID. WARNING: Can return a lot of data if using the `--json` arg.",
     )
@@ -273,109 +321,163 @@
         "-fr",
         "--get-feed-report",
         action="store",
         help="Get specific Report from specific Feed. format: feed_id/report_id",
     )
 
     # alert parser plopped in here under intel
-    parser_intel_alerts = intel_subparsers.add_parser("alerts", help="Interface with PSC Alerts.")
+    parser_intel_alerts = intel_subparsers.add_parser("alerts", help="Interface with Alerts.")
     parser_intel_alerts.add_argument(
         "-a", "--alert-id", dest="alert_ids", default=[], action="append", help="List alert IDs to work with."
     )
     parser_intel_alerts.add_argument("-g", "--get-alert", action="store_true", help="Get Alert information.")
-    parser_intel_alerts.add_argument("-d", "--dismiss-alert", action="store_true", help="Dismiss an Alerts.")
-    parser_intel_alerts.add_argument("-o", "--open-alert", action="store_true", help="Set Alerts to Open (un-dismiss).")
     parser_intel_alerts.add_argument(
-        "-u", "--interactively-update-alert", action="store_true", help="Update Alerts interactively."
+        "-s",
+        "--alerts-status",
+        action="store",
+        choices=["OPEN", "IN_PROGRESS", "CLOSED"],
+        help="Set the status of Alerts.",
+    )
+    parser_intel_alerts.add_argument(
+        "-d",
+        "--determination",
+        action="store",
+        choices=["TRUE_POSITIVE", "FALSE_POSITIVE", "NONE"],
+        help="Set the determination of Alerts. (Optional)",
     )
+
     parser_intel_alerts.add_argument(
         "-r",
-        "--remediation-state",
+        "--closure-reason",
         action="store",
-        help="An Alert remediation state to use with any state change actions.",
+        choices=["NO_REASON", "RESOLVED", "RESOLVED_BENIGN_KNOWN_GOOD", "DUPLICATE_CLEANUP", "OTHER"],
+        help="Reason code for why the Alerts are being updated. (Optional)",
+    )
+    parser_intel_alerts.add_argument(
+        "-n", "--note", action="store", help="Custom message to add to the note added to each modified aler. (Optional)"
     )
     parser_intel_alerts.add_argument(
-        "-c", "--comment", action="store", help="An Alert comment to use with any state change actions."
+        "-u", "--interactively-update-alert", action="store_true", help="Update Alerts interactively."
     )
     parser_intel_alerts.add_argument(
         "--from-stdin", action="store_true", help="Read alert IDs from stdin to work with."
     )
 
     intel_alerts_subparsers = parser_intel_alerts.add_subparsers(dest="intel_alerts_command")
     # alert search parser
     parser_intel_alerts_search = intel_alerts_subparsers.add_parser(
         "search", help="Search Alerts with lucene syntax queries and/or value searches."
     )
-    parser_intel_alerts_search.add_argument("alert_query", action="store", help="The Alert search query.")
-    # TODO Add other arguments to allow for searching via start & end times, specifying rows, start, alert state
     parser_intel_alerts_search.add_argument(
-        "-cr",
-        "--create_time-range",
+        "alert_query",
         action="store",
-        help="Only return alerts created over the previous time range. format:integer_quantity,time_unit ; time_unit in [s,m,h,d,w,y]",
+        help="The lucene-formatted Alert search query. Example: 'watchlists_id:a1B2c3D4zxc AND workflow_status:OPEN'",
     )
     parser_intel_alerts_search.add_argument(
-        "-m",
-        "--max-alerts-result",
+        "-rt",
+        "--relative-time-range",
+        action="store",
+        help="Only return alerts created over the previous time range. Format: <integer_quantity><time_units>; time_units in [M, w, d, h, m, s]. Default=2w",
+    )
+    parser_intel_alerts_search.add_argument(
+        "-et",
+        "--explicit-time-range",
+        action="store",
+        help="Need to specify both start and end timestamps (ISO 8601) separated by a comma. Example: '2024-04-01T01:02:30.000Z,2024-04-03T04:05:06.000Z'",
+    )
+    parser_intel_alerts_search.add_argument(
+        "-c",
+        "--criteria",
+        action="store",
+        type=json.loads,
+        help='Add criteria to the query. Example: \'{"device_os": ["WINDOWS"]}\'',
+    )
+    parser_intel_alerts_search.add_argument(
+        "-ex",
+        "--exclusions",
+        action="store",
+        type=json.loads,
+        help='Add exclusions to the query. Example: \'{"device_location": ["UNKNOWN"], "device_os_version": ["Windows 11 x64"}]\'',
+    )
+    parser_intel_alerts_search.add_argument(
+        "-so",
+        "--sort",
+        action="store",
+        default=[{"field": "backend_update_timestamp", "order": "ASC"}],
+        type=json.loads,
+        help='Sort the results. Default=\'[{"field": "backend_update_timestamp", "order": "ASC"}]\'',
+    )
+    parser_intel_alerts_search.add_argument(
+        "-st",
+        "--pagination-start",
+        action="store",
+        default=1,
+        type=int,
+        help="One-based index of the first result to retrieve. Must be a whole number greater than or equal to 1. Default=1",
+    )
+    parser_intel_alerts_search.add_argument(
+        "-r",
+        "--rows",
         action="store",
         default=100,
         type=int,
-        help="Only return up to this many alerts. Default=100. HINT: set to '0' to return all results.",
+        help="The number of rows to return starting from the pagination start. Increase this value in large queries to reduce waiting time. Default=100",
     )
     parser_intel_alerts_search.add_argument(
-        "-as",
-        "--alert-states",
-        action="append",
-        choices=["DISMISSED", "OPEN"],
-        help="Only return Alerts in these states.",
+        "-m",
+        "--max-alerts-result",
+        action="store",
+        default=500,
+        type=int,
+        help="Only return up to this many alerts. The maximum number of alerts is 10000. Default=500",
     )
-
-    # cb response to psc migration parser
+    # cb response to enterprise edr migration parser
     parser_intel_migration = intel_subparsers.add_parser(
-        "migrate", help="Utilities for migrating response watchlists to PSC EDR intel."
+        "migrate", help="Utilities for migrating response watchlists to Enterprise EDR intel."
     )
     parser_intel_migration.add_argument(
         "response_watchlist_json_data_path",
         help="Path to response watchlist json file. (see cbinterface response_watchlist",
     )
     parser_intel_migration.add_argument(
         "--one-for-one",
         action="store_true",
-        help="Create a PSC Watchlist for every CbR watchlist that passes validation.",
+        help="Create a Enterprise EDR Watchlist for every CbR watchlist that passes validation.",
     )
     parser_intel_migration.add_argument(
         "--many-to-one",
         action="store_true",
-        help="Create a single PSC Watchlist containing all CbR watchlist queries that pass validation.",
+        help="Create a single Enterprise EDR Watchlist containing all CbR watchlist queries that pass validation.",
     )
 
 
-def execute_threathunter_arguments(cb: CbThreatHunterAPI, args: argparse.Namespace) -> bool:
-    """The logic to execute psc ThreatHunter specific command line arguments.
+def execute_eedr_arguments(cb: CBCloudAPI, args: argparse.Namespace) -> bool:
+    """The logic to execute EEDR specific command line arguments.
 
     Args:
-        cb: CbThreatHunterAPI
+        cb: CBCloudAPI
         args: parsed argparse namespace
+
     Returns:
         True or None on success, False on failure.
     """
-    if not isinstance(cb, CbThreatHunterAPI):
-        LOGGER.critical(f"Requires Cb PSC based API. Got '{product}' API.")
+    if not isinstance(cb, CBCloudAPI):
+        LOGGER.critical(f"Requires Cb Enterprise EDR based API. Got '{args.product}' API.")
         return False
 
     # UBS #
     if args.command == "ubs":
         if args.from_stdin:
             args.sha256hashes.extend([line.strip() for line in sys.stdin])
 
         if args.sha256hashes:
 
             set_ubs_args = [arg for arg, value in vars(args).items() if arg.startswith("ubs_") and value is True]
             if not set_ubs_args:
-                LOGGER.debug(f"seting ubs metadata argument as default.")
+                LOGGER.debug("seting ubs metadata argument as default.")
                 args.ubs_get_metadata = True
 
             if args.ubs_get_file:
                 request_and_get_files(cb, sha256hashes=args.sha256hashes)
             if args.ubs_get_device_summary:
                 summary = get_device_summary(cb, args.sha256hashes)
                 if summary:
@@ -394,100 +496,135 @@
                 if file_metadata:
                     print(json.dumps(file_metadata, indent=2))
             if args.ubs_combined_info:
                 results = consolidate_metadata_and_summaries(cb, args.sha256hashes)
                 if results:
                     print(json.dumps(results, indent=2))
         else:
-            LOGGER.error(f"You must specify at least one sha256 with the `--sha256` argument.")
+            LOGGER.error("You must specify at least one sha256 with the `--sha256` argument.")
             return False
 
         return True
 
     # Intel #
     if args.command == "intel":
+        if args.intel_backup:
+            watchlist_ids = get_intel_backup_watchlist_list()
+            if not watchlist_ids:
+                LOGGER.info("No watchlists configured for intel backup tracking.")
+                return None
+            return backup_watchlist_threat_reports(cb, watchlist_ids)
+        if args.track_watchlist_id:
+            return add_watchlist_id_to_intel_backup_list(args.track_watchlist_id)
+        if args.untrack_watchlist_id:
+            return remove_watchlist_id_from_intel_backup_list(args.untrack_watchlist_id)
+
         if args.intel_command == "alerts":
 
-            if args.intel_alerts_command == "search":  #'device_name': ['XW7R17'],
-                # NOTE TODO: implement start and end time argparse options
-                # criteria = {'last_event_time': {'start': '2021-04-13T19:39:30.054855+00:00', 'end': '2021-04-14T19:39:30.054855+00:00'}, 'workflow': ['OPEN']}
-                if args.create_time_range:
-                    criteria["create_time"] = {"range": f"-{args.create_time_range}"}
-                results = get_all_alerts(
-                    cb, query=args.alert_query, workflow_state=args.alert_states, max_results=args.max_alerts_result
+            if args.intel_alerts_command == "search":
+                if args.relative_time_range and args.explicit_time_range:
+                    logging.error("You can only use either explicit or relative time range. Try again.")
+                    return False
+                time_range = None
+                if args.relative_time_range:
+                    time_range = {"range": f"-{args.relative_time_range}"}
+                elif args.explicit_time_range:
+                    start, end = args.explicit_time_range.split(",")
+                    time_range = {"start": start.strip(), "end": end.strip()}
+                results = list(
+                    yield_alerts(
+                        cb,
+                        args.alert_query,
+                        time_range,
+                        args.criteria,
+                        args.exclusions,
+                        args.sort,
+                        args.pagination_start,
+                        args.rows,
+                        args.max_alerts_result,
+                    )
                 )
                 if results:
                     print(json.dumps(results, indent=2))
+                    print(f"\nTotal alerts {len(results)}")
 
                 return True
 
             if args.from_stdin:
                 args.alert_ids.extend([line.strip().strip('"') for line in sys.stdin])
 
             if not args.alert_ids:
-                LOGGER.error(f"You have to supply at least one alert ID.")
+                LOGGER.error("You have to supply at least one alert ID.")
                 return False
 
             if args.get_alert:
                 alerts = [get_alert(cb, alert_id) for alert_id in args.alert_ids]
                 if alerts:
                     print(json.dumps(alerts, indent=2))
 
-            if args.open_alert:
-                results = [
-                    update_alert_state(
-                        cb, alert_id, state="OPEN", remediation_state=args.remediation_state, comment=args.comment
-                    )
-                    for alert_id in args.alert_ids
-                ]
-                if result:
-                    print(json.dumps(results, indent=2))
-
-            if args.dismiss_alert:
-                results = [
-                    update_alert_state(
-                        cb,
-                        alert_id,
-                        state="DISMISSED",
-                        remediation_state=args.remediation_state,
-                        comment=args.comment,
-                    )
-                    for alert_id in args.alert_ids
-                ]
+            if args.alerts_status:
+                results = update_alert_status(
+                    cb,
+                    args.alert_ids,
+                    status=args.alerts_status,
+                    determination=args.determination,
+                    closure_reason=args.closure_reason,
+                    note=args.note,
+                )
                 if results:
                     print(json.dumps(results, indent=2))
 
             if args.interactively_update_alert:
                 results = [interactively_update_alert_state(cb, alert_id) for alert_id in args.alert_ids]
                 if results:
                     print(json.dumps(results, indent=2))
 
         if args.intel_command == "migrate":
             response_watchlists = None
             with open(args.response_watchlist_json_data_path, "r") as fp:
                 response_watchlists = json.load(fp)
 
             if args.one_for_one:
-                results = convert_response_watchlists_to_psc_edr_watchlists(cb, response_watchlists)
+                results = convert_response_watchlists_to_enterprise_edr_watchlists(cb, response_watchlists)
                 LOGGER.info(
-                    f"created {len(results)} PSC watchlists from {len(response_watchlists)} Response watchlists."
+                    f"created {len(results)} Enterprise EDR watchlists from {len(response_watchlists)} Response watchlists."
                 )
                 print("Created watchlists:")
                 for wl in results:
                     print(f" + ID={wl['id']} - Title={wl['name']}")
 
             if args.many_to_one:
-                watchlist = convert_response_watchlists_to_single_psc_edr_watchlist(cb, response_watchlists)
+                watchlist = convert_response_watchlists_to_single_enterprise_edr_watchlist(cb, response_watchlists)
                 if not watchlist:
                     return False
                 LOGGER.info(
                     f"Created \"{watchlist['name']}\" containing {len(watchlist['report_ids'])} intel reports based on {len(response_watchlists)} Response watchlists."
                 )
 
         if args.intel_command == "watchlists":
+            if args.intel_watchlist_command == "new":
+                report_data = {}
+                if not os.path.exists(args.report_path):
+                    LOGGER.error(f"{args.report_path} does not exist.")
+                    return False
+                with open(args.report_path, "r") as fp:
+                    report_data = json.load(fp)
+                if not report_data:
+                    LOGGER.error("failed to load report data")
+                    return False
+                watchlist_data = create_new_report_and_append_to_watchlist(cb, args.watchlist_id, report_data)
+                if watchlist_data:
+                    return True
+
+            if args.write_basic_threat_report_template:
+                result = write_basic_report_template()
+                if result:
+                    LOGGER.info(f"wrote: {result}")
+                return result
+
             if args.list_watchlists:
                 watchlists = get_all_watchlists(cb)
                 if args.json:
                     print(json.dumps(watchlists, indent=2))
                 else:
                     for wl in watchlists:
                         print(Watchlist(cb, initial_data=wl))
@@ -515,34 +652,53 @@
                     report = get_report_with_IOC_status(cb, args.get_watchlist_report)
                     if report:
                         print_report(report)  # specifically helpful with query based IOCs
 
             if args.delete_watchlist_report:
                 result = delete_report(cb, args.delete_watchlist_report)
                 if result.status_code == 204:
-                    LOGGER.info(f"deleted watchlist report")
+                    LOGGER.info("deleted watchlist report")
 
             if args.update_ioc_query:
                 report_id, ioc_id = args.update_ioc_query.split("/", 1)
                 updated_report = interactively_update_report_ioc_query(cb, report_id, ioc_id)
                 if updated_report:
                     LOGGER.info(f"Query IOC ID={ioc_id} of report ID={report_id} successfully updated.")
 
+            if args.get_ioc_status:
+                report_id, ioc_id = args.get_ioc_status.split("/", 1)
+                status = is_ioc_ignored(cb, report_id, ioc_id, check_existence=True)
+                if status is None:
+                    return False
+                status = "IGNORED" if status else "ACTIVE"
+                print(f"IOC ID={ioc_id} in Report ID={report_id} is {status}")
+
+            if args.ignore_ioc:
+                report_id, ioc_id = args.ignore_ioc.split("/", 1)
+                status = ignore_ioc(cb, report_id, ioc_id)
+                status = "IGNORED" if status else "ACTIVE"
+                print(f"IOC ID={ioc_id} in Report ID={report_id} is {status}")
+
+            if args.activate_ioc:
+                report_id, ioc_id = args.activate_ioc.split("/", 1)
+                status = activate_ioc(cb, report_id, ioc_id)
+                status = "ACTIVE" if status else "IGNORED"
+                print(f"IOC ID={ioc_id} in Report ID={report_id} is {status}")
+
         if args.intel_command == "feeds":
             if args.list_feeds:
                 feeds = get_all_feeds(cb)
                 if not feeds:
                     return None
                 if args.json:
                     print(json.dumps(feeds, indent=2))
                 else:
                     for f in feeds:
                         print(Feed(cb, initial_data=f))
                         print()
-
             if args.get_feed:
                 feed = get_feed(cb, args.get_feed)
                 if not feed:
                     return None
                 if args.json:
                     print(json.dumps(feed, indent=2))
                 else:
@@ -565,32 +721,42 @@
                 except ValueError:
                     feed_id, report_id = args.get_feed_report.split("-", 1)
                 report = get_feed_report(cb, feed_id, report_id)
                 print(json.dumps(report, indent=2))
 
         return True
 
-    # Device Quering #
+    # Device Querying #
     if args.command and args.command.startswith("d"):
         LOGGER.info(f"searching {args.environment} environment for device query: {args.device_query}...")
         if args.device_query.upper() == "FIELDS":
-            device_meta_file = os.path.join(os.path.dirname(cbapi_file_path), "psc/defense/models/deviceInfo.yaml")
+            device_meta_file = os.path.join(os.path.dirname(cbc_sdk_file_path), "platform/models/device.yaml")
             model_data = {}
             with open(device_meta_file, "r") as fp:
                 model_data = yaml.safe_load(fp.read())
-            possibly_searchable_props = list(model_data["properties"].keys())
             print("Device model fields:")
             for field_name in list(model_data["properties"].keys()):
                 print(f"\t{field_name}")
             return True
 
         if args.quarantine and args.un_quarantine:
             LOGGER.error("quarantine AND un-quarantine? 🤨 Won't do it.")
             return False
 
+        if args.export:
+            # NOTE: TODO: update device search functionality to use the new direct api method and
+            LOGGER.info(f"attempting to export devices resulting from query: {args.device_query}")
+
+            devices = [device for device in yield_devices(cb, query=args.device_query)]
+            if not devices:
+                LOGGER.warning("No devices returned.")
+                return devices
+            print(json.dumps(devices))
+            return True
+
         devices = make_device_query(cb, args.device_query)
         if not devices:
             return None
 
         # Quarantine?
         if args.quarantine:
             toggle_device_quarantine(cb, devices, True)
@@ -601,42 +767,67 @@
         print_results = True
         if not args.no_warnings and len(devices) > 10:
             prompt = "Print all results? (y/n) [y] "
             print_results = input_with_timeout(prompt, default="y")
             print_results = True if print_results.lower() == "y" else False
 
         if len(devices) > 0 and print_results:
-            print("\n------------------------- PSC DEVICE RESULTS -------------------------")
+            print("\n------------------------- ENTERPRISE EDR DEVICE RESULTS -------------------------")
             for device in devices:
                 if args.all_details:
                     print()
                     print(device)
+                # elif args.json:
+                #    print(json.dumps(device._info, indent=2))
                 else:
                     print(device_info(device))
             print()
         return True
 
-    # Process Quering #
+    # Process Querying #
     if args.command and (args.command.startswith("q") or args.command == "pq"):
         LOGGER.info(f"searching {args.environment} environment..")
+
+        # format datetimes as needed
+        format_string = "%Y-%m-%d %H:%M:%S"
+        if args.start_time and "T" in args.start_time or args.last_time and "T" in args.last_time:
+            format_string = "%Y-%m-%dT%H:%M:%S"
         args.start_time = (
-            datetime.datetime.strptime(args.start_time, "%Y-%m-%d %H:%M:%S") if args.start_time else args.start_time
+            datetime.datetime.strptime(args.start_time, format_string) if args.start_time else args.start_time
         )
-        args.last_time = (
-            datetime.datetime.strptime(args.last_time, "%Y-%m-%d %H:%M:%S") if args.last_time else args.last_time
+        args.last_time = datetime.datetime.strptime(args.last_time, format_string) if args.last_time else args.last_time
+        processes = make_process_query(
+            cb,
+            args.query,
+            fields=[
+                "*",
+                "device_os",
+                "device_external_ip",
+                "device_internal_ip",
+                "parent_hash",
+                "parent_name",
+                "process_reputation",
+                "process_start_time",
+                "process_cmdline",
+                "parent_guid",
+            ],
+            start_time=args.start_time,
+            last_time=args.last_time,
+            raise_exceptions=True,
+            validate_query=True,
         )
-        processes = make_process_query(cb, args.query, start_time=args.start_time, last_time=args.last_time)
 
         if args.facets:
             LOGGER.info("getting facet data...")
-            print_facet_histogram(processes)
+            # print_facet_histogram(processes) - unvailable with CBC SDK
             # NOTE TODO - pick this v2 back up and see if it's more efficient to use
             # knowing we have to remember the childproc_name facet data we like.
-            # from cbinterface.psc.query import print_facet_histogram_v2
-            # print_facet_histogram_v2(cb, args.query)
+            from cbinterface.enterprise_edr.query import print_facet_histogram_v2
+
+            print_facet_histogram_v2(cb, args.query, args.start_time, args.last_time)
 
         # don't display large results by default
         print_results = True
         if not args.no_warnings and len(processes) > 10:
             prompt = "Print all results? (y/n) [y] "
             print_results = input_with_timeout(prompt, default="y")
             print_results = True if print_results.lower() == "y" else False
@@ -649,106 +840,157 @@
                     print(proc)
                 else:
                     print_process_info(proc, raw_print=args.all_details, header=False)
 
         return True
 
     # Enumerations #
-    if args.command and args.command == "enumerate":
+    if args.command and args.command in ["enumerate", "e"]:
         if args.logon_history:
             logon_history(cb, args.logon_history)
             return
 
     # Process Inspection #
     if args.command and (args.command == "proc" or args.command.startswith("i")):
         process_id = args.process_guid_options
-        if not is_psc_guid(process_id):
+        if not is_eedr_guid(process_id):
             # check to see if the analyst passed a local file path, which we assume is a local process json file
             # if os.path.exists(args.process_guid_options):
             # XXX NOTE: create functionality sourced from process json file?
-            LOGGER.error(f"{process_id} is not in the form of a CbThreathunter process guid.")
+            LOGGER.error(f"{process_id} is not in the form of a CB Cloud process guid.")
             return False
 
         try:
-            # proc = Process(cb, process_id)
-            proc = select_process(cb, process_id)
+            proc = make_process_query(
+                cb,
+                f"process_guid:{process_id}",
+                fields=[
+                    "*",
+                    "device_os",
+                    "device_external_ip",
+                    "device_internal_ip",
+                    "parent_hash",
+                    "parent_name",
+                    "process_reputation",
+                    "process_start_time",
+                    "process_cmdline",
+                    "process_terminated",
+                ],
+                raise_exceptions=True,
+                validate_query=False,
+                silent=True,
+            ).first()
             if not proc:
                 LOGGER.warning(f"Process data does not exist for GUID={process_id}")
                 return False
         except Exception as e:
             LOGGER.error(f"unexpected problem finding process: {e}")
             return False
 
+        # format datetimes as needed
+        format_string = "%Y-%m-%d %H:%M:%S"
+        if args.start_time and "T" in args.start_time or args.end_time and "T" in args.end_time:
+            format_string = "%Y-%m-%dT%H:%M:%S"
+        args.start_time = (
+            datetime.datetime.strptime(args.start_time, format_string).replace(tzinfo=tz.gettz("GMT"))
+            if args.start_time
+            else args.start_time
+        )
+        args.end_time = (
+            datetime.datetime.strptime(args.end_time, format_string).replace(tzinfo=tz.gettz("GMT"))
+            if args.end_time
+            else args.end_time
+        )
+
+        if args.event_search:
+            for event in yield_events(
+                proc, query=args.event_search, start_time=args.start_time, end_time=args.end_time
+            ):
+                if args.raw_print_events:
+                    print(json.dumps(event, default=str, indent=2, sort_keys=True))
+                else:
+                    print(format_event_data(event))
+            return True
+
+        if args.json:
+            print(
+                json.dumps(
+                    process_to_dict(proc, start_time=args.start_time, end_time=args.end_time, event_rows=2000),
+                    default=str,
+                )
+            )
+            return
+
         all_inspection_args = [iarg for iarg in vars(args).keys() if iarg.startswith("inspect_")]
         set_inspection_args = [
             iarg for iarg, value in vars(args).items() if iarg.startswith("inspect_") and value is True
         ]
         if not set_inspection_args:
-            LOGGER.debug(f"seting all inspection arguments.")
+            LOGGER.debug("seting all inspection arguments.")
             for iarg in all_inspection_args:
                 args.__setattr__(iarg, True)
 
-        if args.json:
-            print(json.dumps(process_to_dict(proc), default=str))
-            return
-
         if args.walk_and_inspect_tree:
             inspect_process_tree(
                 proc,
                 info=args.inspect_proc_info,
                 filemods=args.inspect_filemods,
                 netconns=args.inspect_netconns,
                 regmods=args.inspect_regmods,
                 modloads=args.inspect_modloads,
                 crossprocs=args.inspect_crossprocs,
                 children=args.inspect_children,
                 scriptloads=args.inspect_scriptloads,
                 raw_print=args.raw_print_events,
+                start_time=args.start_time,
+                end_time=args.end_time,
             )
             return True
 
         if args.inspect_process_ancestry:
             print_ancestry(proc)
             print()
         if args.inspect_process_tree:
-            print_process_tree(proc)
+            print_process_tree(proc, start_time=args.start_time, end_time=args.end_time)
             print()
         if args.inspect_proc_info:
             print_process_info(proc, raw_print=args.raw_print_events)
         if args.inspect_filemods:
-            print_filemods(proc, raw_print=args.raw_print_events)
+            print_filemods(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_netconns:
-            print_netconns(proc, raw_print=args.raw_print_events)
+            print_netconns(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_regmods:
-            print_regmods(proc, raw_print=args.raw_print_events)
+            print_regmods(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_modloads:
-            print_modloads(proc, raw_print=args.raw_print_events)
+            print_modloads(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_crossprocs:
-            print_crossprocs(proc, raw_print=args.raw_print_events)
+            print_crossprocs(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_children:
-            print_childprocs(proc, raw_print=args.raw_print_events)
+            print_childprocs(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
         if args.inspect_scriptloads:
-            print_scriptloads(proc, raw_print=args.raw_print_events)
+            print_scriptloads(proc, raw_print=args.raw_print_events, start_time=args.start_time, end_time=args.end_time)
+
+        return True
 
     # Live Response Actions #
     if args.command and (args.command.lower() == "lr" or args.command.lower().startswith("live")):
         # create a LR session manager
         session_manager = CustomLiveResponseSessionManager(cb, custom_session_keepalive=True)
         # store a list of commands to execute on this device
         commands = []
 
-        LOGGER.info(f"searching for device...")
+        LOGGER.info("searching for device...")
         device = None
         try:  # if device.id
             device = Device(cb, args.name_or_id)
         except ClientError:
             device = find_device_by_hostname(cb, args.name_or_id)
 
         if not device:
-            LOGGER.info(f"could not find a device.")
+            LOGGER.info("could not find a device.")
             return None
 
         if args.execute_command:
             # XXX expand this for more flexibiliy by making an execute parser
             # that can accept more arugments to pass to ExecuteCommand
             cmd = ExecuteCommand(args.execute_command)
             commands.append(cmd)
@@ -883,33 +1125,33 @@
                     LOGGER.warning(f"{timeout} days is a long time. Restricting to max of 30 days.")
                     timeout = 30
 
                 # 86400 seconds in a day
                 timeout = timeout * 86400
 
             if not session_manager.wait_for_active_session(device, timeout=timeout):
-                LOGGER.error(f"reached timeout waiting for active session.")
+                LOGGER.error("reached timeout waiting for active session.")
                 return False
 
             # we have an active session, issue the commands.
             for command in commands:
                 session_manager.submit_command(command, device)
 
         if session_manager.commands:
             # Wait for issued commands to complete and process any results.
             session_manager.process_completed_commands()
 
     # Direct Session Interaction #
     if args.command and args.command.startswith("sess"):
-        cblr = CbThreatHunterAPI(url=cb.credentials.url, token=cb.credentials.lr_token, org_key=cb.credentials.org_key)
+        cblr = CBCloudAPI(url=cb.credentials.url, token=cb.credentials.lr_token, org_key=cb.credentials.org_key)
 
         # if args.list_all_sessions:
-        # Not implemented with PSC
+        # Not implemented with Enterprise EDR
         # if args.list_sensor_sessions:
-        # Not implemented with PSC
+        # Not implemented with Enterprise EDR
 
         if args.get_session_command_list:
             print(json.dumps(get_session_commands(cblr, args.get_session_command_list), indent=2, sort_keys=True))
 
         if args.get_session:
             print(json.dumps(get_session_by_id(cblr, args.get_session), indent=2, sort_keys=True))
```

### Comparing `cbinterface-2.3.9/cbinterface/psc/enumerations.py` & `cbinterface-3.0.0/cbinterface/enterprise_edr/enumerations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 """Functions for enumerations or correlations.
 
 Example, enumerating USB activity on a sensor from a programatic
 analysis of registry modifications.
 """
+
 import os
 import logging
 
-from cbapi.psc.rest_api import CbPSCBaseAPI
+from cbc_sdk import CBCloudAPI
 
 from cbinterface.helpers import as_configured_timezone
 
 
-LOGGER = logging.getLogger("cbinterface.psc.enumerations")
+LOGGER = logging.getLogger("cbinterface.enterprise_edr.enumerations")
 
 
-def search_for_usb_devices(cb: CbPSCBaseAPI, query):
+def search_for_usb_devices(cb: CBCloudAPI, query):
     # XXX - This doesn't look implemented in TH?
     uri = f"/device_control/v3/orgs/{cb.credentials.org_key}/devices/_search"
     data = {"query": query}
     return cb.post_object(uri, data).json()
 
 
-def logon_history(cb: CbPSCBaseAPI, hostname_or_username_query) -> None:
+def logon_history(cb: CBCloudAPI, hostname_or_username_query) -> None:
     """Given hostname or username, enumerate logon history.
 
     Note, this is an analysis of the WINDOWS behavior when a new user
     session is started. It's informative for analysts, not authoritative.
     It will NOT show processes ran under other users, as often is the case
     with enterprise admin activity.
     """
-    from cbinterface.psc.query import make_process_query
+    from cbinterface.enterprise_edr.query import make_process_query
 
     if not (
         hostname_or_username_query.startswith("device_name:")
         or hostname_or_username_query.startswith("process_username:")
     ):
-        LOGGER.info(f"use 'device_name:' or 'process_username:' field to narrow enumeration search.")
+        LOGGER.info("use 'device_name:' or 'process_username:' field to narrow enumeration search.")
 
     # query = f"process_name:userinit.exe parent_name:winlogon.exe {hostname_or_username_query}"
     # XXX will catch more than "log on"
     query = f"process_name:explorer.exe {hostname_or_username_query}"
 
     processes = make_process_query(cb, query)
     if processes and len(processes) > 0:
         timezone_string = os.environ.get("CBINTERFACE_TIMEZONE", "GMT")
-        print(f"\n\t{timezone_string} Time    \t|\tUsername\t|\tHostname")
+        print(f"\n\t{timezone_string} Time        \t|\tUsername\t|\tHostname")
         for proc in processes:
             start_time = as_configured_timezone(proc.process_start_time, apply_time_format="%Y-%m-%d %H:%M:%S%z")
             username = proc.process_username[0]
-            print("  {}\t    {}\t\t{}".format(start_time, username, proc.device_name))
+            print("  {}\t     {}\t\t{}".format(start_time, username, proc.device_name))
         print()
     return
```

### Comparing `cbinterface-2.3.9/cbinterface/scripted_live_response.py` & `cbinterface-3.0.0/cbinterface/scripted_live_response.py`

 * *Files identical despite different names*

### Comparing `cbinterface-2.3.9/cbinterface/cli.py` & `cbinterface-3.0.0/cbinterface/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,85 +1,93 @@
 # PYTHON_ARGCOMPLETE_OK
 
 import os
-import re
-
-import time
 import argparse
 import argcomplete
 import logging
 import coloredlogs
-import datetime
-import json
+
 import signal
-import yaml
 
 import cbapi.auth
-from cbapi.psc.threathunter import CbThreatHunterAPI
+from cbc_sdk import CBCloudAPI
 from cbapi.response import CbResponseAPI
-from cbapi.errors import ConnectionError, UnauthorizedError, ServerError
+from cbc_sdk.errors import ConnectionError, UnauthorizedError, ServerError, CredentialError
 
-from cbinterface.helpers import is_uuid, clean_exit, input_with_timeout
+from cbinterface.helpers import clean_exit
 from cbinterface.config import (
     set_timezone,
     save_configuration,
-    get_default_cbapi_product,
-    get_default_cbapi_profile,
-    set_default_cbapi_profile,
-    set_default_cbapi_product,
+    get_default_cb_product,
+    get_default_cb_profile,
+    set_default_cb_profile,
+    set_default_cb_product,
     get_playbook_map,
 )
 
 from cbinterface.response.cli import add_response_arguments_to_parser, execute_response_arguments
-from cbinterface.psc.cli import add_psc_arguments_to_parser, execute_threathunter_arguments
+from cbinterface.enterprise_edr.cli import add_eedr_arguments_to_parser, execute_eedr_arguments
 from cbinterface.scripted_live_response import write_playbook_template, write_remediation_template
 
 LOGGER = logging.getLogger("cbinterface.cli")
 
+SUPPORTED_PRODUCTS = ["response", "psc"]
+
+
+def load_configured_environments():
+    """Load Carbon Black environments from config files."""
+    configured_environments = {}
+    for product in SUPPORTED_PRODUCTS:
+        configured_environments[product] = []
+        for profile in cbapi.auth.FileCredentialStore(product).get_profiles():
+            configured_environments[product].append(profile)
+    # PSC was renamed to Enterprise EDR...
+    if "psc" in configured_environments.keys():
+        configured_environments["enterprise_edr"] = configured_environments.pop("psc")
+    return configured_environments
+
 
 def main():
     """Main entry point for cbinterface."""
-
     # configure logging #
-    logging.basicConfig(level=logging.INFO, format="%(asctime)s - %(name)s - [%(levelname)s] %(message)s")
-    coloredlogs.install(level="INFO", logger=logging.getLogger())
+    logging.basicConfig(level=logging.INFO, format="%(asctime)s %(name)s:%(lineno)d %(levelname)s %(message)s")
+    coloredlogs.install(
+        level="INFO",
+        logger=logging.getLogger(),
+        fmt="%(asctime)s %(name)s:%(lineno)d %(levelname)s %(message)s",
+    )
 
     # set clean exit signal
     signal.signal(signal.SIGINT, clean_exit)
 
     # load carbonblack environment profiles #
-
-    # set custom attributes
-    default_profile = cbapi.auth.default_profile
-    default_profile["lr_token"] = None  # needed for psc
-
-    # locate configured environments
-    supported_products = ["response", "psc"]
+    configured_environments = load_configured_environments()
     environments = []
-    configured_products = {}
-    for product in supported_products:
-        configured_products[product] = False
-        # FileCredentialStore loads `default_profile`
-        for profile in cbapi.auth.FileCredentialStore(product).get_profiles():
-            configured_products[product] = True
+    # create human friendly options for the CLI
+    for product, profiles in configured_environments.items():
+        for profile in profiles:
             environments.append(f"{product}:{profile}")
 
     # chose the default environment
-    default_product_name = get_default_cbapi_product()
-    default_profile_name = get_default_cbapi_profile()
+    default_product_name = get_default_cb_product()
+    default_profile_name = get_default_cb_profile()
     default_environments = [env for env in environments if env.startswith(default_product_name)]
     default_environment = f"{default_product_name}:{default_profile_name}"
-    default_environment = (
-        default_environment if default_environments and default_environment in default_environments else environments[0]
-    )
-
+    if environments:
+        default_environment = (
+            default_environment
+            if default_environments and default_environment in default_environments
+            else environments[0]
+        )
+    else:
+        LOGGER.warning("no carbon black configurations found.")
     parser = argparse.ArgumentParser(description="Interface to Carbon Black for IDR teams.")
     parser.add_argument("-d", "--debug", action="store_true", help="Turn on debug logging.")
     parser.add_argument(
-        "-e",
+        "-env",
         "--environment",
         action="store",
         choices=environments,
         default=default_environment,
         help=f"specify an environment to work with. Default={default_environment}",
     )
     parser.add_argument(
@@ -108,21 +116,21 @@
         "query", aliases=["pq", "q"], help="Execute a process search query. 'query -h' for more"
     )
     parser_query.add_argument("query", help="the process search query you'd like to execute")
     parser_query.add_argument(
         "-s",
         "--start-time",
         action="store",
-        help="Start time of the process.  Format:'Y-m-d H:M:S' UTC",
+        help="Start time of the process.  Format:'Y-m-d H:M:S' OR 'Y-m-dTH:M:S' UTC",
     )
     parser_query.add_argument(
         "-e",
         "--last-time",
         action="store",
-        help="Narrow to processes with start times BEFORE this end/last time. Format:'Y-m-d H:M:S' UTC",
+        help="Narrow to processes with start times BEFORE this end/last time. Format:'Y-m-d H:M:S' OR 'Y-m-dTH:M:S' UTC",
     )
     parser_query.add_argument(
         "-nw",
         "--no-warnings",
         action="store_true",
         default=False,
         help="Don't warn before printing large query results",
@@ -185,15 +193,19 @@
     parser_inspect.add_argument(
         "-rm", "--regmods", dest="inspect_regmods", action="store_true", help="print registry modifications"
     )
     parser_inspect.add_argument(
         "-ml", "--modloads", dest="inspect_modloads", action="store_true", help="print modloads"
     )
     parser_inspect.add_argument(
-        "-sl", "--scriptloads", dest="inspect_scriptloads", action="store_true", help="print scriptloads (PSC)"
+        "-sl",
+        "--scriptloads",
+        dest="inspect_scriptloads",
+        action="store_true",
+        help="print scriptloads (Enterprise EDR)",
     )
     parser_inspect.add_argument(
         "-cp", "--crossprocs", dest="inspect_crossprocs", action="store_true", help="print crossprocs"
     )
     parser_inspect.add_argument(
         "-rpe",
         "--raw-print-events",
@@ -209,46 +221,59 @@
     parser_inspect.add_argument(
         "--segment-limit",
         action="store",
         type=int,
         default=None,
         help="stop processing events into json after this many process segments",
     )
+    parser_inspect.add_argument("-es", "--event-search", action="store", help="Search process events.")
+    parser_inspect.add_argument(
+        "-st",
+        "--start-time",
+        action="store",
+        help="Return events that occurred AFTER this start time.  Format:'Y-m-d H:M:S' OR 'Y-m-dTH:M:S' UTC",
+    )
+    parser_inspect.add_argument(
+        "-et",
+        "--end-time",
+        action="store",
+        help="Return events that occurred BEFORE this end time. Format:'Y-m-d H:M:S' OR 'Y-m-dTH:M:S' UTC",
+    )
 
     # live response parser
     parser_lr = subparsers.add_parser(
         "live-response", aliases=["lr"], help="Perform live response actions on a device/sensor."
     )
     parser_lr.add_argument("name_or_id", help="the hostname or sensor/device id to go live with.")
     parser_lr.add_argument(
         "-e", "--execute-command", action="store", help="Execute this command on the sensor. NOTE: waits for output."
     )
     parser_lr.add_argument("-cr", "--create-regkey", action="store", help="Create this regkey.")
     parser_lr.add_argument("-sr", "--set-regkey-value", action="append", help="Set this regkey value.")
-    if configured_products["response"]:
+    if configured_environments["response"]:
         parser_lr.add_argument(
             "-i",
             "--sensor-isolation-toggle",
             action="store_true",
             help="Sensor hostname/ID to isolation/unisolate (on/off). (CB Response)",
         )
-    if configured_products["psc"]:
+    if configured_environments["enterprise_edr"]:
         parser_lr.add_argument(
             "-q",
             "--quarantine",
             action="store_true",
             default=False,
-            help="Quarantine the devices returned by the query. (PSC)",
+            help="Quarantine the devices returned by the query. (Enterprise EDR)",
         )
         parser_lr.add_argument(
             "-uq",
             "--un_quarantine",
             action="store_true",
             default=False,
-            help="UN-Quarantine the devices returned by the query. (PSC)",
+            help="UN-Quarantine the devices returned by the query. (Enterprise EDR)",
         )
 
     # live response subparser
     lr_subparsers = parser_lr.add_subparsers(dest="live_response_command")
 
     # live response put file parser
     parser_put_file = lr_subparsers.add_parser("put", help="Put a file on the device/sensor.")
@@ -314,28 +339,28 @@
     parser_remediate.add_argument("-drv", "--delete-regkeyvalue", action="store", help="Delete the regkey value.")
     parser_remediate.add_argument(
         "--delete-entire-regkey", action="store", help="Delete the registry key and all values. BE CAREFUL."
     )
     parser_remediate.add_argument("-rs", "--remediation-script", action="store", help="Path to a remediaiton script.")
     parser_remediate.add_argument("--write-template", action="store_true", help="write a remediation template.")
 
-    # session parser - NOTE: functionality is limited on the PSC side, and it's specifically annoying that
-    # we can not get a list of active psc lr sessions... or at least I haven't figure out how to do that.
+    # session parser - NOTE: functionality is limited on the Enterprise EDR side, and it's specifically annoying that
+    # we can not get a list of active enterprise edr lr sessions... or at least I haven't figure out how to do that.
     parser_session = subparsers.add_parser("session", help="Interact with Cb live response server sessions.")
-    if configured_products["response"]:
+    if configured_environments["response"]:
         parser_session.add_argument(
             "-lss",
             "--list-sensor-sessions",
             action="store",
             help="list all CbLR sessions associated to this sensor ID (Response only).",
         )
     parser_session.add_argument(
         "-gsc", "--get-session-command-list", action="store", help="list commands associated to this session"
     )
-    if configured_products["response"]:
+    if configured_environments["response"]:
         parser_session.add_argument(
             "-a", "--list-all-sessions", action="store_true", help="list all CbLR sessions (Response only)."
         )
     parser_session.add_argument("-g", "--get-session", action="store", help="get live response session by id.")
     parser_session.add_argument("-c", "--close-session", action="store", help="close live response session by id.")
     parser_session.add_argument(
         "-gcr", "--get-command-result", action="store", help="get any results for this command."
@@ -352,46 +377,50 @@
         "-lh",
         "--logon-history",
         action="store",
         help="Given process username or device name, roughly enumerate logon history (Windows OS).",
     )
 
     # only add independent product args if product is a configured option
-    if configured_products["response"]:
+    if configured_environments["response"]:
         add_response_arguments_to_parser(subparsers)
-    if configured_products["psc"]:
-        add_psc_arguments_to_parser(subparsers)
+    if configured_environments["enterprise_edr"]:
+        add_eedr_arguments_to_parser(subparsers)
 
     argcomplete.autocomplete(parser)
     args = parser.parse_args()
-
     if args.debug:
         logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
-        coloredlogs.install(level="DEBUG", logger=logging.getLogger())
+        coloredlogs.install(
+            level="DEBUG",
+            logger=logging.getLogger(),
+            fmt="%(asctime)s %(name)s:%(lineno)d %(levelname)s %(message)s",
+        )
 
     if args.time_zone:
         set_timezone(args.time_zone)
 
     if args.set_default_timezone:
         set_timezone(args.set_default_timezone)
         save_configuration()
 
     if args.set_default_environment:
         product, profile = args.set_default_environment.split(":", 1)
-        set_default_cbapi_product(product)
-        set_default_cbapi_profile(profile)
+        set_default_cb_product(product)
+        set_default_cb_profile(profile)
         save_configuration()
 
     # Functionality that doesn't require a Cb connection.
+    # XTODO
     if args.command and (args.command.lower() == "lr" or args.command.lower().startswith("live")):
         if args.live_response_command and (
             args.live_response_command.startswith("play") or args.live_response_command == "pb"
         ):
             if args.list_playbooks:
-                print(f"\nConfigured Playbooks:")
+                print("\nConfigured Playbooks:")
                 for pb_key, pb_metadata in playbook_map.items():
                     print(f"\t{pb_metadata['name']} : {pb_metadata['description']}")
                 print()
                 return True
             if args.write_template:
                 template_path = write_playbook_template()
                 if os.path.exists(template_path):
@@ -408,18 +437,20 @@
     product, profile = args.environment.split(":", 1)
     LOGGER.debug(f"using '{profile}' profile via the configured '{product}' product.")
     try:
         if product == "response":
             cb = CbResponseAPI(profile=profile)
             execute_response_arguments(cb, args)
 
-        elif product == "psc":
-            cb = CbThreatHunterAPI(profile=profile)
-            execute_threathunter_arguments(cb, args)
+        elif product == "enterprise_edr":
+            cb = CBCloudAPI(profile=profile)
+            execute_eedr_arguments(cb, args)
     except ConnectionError as e:
         LOGGER.critical(f"Couldn't connect to {product} {profile}: {e}")
     except UnauthorizedError as e:
         LOGGER.critical(f"{e}")
     except ServerError as e:
         LOGGER.critical(f"CB ServerError 😒 (try again) : {e}")
     except TimeoutError as e:
         LOGGER.critical(f"TimeoutError waiting for CB server 🙄 (try again) : {e}")
+    except CredentialError as e:
+        LOGGER.critical(f"CredentialError : {e}")
```

### Comparing `cbinterface-2.3.9/cbinterface/commands.py` & `cbinterface-3.0.0/cbinterface/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,24 +34,25 @@
         self._hostname = None
         self.placeholders = placeholders
         self.post_completion_command = post_completion_command
 
     def fill_placeholders(self, string_item: str, placeholders={}):
         # fill common placeholders
         placeholders = placeholders if placeholders else self.placeholders
-        placeholders["HOSTNAME"] = placeholders.get("HOSTNAME", self.hostname)
+        hostname = self.hostname[self.hostname.rfind('\\')+1:] if '\\' in self.hostname else self.hostname
+        placeholders["HOSTNAME"] = placeholders.get("HOSTNAME", hostname)
         placeholders["SENSOR_ID"] = placeholders.get("SENSOR_ID", self.sensor_id)
         placeholders["DEVICE_ID"] = placeholders.get("DEVICE_ID", self.sensor_id)
         placeholders["WORK_DIR"] = placeholders.get("WORK_DIR", "C:\\Program Files")
         string_item = string_item.format(**placeholders)
         return string_item
 
     @property
     def hostname(self):
-        # NOTE: Appears this is set to None for psc. So, custom
+        # NOTE: Appears this is set to None for enterprise edr. So, custom
         # session manager sets it right before job submission.
         return self.session_data.get("hostname") or self._hostname
 
     @property
     def sensor_id(self):
         return self.session_data.get("sensor_id") or self._sensor_id
 
@@ -95,30 +96,31 @@
                 return "error"
             if self.has_result:
                 return "complete"
         return "pending"
 
     def run(self):
         """The function to implement the live response command logic."""
-        raise NotImplemented()
+        raise NotImplementedError()
 
     def process_result(self):
         """Implement logic to process any results."""
         pass
 
     def execute_post_completion(self):
         if not self.post_completion_command:
             return None
         if self.status != "complete":
             return False
         self.post_completion_command = self.fill_placeholders(self.post_completion_command)
         if self.post_completion_command.startswith("tools/"):
             self.post_completion_command = f"{BASE_DIR}/{self.post_completion_command}"
         LOGGER.info(f"executing post completion command: {self.post_completion_command}")
-        import shlex, subprocess
+        import shlex
+        import subprocess
 
         try:
             args = shlex.split(self.post_completion_command)
             return subprocess.run(args=args)
         except Exception as e:
             LOGGER.error(f"caught exception executing post completion command: {e}")
             return False
@@ -398,15 +400,15 @@
 class GetSystemMemoryDump(BaseSessionCommand):
     """Perform a memory dump operation on the sensor.
 
     NOTE: Not a fan of Cb's implementation.
     """
 
     def __init__(self, local_filename: str = "", compress=True):
-        super().__init__(description=f"Dump System Memory")
+        super().__init__(description="Dump System Memory")
         self.local_filename = local_filename
         self.compress = compress
         self._memdump_id = None
         self._cb = None
 
     def run(self, session: CbLRSessionBase):
         # store a pointer to the CbR object for later
@@ -423,51 +425,52 @@
 
     def process_result(self):
         from cbinterface.response.sessions import get_command_result
 
         # should only make it here if an error was not raise
         # check to see if the command has success status with server
         # and if the local file exists
-        memdump_cmd = get_command_result(self._cb, self.session_id, self._memdump_id)
+        get_command_result(self._cb, self.session_id, self._memdump_id)
         if memdump["status"] != "complete":
             LOGGER.error(f"problem completing memory dump: command status: {memdump['status']}")
             return False
         if os.path.exits(self.local_filename):
             LOGGER.info(f" +  wrote: {self.local_filename}")
             return True
         else:
-            LOGGER.error(f"Memory dump completed but failed to get a local copy of the memory dump.")
+            LOGGER.error("Memory dump completed but failed to get a local copy of the memory dump.")
             return False
 
 
 class GetFile(BaseSessionCommand):
     """Object that retrieves a file via Live Response."""
 
     def __init__(self, file_path, output_filename: Union[str, bool] = None, **kwargs):
-        """
-        Initialize the GetFile command.
+        """Initialize the GetFile command.
 
         Args:
             file_path (str): The file path to be fetched.
             output_filename: optional path to write the file content.
+
         Returns:
             True on success, False on failure.
         """
         super().__init__(description=f"getFile @ '{file_path}'", **kwargs)
         self._file_path = file_path
 
         self.output_filename = output_filename
 
     def run(self, session: CbLRSessionBase):
-        """
-        Execute the file transfer.
+        """Execute the file transfer.
+
         Args:
             session (CbLRSessionBase): The Live Response session being used.
+
         Returns:
-            File content
+            File content.
         """
         if "{WILDMATCH}" in self._file_path:
             # split on "{WILDMATCH}" and search for the first match to collect
             from cbinterface.helpers import get_os_independent_filepath
 
             file_path_parts = [self.fill_placeholders(fpp) for fpp in self._file_path.split("{WILDMATCH}")]
             dir_path = get_os_independent_filepath(file_path_parts[0]).parent
@@ -519,16 +522,16 @@
 ########################
 # Remediaiton Commands #
 ########################
 class DeleteFile(BaseSessionCommand):
     """Object that deletes a file via Live Response."""
 
     def __init__(self, file_path):
-        """
-        Delete the specified file name on the remote machine.
+        """Delete the specified file name on the remote machine.
+
         Args:
             filename (str): Name of the file to be deleted.
         """
         super().__init__(description=f"Delete File @ '{file_path}'")
         self._file_path = file_path
 
     def run(self, session: CbLRSessionBase):
@@ -536,18 +539,19 @@
 
     def process_result(self):
         LOGGER.info(f"deleted '{self._file_path}' on {self.hostname} via session {self.session_id}")
         return True
 
 
 class KillProcessByID(BaseSessionCommand):
-    """
-    Terminate a process by process id.
+    """Terminate a process by process id.
+
     Args:
         pid (int): Process ID to be terminated.
+
     Returns:
         bool: True if success, False if failure.
     """
 
     def __init__(self, pid):
         super().__init__(description=f"Kill Process with ID={pid}")
         self.pid = pid
@@ -589,18 +593,19 @@
         return session.delete_registry_key(self.regkey)
 
     def process_result(self):
         LOGGER.info(f"Deleted '{self.regkey}' on {self.hostname}")
 
 
 class KillProcessByName(BaseSessionCommand):
-    """
-    Terminate a process by process name.
+    """Terminate a process by process name.
+
     Args:
         process_name (str): Process name(s) to be terminated.
+
     Returns:
         bool: True if success, False if failure.
     """
 
     def __init__(self, process_name):
         super().__init__(description=f"Kill Processes with name like '{process_name}'")
         self.pname = process_name
```

### Comparing `cbinterface-2.3.9/setup.py` & `cbinterface-3.0.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
+
 # To use a consistent encoding
 from codecs import open
 from os import path
 
 # assumes we're at the repo root
 from cbinterface import __version__
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 # Load requirements
-with open(path.join(here, 'requirements.txt'), encoding='utf-8') as f:
+with open(path.join(here, "requirements.txt"), encoding="utf-8") as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
-    name='cbinterface',
+    name="cbinterface",
     version=__version__,
-    description="Command line tool for interfacing with carbonblack environments (PSC & Response) for analysis/investigations and live response playbooks.",
+    description="Command line tool for interfacing with carbonblack environments (Enterprise EDR & Response) for analysis/investigations and live response playbooks.",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     url="https://github.com/ace-ecosystem/cbinterface2",
-    author='Sean McFeely',
-    author_email='mcfeelynaes@gmail.com',
-    license='Apache-2.0',
+    author="Sean McFeely",
+    author_email="mcfeelynaes@gmail.com",
+    license="Apache-2.0",
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3',
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "License :: OSI Approved :: Apache Software License",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3",
     ],
-    keywords='Carbon Black,carbonblack',
+    keywords="Carbon Black,carbonblack",
     packages=find_packages(),
     include_package_data=True,
     install_requires=requirements,
-    scripts=['bin/cbinterface'],
+    scripts=["bin/cbinterface"],
 )
```

### Comparing `cbinterface-2.3.9/LICENSE` & `cbinterface-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cbinterface-2.3.9/pyproject.toml` & `cbinterface-3.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "cbinterface"
-version = "2.3.9"
+version = "3.0.0"
 description = "command line tool for interfacing with multiple carbonblack environments to perform analysis and live response functions"
 authors = ["Sean McFeely <mcfeelynaes@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ace-ecosystem/cbinterface2"
 keywords = ["Carbon Black", "carbonblack"]
 include = ["README.md"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 cbapi = "^1.7.3"
 coloredlogs = "^15.0"
-argcomplete = "^1.12.2"
+argcomplete = ">=1.12.2,2.*"
+carbon-black-cloud-sdk = "^1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pytest-mock = "^3.5.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

