# Comparing `tmp/invenio-search-ui-2.8.5.tar.gz` & `tmp/invenio-search-ui-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-search-ui-2.8.5.tar", last modified: Mon Mar  4 14:25:51 2024, max compression
+gzip compressed data, was "dist/invenio-search-ui-2.8.6.tar", last modified: Fri Apr 19 13:38:01 2024, max compression
```

## Comparing `invenio-search-ui-2.8.5.tar` & `invenio-search-ui-2.8.6.tar`

### file list

```diff
@@ -1,470 +1,470 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/babel-js.ini
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/customizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/scss/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/context.js
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/defaultComponents.js
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)   124321 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/searchconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/count.html
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/facets.html
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/loading.html
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/pagination.html
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/range.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/results.html
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/selectbox.html
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/togglebutton.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/invenio_search_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/invenio_search_ui/search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/messages-js.pot
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/invenio_search_ui/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-04 14:25:50.000000 invenio-search-ui-2.8.5/invenio_search_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      522 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/tests/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 14:25:51.000000 invenio-search-ui-2.8.5/tests/templates/invenio_search_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/templates/invenio_search_ui/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/templates/invenio_search_ui/base_header.html
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/test_ng_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-04 14:25:46.000000 invenio-search-ui-2.8.5/tests/test_rsk_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/babel-js.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10178 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/customizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/scss/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/context.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/defaultComponents.js
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)   124321 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/searchconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/count.html
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/error.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/facets.html
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/loading.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/range.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/results.html
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/selectbox.html
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/togglebutton.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/invenio_search_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/invenio_search_ui/search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/messages-js.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/invenio_search_ui/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/invenio_search_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      522 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/tests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:38:01.000000 invenio-search-ui-2.8.6/tests/templates/invenio_search_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/templates/invenio_search_ui/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/templates/invenio_search_ui/base_header.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/test_ng_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 13:37:56.000000 invenio-search-ui-2.8.6/tests/test_rsk_templates.py
```

### Comparing `invenio-search-ui-2.8.5/.editorconfig` & `invenio-search-ui-2.8.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/.github/workflows/i18n-push.yml` & `invenio-search-ui-2.8.6/.github/workflows/i18n-push.yml`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/.github/workflows/pypi-publish.yml` & `invenio-search-ui-2.8.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/.github/workflows/tests.yml` & `invenio-search-ui-2.8.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/.tx/config` & `invenio-search-ui-2.8.6/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/CHANGES.rst` & `invenio-search-ui-2.8.6/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 2.8.6
+
+- a11y: allow users to tab across the search button
+
 Version 2.8.5 (released 2024-03-04)
 
 - relax major upper pin of invenio-assets, as v3 only upgrades webpack to
   v5 and do not introduce breaking changes to Python modules.
 
 Version 2.8.4 (released 2024-03-04)
```

### Comparing `invenio-search-ui-2.8.5/CONTRIBUTING.rst` & `invenio-search-ui-2.8.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/LICENSE` & `invenio-search-ui-2.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/MANIFEST.in` & `invenio-search-ui-2.8.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/PKG-INFO` & `invenio-search-ui-2.8.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-search-ui
-Version: 2.8.5
+Version: 2.8.6
 Summary: UI for Invenio-Search.
 Home-page: https://github.com/inveniosoftware/invenio-search-ui
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.8.6
+        
+        - a11y: allow users to tab across the search button
+        
         Version 2.8.5 (released 2024-03-04)
         
         - relax major upper pin of invenio-assets, as v3 only upgrades webpack to
           v5 and do not introduce breaking changes to Python modules.
         
         Version 2.8.4 (released 2024-03-04)
