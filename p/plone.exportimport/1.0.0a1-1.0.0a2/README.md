# Comparing `tmp/plone.exportimport-1.0.0a1.tar.gz` & `tmp/plone.exportimport-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.exportimport-1.0.0a1.tar", last modified: Wed Apr 17 17:50:21 2024, max compression
+gzip compressed data, was "plone.exportimport-1.0.0a2.tar", last modified: Thu Apr 18 23:23:21 2024, max compression
```

## Comparing `plone.exportimport-1.0.0a1.tar` & `plone.exportimport-1.0.0a2.tar`

### file list

```diff
@@ -1,222 +1,228 @@
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.561632 plone.exportimport-1.0.0a1/
--rw-r--r--   0 davisagli   (501) staff       (20)     1381 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/.editorconfig
--rw-r--r--   0 davisagli   (501) staff       (20)      538 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/.flake8
--rw-r--r--   0 davisagli   (501) staff       (20)      722 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/.gitignore
--rw-r--r--   0 davisagli   (501) staff       (20)      788 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/.meta.toml
--rw-r--r--   0 davisagli   (501) staff       (20)     2023 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0 davisagli   (501) staff       (20)      728 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/CHANGES.md
--rw-r--r--   0 davisagli   (501) staff       (20)       95 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/CONTRIBUTING.md
--rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/LICENSE
--rw-r--r--   0 davisagli   (501) staff       (20)      320 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/MANIFEST.in
--rw-r--r--   0 davisagli   (501) staff       (20)     3920 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/Makefile
--rw-r--r--   0 davisagli   (501) staff       (20)     2664 2024-04-17 17:50:21.561506 plone.exportimport-1.0.0a1/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)      731 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/README.md
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/constraints.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      322 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/dependabot.yml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.544124 plone.exportimport-1.0.0a1/docs/
--rw-r--r--   0 davisagli   (501) staff       (20)     7078 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/Makefile
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.544633 plone.exportimport-1.0.0a1/docs/_static/
--rw-r--r--   0 davisagli   (501) staff       (20)     5430 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/_static/favicon.ico
--rw-r--r--   0 davisagli   (501) staff       (20)     3775 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/_static/logo.svg
--rw-r--r--   0 davisagli   (501) staff       (20)       30 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/_static/print.css
--rw-r--r--   0 davisagli   (501) staff       (20)     7814 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/_static/styles.css
--rw-r--r--   0 davisagli   (501) staff       (20)     2813 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/conf.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1310 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/develop.md
--rw-r--r--   0 davisagli   (501) staff       (20)     3374 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/features.md
--rw-r--r--   0 davisagli   (501) staff       (20)      722 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/index.md
--rw-r--r--   0 davisagli   (501) staff       (20)     1135 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/docs/installation.md
--rw-r--r--   0 davisagli   (501) staff       (20)      158 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/instance.yaml
--rw-r--r--   0 davisagli   (501) staff       (20)      251 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/mx.ini
--rw-r--r--   0 davisagli   (501) staff       (20)     4707 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/pyproject.toml
--rw-r--r--   0 davisagli   (501) staff       (20)     1032 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/requirements-docs.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       33 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/requirements.txt
--rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-17 17:50:21.561670 plone.exportimport-1.0.0a1/setup.cfg
--rw-r--r--   0 davisagli   (501) staff       (20)     2803 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/setup.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.536307 plone.exportimport-1.0.0a1/src/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.544759 plone.exportimport-1.0.0a1/src/plone/
--rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.546275 plone.exportimport-1.0.0a1/src/plone/exportimport/
--rw-r--r--   0 davisagli   (501) staff       (20)      130 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/__init__.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.546392 plone.exportimport-1.0.0a1/src/plone/exportimport/cli/
--rw-r--r--   0 davisagli   (501) staff       (20)     2607 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/cli/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)      667 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.546826 plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1670 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/blob.py
--rw-r--r--   0 davisagli   (501) staff       (20)      626 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/blocks.py
--rw-r--r--   0 davisagli   (501) staff       (20)      193 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/configure.zcml
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.547818 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/
--rw-r--r--   0 davisagli   (501) staff       (20)     2463 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1979 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1568 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     6123 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/content.py
--rw-r--r--   0 davisagli   (501) staff       (20)      700 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)      828 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/principals.py
--rw-r--r--   0 davisagli   (501) staff       (20)      660 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)      660 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)      709 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/translations.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.548832 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/
--rw-r--r--   0 davisagli   (501) staff       (20)     1943 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1946 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/base.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1568 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)     5277 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/content.py
--rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1355 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/principals.py
--rw-r--r--   0 davisagli   (501) staff       (20)      597 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)      597 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)      617 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/importers/translations.py
--rw-r--r--   0 davisagli   (501) staff       (20)      568 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/interfaces.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.549294 plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4118 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/blob.py
--rw-r--r--   0 davisagli   (501) staff       (20)      611 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/blocks.py
--rw-r--r--   0 davisagli   (501) staff       (20)      388 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/configure.zcml
--rw-r--r--   0 davisagli   (501) staff       (20)      498 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/settings.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.549412 plone.exportimport-1.0.0a1/src/plone/exportimport/testing/
--rw-r--r--   0 davisagli   (501) staff       (20)      762 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/testing/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1613 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/types.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.550594 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/
--rw-r--r--   0 davisagli   (501) staff       (20)       42 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1747 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/cli.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.551397 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/
--rw-r--r--   0 davisagli   (501) staff       (20)      825 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1359 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/blocks.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3005 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/core.py
--rw-r--r--   0 davisagli   (501) staff       (20)    10137 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/export_helpers.py
--rw-r--r--   0 davisagli   (501) staff       (20)    10119 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/import_helpers.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1558 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/revisions.py
--rw-r--r--   0 davisagli   (501) staff       (20)      592 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/dates.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5169 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)      627 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/path.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.551940 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/
--rw-r--r--   0 davisagli   (501) staff       (20)      172 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/__init__.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1741 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/groups.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1184 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/helpers.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4217 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/members.py
--rw-r--r--   0 davisagli   (501) staff       (20)      999 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3567 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5259 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/translations.py
--rw-r--r--   0 davisagli   (501) staff       (20)      468 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone/exportimport/utils/zca.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.545703 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/
--rw-r--r--   0 davisagli   (501) staff       (20)     2664 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/PKG-INFO
--rw-r--r--   0 davisagli   (501) staff       (20)     7532 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/SOURCES.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/dependency_links.txt
--rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/entry_points.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/namespace_packages.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/not-zip-safe
--rw-r--r--   0 davisagli   (501) staff       (20)      495 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/requires.txt
--rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/top_level.txt
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.552083 plone.exportimport-1.0.0a1/tests/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.538360 plone.exportimport-1.0.0a1/tests/_resources/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.552761 plone.exportimport-1.0.0a1/tests/_resources/base_import/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.552906 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553051 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/
--rw-r--r--   0 davisagli   (501) staff       (20)     1404 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553186 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/
--rw-r--r--   0 davisagli   (501) staff       (20)     1135 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553331 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/
--rw-r--r--   0 davisagli   (501) staff       (20)     7903 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553476 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/
--rw-r--r--   0 davisagli   (501) staff       (20)     1447 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553622 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/
--rw-r--r--   0 davisagli   (501) staff       (20)     1638 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553773 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/
--rw-r--r--   0 davisagli   (501) staff       (20)     1455 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.553968 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/
--rw-r--r--   0 davisagli   (501) staff       (20)     1903 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.554139 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/
--rw-r--r--   0 davisagli   (501) staff       (20)    66267 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.554348 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/
--rw-r--r--   0 davisagli   (501) staff       (20)     1256 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.554505 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/
--rw-r--r--   0 davisagli   (501) staff       (20)    40383 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png
--rw-r--r--   0 davisagli   (501) staff       (20)     2349 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/__metadata__.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.554684 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/
--rw-r--r--   0 davisagli   (501) staff       (20)     3720 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.554837 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/plone_site_root/
--rw-r--r--   0 davisagli   (501) staff       (20)    18437 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/content/plone_site_root/data.json
--rw-r--r--   0 davisagli   (501) staff       (20)     4827 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/discussions.json
--rw-r--r--   0 davisagli   (501) staff       (20)     1877 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/principals.json
--rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/redirects.json
--rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/relations.json
--rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/base_import/translations.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.555002 plone.exportimport-1.0.0a1/tests/_resources/empty_import/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/empty_import/.gitkeep
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.555660 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.555787 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.555922 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/
--rw-r--r--   0 davisagli   (501) staff       (20)     1168 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556047 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/
--rw-r--r--   0 davisagli   (501) staff       (20)     1468 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556170 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/
--rw-r--r--   0 davisagli   (501) staff       (20)     1297 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556293 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/
--rw-r--r--   0 davisagli   (501) staff       (20)     1502 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556418 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/
--rw-r--r--   0 davisagli   (501) staff       (20)     1428 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556538 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/
--rw-r--r--   0 davisagli   (501) staff       (20)     1177 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556666 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/
--rw-r--r--   0 davisagli   (501) staff       (20)     1463 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556790 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/
--rw-r--r--   0 davisagli   (501) staff       (20)     1295 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.556911 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/
--rw-r--r--   0 davisagli   (501) staff       (20)     1419 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557026 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/
--rw-r--r--   0 davisagli   (501) staff       (20)     1286 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557153 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/
--rw-r--r--   0 davisagli   (501) staff       (20)     1520 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json
--rw-r--r--   0 davisagli   (501) staff       (20)     4390 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/__metadata__.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557269 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/
--rw-r--r--   0 davisagli   (501) staff       (20)     1520 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557390 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/
--rw-r--r--   0 davisagli   (501) staff       (20)     1502 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557516 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/
--rw-r--r--   0 davisagli   (501) staff       (20)     1419 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557642 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/
--rw-r--r--   0 davisagli   (501) staff       (20)     1511 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557758 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/
--rw-r--r--   0 davisagli   (501) staff       (20)     1472 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557874 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/
--rw-r--r--   0 davisagli   (501) staff       (20)     1173 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.557989 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/
--rw-r--r--   0 davisagli   (501) staff       (20)     1529 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.558102 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/plone_site_root/
--rw-r--r--   0 davisagli   (501) staff       (20)      738 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/plone_site_root/data.json
--rw-r--r--   0 davisagli   (501) staff       (20)     4888 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/discussions.json
--rw-r--r--   0 davisagli   (501) staff       (20)     1877 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/principals.json
--rw-r--r--   0 davisagli   (501) staff       (20)       41 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/redirects.json
--rw-r--r--   0 davisagli   (501) staff       (20)      452 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/relations.json
--rw-r--r--   0 davisagli   (501) staff       (20)      928 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/translations.json
--rw-r--r--   0 davisagli   (501) staff       (20)     7068 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/conftest.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.559107 plone.exportimport-1.0.0a1/tests/exporters/
--rw-r--r--   0 davisagli   (501) staff       (20)      864 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3239 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters.py
--rw-r--r--   0 davisagli   (501) staff       (20)     2556 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_content.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1942 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1303 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_principals.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1294 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1861 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1890 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/exporters/test_exporters_translations.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.560121 plone.exportimport-1.0.0a1/tests/importers/
--rw-r--r--   0 davisagli   (501) staff       (20)      666 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1533 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1118 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_content.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1437 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1434 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_principals.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1413 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1413 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1446 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/importers/test_importers_translations.py
-drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.561338 plone.exportimport-1.0.0a1/tests/utils/
--rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/conftest.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3700 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_content_core.py
--rw-r--r--   0 davisagli   (501) staff       (20)      860 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_content_revisions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1304 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_dates.py
--rw-r--r--   0 davisagli   (501) staff       (20)     3688 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_discussions.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1365 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_path.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1023 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_principals_groups.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1184 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_principals_members.py
--rw-r--r--   0 davisagli   (501) staff       (20)     1252 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_redirects.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5384 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_relations.py
--rw-r--r--   0 davisagli   (501) staff       (20)     5186 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tests/utils/test_utils_translations.py
--rw-r--r--   0 davisagli   (501) staff       (20)     4873 2024-04-17 17:50:21.000000 plone.exportimport-1.0.0a1/tox.ini
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.414432 plone.exportimport-1.0.0a2/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1381 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/.editorconfig
+-rw-r--r--   0 davisagli   (501) staff       (20)      538 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/.flake8
+-rw-r--r--   0 davisagli   (501) staff       (20)      722 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/.gitignore
+-rw-r--r--   0 davisagli   (501) staff       (20)      828 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/.meta.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)     2023 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/.pre-commit-config.yaml
+-rw-r--r--   0 davisagli   (501) staff       (20)      861 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/CHANGES.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       95 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/CONTRIBUTING.md
+-rw-r--r--   0 davisagli   (501) staff       (20)    18092 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/LICENSE
+-rw-r--r--   0 davisagli   (501) staff       (20)      320 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/MANIFEST.in
+-rw-r--r--   0 davisagli   (501) staff       (20)     3920 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/Makefile
+-rw-r--r--   0 davisagli   (501) staff       (20)     2797 2024-04-18 23:23:21.414267 plone.exportimport-1.0.0a2/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)      731 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/README.md
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/constraints.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      322 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/dependabot.yml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.391469 plone.exportimport-1.0.0a2/docs/
+-rw-r--r--   0 davisagli   (501) staff       (20)     7078 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/Makefile
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.392114 plone.exportimport-1.0.0a2/docs/_static/
+-rw-r--r--   0 davisagli   (501) staff       (20)     5430 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/_static/favicon.ico
+-rw-r--r--   0 davisagli   (501) staff       (20)     3775 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/_static/logo.svg
+-rw-r--r--   0 davisagli   (501) staff       (20)       30 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/_static/print.css
+-rw-r--r--   0 davisagli   (501) staff       (20)     7814 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/_static/styles.css
+-rw-r--r--   0 davisagli   (501) staff       (20)     2813 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/conf.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1310 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/develop.md
+-rw-r--r--   0 davisagli   (501) staff       (20)     3374 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/features.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      722 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/index.md
+-rw-r--r--   0 davisagli   (501) staff       (20)     1135 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/docs/installation.md
+-rw-r--r--   0 davisagli   (501) staff       (20)      158 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/instance.yaml
+-rw-r--r--   0 davisagli   (501) staff       (20)      251 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/mx.ini
+-rw-r--r--   0 davisagli   (501) staff       (20)     4747 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/pyproject.toml
+-rw-r--r--   0 davisagli   (501) staff       (20)     1032 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/requirements-docs.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       33 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/requirements.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)       38 2024-04-18 23:23:21.414474 plone.exportimport-1.0.0a2/setup.cfg
+-rw-r--r--   0 davisagli   (501) staff       (20)     2834 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/setup.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.381770 plone.exportimport-1.0.0a2/src/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.392309 plone.exportimport-1.0.0a2/src/plone/
+-rw-r--r--   0 davisagli   (501) staff       (20)       56 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.394529 plone.exportimport-1.0.0a2/src/plone/exportimport/
+-rw-r--r--   0 davisagli   (501) staff       (20)      130 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/__init__.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.394696 plone.exportimport-1.0.0a2/src/plone/exportimport/cli/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2607 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/cli/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      667 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.395363 plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1670 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/blob.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      626 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/blocks.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      193 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/configure.zcml
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.397070 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2459 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1979 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1933 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     6123 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/content.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      700 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      651 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/portlets.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      828 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/principals.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      660 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      660 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      709 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/translations.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.398796 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1938 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1946 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/base.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1933 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)     5277 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/content.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      613 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      581 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/portlets.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1355 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/principals.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      597 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      597 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      617 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/importers/translations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      568 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/interfaces.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.399346 plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4118 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/blob.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      611 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/blocks.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      388 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/configure.zcml
+-rw-r--r--   0 davisagli   (501) staff       (20)      498 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/settings.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.399492 plone.exportimport-1.0.0a2/src/plone/exportimport/testing/
+-rw-r--r--   0 davisagli   (501) staff       (20)      762 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/testing/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1613 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/types.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.400903 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/
+-rw-r--r--   0 davisagli   (501) staff       (20)       42 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1747 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/cli.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.401758 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/
+-rw-r--r--   0 davisagli   (501) staff       (20)      825 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1359 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/blocks.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3005 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/core.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    10137 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/export_helpers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)    10119 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/import_helpers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1558 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/revisions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      592 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/dates.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5169 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      627 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/path.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     8820 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/portlets.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.402387 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/
+-rw-r--r--   0 davisagli   (501) staff       (20)      172 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/__init__.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1741 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/groups.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1184 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/helpers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4217 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/members.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      999 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3567 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5259 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/translations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      468 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/src/plone/exportimport/utils/zca.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.393658 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/
+-rw-r--r--   0 davisagli   (501) staff       (20)     2797 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/PKG-INFO
+-rw-r--r--   0 davisagli   (501) staff       (20)     7792 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/SOURCES.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/dependency_links.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)      165 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/entry_points.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/namespace_packages.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        1 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/not-zip-safe
+-rw-r--r--   0 davisagli   (501) staff       (20)      515 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/requires.txt
+-rw-r--r--   0 davisagli   (501) staff       (20)        6 2024-04-18 23:23:21.000000 plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/top_level.txt
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.402545 plone.exportimport-1.0.0a2/tests/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.384557 plone.exportimport-1.0.0a2/tests/_resources/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.403477 plone.exportimport-1.0.0a2/tests/_resources/base_import/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.403635 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.403797 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1404 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.403957 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1135 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404134 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/
+-rw-r--r--   0 davisagli   (501) staff       (20)     7903 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404302 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1447 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404470 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1638 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404651 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1455 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404818 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1903 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.404995 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/
+-rw-r--r--   0 davisagli   (501) staff       (20)    66267 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.405219 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1256 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.405382 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/
+-rw-r--r--   0 davisagli   (501) staff       (20)    40383 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png
+-rw-r--r--   0 davisagli   (501) staff       (20)     2349 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/__metadata__.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.405568 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/
+-rw-r--r--   0 davisagli   (501) staff       (20)     3720 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.405729 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/plone_site_root/
+-rw-r--r--   0 davisagli   (501) staff       (20)    18437 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/content/plone_site_root/data.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     4827 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/discussions.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     1583 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/portlets.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     1877 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/principals.json
+-rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/redirects.json
+-rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/relations.json
+-rw-r--r--   0 davisagli   (501) staff       (20)        3 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/base_import/translations.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.405914 plone.exportimport-1.0.0a2/tests/_resources/empty_import/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/empty_import/.gitkeep
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.406681 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.406832 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.406991 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1168 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407156 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1468 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407314 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1297 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407475 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1502 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407631 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1428 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407786 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1177 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.407954 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1463 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.408120 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1295 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.408278 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1419 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.408629 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1286 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.408776 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1520 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     4390 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/__metadata__.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.408919 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1520 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409060 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1502 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409208 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1419 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409350 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1511 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409499 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1472 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409664 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1173 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409827 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/
+-rw-r--r--   0 davisagli   (501) staff       (20)     1529 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.409966 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/plone_site_root/
+-rw-r--r--   0 davisagli   (501) staff       (20)      738 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/plone_site_root/data.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     4888 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/discussions.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     1877 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/principals.json
+-rw-r--r--   0 davisagli   (501) staff       (20)       41 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/redirects.json
+-rw-r--r--   0 davisagli   (501) staff       (20)      452 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/relations.json
+-rw-r--r--   0 davisagli   (501) staff       (20)      928 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/translations.json
+-rw-r--r--   0 davisagli   (501) staff       (20)     7068 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/conftest.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.411230 plone.exportimport-1.0.0a2/tests/exporters/
+-rw-r--r--   0 davisagli   (501) staff       (20)      864 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/conftest.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3239 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     2556 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_content.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1942 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1966 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_portlets.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1303 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_principals.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1294 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1861 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1890 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/exporters/test_exporters_translations.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.412519 plone.exportimport-1.0.0a2/tests/importers/
+-rw-r--r--   0 davisagli   (501) staff       (20)      666 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/conftest.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1533 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1118 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_content.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1437 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1517 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_portlets.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1434 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_principals.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1413 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1413 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1446 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/importers/test_importers_translations.py
+drwxr-xr-x   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:21.414029 plone.exportimport-1.0.0a2/tests/utils/
+-rw-r--r--   0 davisagli   (501) staff       (20)        0 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/conftest.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3700 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_content_core.py
+-rw-r--r--   0 davisagli   (501) staff       (20)      860 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_content_revisions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1304 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_dates.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     3688 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_discussions.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1365 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_path.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1023 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_principals_groups.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1184 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_principals_members.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     1252 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_redirects.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5384 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_relations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     5186 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tests/utils/test_utils_translations.py
+-rw-r--r--   0 davisagli   (501) staff       (20)     4873 2024-04-18 23:23:20.000000 plone.exportimport-1.0.0a2/tox.ini
```

### Comparing `plone.exportimport-1.0.0a1/.editorconfig` & `plone.exportimport-1.0.0a2/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/.flake8` & `plone.exportimport-1.0.0a2/.flake8`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/.gitignore` & `plone.exportimport-1.0.0a2/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/.meta.toml` & `plone.exportimport-1.0.0a2/.meta.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [meta]
 template = "default"
 commit-id = "fafcd936"
 
 [pyproject]
 codespell_skip = "*.min.js"
 codespell_ignores = "vew"
-dependencies_ignores = "['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']"
+dependencies_ignores = "['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing', 'plone.portlets', 'plone.app.portlets']"
 dependencies_mappings = [
     "Plone = ['Products.CMFPlone', 'Products.CMFCore', 'Products.GenericSetup']",
     ]
 
 [tox]
 test_runner = "pytest"
 test_path = "/tests"
```

