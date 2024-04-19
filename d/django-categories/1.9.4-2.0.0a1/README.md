# Comparing `tmp/django-categories-1.9.4.tar.gz` & `tmp/django-categories-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-categories-1.9.4.tar", last modified: Fri Apr 19 08:51:23 2024, max compression
+gzip compressed data, was "django-categories-2.0.0a1.tar", last modified: Wed Apr 17 14:36:57 2024, max compression
```

## Comparing `django-categories-1.9.4.tar` & `django-categories-2.0.0a1.tar`

### file list

```diff
@@ -1,186 +1,186 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.433283 django-categories-1.9.4/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3338 2024-04-19 08:51:22.000000 django-categories-1.9.4/.changelog-config.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-19 08:51:22.000000 django-categories-1.9.4/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.417284 django-categories-1.9.4/.github/changelog_templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-19 08:51:22.000000 django-categories-1.9.4/.github/changelog_templates/commit.md.jinja
--rw-rw-r--   0 petr      (1000) petr      (1000)      214 2024-04-19 08:51:22.000000 django-categories-1.9.4/.github/changelog_templates/version_heading.md.jinja
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.417284 django-categories-1.9.4/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)      878 2024-04-19 08:51:22.000000 django-categories-1.9.4/.github/workflows/publish-docs.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)     1153 2024-04-19 08:51:22.000000 django-categories-1.9.4/.github/workflows/publish-package.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)     1188 2024-04-19 08:51:22.000000 django-categories-1.9.4/.github/workflows/run-tests.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)     2516 2024-04-19 08:51:22.000000 django-categories-1.9.4/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)     1507 2024-04-19 08:51:22.000000 django-categories-1.9.4/.pre-commit-config.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-19 08:51:22.000000 django-categories-1.9.4/.readthedocs.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)    98110 2024-04-19 08:51:22.000000 django-categories-1.9.4/CHANGELOG.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-19 08:51:22.000000 django-categories-1.9.4/CONTRIBUTING.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      589 2024-04-19 08:51:22.000000 django-categories-1.9.4/CREDITS.md
--rw-rw-r--   0 petr      (1000) petr      (1000)    11357 2024-04-19 08:51:22.000000 django-categories-1.9.4/LICENSE.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      600 2024-04-19 08:51:22.000000 django-categories-1.9.4/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     3168 2024-04-19 08:51:22.000000 django-categories-1.9.4/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-19 08:51:22.000000 django-categories-1.9.4/NOTICES.txt
--rw-r--r--   0 petr      (1000) petr      (1000)     2653 2024-04-19 08:51:23.433283 django-categories-1.9.4/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2253 2024-04-19 08:51:22.000000 django-categories-1.9.4/README.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.417284 django-categories-1.9.4/categories/
--rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3461 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/admin.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.417284 django-categories-1.9.4/categories/api/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/api/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1408 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/apps.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6202 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/base.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/editor/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/editor/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/editor/locale/de/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/editor/locale/de/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      443 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)     1093 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 petr      (1000) petr      (1000)       30 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      426 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/editor/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/editor/static/editor/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1820 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/jquery.treeTable.css
--rw-rw-r--   0 petr      (1000) petr      (1000)    13042 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/jquery.treeTable.js
--rw-rw-r--   0 petr      (1000) petr      (1000)     2886 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/toggle-collapse-dark.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     2864 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/toggle-collapse-light.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     2894 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/toggle-expand-dark.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     2863 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/static/editor/toggle-expand-light.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/editor/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/editor/templates/admin/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/editor/templates/admin/editor/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1921 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templates/admin/editor/grappelli_tree_editor.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1165 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templates/admin/editor/grappelli_tree_list_results.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1731 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templates/admin/editor/tree_editor.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1593 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templates/admin/editor/tree_list_results.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/editor/templatetags/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templatetags/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6033 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/templatetags/admin_tree_list_tags.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    12350 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/tree_editor.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      401 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/editor/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      681 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fields.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      318 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fixtures/categories.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     5076 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fixtures/genres.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)    69136 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fixtures/musicgenres.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      124 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fixtures/test_category_spaces.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/fixtures/test_category_tabs.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     1618 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/genericcollection.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.409284 django-categories-1.9.4/categories/locale/de/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/locale/de/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3595 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)     4408 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/locale/fr/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3976 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)     5156 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/locale/it/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.421284 django-categories-1.9.4/categories/locale/it/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3877 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)     5024 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      932 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/management/commands/add_category_fields.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1097 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/management/commands/drop_category_field.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2864 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/management/commands/import_categories.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2671 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migration.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4891 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      866 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migrations/0002_auto_20170217_1111.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1409 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migrations/0003_auto_20200306_1050.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      617 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migrations/0004_auto_20200517_1832.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5117 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6952 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/registration.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1994 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/static/js/
--rw-rw-r--   0 petr      (1000) petr      (1000)      806 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/static/js/genericcollections.js
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/categories/templates/admin/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/templates/admin/edit_inline/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3066 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/admin/edit_inline/gen_coll_tabular.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/templates/categories/
--rw-rw-r--   0 petr      (1000) petr      (1000)      427 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/ancestors_ul.html
--rw-rw-r--   0 petr      (1000) petr      (1000)       61 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/breadcrumbs.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      960 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/category_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      216 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/category_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      462 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templates/categories/ul_tree.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.425283 django-categories-1.9.4/categories/templatetags/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templatetags/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    16325 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/templatetags/category_tags.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/categories/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3105 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2261 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_category_import.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9554 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_image.jpg
--rw-rw-r--   0 petr      (1000) petr      (1000)      679 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_manager.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1007 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_mgmt_commands.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1038 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1951 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_registration.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3434 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_templatetags.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      814 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3342 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      314 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5882 2024-04-19 08:51:22.000000 django-categories-1.9.4/categories/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.433283 django-categories-1.9.4/django_categories.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     2653 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     4922 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       12 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       11 2024-04-19 08:51:23.000000 django-categories-1.9.4/django_categories.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/doc_src/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/doc_src/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/doc_src/_static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)      516 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/_static/css/custom.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.413284 django-categories-1.9.4/doc_src/_templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/doc_src/_templates/autosummary/
--rw-rw-r--   0 petr      (1000) petr      (1000)      208 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/_templates/autosummary/base.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      672 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/_templates/autosummary/class.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1387 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/_templates/autosummary/module.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/doc_src/api/
--rw-rw-r--   0 petr      (1000) petr      (1000)       69 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/api/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/changelog.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1999 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2448 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/getting_started.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      766 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1071 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3091 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/make.bat
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.429283 django-categories-1.9.4/doc_src/reference/
--rw-rw-r--   0 petr      (1000) petr      (1000)      135 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/reference/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/reference/management_commands.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3269 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/reference/models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3644 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/reference/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9483 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/reference/templatetags.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       43 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.433283 django-categories-1.9.4/doc_src/user_guide/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1699 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/adding_the_fields.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1717 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/admin_settings.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.433283 django-categories-1.9.4/doc_src/user_guide/code_examples/
--rw-rw-r--   0 petr      (1000) petr      (1000)      200 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories1.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories2.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1185 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories3.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories4.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      174 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories5.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      411 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories6.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      704 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories7.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2420 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/custom_categories.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/index.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     4542 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/registering_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2259 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      837 2024-04-19 08:51:22.000000 django-categories-1.9.4/doc_src/user_guide/usage_example_template.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2024-04-19 08:51:22.000000 django-categories-1.9.4/pyproject.toml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-19 08:51:23.433283 django-categories-1.9.4/requirements/
--rw-rw-r--   0 petr      (1000) petr      (1000)       80 2024-04-19 08:51:22.000000 django-categories-1.9.4/requirements/dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       12 2024-04-19 08:51:22.000000 django-categories-1.9.4/requirements/prod.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      143 2024-04-19 08:51:22.000000 django-categories-1.9.4/requirements/test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-19 08:51:22.000000 django-categories-1.9.4/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     1448 2024-04-19 08:51:23.433283 django-categories-1.9.4/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1421 2024-04-19 08:51:22.000000 django-categories-1.9.4/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1214 2024-04-19 08:51:22.000000 django-categories-1.9.4/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3338 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.changelog-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.876835 django-categories-2.0.0a1/.github/changelog_templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.github/changelog_templates/commit.md.jinja
+-rw-rw-r--   0 petr      (1000) petr      (1000)      214 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.github/changelog_templates/version_heading.md.jinja
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.876835 django-categories-2.0.0a1/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      878 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.github/workflows/publish-docs.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1153 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.github/workflows/publish-package.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1188 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.github/workflows/run-tests.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2516 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1507 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.pre-commit-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/.readthedocs.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)    98622 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/CHANGELOG.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/CONTRIBUTING.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      589 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/CREDITS.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11357 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/LICENSE.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      600 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3168 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/NOTICES.txt
+-rw-r--r--   0 petr      (1000) petr      (1000)     2686 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2253 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/README.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.876835 django-categories-2.0.0a1/categories/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      114 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3461 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/admin.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.876835 django-categories-2.0.0a1/categories/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/api/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1408 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/apps.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6216 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/base.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.876835 django-categories-2.0.0a1/categories/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/categories/editor/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/categories/editor/locale/de/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/editor/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      443 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1093 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 petr      (1000) petr      (1000)       30 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      426 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/categories/editor/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/editor/static/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1820 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/jquery.treeTable.css
+-rw-rw-r--   0 petr      (1000) petr      (1000)    13042 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/jquery.treeTable.js
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2886 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/toggle-collapse-dark.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2864 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/toggle-collapse-light.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2894 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/toggle-expand-dark.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2863 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/static/editor/toggle-expand-light.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/categories/editor/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.868835 django-categories-2.0.0a1/categories/editor/templates/admin/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/editor/templates/admin/editor/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1921 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templates/admin/editor/grappelli_tree_editor.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1165 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templates/admin/editor/grappelli_tree_list_results.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1731 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templates/admin/editor/tree_editor.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1593 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templates/admin/editor/tree_list_results.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/editor/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6033 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/templatetags/admin_tree_list_tags.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    12350 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/tree_editor.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      401 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/editor/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      631 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fields.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      318 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fixtures/categories.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5076 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fixtures/genres.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)    69138 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fixtures/musicgenres.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      124 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fixtures/test_category_spaces.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      106 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/fixtures/test_category_tabs.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1618 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/genericcollection.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/locale/de/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3595 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4408 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/locale/fr/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3976 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5156 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/locale/it/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3877 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5024 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.880835 django-categories-2.0.0a1/categories/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      932 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/management/commands/add_category_fields.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1097 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/management/commands/drop_category_field.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2862 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/management/commands/import_categories.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2671 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4891 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      866 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/0002_auto_20170217_1111.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1409 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/0003_auto_20200306_1050.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      617 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/0004_auto_20200517_1832.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1159 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/0005_unique_category_slug.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5117 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6952 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/registration.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1994 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/static/js/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      806 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/static/js/genericcollections.js
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/categories/templates/admin/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/templates/admin/edit_inline/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3066 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/admin/edit_inline/gen_coll_tabular.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/templates/categories/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      427 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/ancestors_ul.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)       61 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      179 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/breadcrumbs.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      960 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/category_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      216 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/category_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      462 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templates/categories/ul_tree.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/templatetags/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templatetags/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16325 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/templatetags/category_tags.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.884835 django-categories-2.0.0a1/categories/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3105 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2263 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_category_import.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9554 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_image.jpg
+-rw-rw-r--   0 petr      (1000) petr      (1000)      679 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_manager.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1007 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_mgmt_commands.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1608 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_migrations.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1038 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1951 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_registration.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3434 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_templatetags.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3342 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      435 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5882 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/categories/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/django_categories.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     2686 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4958 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       11 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/django_categories.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.888835 django-categories-2.0.0a1/doc_src/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/doc_src/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.888835 django-categories-2.0.0a1/doc_src/_static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      516 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/_static/css/custom.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.872835 django-categories-2.0.0a1/doc_src/_templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.888835 django-categories-2.0.0a1/doc_src/_templates/autosummary/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      208 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/_templates/autosummary/base.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      672 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/_templates/autosummary/class.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1387 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/_templates/autosummary/module.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.888835 django-categories-2.0.0a1/doc_src/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       69 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/api/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/changelog.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1999 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2448 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/getting_started.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      766 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1071 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3091 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/make.bat
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.888835 django-categories-2.0.0a1/doc_src/reference/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      135 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/reference/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/reference/management_commands.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3269 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/reference/models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3644 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/reference/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9483 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/reference/templatetags.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       43 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/doc_src/user_guide/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1699 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/adding_the_fields.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1717 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/admin_settings.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/doc_src/user_guide/code_examples/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      200 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories1.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories2.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1185 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories3.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories4.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      174 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories5.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      411 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories6.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      704 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories7.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2420 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/custom_categories.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/index.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4542 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/registering_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2259 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      837 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/doc_src/user_guide/usage_example_template.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/pyproject.toml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/requirements/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       80 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/requirements/dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       28 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/requirements/prod.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      143 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/requirements/test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1448 2024-04-17 14:36:57.892835 django-categories-2.0.0a1/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1421 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1333 2024-04-17 14:36:57.000000 django-categories-2.0.0a1/tox.ini
```

### Comparing `django-categories-1.9.4/.changelog-config.yaml` & `django-categories-2.0.0a1/.changelog-config.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/.github/workflows/publish-docs.yml` & `django-categories-2.0.0a1/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/.github/workflows/publish-package.yml` & `django-categories-2.0.0a1/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/.github/workflows/run-tests.yaml` & `django-categories-2.0.0a1/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/.gitignore` & `django-categories-2.0.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/.pre-commit-config.yaml` & `django-categories-2.0.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/CHANGELOG.md` & `django-categories-2.0.0a1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 # Changelog
 