```

### Comparing `invenio-search-ui-2.8.5/README.rst` & `invenio-search-ui-2.8.6/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/docs/Makefile` & `invenio-search-ui-2.8.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/docs/conf.py` & `invenio-search-ui-2.8.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/docs/customizing.rst` & `invenio-search-ui-2.8.6/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/docs/index.rst` & `invenio-search-ui-2.8.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/docs/make.bat` & `invenio-search-ui-2.8.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/__init__.py` & `invenio-search-ui-2.8.6/invenio_search_ui/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,10 +323,10 @@
         <p>{{ record.metadata.description }}</p>
       </li>
     </ul>
 """
 
 from .ext import InvenioSearchUI
 
-__version__ = "2.8.5"
+__version__ = "2.8.6"
 
 __all__ = ("__version__", "InvenioSearchUI")
```

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/js/invenio_search_ui/app.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/bootstrap3/scss/invenio_search_ui/search.scss`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/InvenioSearchPagination.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/MultipleOptionsSearchBar.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -84,29 +84,27 @@
         value
     }) => {
         this.setState({
             queryString: value
         });
     };
 
-    handleFocus = (e) => {
-        e.persist();
-        if (e.target.nodeName === "BUTTON") this.handleOnSearchClick();
-    }
-
     render() {
         const {
             placeholder,
             options
         } = this.props;
         const {
             queryString
         } = this.state;
         const button = ( <
             Button icon className = "right-floated search"
+            onMouseDown = {
+                this.handleOnSearchClick
+            } // not onClick as button moves after focus
             onClick = {
                 this.handleOnSearchClick
             }
             aria - label = {
                 i18next.t("Search")
             } >
             <
@@ -123,17 +121,14 @@
             }
             onSearchChange = {
                 this.handleOnSearchChange
             }
             resultRenderer = {
                 (props) => resultRenderer(props, queryString)
             }
-            onFocus = {
-                this.handleFocus
-            }
             results = {
                 options
             }
             value = {
                 queryString
             }
             placeholder = {
@@ -203,27 +198,25 @@
     }) => {
         const {
             onInputChange
         } = this.props;
         onInputChange(value);
     };
 
-    handleFocus = (e) => {
-        e.persist();
-        if (e.target.nodeName === "BUTTON") this.onBtnSearchClick();
-    }
-
     render() {
         const {
             placeholder,
             queryString,
             options
         } = this.props;
         const button = ( <
             Button icon className = "right-floated search"
+            onMouseDown = {
+                this.handleOnSearchClick
+            } // not onClick as button moves after focus
             onClick = {
                 this.onBtnSearchClick
             }
             aria - label = {
                 i18next.t("Search")
             } >
             <
@@ -241,17 +234,14 @@
             }
             onSearchChange = {
                 this.handleOnSearchChange
             }
             resultRenderer = {
                 (props) => resultRenderer(props, queryString)
             }
-            onFocus = {
-                this.handleFocus
-            }
             results = {
                 options
             }
             value = {
                 queryString
             }
             placeholder = {
```

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/Results.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsGridItem.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/ResultsListItem.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchApp.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppFacets.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchAppResultsPane.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchBar.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchDropdowns.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/SearchFilters.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/common/facets.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/components/index.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/js/invenio_search_ui/util.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next-scanner.config.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/af/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ar/translations.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/bg/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ca/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/cs/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/da/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_AT/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/de_DE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/el/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_AT/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/en_HU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_CU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/es_MX/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/et_EE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fa_IR/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_CI/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/fr_FR/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/gl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hi_IN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/hu_HU/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/index.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/it/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ja/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ka/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/lt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ne/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/no/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pl/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/pt/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ro/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/ru/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/rw/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/sv_SE/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/tr/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/uk_UA/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_CN/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/messages/zh_TW/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package-lock.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/package.json`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/compileCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/scripts/initCatalog.js`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot` & `invenio-search-ui-2.8.6/invenio_search_ui/assets/semantic-ui/translations/invenio_search_ui/translations.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/config.py` & `invenio-search-ui-2.8.6/invenio_search_ui/config.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/ext.py` & `invenio-search-ui-2.8.6/invenio_search_ui/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/searchconfig.py` & `invenio-search-ui-2.8.6/invenio_search_ui/searchconfig.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/count.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/count.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/facets.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/facets.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/pagination.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/pagination.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/range.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/range.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/results.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/results.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html` & `invenio-search-ui-2.8.6/invenio_search_ui/static/templates/invenio_search_ui/searchbar.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/templates/invenio_search_ui/header.html` & `invenio-search-ui-2.8.6/invenio_search_ui/templates/invenio_search_ui/header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/templates/invenio_search_ui/search.html` & `invenio-search-ui-2.8.6/invenio_search_ui/templates/invenio_search_ui/search.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html` & `invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/invenio_search_ui/header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html` & `invenio-search-ui-2.8.6/invenio_search_ui/templates/semantic-ui/invenio_search_ui/search.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/af/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/da/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/el/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/et/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/et/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/it/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/messages-js.pot` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/messages-js.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/messages.pot` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ne/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/no/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages-js.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po` & `invenio-search-ui-2.8.6/invenio_search_ui/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/views.py` & `invenio-search-ui-2.8.6/invenio_search_ui/views.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui/webpack.py` & `invenio-search-ui-2.8.6/invenio_search_ui/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui.egg-info/PKG-INFO` & `invenio-search-ui-2.8.6/invenio_search_ui.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-search-ui
-Version: 2.8.5
+Version: 2.8.6
 Summary: UI for Invenio-Search.
 Home-page: https://github.com/inveniosoftware/invenio-search-ui
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -41,14 +41,18 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 2.8.6
+        
+        - a11y: allow users to tab across the search button
+        
         Version 2.8.5 (released 2024-03-04)
         
         - relax major upper pin of invenio-assets, as v3 only upgrades webpack to
           v5 and do not introduce breaking changes to Python modules.
         
         Version 2.8.4 (released 2024-03-04)
```

### Comparing `invenio-search-ui-2.8.5/invenio_search_ui.egg-info/SOURCES.txt` & `invenio-search-ui-2.8.6/invenio_search_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/requirements-devel.txt` & `invenio-search-ui-2.8.6/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/run-tests.sh` & `invenio-search-ui-2.8.6/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/setup.cfg` & `invenio-search-ui-2.8.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/conftest.py` & `invenio-search-ui-2.8.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/templates/invenio_search_ui/base.html` & `invenio-search-ui-2.8.6/tests/templates/invenio_search_ui/base.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/templates/invenio_search_ui/base_header.html` & `invenio-search-ui-2.8.6/tests/templates/invenio_search_ui/base_header.html`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/test_app.py` & `invenio-search-ui-2.8.6/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/test_ng_templates.py` & `invenio-search-ui-2.8.6/tests/test_ng_templates.py`

 * *Files identical despite different names*

### Comparing `invenio-search-ui-2.8.5/tests/test_rsk_templates.py` & `invenio-search-ui-2.8.6/tests/test_rsk_templates.py`

 * *Files identical despite different names*