### Comparing `plone.exportimport-1.0.0a1/.pre-commit-config.yaml` & `plone.exportimport-1.0.0a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/CHANGES.md` & `plone.exportimport-1.0.0a2/CHANGES.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2024-04-18)
+
+
+### New features:
+
+- Support export/import of portlets if plone.app.portlets is installed. @davisagli #8
+
+
 ## 1.0.0a1 (2024-04-17)
 
 
 ### New features:
 
 - Implement exporter and importer for content [@ericof] #1
 - Implement exporter and importer for members and groups [@ericof] #2
```

### Comparing `plone.exportimport-1.0.0a1/LICENSE` & `plone.exportimport-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/Makefile` & `plone.exportimport-1.0.0a2/Makefile`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/PKG-INFO` & `plone.exportimport-1.0.0a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.exportimport
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Plone content export / import support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -57,14 +57,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2024-04-18)
+
+
+### New features:
+
+- Support export/import of portlets if plone.app.portlets is installed. @davisagli #8
+
+
 ## 1.0.0a1 (2024-04-17)
 
 
 ### New features:
 
 - Implement exporter and importer for content [@ericof] #1
 - Implement exporter and importer for members and groups [@ericof] #2
```

### Comparing `plone.exportimport-1.0.0a1/README.md` & `plone.exportimport-1.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/Makefile` & `plone.exportimport-1.0.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/_static/favicon.ico` & `plone.exportimport-1.0.0a2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/_static/logo.svg` & `plone.exportimport-1.0.0a2/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/_static/styles.css` & `plone.exportimport-1.0.0a2/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/conf.py` & `plone.exportimport-1.0.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/develop.md` & `plone.exportimport-1.0.0a2/docs/develop.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/features.md` & `plone.exportimport-1.0.0a2/docs/features.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/index.md` & `plone.exportimport-1.0.0a2/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/docs/installation.md` & `plone.exportimport-1.0.0a2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/pyproject.toml` & `plone.exportimport-1.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
   'zope.sendmail', 'Zope'
 ]
 'plone.base' = [
   'plone.batching', 'plone.registry', 'plone.schema','plone.z3cform',
   'Products.CMFCore', 'Products.CMFDynamicViewFTI',
 ]
 python-dateutil = ['dateutil']
