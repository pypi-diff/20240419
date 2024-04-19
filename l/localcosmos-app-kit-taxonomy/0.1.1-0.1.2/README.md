# Comparing `tmp/localcosmos_app_kit_taxonomy-0.1.1.tar.gz` & `tmp/localcosmos_app_kit_taxonomy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localcosmos_app_kit_taxonomy-0.1.1.tar", last modified: Wed Apr 10 13:13:13 2024, max compression
+gzip compressed data, was "localcosmos_app_kit_taxonomy-0.1.2.tar", last modified: Fri Apr 19 07:17:38 2024, max compression
```

## Comparing `localcosmos_app_kit_taxonomy-0.1.1.tar` & `localcosmos_app_kit_taxonomy-0.1.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.807989 localcosmos_app_kit_taxonomy-0.1.1/
--rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit_taxonomy-0.1.1/LICENCE
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-10 13:12:47.000000 localcosmos_app_kit_taxonomy-0.1.1/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)      650 2024-04-10 13:13:13.807989 localcosmos_app_kit_taxonomy-0.1.1/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)       68 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)      650 2024-04-10 13:13:13.000000 localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2441 2024-04-10 13:13:13.000000 localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-10 13:13:13.000000 localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        9 2024-04-10 13:13:13.000000 localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-10 13:13:13.807989 localcosmos_app_kit_taxonomy-0.1.1/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      921 2024-04-10 13:12:56.000000 localcosmos_app_kit_taxonomy-0.1.1/setup.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)     1251 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/DBRouter.py
--rw-r--r--   0 tom       (1000) tom       (1000)     4361 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/TaxonSearch.py
--rw-r--r--   0 tom       (1000) tom       (1000)       73 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      149 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5980 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/lazy.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7625 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/taxonomy_recreate_indices.py
--rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/update_taxonomic_database.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     1298 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/0002_auto_20220503_0747.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9825 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1664 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/signals.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/
--rw-r--r--   0 tom       (1000) tom       (1000)    37032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/TaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/
--rw-r--r--   0 tom       (1000) tom       (1000)    50987 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/AlgaebaseManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/apps.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.801323 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4336 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/
--rw-r--r--   0 tom       (1000) tom       (1000)    10255 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/ColTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)     8228 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/ColTaxonSourceManager2015.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)       98 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/apps.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4207 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      928 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/models.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)     5699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/tests/TestColTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/admin.py
--rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2690 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/forms.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/migrations/
--rw-r--r--   0 tom       (1000) tom       (1000)     4246 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/migrations/0001_initial.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/migrations/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)      756 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/models.py
--rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/tests.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10323 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/views.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.797990 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/
--rw-r--r--   0 tom       (1000) tom       (1000)      522 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/taxontreeview.html
--rw-r--r--   0 tom       (1000) tom       (1000)      324 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/treeview_children.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/
--rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget.html
--rw-r--r--   0 tom       (1000) tom       (1000)     1784 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html
--rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-10 13:13:13.804656 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/
--rw-r--r--   0 tom       (1000) tom       (1000)    49583 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/TestTaxonSourceManager.py
--rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/__init__.py
--rw-r--r--   0 tom       (1000) tom       (1000)     5567 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/test_lazy.py
--rw-r--r--   0 tom       (1000) tom       (1000)      560 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/utils.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3200 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.1/taxonomy/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1086 2024-04-05 12:51:29.000000 localcosmos_app_kit_taxonomy-0.1.2/LICENCE
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2024-04-10 13:12:47.000000 localcosmos_app_kit_taxonomy-0.1.2/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)       68 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)      649 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2441 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        9 2024-04-19 07:17:38.000000 localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      920 2024-04-19 07:15:54.000000 localcosmos_app_kit_taxonomy-0.1.2/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1251 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/DBRouter.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     4361 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/TaxonSearch.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       73 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      149 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5980 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/lazy.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7625 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/taxonomy_recreate_indices.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      634 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/update_taxonomic_database.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1298 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      553 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0002_auto_20220503_0747.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9825 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1664 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/signals.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/
+-rw-r--r--   0 tom       (1000) tom       (1000)    37032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/TaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/
+-rw-r--r--   0 tom       (1000) tom       (1000)    50987 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/AlgaebaseManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      110 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/apps.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4336 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/
+-rw-r--r--   0 tom       (1000) tom       (1000)    10255 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     8228 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager2015.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       98 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/apps.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4207 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      928 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/models.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)     5699 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/TestColTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.143975 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       63 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/admin.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      104 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2690 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/forms.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/
+-rw-r--r--   0 tom       (1000) tom       (1000)     4246 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/0001_initial.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      756 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/models.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       60 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/tests.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1032 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10323 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/views.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.140642 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/
+-rw-r--r--   0 tom       (1000) tom       (1000)      522 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/taxontreeview.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      324 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/treeview_children.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/
+-rw-r--r--   0 tom       (1000) tom       (1000)       69 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget.html
+-rw-r--r--   0 tom       (1000) tom       (1000)     1784 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html
+-rw-r--r--   0 tom       (1000) tom       (1000)      642 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2024-04-19 07:17:38.147308 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/
+-rw-r--r--   0 tom       (1000) tom       (1000)    49583 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/TestTaxonSourceManager.py
+-rw-r--r--   0 tom       (1000) tom       (1000)        0 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/__init__.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     5567 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/test_lazy.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      560 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2174 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/utils.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3200 2024-04-09 13:45:54.000000 localcosmos_app_kit_taxonomy-0.1.2/taxonomy/views.py
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/LICENCE` & `localcosmos_app_kit_taxonomy-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/PKG-INFO` & `localcosmos_app_kit_taxonomy-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit_taxonomy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Local Cosmos Taxonomy django app
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity,taxonomy
 Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # App Kit Taxonomy
 
 Taxonomy django app for the Local Cosmo App Kit.
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO` & `localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: localcosmos_app_kit_taxonomy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Local Cosmos Taxonomy django app
 Home-page: https://github.com/localcosmos/app-kit
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,localcosmos,localcosmos server,biodiversity,taxonomy
 Platform: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENCE
 
 # App Kit Taxonomy
 
 Taxonomy django app for the Local Cosmo App Kit.
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt` & `localcosmos_app_kit_taxonomy-0.1.2/localcosmos_app_kit_taxonomy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/setup.py` & `localcosmos_app_kit_taxonomy-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 install_requires = [
 
 ]
 
 setup(
     name='localcosmos_app_kit_taxonomy',
-    version='0.1.1',
+    version='0.1.2',
     description='Local Cosmos Taxonomy django app',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, localcosmos, localcosmos server, biodiversity, taxonomy',
     author='Thomas Uher',
@@ -21,11 +21,11 @@
     url='https://github.com/localcosmos/app-kit',
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.10',
+    python_requires='>=3.6',
     include_package_data=True,
     install_requires=install_requires,
 )