-## 1.9.4 (2024-04-18)
 
-- Remove dependency on unicode-slugify, use Django builtin function
+## 2.0.0-alpha.1 (unreleased)
 
-## 1.9.3 (2024-04-17)
+### WARNING
+
+**Breaking change:** Starting with version the 2.0.0 the category slugs are unique.
+While this brings big advantage for simplified category addressing, it can break projects that are containing categories with duplicated slugs.
+If your database contains colliding slugs, they will be automatically renamed by the migration.
+Three categories with slugs ``foo`` will be renamed to ``foo``, ``foo-1``, ``foo-2``.
+If this causes problems in your project, you can rename the categories yourself before running the migration.
+
+- Django 2.1 is no longer supported
+
+
+## 1.9.3 (unreleased)
 
 - Update of Django/Python versions.
 - Supported versions are now Django 2.1-5.0, Python 3.7-3.12
 - Removed code for obsolete versions
 - Add support for Django 4.12 new File storage API (STORAGES)
 
 ## 1.9.2 (2022-09-22)
```

### Comparing `django-categories-1.9.4/CREDITS.md` & `django-categories-2.0.0a1/CREDITS.md`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/LICENSE.txt` & `django-categories-2.0.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/MANIFEST.in` & `django-categories-2.0.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/Makefile` & `django-categories-2.0.0a1/Makefile`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/PKG-INFO` & `django-categories-2.0.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: django-categories
-Version: 1.9.4
+Version: 2.0.0a1
 Summary: A way to handle one or more hierarchical category trees in django.
 Home-page: http://github.com/jazzband/django-categories
 Author: Corey Oordt
 Author-email: coreyoordt@gmail.com
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICES.txt
 Requires-Dist: django-mptt