-ignore-packages = ['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing']
+ignore-packages = ['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing', 'plone.portlets', 'plone.app.portlets']
 Plone = ['Products.CMFPlone', 'Products.CMFCore', 'Products.GenericSetup']
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pyproject]
 #  dependencies_ignores = "['zestreleaser.towncrier']"
 #  dependencies_mappings = [
```

### Comparing `plone.exportimport-1.0.0a1/requirements-docs.txt` & `plone.exportimport-1.0.0a2/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/setup.py` & `plone.exportimport-1.0.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.exportimport",
-    version="1.0.0a1",
+    version="1.0.0a2",
     description="Plone content export / import support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -50,14 +50,15 @@
         "python-dateutil",
         "plone.api",
         "plone.app.contenttypes",
         "plone.app.dexterity",
         "plone.app.discussion",
         "plone.app.multilingual",
         "plone.app.redirector",
+        "plone.app.textfield",
         "plone.app.users",
         "plone.base",
         "plone.dexterity",
         "plone.namedfile",
         "plone.restapi",
         "plone.uuid",
         "Products.CMFEditions",
```

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/cli/__init__.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/configure.zcml` & `plone.exportimport-1.0.0a2/src/plone/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/blob.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/blob.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/deserializers/blocks.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/deserializers/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/__init__.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,39 +11,42 @@
 from typing import Optional
 from zope.component import getAdapter
 from zope.component import hooks
 from zope.component import queryAdapter
 from zope.interface import implementer
 
 
+EXPORTER_NAMES = [
+    "plone.exporter.content",
+    "plone.exporter.principals",
+    "plone.exporter.redirects",
+    "plone.exporter.relations",
+    "plone.exporter.translations",
+    "plone.exporter.discussions",
+    "plone.exporter.portlets",
+]
+
+
 ExporterMapping = Dict[str, BaseExporter]
 
 
 @implementer(interfaces.IExporter)
 class Exporter:
     """Export content from a Plone Site."""
 
-    exporter_names = (
-        "plone.exporter.content",
-        "plone.exporter.principals",
-        "plone.exporter.redirects",
-        "plone.exporter.relations",
-        "plone.exporter.translations",
-        "plone.exporter.discussions",
-    )
     exporters: ExporterMapping
 
     def __init__(self, site):
         self.site = site
         self.exporters = self.all_exporters()
 
     def all_exporters(self) -> ExporterMapping:
         """Return all exporters."""
         exporters = {}
-        for exporter_name in self.exporter_names:
+        for exporter_name in EXPORTER_NAMES:
             exporter = queryAdapter(
                 self.site, interfaces.INamedExporter, name=exporter_name
             )
             if exporter:
                 exporters[exporter_name] = exporter
         return exporters
```

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/base.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/base.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/configure.zcml` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/configure.zcml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-<configure xmlns="http://namespaces.zope.org/zope">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
   <!-- Main exporter -->
   <adapter
       factory=".Exporter"
       for="plone.base.interfaces.siteroot.IPloneSiteRoot"
       />
 
   <!-- Exporters -->
@@ -39,9 +42,17 @@
   <adapter
       factory=".discussions.DiscussionsExporter"
       provides="plone.exportimport.interfaces.INamedExporter"
       for="plone.base.interfaces.siteroot.IPloneSiteRoot"
       name="plone.exporter.discussions"
       />
 
+  <configure zcml:condition="installed plone.app.portlets">
+    <adapter
+        factory=".portlets.PortletsExporter"
+        provides="plone.exportimport.interfaces.INamedExporter"
+        for="plone.base.interfaces.siteroot.IPloneSiteRoot"
+        name="plone.exporter.portlets"
+        />
+  </configure>
 
 </configure>
```

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/content.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/discussions.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/principals.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/redirects.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/relations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/exporters/translations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/exporters/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/__init__.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,39 +8,41 @@
 from typing import List
 from zope.component import getAdapter
 from zope.component import hooks
 from zope.component import queryAdapter
 from zope.interface import implementer
 
 