```

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/DBRouter.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/DBRouter.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/TaxonSearch.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/TaxonSearch.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/lazy.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/lazy.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/taxonomy_recreate_indices.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/taxonomy_recreate_indices.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/management/commands/update_taxonomic_database.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/management/commands/update_taxonomic_database.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/migrations/0002_auto_20220503_0747.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/migrations/0002_auto_20220503_0747.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/models.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/signals.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/signals.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/TaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/TaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/AlgaebaseManager.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/AlgaebaseManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/algaebase/models.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/algaebase/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/ColTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/ColTaxonSourceManager2015.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/ColTaxonSourceManager2015.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/models.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/col/tests/TestColTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/col/tests/TestColTaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/forms.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/forms.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/migrations/0001_initial.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/models.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/models.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/urls.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/sources/custom/views.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/sources/custom/views.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/taxontreeview.html` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/taxontreeview.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_base.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/templates/taxonomy/widgets/taxon_autocomplete_widget_fixed_source.html`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/TestTaxonSourceManager.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/TestTaxonSourceManager.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/tests/test_lazy.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/tests/test_lazy.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/urls.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/urls.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/utils.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/utils.py`

 * *Files identical despite different names*

### Comparing `localcosmos_app_kit_taxonomy-0.1.1/taxonomy/views.py` & `localcosmos_app_kit_taxonomy-0.1.2/taxonomy/views.py`

 * *Files identical despite different names*

