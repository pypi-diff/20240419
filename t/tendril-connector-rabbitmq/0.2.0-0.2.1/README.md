# Comparing `tmp/tendril_connector_rabbitmq-0.2.0.tar.gz` & `tmp/tendril_connector_rabbitmq-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril_connector_rabbitmq-0.2.0.tar", last modified: Tue Apr 16 18:38:39 2024, max compression
+gzip compressed data, was "tendril_connector_rabbitmq-0.2.1.tar", last modified: Thu Apr 18 22:03:36 2024, max compression
```

## Comparing `tendril_connector_rabbitmq-0.2.0.tar` & `tendril_connector_rabbitmq-0.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.197510 tendril_connector_rabbitmq-0.2.0/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/MANIFEST.in
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-16 18:38:39.193510 tendril_connector_rabbitmq-0.2.0/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.181510 tendril_connector_rabbitmq-0.2.0/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_rabbitmq-0.2.0/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-16 18:38:39.197510 tendril_connector_rabbitmq-0.2.0/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril_connector_rabbitmq-0.2.0/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.177510 tendril_connector_rabbitmq-0.2.0/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq_core.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.185510 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     5677 2024-04-16 18:27:08.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril/core/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2716 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      816 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio_base.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/tx.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/
--rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-16 18:38:39.000000 tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-16 18:38:39.189510 tendril_connector_rabbitmq-0.2.0/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.0/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.053965 tendril_connector_rabbitmq-0.2.1/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/MANIFEST.in
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-18 22:03:36.049965 tendril_connector_rabbitmq-0.2.1/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2368 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.033965 tendril_connector_rabbitmq-0.2.1/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-11-21 18:38:28.000000 tendril_connector_rabbitmq-0.2.1/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      128 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13482 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      895 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1602 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-18 22:03:36.053965 tendril_connector_rabbitmq-0.2.1/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3285 2023-08-15 05:25:44.000000 tendril_connector_rabbitmq-0.2.1/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.025965 tendril_connector_rabbitmq-0.2.1/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       66 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2021-03-26 08:21:36.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     4484 2023-09-06 12:05:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1439 2021-06-17 11:57:47.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq_core.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.037965 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:06:39.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-03 06:03:50.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     5773 2024-04-17 22:19:49.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     8866 2023-09-09 06:47:04.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/core/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2023-08-03 06:03:13.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.041965 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-04 13:00:08.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2715 2024-04-18 22:01:58.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      816 2024-04-16 18:25:58.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio_base.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      163 2023-08-14 12:34:45.000000 tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/tx.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.045965 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/
+-rw-r--r--   0 chintal   (1000) chintal   (1000)     5591 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1088 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      568 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-18 22:03:35.000000 tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-18 22:03:36.045965 tendril_connector_rabbitmq-0.2.1/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      787 2023-08-02 20:11:04.000000 tendril_connector_rabbitmq-0.2.1/tox.ini
```

### Comparing `tendril_connector_rabbitmq-0.2.0/.gitignore` & `tendril_connector_rabbitmq-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/.readthedocs.yml` & `tendril_connector_rabbitmq-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/.travis.yml` & `tendril_connector_rabbitmq-0.2.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/LICENSE` & `tendril_connector_rabbitmq-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/PKG-INFO` & `tendril_connector_rabbitmq-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-connector-rabbitmq
-Version: 0.2.0
+Version: 0.2.1
 Summary: RabbitMQ Connector for Tendril
 Home-page: https://github.com/tendril-framework/tendril-connector-rabbitmq
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-connector-rabbitmq.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-connector-rabbitmq/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-connector-rabbitmq
```

### Comparing `tendril_connector_rabbitmq-0.2.0/README.rst` & `tendril_connector_rabbitmq-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/Makefile` & `tendril_connector_rabbitmq-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/_static/custom.css` & `tendril_connector_rabbitmq-0.2.1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/_static/favicon.ico` & `tendril_connector_rabbitmq-0.2.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/_static/logo.png` & `tendril_connector_rabbitmq-0.2.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/_static/logo_packed.png` & `tendril_connector_rabbitmq-0.2.1/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/_templates/about.html` & `tendril_connector_rabbitmq-0.2.1/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/conf.py` & `tendril_connector_rabbitmq-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/index.rst` & `tendril_connector_rabbitmq-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/docs/installation.rst` & `tendril_connector_rabbitmq-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/setup.py` & `tendril_connector_rabbitmq-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/config/__init__.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/config/mq_core.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/config/mq_core.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/aio.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,21 @@
     scheme = 'amqp'
 
 def _build_conn_string(p: ConnectionParameters):
     return f"{scheme}://{p.credentials.username}:{p.credentials.password}" \
            f"@{p.host}:{p.port}/{p.virtual_host}"
 
 
+def _pp(code):
+    if code == 'default':
+        return ''
+    else:
+        return code
+
+
 class RabbitMQAsyncManager(GenericMQAsyncManager):
     _instance = None
 
     @classmethod
     async def get_instance(cls):
         if cls._instance is None:
             cls._instance = RabbitMQAsyncManager()
@@ -107,15 +114,15 @@
     def __init__(self, channel, code='default'):
         self.channel = channel
         self._code = code
         self._exchange = None
 
     async def exchange(self):
         if not self._exchange:
-            mq_server_exchange = getattr(config, 'MQ{}_SERVER_EXCHANGE'.format(self._code))
+            mq_server_exchange = getattr(config, 'MQ{}_SERVER_EXCHANGE'.format(_pp(self._code)))
             self._exchange = await self.channel.get_exchange(mq_server_exchange)
         return self._exchange
 
     async def publish(self, key: str, data: str):
         message = Message(data.encode(), delivery_mode=DeliveryMode.PERSISTENT)
         exchange = await self.exchange()
         await exchange.publish(message, routing_key=key)
```

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/connectors/rabbitmq/tx.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/connectors/rabbitmq/tx.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     for modname in get_namespace_package_names(prefix):
         try:
             globals()[modname] = importlib.import_module(modname)
             if hasattr(globals()[modname], 'create_mq_topology'):
                 logger.debug(f"Installing MQ Topology from {modname}")
                 await globals()[modname].create_mq_topology()
         except MQServerNotEnabled as e:
-            logger.debug(f"Skipping topology installation on disabled MQ Server {e.code}")
+            logger.info(f"Skipping topology installation on disabled MQ Server {e.code}")
         except ImportError as e:
             logger.debug(e)
 
 
 async def startup():
     manager = await MQManager.get_instance()
     await manager.init(loop=asyncio.get_running_loop())
```

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril/core/mq/aio_base.py` & `tendril_connector_rabbitmq-0.2.1/src/tendril/core/mq/aio_base.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/PKG-INFO` & `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-connector-rabbitmq
-Version: 0.2.0
+Version: 0.2.1
 Summary: RabbitMQ Connector for Tendril
 Home-page: https://github.com/tendril-framework/tendril-connector-rabbitmq
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-connector-rabbitmq.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-connector-rabbitmq/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-connector-rabbitmq
```

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt` & `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/src/tendril_connector_rabbitmq.egg-info/requires.txt` & `tendril_connector_rabbitmq-0.2.1/src/tendril_connector_rabbitmq.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/tests/coveralls.py` & `tendril_connector_rabbitmq-0.2.1/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril_connector_rabbitmq-0.2.0/tox.ini` & `tendril_connector_rabbitmq-0.2.1/tox.ini`

 * *Files identical despite different names*