+IMPORTER_NAMES = [
+    "plone.importer.content",
+    "plone.importer.principals",
+    "plone.importer.redirects",
+    "plone.importer.relations",
+    "plone.importer.translations",
+    "plone.importer.discussions",
+    "plone.importer.portlets",
+]
+
 ImporterMapping = Dict[str, BaseImporter]
 
 
 @implementer(interfaces.IImporter)
 class Importer:
     """Import content into a Plone Site."""
 
-    importer_names = (
-        "plone.importer.content",
-        "plone.importer.principals",
-        "plone.importer.redirects",
-        "plone.importer.relations",
-        "plone.importer.translations",
-        "plone.importer.discussions",
-    )
     importers: ImporterMapping
 
     def __init__(self, site):
         self.site = site
         self.importers = self.all_importers()
 
     def all_importers(self) -> List[BaseImporter]:
         """Return all importers."""
         importers = {}
-        for importer_name in self.importer_names:
+        for importer_name in IMPORTER_NAMES:
             importer = queryAdapter(
                 self.site, interfaces.INamedImporter, name=importer_name
             )
             if importer:
                 importers[importer_name] = importer
         return importers
```

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/base.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/base.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/configure.zcml` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/configure.zcml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-<configure xmlns="http://namespaces.zope.org/zope">
+<configure
+    xmlns="http://namespaces.zope.org/zope"
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    >
   <!-- Main importer -->
   <adapter
       factory=".Importer"
       for="plone.base.interfaces.siteroot.IPloneSiteRoot"
       />
 
   <!-- Importers -->