+Requires-Dist: unicode-slugify
 
 # Django Categories
 
 [![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)
 [![codecov](https://codecov.io/gh/jazzband/django-categories/branch/master/graph/badge.svg?token=rW8mpdZqWQ)](https://codecov.io/gh/jazzband/django-categories)
 
 Django Categories grew out of our need to provide a basic hierarchical taxonomy management system that multiple applications could use independently or in concert.
```

### Comparing `django-categories-1.9.4/README.md` & `django-categories-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/admin.py` & `django-categories-2.0.0a1/categories/admin.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/apps.py` & `django-categories-2.0.0a1/categories/apps.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/base.py` & `django-categories-2.0.0a1/categories/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from django.contrib import admin
 from django.db import models
 from django.utils.encoding import force_str
 from django.utils.translation import gettext_lazy as _
 from mptt.fields import TreeForeignKey
 from mptt.managers import TreeManager
 from mptt.models import MPTTModel
+from slugify import slugify
 
 from .editor.tree_editor import TreeEditor
 from .settings import ALLOW_SLUG_CHANGE, SLUG_TRANSLITERATOR
-from .utils import slugify
 
 
 class CategoryManager(models.Manager):
     """
     A manager that adds an "active()" method for all active categories.
     """
 
@@ -42,15 +42,15 @@
         on_delete=models.CASCADE,
         blank=True,
         null=True,
         related_name="children",
         verbose_name=_("parent"),
     )
     name = models.CharField(max_length=100, verbose_name=_("name"))
-    slug = models.SlugField(verbose_name=_("slug"))
+    slug = models.SlugField(verbose_name=_("slug"), unique=True)
     active = models.BooleanField(default=True, verbose_name=_("active"))
 
     objects = CategoryManager()
     tree = TreeManager()
 
     def save(self, *args, **kwargs):
         """
```

### Comparing `django-categories-1.9.4/categories/editor/locale/de/LC_MESSAGES/django.po` & `django-categories-2.0.0a1/categories/editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/jquery.treeTable.css` & `django-categories-2.0.0a1/categories/editor/static/editor/jquery.treeTable.css`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/jquery.treeTable.js` & `django-categories-2.0.0a1/categories/editor/static/editor/jquery.treeTable.js`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/toggle-collapse-dark.png` & `django-categories-2.0.0a1/categories/editor/static/editor/toggle-collapse-dark.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/toggle-collapse-light.png` & `django-categories-2.0.0a1/categories/editor/static/editor/toggle-collapse-light.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/toggle-expand-dark.png` & `django-categories-2.0.0a1/categories/editor/static/editor/toggle-expand-dark.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/static/editor/toggle-expand-light.png` & `django-categories-2.0.0a1/categories/editor/static/editor/toggle-expand-light.png`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/templates/admin/editor/grappelli_tree_editor.html` & `django-categories-2.0.0a1/categories/editor/templates/admin/editor/grappelli_tree_editor.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/templates/admin/editor/grappelli_tree_list_results.html` & `django-categories-2.0.0a1/categories/editor/templates/admin/editor/grappelli_tree_list_results.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/templates/admin/editor/tree_editor.html` & `django-categories-2.0.0a1/categories/editor/templates/admin/editor/tree_editor.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/templates/admin/editor/tree_list_results.html` & `django-categories-2.0.0a1/categories/editor/templates/admin/editor/tree_list_results.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/templatetags/admin_tree_list_tags.py` & `django-categories-2.0.0a1/categories/editor/templatetags/admin_tree_list_tags.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/editor/tree_editor.py` & `django-categories-2.0.0a1/categories/editor/tree_editor.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/fields.py` & `django-categories-2.0.0a1/categories/fields.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,23 +3,19 @@
 from django.db.models import ForeignKey, ManyToManyField
 
 
 class CategoryM2MField(ManyToManyField):
     """A many to many field to a Category model."""
 
     def __init__(self, **kwargs):
-        from .models import Category
-
         if "to" in kwargs:
             kwargs.pop("to")
-        super(CategoryM2MField, self).__init__(to=Category, **kwargs)
+        super(CategoryM2MField, self).__init__(to="categories.Category", **kwargs)
 
 
 class CategoryFKField(ForeignKey):
     """A foreign key to the Category model."""
 
     def __init__(self, **kwargs):
-        from .models import Category
-
         if "to" in kwargs:
             kwargs.pop("to")
-        super(CategoryFKField, self).__init__(to=Category, **kwargs)
+        super(CategoryFKField, self).__init__(to="categories.Category", **kwargs)
```

### Comparing `django-categories-1.9.4/categories/fixtures/genres.txt` & `django-categories-2.0.0a1/categories/fixtures/genres.txt`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/fixtures/musicgenres.json` & `django-categories-2.0.0a1/categories/fixtures/musicgenres.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999645691609979%*

 * *Differences: {'152': "{'fields': {'slug': 'country-pop_1'}}"}*

```diff
@@ -2131,15 +2131,15 @@
         "fields": {
             "level": 1,
             "lft": 100,
             "name": "Country pop",
             "order": 1,
             "parent": 142,
             "rght": 101,
-            "slug": "country-pop",
+            "slug": "country-pop_1",
             "tree_id": 10
         },
         "model": "categories.category",
         "pk": 153
     },
     {
         "fields": {
```

### Comparing `django-categories-1.9.4/categories/genericcollection.py` & `django-categories-2.0.0a1/categories/genericcollection.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/de/LC_MESSAGES/django.mo` & `django-categories-2.0.0a1/categories/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/de/LC_MESSAGES/django.po` & `django-categories-2.0.0a1/categories/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/fr/LC_MESSAGES/django.mo` & `django-categories-2.0.0a1/categories/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/fr/LC_MESSAGES/django.po` & `django-categories-2.0.0a1/categories/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/it/LC_MESSAGES/django.mo` & `django-categories-2.0.0a1/categories/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/locale/it/LC_MESSAGES/django.po` & `django-categories-2.0.0a1/categories/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/management/commands/add_category_fields.py` & `django-categories-2.0.0a1/categories/management/commands/add_category_fields.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/management/commands/drop_category_field.py` & `django-categories-2.0.0a1/categories/management/commands/drop_category_field.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/management/commands/import_categories.py` & `django-categories-2.0.0a1/categories/management/commands/import_categories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Import category trees from a file."""
 
 from django.core.management.base import BaseCommand, CommandError
 from django.db import transaction
+from slugify import slugify
 
 from categories.models import Category
 from categories.settings import SLUG_TRANSLITERATOR
 
-from ...utils import slugify
-
 
 class Command(BaseCommand):
     """Import category trees from a file."""
 
     help = (
         "Imports category tree(s) from a file. Sub categories must be indented by the same multiple of spaces or tabs."
     )
```

### Comparing `django-categories-1.9.4/categories/migration.py` & `django-categories-2.0.0a1/categories/migration.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/migrations/0001_initial.py` & `django-categories-2.0.0a1/categories/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/migrations/0002_auto_20170217_1111.py` & `django-categories-2.0.0a1/categories/migrations/0002_auto_20170217_1111.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/migrations/0003_auto_20200306_1050.py` & `django-categories-2.0.0a1/categories/migrations/0003_auto_20200306_1050.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/migrations/0004_auto_20200517_1832.py` & `django-categories-2.0.0a1/categories/migrations/0004_auto_20200517_1832.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/models.py` & `django-categories-2.0.0a1/categories/models.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/registration.py` & `django-categories-2.0.0a1/categories/registration.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/settings.py` & `django-categories-2.0.0a1/categories/settings.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/static/js/genericcollections.js` & `django-categories-2.0.0a1/categories/static/js/genericcollections.js`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/templates/admin/edit_inline/gen_coll_tabular.html` & `django-categories-2.0.0a1/categories/templates/admin/edit_inline/gen_coll_tabular.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/templates/categories/category_detail.html` & `django-categories-2.0.0a1/categories/templates/categories/category_detail.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/templatetags/category_tags.py` & `django-categories-2.0.0a1/categories/templatetags/category_tags.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_admin.py` & `django-categories-2.0.0a1/categories/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_category_import.py` & `django-categories-2.0.0a1/categories/tests/test_category_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,13 +54,13 @@
         self.assertEqual(items[2].name, "Category 1-2")
 
     def testMixingTabsSpaces(self):
         """
         Should raise an exception.
         """
         string1 = ["cat1", "    cat1-1", "\tcat1-2-FAIL!", ""]
-        string2 = ["cat1", "\tcat1-1", "    cat1-2-FAIL!", ""]
+        string2 = ["cat1a", "\tcat1-1a", "    cat1-2-FAIL!", ""]
         cmd = Command()
 
         # raise Exception
         self.assertRaises(CommandError, cmd.parse_lines, string1)
         self.assertRaises(CommandError, cmd.parse_lines, string2)
```

### Comparing `django-categories-1.9.4/categories/tests/test_image.jpg` & `django-categories-2.0.0a1/categories/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_manager.py` & `django-categories-2.0.0a1/categories/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_mgmt_commands.py` & `django-categories-2.0.0a1/categories/tests/test_mgmt_commands.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_models.py` & `django-categories-2.0.0a1/categories/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_registration.py` & `django-categories-2.0.0a1/categories/tests/test_registration.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_templatetags.py` & `django-categories-2.0.0a1/categories/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/tests/test_views.py` & `django-categories-2.0.0a1/categories/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/categories/views.py` & `django-categories-2.0.0a1/categories/views.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/django_categories.egg-info/PKG-INFO` & `django-categories-2.0.0a1/django_categories.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: django-categories
-Version: 1.9.4
+Version: 2.0.0a1
 Summary: A way to handle one or more hierarchical category trees in django.
 Home-page: http://github.com/jazzband/django-categories
 Author: Corey Oordt
 Author-email: coreyoordt@gmail.com
 Classifier: Framework :: Django
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICES.txt
 Requires-Dist: django-mptt
+Requires-Dist: unicode-slugify
 
 # Django Categories
 
 [![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)
 [![codecov](https://codecov.io/gh/jazzband/django-categories/branch/master/graph/badge.svg?token=rW8mpdZqWQ)](https://codecov.io/gh/jazzband/django-categories)
 
 Django Categories grew out of our need to provide a basic hierarchical taxonomy management system that multiple applications could use independently or in concert.
```

### Comparing `django-categories-1.9.4/django_categories.egg-info/SOURCES.txt` & `django-categories-2.0.0a1/django_categories.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 categories/fields.py
 categories/genericcollection.py
 categories/migration.py
 categories/models.py
 categories/registration.py
 categories/settings.py
 categories/urls.py
-categories/utils.py
 categories/views.py
 categories/api/__init__.py
 categories/editor/__init__.py
 categories/editor/models.py
 categories/editor/settings.py
 categories/editor/tree_editor.py
 categories/editor/utils.py
@@ -70,14 +69,15 @@
 categories/management/commands/add_category_fields.py
 categories/management/commands/drop_category_field.py
 categories/management/commands/import_categories.py
 categories/migrations/0001_initial.py
 categories/migrations/0002_auto_20170217_1111.py
 categories/migrations/0003_auto_20200306_1050.py
 categories/migrations/0004_auto_20200517_1832.py
+categories/migrations/0005_unique_category_slug.py
 categories/migrations/__init__.py
 categories/static/js/genericcollections.js
 categories/templates/admin/edit_inline/gen_coll_tabular.html
 categories/templates/categories/ancestors_ul.html
 categories/templates/categories/base.html
 categories/templates/categories/breadcrumbs.html
 categories/templates/categories/category_detail.html
@@ -87,18 +87,18 @@
 categories/templatetags/category_tags.py
 categories/tests/__init__.py
 categories/tests/test_admin.py
 categories/tests/test_category_import.py
 categories/tests/test_image.jpg
 categories/tests/test_manager.py
 categories/tests/test_mgmt_commands.py
+categories/tests/test_migrations.py
 categories/tests/test_models.py
 categories/tests/test_registration.py
 categories/tests/test_templatetags.py
-categories/tests/test_utils.py
 categories/tests/test_views.py
 django_categories.egg-info/PKG-INFO
 django_categories.egg-info/SOURCES.txt
 django_categories.egg-info/dependency_links.txt
 django_categories.egg-info/not-zip-safe
 django_categories.egg-info/requires.txt
 django_categories.egg-info/top_level.txt
```

### Comparing `django-categories-1.9.4/doc_src/Makefile` & `django-categories-2.0.0a1/doc_src/Makefile`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/_static/css/custom.css` & `django-categories-2.0.0a1/doc_src/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/_templates/autosummary/class.rst` & `django-categories-2.0.0a1/doc_src/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/_templates/autosummary/module.rst` & `django-categories-2.0.0a1/doc_src/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/conf.py` & `django-categories-2.0.0a1/doc_src/conf.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/getting_started.rst` & `django-categories-2.0.0a1/doc_src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/index.rst` & `django-categories-2.0.0a1/doc_src/index.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/installation.rst` & `django-categories-2.0.0a1/doc_src/installation.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/make.bat` & `django-categories-2.0.0a1/doc_src/make.bat`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/reference/management_commands.rst` & `django-categories-2.0.0a1/doc_src/reference/management_commands.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/reference/models.rst` & `django-categories-2.0.0a1/doc_src/reference/models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/reference/settings.rst` & `django-categories-2.0.0a1/doc_src/reference/settings.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/reference/templatetags.rst` & `django-categories-2.0.0a1/doc_src/reference/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/adding_the_fields.rst` & `django-categories-2.0.0a1/doc_src/user_guide/adding_the_fields.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/admin_settings.rst` & `django-categories-2.0.0a1/doc_src/user_guide/admin_settings.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories3.py` & `django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories3.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories4.py` & `django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories4.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/code_examples/custom_categories7.py` & `django-categories-2.0.0a1/doc_src/user_guide/code_examples/custom_categories7.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/custom_categories.rst` & `django-categories-2.0.0a1/doc_src/user_guide/custom_categories.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/registering_models.rst` & `django-categories-2.0.0a1/doc_src/user_guide/registering_models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/usage.rst` & `django-categories-2.0.0a1/doc_src/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/doc_src/user_guide/usage_example_template.html` & `django-categories-2.0.0a1/doc_src/user_guide/usage_example_template.html`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/pyproject.toml` & `django-categories-2.0.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/setup.cfg` & `django-categories-2.0.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/setup.py` & `django-categories-2.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `django-categories-1.9.4/tox.ini` & `django-categories-2.0.0a1/tox.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [tox]
 envlist =
     begin
     py37-lint
-    py{37}-django{21}
     py{37,38,39}-django{22,3,31}
     py{37,38,39,310}-django{32}
     py{38,39,310}-django{40}
     py{38,39,310,311}-django{41}
     py{310,311,312}-django{42,50}
     coverage-report
 
@@ -18,28 +17,31 @@
     3.10: py310
     3.11: py311
 
 [testenv]
 passenv = GITHUB_*
 
 deps=
-    django2: Django>=2.0,<2.1
-    django21: Django>=2.1,<2.2
     django22: Django>=2.2,<2.3
     django3: Django>=3.0,<3.1
     django31: Django>=3.1,<3.2
     django32: Django>=3.2,<4.0
     django40: Django>=4.0,<4.1
     django41: Django>=4.1,<4.2
     django42: Django>=4.2,<5.0
     django50: Django>=5.0,<5.1
     coverage[toml]
     pillow
     ipdb
     codecov
+    django-test-migrations
+    django21: django-test-migrations<=1.2.0
+    django22: django-test-migrations<=1.2.0
+    django3: django-test-migrations<=1.2.0
+    django31: django-test-migrations<=1.2.0
     -r{toxinidir}/requirements.txt
 
 commands=
   coverage erase
   coverage run \
     --source=categories \
     --omit='.tox/*,example/*,*/tests/*' \
```

