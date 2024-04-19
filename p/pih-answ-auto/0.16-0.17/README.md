# Comparing `tmp/pih-answ_auto-0.16.tar.gz` & `tmp/pih-answ_auto-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-answ_auto-0.16.tar", last modified: Tue Apr 16 00:45:13 2024, max compression
+gzip compressed data, was "pih-answ_auto-0.17.tar", last modified: Fri Apr 19 02:20:38 2024, max compression
```

## Comparing `pih-answ_auto-0.16.tar` & `pih-answ_auto-0.17.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 00:45:13.791914 pih-answ_auto-0.16/
-drwxrwxrwx   0        0        0        0 2024-04-16 00:45:13.264186 pih-answ_auto-0.16/AnswerAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.16/AnswerAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.16/AnswerAutomationService/__main__.py
--rw-rw-rw-   0        0        0      412 2024-04-16 00:44:21.000000 pih-answ_auto-0.16/AnswerAutomationService/const.py
--rw-rw-rw-   0        0        0     4035 2024-04-16 00:17:31.000000 pih-answ_auto-0.16/AnswerAutomationService/service.py
--rw-rw-rw-   0        0        0      283 2024-04-16 00:45:13.712704 pih-answ_auto-0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 00:45:13.665806 pih-answ_auto-0.16/pih_answ_auto.egg-info/
--rw-rw-rw-   0        0        0      283 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-16 00:45:12.000000 pih-answ_auto-0.16/pih_answ_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 00:45:13.807528 pih-answ_auto-0.16/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-19 02:20:38.511806 pih-answ_auto-0.17/
+drwxrwxrwx   0        0        0        0 2024-04-19 02:20:37.597884 pih-answ_auto-0.17/AnswerAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-answ_auto-0.17/AnswerAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-16 00:17:31.000000 pih-answ_auto-0.17/AnswerAutomationService/__main__.py
+-rw-rw-rw-   0        0        0      412 2024-04-19 00:58:50.000000 pih-answ_auto-0.17/AnswerAutomationService/const.py
+-rw-rw-rw-   0        0        0     7997 2024-04-19 01:17:29.000000 pih-answ_auto-0.17/AnswerAutomationService/service.py
+-rw-rw-rw-   0        0        0      283 2024-04-19 02:20:38.479533 pih-answ_auto-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-19 02:20:38.432676 pih-answ_auto-0.17/pih_answ_auto.egg-info/
+-rw-rw-rw-   0        0        0      283 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-19 02:20:37.000000 pih-answ_auto-0.17/pih_answ_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-19 02:20:38.527450 pih-answ_auto-0.17/setup.cfg
```