@@ -39,9 +42,17 @@
   <adapter
       factory=".discussions.DiscussionsImporter"
       provides="plone.exportimport.interfaces.INamedImporter"
       for="plone.base.interfaces.siteroot.IPloneSiteRoot"
       name="plone.importer.discussions"
       />
 
+  <configure zcml:condition="installed plone.app.portlets">
+    <adapter
+        factory=".portlets.PortletsImporter"
+        provides="plone.exportimport.interfaces.INamedImporter"
+        for="plone.base.interfaces.siteroot.IPloneSiteRoot"
+        name="plone.importer.portlets"
+        />
+  </configure>
 
 </configure>
```

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/content.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/discussions.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/principals.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/redirects.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/relations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/importers/translations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/importers/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/interfaces.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/blob.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/blob.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/serializers/blocks.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/serializers/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/testing/__init__.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/types.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/types.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/cli.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/cli.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/__init__.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/blocks.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/core.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/core.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/export_helpers.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/export_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/import_helpers.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/import_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/content/revisions.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/content/revisions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/dates.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/dates.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/discussions.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/path.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/path.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/groups.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/groups.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/helpers.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/principals/members.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/principals/members.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/redirects.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/relations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone/exportimport/utils/translations.py` & `plone.exportimport-1.0.0a2/src/plone/exportimport/utils/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/PKG-INFO` & `plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.exportimport
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: Plone content export / import support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -57,14 +57,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a2 (2024-04-18)
+
+
+### New features:
+
+- Support export/import of portlets if plone.app.portlets is installed. @davisagli #8
+
+
 ## 1.0.0a1 (2024-04-17)
 
 
 ### New features:
 
 - Implement exporter and importer for content [@ericof] #1
 - Implement exporter and importer for members and groups [@ericof] #2
```

### Comparing `plone.exportimport-1.0.0a1/src/plone.exportimport.egg-info/SOURCES.txt` & `plone.exportimport-1.0.0a2/src/plone.exportimport.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -48,37 +48,40 @@
 src/plone/exportimport/deserializers/blocks.py
 src/plone/exportimport/deserializers/configure.zcml
 src/plone/exportimport/exporters/__init__.py
 src/plone/exportimport/exporters/base.py
 src/plone/exportimport/exporters/configure.zcml
 src/plone/exportimport/exporters/content.py
 src/plone/exportimport/exporters/discussions.py
+src/plone/exportimport/exporters/portlets.py
 src/plone/exportimport/exporters/principals.py
 src/plone/exportimport/exporters/redirects.py
 src/plone/exportimport/exporters/relations.py
 src/plone/exportimport/exporters/translations.py
 src/plone/exportimport/importers/__init__.py
 src/plone/exportimport/importers/base.py
 src/plone/exportimport/importers/configure.zcml
 src/plone/exportimport/importers/content.py
 src/plone/exportimport/importers/discussions.py
+src/plone/exportimport/importers/portlets.py
 src/plone/exportimport/importers/principals.py
 src/plone/exportimport/importers/redirects.py
 src/plone/exportimport/importers/relations.py
 src/plone/exportimport/importers/translations.py
 src/plone/exportimport/serializers/__init__.py
 src/plone/exportimport/serializers/blob.py
 src/plone/exportimport/serializers/blocks.py
 src/plone/exportimport/serializers/configure.zcml
 src/plone/exportimport/testing/__init__.py
 src/plone/exportimport/utils/__init__.py
 src/plone/exportimport/utils/cli.py
 src/plone/exportimport/utils/dates.py
 src/plone/exportimport/utils/discussions.py
 src/plone/exportimport/utils/path.py
+src/plone/exportimport/utils/portlets.py
 src/plone/exportimport/utils/redirects.py
 src/plone/exportimport/utils/relations.py
 src/plone/exportimport/utils/translations.py
 src/plone/exportimport/utils/zca.py
 src/plone/exportimport/utils/content/__init__.py
 src/plone/exportimport/utils/content/blocks.py
 src/plone/exportimport/utils/content/core.py
@@ -87,14 +90,15 @@
 src/plone/exportimport/utils/content/revisions.py
 src/plone/exportimport/utils/principals/__init__.py
 src/plone/exportimport/utils/principals/groups.py
 src/plone/exportimport/utils/principals/helpers.py
 src/plone/exportimport/utils/principals/members.py
 tests/conftest.py
 tests/_resources/base_import/discussions.json
+tests/_resources/base_import/portlets.json
 tests/_resources/base_import/principals.json
 tests/_resources/base_import/redirects.json
 tests/_resources/base_import/relations.json
 tests/_resources/base_import/translations.json
 tests/_resources/base_import/content/__metadata__.json
 tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json
 tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json
@@ -134,22 +138,24 @@
 tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
 tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
 tests/_resources/multilingual_import/content/plone_site_root/data.json
 tests/exporters/conftest.py
 tests/exporters/test_exporters.py
 tests/exporters/test_exporters_content.py
 tests/exporters/test_exporters_discussions.py
+tests/exporters/test_exporters_portlets.py
 tests/exporters/test_exporters_principals.py
 tests/exporters/test_exporters_redirects.py
 tests/exporters/test_exporters_relations.py
 tests/exporters/test_exporters_translations.py
 tests/importers/conftest.py
 tests/importers/test_importers.py
 tests/importers/test_importers_content.py
 tests/importers/test_importers_discussions.py
+tests/importers/test_importers_portlets.py
 tests/importers/test_importers_principals.py
 tests/importers/test_importers_redirects.py
 tests/importers/test_importers_relations.py
 tests/importers/test_importers_translations.py
 tests/utils/conftest.py
 tests/utils/test_utils_content_core.py
 tests/utils/test_utils_content_revisions.py
```

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/__metadata__.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/__metadata__.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/content/plone_site_root/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/content/plone_site_root/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/discussions.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/discussions.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/base_import/principals.json` & `plone.exportimport-1.0.0a2/tests/_resources/base_import/principals.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/__metadata__.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/__metadata__.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/content/plone_site_root/data.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/content/plone_site_root/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/discussions.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/discussions.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/principals.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/principals.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/_resources/multilingual_import/translations.json` & `plone.exportimport-1.0.0a2/tests/_resources/multilingual_import/translations.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/conftest.py` & `plone.exportimport-1.0.0a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/conftest.py` & `plone.exportimport-1.0.0a2/tests/exporters/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def test_exporter_is_correct_instance(self):
         assert isinstance(self.exporter, Exporter)
 
     def test_all_exporters(self):
         exporters = self.exporter.all_exporters()
         assert isinstance(exporters, dict)
-        assert len(exporters) == 6
+        assert len(exporters) >= 6
 
     @pytest.mark.parametrize(
         "exporter_name",
         [
             "plone.exporter.content",
             "plone.exporter.principals",
             "plone.exporter.redirects",
@@ -81,8 +81,8 @@
 
     def test_exporter_is_correct_instance(self):
         assert isinstance(self.exporter, Exporter)
 
     def test_all_exporters(self):
         exporters = self.exporter.all_exporters()
         assert isinstance(exporters, dict)
-        assert len(exporters) == 6
+        assert len(exporters) >= 6
```

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_content.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_discussions.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_principals.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_redirects.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_relations.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/exporters/test_exporters_translations.py` & `plone.exportimport-1.0.0a2/tests/exporters/test_exporters_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/conftest.py` & `plone.exportimport-1.0.0a2/tests/importers/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def test_importer_is_correct_class(self):
         assert isinstance(self.importer, Importer)
 
     def test_all_importers(self):
         importers = self.importer.all_importers()
         assert isinstance(importers, dict)
-        assert len(importers) == 6
+        assert len(importers) >= 6
 
     @pytest.mark.parametrize(
         "importer_name",
         [
             "plone.importer.content",
             "plone.importer.principals",
             "plone.importer.redirects",
@@ -41,9 +41,9 @@
             "RedirectsImporter: Imported 0 redirects",
         ],
     )
     def test_import_site(self, base_import_path, msg: str):
         results = self.importer.import_site(base_import_path)
         assert isinstance(results, list)
         # One entry per importer
-        assert len(results) == 6
+        assert len(results) >= 6
         assert msg in results
```

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_content.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_discussions.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_principals.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_redirects.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_relations.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/importers/test_importers_translations.py` & `plone.exportimport-1.0.0a2/tests/importers/test_importers_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_content_core.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_content_core.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_content_revisions.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_content_revisions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_dates.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_dates.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_discussions.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_path.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_path.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_principals_groups.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_principals_groups.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_principals_members.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_principals_members.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_redirects.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_relations.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tests/utils/test_utils_translations.py` & `plone.exportimport-1.0.0a2/tests/utils/test_utils_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a1/tox.ini` & `plone.exportimport-1.0.0a2/tox.ini`

 * *Files identical despite different names*

