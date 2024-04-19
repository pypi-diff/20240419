# Comparing `tmp/ludic-0.3.1.tar.gz` & `tmp/ludic-0.4.0.tar.gz`

## Comparing `ludic-0.3.1.tar` & `ludic-0.4.0.tar`

### file list

```diff
@@ -1,79 +1,83 @@
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.3.1/.readthedocs.yaml
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.3.1/_version.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.3.1/mkdocs.yaml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.3.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/catalog.md
--rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/components.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/examples.md
--rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/getting-started.md
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/htmx.md
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/index.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/requirements.txt
--rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/styles.md
--rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/web-framework.md
--rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.3.1/docs/assets/ludic.png
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/README.md
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/__init__.py
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/bulk_update.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/click_to_edit.py
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/click_to_load.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/delete_row.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/edit_row.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/infinite_scroll.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/lazy_loading.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 ludic-0.3.1/examples/web.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/__init__.py
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/attrs.py
--rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/base.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/components.py
--rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/format.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/html.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/py.typed
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/types.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/utils.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/__init__.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/buttons.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/forms.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/items.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/lists.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/loaders.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/navigation.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/quotes.py
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/tables.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/typography.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/catalog/utils.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/collect.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/themes.py
--rw-r--r--   0        0        0    19669 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/types.py
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/styles/utils.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/__init__.py
--rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/app.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/datastructures.py
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/endpoints.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/exceptions.py
--rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/parsers.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/requests.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/responses.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.3.1/ludic/web/routing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3998 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_components.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_elements.py
--rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_examples.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_formatting.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_styles.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_themes.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/test_types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/test_datastructures.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.3.1/tests/web/test_requests.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.3.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.3.1/LICENCE
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.3.1/README.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ludic-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 ludic-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 ludic-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ludic-0.4.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 ludic-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ludic-0.4.0/_version.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 ludic-0.4.0/mkdocs.yaml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 ludic-0.4.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     9401 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/catalog.md
+-rw-r--r--   0        0        0    11704 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/components.md
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/examples.md
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/getting-started.md
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/htmx.md
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0     9658 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/styles.md
+-rw-r--r--   0        0        0    11976 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/web-framework.md
+-rw-r--r--   0        0        0   127587 2020-02-02 00:00:00.000000 ludic-0.4.0/docs/assets/ludic.png
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/README.md
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/__init__.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/bulk_update.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/click_to_edit.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/click_to_load.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/delete_row.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/edit_row.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/infinite_scroll.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/lazy_loading.py
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 ludic-0.4.0/examples/web.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/__init__.py
+-rw-r--r--   0        0        0    15514 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/attrs.py
+-rw-r--r--   0        0        0    10080 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/base.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/components.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/format.py
+-rw-r--r--   0        0        0    11727 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/html.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/py.typed
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/types.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/utils.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/__init__.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/buttons.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/forms.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/headers.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/items.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/layouts.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/lists.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/loaders.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/navigation.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/pages.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/quotes.py
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/tables.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/typography.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/catalog/utils.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/collect.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/themes.py
+-rw-r--r--   0        0        0    22591 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/types.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/styles/utils.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/__init__.py
+-rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/app.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/datastructures.py
+-rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/endpoints.py
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/exceptions.py
+-rw-r--r--   0        0        0     5295 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/parsers.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/requests.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/responses.py
+-rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 ludic-0.4.0/ludic/web/routing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_components.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_elements.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_examples.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_formatting.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/test_types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/__init__.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/test_styles.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/styles/test_themes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/test_datastructures.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 ludic-0.4.0/tests/web/test_requests.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 ludic-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ludic-0.4.0/LICENCE
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 ludic-0.4.0/README.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 ludic-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 ludic-0.4.0/PKG-INFO
```

### Comparing `ludic-0.3.1/.pre-commit-config.yaml` & `ludic-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/CONTRIBUTING.md` & `ludic-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/mkdocs.yaml` & `ludic-0.4.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/.github/workflows/publish.yaml` & `ludic-0.4.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/.github/workflows/test.yaml` & `ludic-0.4.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/catalog.md` & `ludic-0.4.0/docs/catalog.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/components.md` & `ludic-0.4.0/docs/components.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/getting-started.md` & `ludic-0.4.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/htmx.md` & `ludic-0.4.0/docs/htmx.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/index.md` & `ludic-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/styles.md` & `ludic-0.4.0/docs/styles.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/web-framework.md` & `ludic-0.4.0/docs/web-framework.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/docs/assets/ludic.png` & `ludic-0.4.0/docs/assets/ludic.png`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/examples/README.md` & `ludic-0.4.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/examples/__init__.py` & `ludic-0.4.0/ludic/catalog/pages.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,156 +1,123 @@
-from dataclasses import asdict, dataclass
-from typing import Any, override
+from typing import override
 
-from ludic.attrs import NoAttrs
-from ludic.html import (
-    body,
-    div,
-    h1,
-    head,
-    header,
-    html,
-    main,
-    meta,
-    script,
-    style,
-    title,
-)
-from ludic.types import (
-    AnyChildren,
-    BaseElement,
-    Component,
-    ComponentStrict,
-    PrimitiveChildren,
-)
-
-
-@dataclass
-class Model:
-    def dict(self) -> dict[str, Any]:
-        return asdict(self)
-
-
-@dataclass
-class ContactData(Model):
-    id: str
-    first_name: str
-    last_name: str
-    email: str
-
-
-@dataclass
-class PersonData(Model):
-    id: str
-    name: str
-    email: str
-    active: bool = True
-
-
-@dataclass
-class DB:
-    contacts: dict[str, ContactData]
-    people: dict[str, PersonData]
-
-
-def init_db() -> DB:
-    return DB(
-        contacts={
-            "1": ContactData(
-                id="1",
-                first_name="John",
-                last_name="Doe",
-                email="qN6Z8@example.com",
-            )
-        },
-        people={
-            "1": PersonData(
-                id="1",
-                name="Joe Smith",
-                email="joe@smith.org",
-                active=True,
-            ),
-            "2": PersonData(
-                id="2",
-                name="Angie MacDowell",
-                email="angie@macdowell.org",
-                active=True,
-            ),
-            "3": PersonData(
-                id="3",
-                name="Fuqua Tarkenton",
-                email="fuqua@tarkenton.org",
-                active=True,
-            ),
-            "4": PersonData(
-                id="4",
-                name="Kim Yee",
-                email="kim@yee.org",
-                active=False,
-            ),
-        },
-    )
+from ludic.attrs import Attrs, NoAttrs
+from ludic.html import body, head, html, script, style, title
+from ludic.types import AnyChildren, Component, ComponentStrict
 
 
-class Page(Component[AnyChildren, NoAttrs]):
-    styles = style.use(
-        lambda theme: {
-            "body": {
-                "color": theme.colors.dark,
-                "background-color": theme.colors.white,
-                "display": "flex",
-                "flex-direction": "column",
-                "align-items": "center",
-                "min-height": "100vh",
-                "margin": "0",
-                "font-family": "'Arial', sans-serif",
-            },
-            "main": {
-                "width": "80%",
-                "max-width": "800px",
-                "padding": "20px",
-            },
-        }
-    )
+class HtmlHeadAttrs(Attrs, total=False):
+    title: str
+
+
+class HtmlBodyAttrs(Attrs, total=False):
+    htmx_path: str
+    htmx_enabled: bool
+    htmx_version: str
 
+
+class Head(Component[AnyChildren, HtmlHeadAttrs]):
     @override
-    def render(self) -> BaseElement:
-        return html(
-            head(
-                title("Ludic Example"),
-                style.load(cache=True),
-                meta(charset="utf-8"),
-                meta(name="viewport", content="width=device-width, initial-scale=1.0"),
-            ),
-            body(
-                main(*self.children),
-                script(src="https://unpkg.com/htmx.org@1.9.10"),
-            ),
+    def render(self) -> head:
+        return head(
+            title(self.attrs.get("title", "Ludic App")),
+            style.load(cache=True),
+            *self.children,
         )
 
 
-class Header(ComponentStrict[PrimitiveChildren, NoAttrs]):
+class Body(Component[AnyChildren, HtmlBodyAttrs]):
+    @override
+    def render(self) -> body:
+        scripts = []
+        if htmx_path := self.attrs.get("htmx_path"):
+            scripts.append(script(src=htmx_path))
+        elif self.attrs.get("htmx_enabled", "htmx_version" in self.attrs):
+            htmx_version = self.attrs.get("htmx_version", "latest")
+            scripts.append(script(src=f"https://unpkg.com/htmx.org@{htmx_version}"))
+        return body(*self.children, *scripts)
+
+
+class HtmlPage(ComponentStrict[Head, Body, NoAttrs]):
     styles = style.use(
         lambda theme: {
-            "header": {
-                "text-align": "center",
+            # global styling
+            "*": {
+                "box-sizing": "border-box",
+                "max-inline-size": theme.measure,
+                "font-family": theme.fonts.plain,
+                "font-size": theme.fonts.size,
+                "color": theme.colors.dark,
+                "overflow-wrap": "break-word",
+                "margin": "0",
+                "padding": "0",
+                "line-height": theme.line_height,
+            },
+            ("html", "body", "div", "header", "nav", "main", "footer"): {
+                "max-inline-size": "none",
+            },
+            # elements styling
+            "h1": {
+                "font-size": theme.headers.h1.size,
             },
-            "header h1": {
-                "font-size": "3.5em",
-                "line-height": "1.2",
-                "margin-bottom": "35px",
-                "font-family": theme.fonts.families.headers,
+            "h2": {
+                "font-size": theme.headers.h2.size,
+            },
+            "h3": {
+                "font-size": theme.headers.h3.size,
+            },
+            "h4": {
+                "font-size": theme.headers.h4.size,
+            },
+            "h5": {
+                "font-size": theme.headers.h5.size,
+            },
+            "h6": {
+                "font-size": theme.headers.h6.size,
+            },
+            "a": {
+                "color": theme.colors.primary.darken(0.3),
+                "text-decoration": "none",
+            },
+            "a:hover": {
+                "text-decoration": "underline",
+            },
+            "dl": {
+                "margin-block": "0",
+            },
+            "dl dt": {
+                "margin-block-start": theme.sizes.xxs,
+            },
+            "dl dd": {
+                "margin-block-start": theme.sizes.xxxs,
+            },
+            "dt": {
+                "font-weight": "bold",
+            },
+            "dd": {
+                "margin-left": "0",
+            },
+            ("ul", "ol"): {
+                "padding-inline-start": theme.sizes.xl,
+            },
+            "li": {
+                "margin-block-start": theme.sizes.xxxs,
+            },
+            ("img", "svg"): {
+                "width": "100%",
+            },
+            "button": {
+                "line-height": theme.line_height - 0.2,
+            },
+            # utilities
+            ".text-align-center": {
+                "text-align": "center",
             },
         }
     )
 
     @override
-    def render(self) -> header:
-        return header(
-            h1(self.children[0]),
+    def render(self) -> html:
+        return html(
+            self.children[0].render(),
+            self.children[1].render(),
         )
-
-
-class Body(Component[AnyChildren, NoAttrs]):
-    @override
-    def render(self) -> div:
-        return div(*self.children)
```

### Comparing `ludic-0.3.1/examples/bulk_update.py` & `ludic-0.4.0/examples/bulk_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import Annotated, Self, override
 
-from examples import Body, Header, Page, init_db
+from examples import Page, init_db
 
 from ludic.catalog.buttons import ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form
+from ludic.catalog.headers import H1, H2
+from ludic.catalog.layouts import Cluster
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import ColumnMeta, Table, create_rows
 from ludic.html import span, style
 from ludic.types import Attrs
 from ludic.web import Endpoint, LudicApp
 from ludic.web.parsers import ListParser
 
@@ -32,16 +34,16 @@
 class Toast(span):
     id: str = "toast"
     target: str = f"#{id}"
     styles = style.use(
         lambda theme: {
             Toast.target: {
                 "background": theme.colors.success,
-                "margin": "10px 20px",
-                "padding": "5px 8px",
+                "padding": f"{theme.sizes.xxxxs} {theme.sizes.xxxs}",
+                "font-size": theme.fonts.size.scale(0.9),
                 "border-radius": "3px",
                 "opacity": "0",
                 "transition": "opacity 3s ease-out",
             },
             f"{Toast.target}.htmx-settling": {
                 "opacity": "100",
             },
@@ -52,23 +54,22 @@
     def render(self) -> span:
         return span(*self.children, id=self.id)
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
-        Header("Bulk Update"),
-        Body(
-            Quote(
-                "This demo shows how to implement a common pattern where rows are "
-                "selected and then bulk updated.",
-                source_url="https://htmx.org/examples/bulk-update/",
-            ),
-            await PeopleTable.get(),
+        H1("Bulk Update"),
+        Quote(
+            "This demo shows how to implement a common pattern where rows are "
+            "selected and then bulk updated.",
+            source_url="https://htmx.org/examples/bulk-update/",
         ),
+        H2("Demo"),
+        await PeopleTable.get(),
     )
 
 
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     @classmethod
     async def post(cls, data: ListParser[PersonAttrs]) -> Toast:
@@ -87,13 +88,15 @@
     async def get(cls) -> Self:
         return cls(people=[person.dict() for person in db.people.values()])
 
     @override
     def render(self) -> Form:
         return Form(
             Table(*create_rows(self.attrs["people"], spec=PersonAttrs)),
-            ButtonPrimary("Bulk Update", type="submit"),
-            Toast(),
+            Cluster(
+                ButtonPrimary("Bulk Update", type="submit"),
+                Toast(),
+            ),
             hx_post=self.url_for(PeopleTable),
             hx_target=Toast.target,
             hx_swap="outerHTML settle:3s",
         )
```

### Comparing `ludic-0.3.1/examples/click_to_edit.py` & `ludic-0.4.0/examples/click_to_edit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from typing import Annotated, NotRequired, Self, override
 
-from examples import Body, Header, Page, init_db
+from examples import Page, init_db
 
 from ludic.catalog.buttons import Button, ButtonDanger, ButtonPrimary
 from ludic.catalog.forms import FieldMeta, Form, create_fields
+from ludic.catalog.headers import H1, H2
 from ludic.catalog.items import Pairs
+from ludic.catalog.layouts import Box, Cluster, Stack
 from ludic.catalog.quotes import Quote
-from ludic.html import div
 from ludic.types import Attrs
 from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser, ValidationError
 
 db = init_db()
 app = LudicApp(debug=True)
@@ -30,23 +31,22 @@
         str, FieldMeta(label="Email", type="email", parser=email_validator)
     ]
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
-        Header("Click To Edit"),
-        Body(
-            Quote(
-                "The click to edit pattern provides a way to offer inline editing "
-                "of all or part of a record without a page refresh.",
-                source_url="https://htmx.org/examples/click-to-edit/",
-            ),
-            *[Contact(**contact.dict()) for contact in db.contacts.values()],
+        H1("Click To Edit"),
+        Quote(
+            "The click to edit pattern provides a way to offer inline editing "
+            "of all or part of a record without a page refresh.",
+            source_url="https://htmx.org/examples/click-to-edit/",
         ),
+        H2("Demo"),
+        Box(*[Contact(**contact.dict()) for contact in db.contacts.values()]),
     )
 
 
 @app.endpoint("/contacts/{id}")
 class Contact(Endpoint[ContactAttrs]):
     @classmethod
     async def get(cls, id: str) -> Self:
@@ -66,20 +66,22 @@
 
         for key, value in attrs.validate().items():
             setattr(contact, key, value)
 
         return cls(**contact.dict())
 
     @override
-    def render(self) -> div:
-        return div(
+    def render(self) -> Stack:
+        return Stack(
             Pairs(items=self.attrs.items()),
-            Button(
-                "Click To Edit",
-                hx_get=self.url_for(ContactForm),
+            Cluster(
+                Button(
+                    "Click To Edit",
+                    hx_get=self.url_for(ContactForm),
+                ),
             ),
             hx_target="this",
             hx_swap="outerHTML",
         )
 
 
 @app.endpoint("/contacts/{id}/form/")
@@ -93,13 +95,15 @@
 
         return cls(**contact.dict())
 
     @override
     def render(self) -> Form:
         return Form(
             *create_fields(self.attrs, spec=ContactAttrs),
-            ButtonPrimary("Submit"),
-            ButtonDanger("Cancel", hx_get=self.url_for(Contact)),
+            Cluster(
+                ButtonPrimary("Submit"),
+                ButtonDanger("Cancel", hx_get=self.url_for(Contact)),
+            ),
             hx_put=self.url_for(Contact),
             hx_target="this",
             hx_swap="outerHTML",
         )
```

### Comparing `ludic-0.3.1/examples/click_to_load.py` & `ludic-0.4.0/examples/click_to_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Self, override
 
-from examples import Body, Header, Page
+from examples import Page
 
-from ludic.attrs import ButtonAttrs
 from ludic.catalog.buttons import ButtonPrimary
+from ludic.catalog.headers import H1, H2
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.html import td
 from ludic.types import Attrs, Blank, Component, ComponentStrict
 from ludic.web import Endpoint, LudicApp
 from ludic.web.datastructures import QueryParams
 
@@ -21,15 +21,15 @@
 
 
 class ContactsSliceAttrs(Attrs):
     page: int
     contacts: list[ContactAttrs]
 
 
-class LoadMoreAttrs(ButtonAttrs):
+class LoadMoreAttrs(Attrs):
     url: str
 
 
 def load_contacts(page: int) -> list[ContactAttrs]:
     return [
         ContactAttrs(
             id=str(page * 10 + idx),
@@ -52,23 +52,22 @@
             hx_swap="outerHTML",
         )
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
-        Header("Click To Edit"),
-        Body(
-            Quote(
-                "This example shows how to implement click-to-load the next page in "
-                "a table of data.",
-                source_url="https://htmx.org/examples/click-to-load/",
-            ),
-            ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
+        H1("Click To Load"),
+        Quote(
+            "This example shows how to implement click-to-load the next page in "
+            "a table of data.",
+            source_url="https://htmx.org/examples/click-to-load/",
         ),
+        H2("Demo"),
+        ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
     )
 
 
 @app.endpoint("/contacts/")
 class ContactsSlice(Endpoint[ContactsSliceAttrs]):
     @classmethod
     async def get(cls, params: QueryParams) -> Self:
@@ -84,24 +83,24 @@
                 for contact in self.attrs["contacts"]
             ),
             TableRow(
                 td(
                     LoadMoreButton(
                         url=self.url_for(ContactsSlice).include_query_params(
                             page=next_page
-                        )
+                        ),
                     ),
                     colspan=3,
                 ),
                 id=LoadMoreButton.target,
             ),
         )
 
 
 class ContactsTable(Component[ContactsSlice, Attrs]):
     @override
     def render(self) -> Table[TableHead, ContactsSlice]:
         return Table(
             TableHead("ID", "Name", "Email"),
             *self.children,
-            style={"text-align": "center"},
+            classes=["text-align-center"],
         )
```

### Comparing `ludic-0.3.1/examples/delete_row.py` & `ludic-0.4.0/examples/delete_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Self, override
 
-from examples import Body, Header, Page, init_db
+from examples import Page, init_db
 
 from ludic.attrs import Attrs, HtmxAttrs
 from ludic.catalog.buttons import ButtonDanger
+from ludic.catalog.headers import H1, H2
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 
 db = init_db()
 app = LudicApp(debug=True)
@@ -23,23 +24,22 @@
 class PeopleAttrs(Attrs):
     people: list[PersonAttrs]
 
 
 @app.get("/")
 def index() -> Page:
     return Page(
-        Header("Delete Row"),
-        Body(
-            Quote(
-                "This example shows how to implement a delete button that removes "
-                "a table row upon completion.",
-                source_url="https://htmx.org/examples/delete-row/",
-            ),
-            PeopleTable.get(),
+        H1("Delete Row"),
+        Quote(
+            "This example shows how to implement a delete button that removes "
+            "a table row upon completion.",
+            source_url="https://htmx.org/examples/delete-row/",
         ),
+        H2("Demo"),
+        PeopleTable.get(),
     )
 
 
 @app.endpoint("/people/{id}")
 class PersonRow(Endpoint[PersonAttrs]):
     @classmethod
     def delete(cls, id: str) -> None:
@@ -50,15 +50,17 @@
 
     @override
     def render(self) -> TableRow:
         return TableRow(
             self.attrs["name"],
             self.attrs["email"],
             "Active" if self.attrs["active"] else "Inactive",
-            ButtonDanger("Delete", hx_delete=self.url_for(PersonRow)),
+            ButtonDanger(
+                "Delete", hx_delete=self.url_for(PersonRow), classes=["small"]
+            ),
         )
 
 
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     styles = {
         "tr.htmx-swapping td": {
@@ -77,9 +79,9 @@
             TableHead("Name", "Email", "Active", ""),
             *(PersonRow(**person) for person in self.attrs["people"]),
             body_attrs=HtmxAttrs(
                 hx_confirm="Are you sure?",
                 hx_target="closest tr",
                 hx_swap="outerHTML swap:1s",
             ),
-            style={"text-align": "center"},
+            classes=["text-align-center"],
         )
```

### Comparing `ludic-0.3.1/examples/edit_row.py` & `ludic-0.4.0/examples/edit_row.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Annotated, NotRequired, Self, override
 
-from examples import Body, Header, Page, init_db
+from examples import Page, init_db
 
 from ludic.attrs import Attrs, HtmxAttrs
 from ludic.catalog.buttons import (
     ButtonPrimary,
     ButtonSecondary,
     ButtonSuccess,
 )
 from ludic.catalog.forms import InputField
+from ludic.catalog.headers import H1, H2
+from ludic.catalog.layouts import Cluster
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import ColumnMeta, Table, TableHead, TableRow
-from ludic.html import div
 from ludic.types import JavaScript
 from ludic.web import Endpoint, LudicApp
 from ludic.web.exceptions import NotFoundError
 from ludic.web.parsers import Parser
 
 db = init_db()
 app = LudicApp(debug=True)
@@ -30,22 +31,21 @@
 class PeopleAttrs(Attrs):
     people: list[PersonAttrs]
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
-        Header("Edit Row"),
-        Body(
-            Quote(
-                "This example shows how to implement editable rows.",
-                source_url="https://htmx.org/examples/edit-row/",
-            ),
-            await PeopleTable.get(),
+        H1("Edit Row"),
+        Quote(
+            "This example shows how to implement editable rows.",
+            source_url="https://htmx.org/examples/edit-row/",
         ),
+        H2("Demo"),
+        await PeopleTable.get(),
     )
 
 
 @app.endpoint("/people/{id}")
 class PersonRow(Endpoint[PersonAttrs]):
     on_click_script: JavaScript = JavaScript(
         """
@@ -86,14 +86,15 @@
             self.attrs["name"],
             self.attrs["email"],
             ButtonPrimary(
                 "Edit",
                 hx_get=self.url_for(PersonForm),
                 hx_trigger="edit",
                 on_click=self.on_click_script,
+                classes=["small"],
             ),
         )
 
 
 @app.endpoint("/people/{id}/form/")
 class PersonForm(Endpoint[PersonAttrs]):
     @classmethod
@@ -106,23 +107,29 @@
         return cls(**person.dict())
 
     @override
     def render(self) -> TableRow:
         return TableRow(
             InputField(name="name", value=self.attrs["name"]),
             InputField(name="email", value=self.attrs["email"]),
-            div(
-                ButtonSecondary("Cancel", hx_get=self.url_for(PersonRow)),
+            Cluster(
+                ButtonSecondary(
+                    "Cancel",
+                    hx_get=self.url_for(PersonRow),
+                    classes=["small"],
+                ),
                 ButtonSuccess(
                     "Save",
                     hx_put=self.url_for(PersonRow),
                     hx_include="closest tr",
+                    classes=["small"],
                 ),
+                classes=["cluster-small"],
             ),
-            class_="editing",
+            classes=["editing"],
         )
 
 
 @app.endpoint("/people/")
 class PeopleTable(Endpoint[PeopleAttrs]):
     @classmethod
     async def get(cls) -> Self:
@@ -130,9 +137,9 @@
 
     @override
     def render(self) -> Table[TableHead, PersonRow]:
         return Table[TableHead, PersonRow](
             TableHead("Name", "Email", "Action"),
             *(PersonRow(**person) for person in self.attrs["people"]),
             body_attrs=HtmxAttrs(hx_target="closest tr", hx_swap="outerHTML"),
-            style={"text-align": "center"},
+            classes=["text-align-center"],
         )
```

### Comparing `ludic-0.3.1/examples/infinite_scroll.py` & `ludic-0.4.0/examples/infinite_scroll.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Self, override
 
-from examples import Body, Header, Page
+from examples import Page
 
+from ludic.catalog.headers import H1, H2
 from ludic.catalog.quotes import Quote
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.types import Attrs, Blank, Component
 from ludic.web import Endpoint, LudicApp
 from ludic.web.datastructures import QueryParams
 
 app = LudicApp(debug=True)
@@ -32,23 +33,22 @@
         for idx in range(10)
     ]
 
 
 @app.get("/")
 async def index() -> Page:
     return Page(
-        Header("Infinite Scroll"),
-        Body(
-            Quote(
-                "The infinite scroll pattern provides a way to load content dynamically"
-                "on user scrolling action.",
-                source_url="https://htmx.org/examples/infinite-scroll/",
-            ),
-            ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
+        H1("Infinite Scroll"),
+        Quote(
+            "The infinite scroll pattern provides a way to load content dynamically"
+            "on user scrolling action.",
+            source_url="https://htmx.org/examples/infinite-scroll/",
         ),
+        H2("Demo"),
+        ContactsTable(await ContactsSlice.get(QueryParams(page=1))),
     )
 
 
 @app.endpoint("/contacts/")
 class ContactsSlice(Endpoint[ContactsSliceAttrs]):
     @classmethod
     async def get(cls, params: QueryParams) -> Self:
@@ -76,9 +76,9 @@
 
 class ContactsTable(Component[ContactsSlice, Attrs]):
     @override
     def render(self) -> Table[TableHead, ContactsSlice]:
         return Table(
             TableHead("ID", "Name", "Email"),
             *self.children,
-            style={"text-align": "center"},
+            classes=["text-align-center"],
         )
```

### Comparing `ludic-0.3.1/examples/lazy_loading.py` & `ludic-0.4.0/examples/lazy_loading.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,42 @@
 import asyncio
 
-from examples import Body, Header, Page
+from examples import Page
 
+from ludic.catalog.headers import H1, H2
 from ludic.catalog.loaders import LazyLoader
 from ludic.catalog.quotes import Quote
-from ludic.html import div, svg
+from ludic.html import svg
 from ludic.types import Safe
 from ludic.web import LudicApp, Request
 
 app = LudicApp(debug=True)
 
 
 @app.get("/")
 async def index(request: Request) -> Page:
     return Page(
-        Header("Lazy Loading"),
-        Body(
-            Quote(
-                "This example shows how to lazily load an element on a page.",
-                source_url="https://htmx.org/examples/lazy-load/",
-            ),
-            div(
-                LazyLoader(load_url=request.url_for(load_svg, seconds=3)),
-                style={"text-align": "center"},
-            ),
+        H1("Lazy Loading"),
+        Quote(
+            "This example shows how to lazily load an element on a page.",
+            source_url="https://htmx.org/examples/lazy-load/",
         ),
+        H2("Demo"),
+        LazyLoader(load_url=request.url_for(load_svg, seconds=3)),
     )
 
 
 @app.get("/load/{seconds:int}")
 async def load_svg(seconds: int) -> svg:
     await asyncio.sleep(seconds)
     return svg(
         Safe(
             '<rect width="100%" height="100%" fill="#eee" />\n'
-            '<text x="350" y="225" font-size="60" text-anchor="middle" fill="#555">'
+            '<text x="310" y="215" text-anchor="middle" fill="#555">'
             "Content Loaded"
             "</text>"
         ),
         version="1.1",
         width="700",
         height="400",
+        style={"font-size": "2em"},
     )
```

### Comparing `ludic-0.3.1/examples/web.py` & `ludic-0.4.0/examples/web.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from collections.abc import AsyncIterator
 from contextlib import asynccontextmanager
 
 from examples import (
-    Body,
-    Header,
     Page,
     bulk_update,
     click_to_edit,
     click_to_load,
     delete_row,
     edit_row,
     infinite_scroll,
     lazy_loading,
 )
 
+from ludic.catalog.headers import H1
 from ludic.catalog.lists import List
 from ludic.catalog.typography import Link, Paragraph
 from ludic.html import style
 from ludic.web import LudicApp, Request
 from ludic.web.routing import Mount
 
 
@@ -41,40 +40,38 @@
     ],
 )
 
 
 @app.get("/")
 async def homepage(request: Request) -> Page:
     return Page(
-        Header("Ludic Examples"),
-        Body(
-            Paragraph(
-                "Here are examples demonstrating how to use the framework "
-                f"together with {Link("htmx.org", to="https://htmx.org")}:"
-            ),
-            List(
-                Link("Bulk Update", to=request.url_for("bulk_update:index")),
-                Link("Click to Edit", to=request.url_for("click_to_edit:index")),
-                Link("Click to Load", to=request.url_for("click_to_load:index")),
-                Link("Delete Row", to=request.url_for("delete_row:index")),
-                Link("Edit Row", to=request.url_for("edit_row:index")),
-                Link("Infinite Scroll", to=request.url_for("infinite_scroll:index")),
-                Link("Lazy Loading", to=request.url_for("lazy_loading:index")),
-            ),
+        H1("Ludic Examples"),
+        Paragraph(
+            "Here are examples demonstrating how to use the framework "
+            f"together with {Link("htmx.org", to="https://htmx.org")}:"
+        ),
+        List(
+            Link("Bulk Update", to=request.url_for("bulk_update:index")),
+            Link("Click to Edit", to=request.url_for("click_to_edit:index")),
+            Link("Click to Load", to=request.url_for("click_to_load:index")),
+            Link("Delete Row", to=request.url_for("delete_row:index")),
+            Link("Edit Row", to=request.url_for("edit_row:index")),
+            Link("Infinite Scroll", to=request.url_for("infinite_scroll:index")),
+            Link("Lazy Loading", to=request.url_for("lazy_loading:index")),
         ),
     )
 
 
 @app.exception_handler(404)
 async def not_found() -> Page:
     return Page(
-        Header("Page Not Found"),
-        Body(Paragraph("The page you are looking for was not found.")),
+        H1("Page Not Found"),
+        Paragraph("The page you are looking for was not found."),
     )
 
 
 @app.exception_handler(500)
 async def server_error() -> Page:
     return Page(
-        Header("Server Error"),
-        Body(Paragraph("Server encountered an error during processing.")),
+        H1("Server Error"),
+        Paragraph("Server encountered an error during processing."),
     )
```

### Comparing `ludic-0.3.1/ludic/attrs.py` & `ludic-0.4.0/ludic/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class HtmlAttrs(Attrs, total=False):
     """Common attributes for HTML elements."""
 
     id: str
     accesskey: str
     class_: Annotated[str, Alias("class")]
+    classes: Annotated[list[str], Alias("class")]  # merged with class_
     contenteditable: Literal["true", "false"]
     dir: Literal["ltr", "rtl", "auto"]
     draggable: Literal["true", "false"]
     enterkeyhint: Literal["enter", "done", "go", "next", "previous", "search", "send"]
     hidden: Literal["true", "false"]
     inert: bool
     inputmode: Literal[
```

### Comparing `ludic-0.3.1/ludic/base.py` & `ludic-0.4.0/ludic/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
             rendered_dom.context.update(dom.context)
             dom = rendered_dom
             classes += dom.classes
 
         element_tag = f"{dom.html_header}\n" if dom.html_header else ""
 
         hidden = dom.html_name == "__hidden__"
-        element_tag = "" if hidden else f"<{dom.html_name}"
+        element_tag += "" if hidden else f"<{dom.html_name}"
 
         if not hidden and (dom.has_attributes() or classes):
             attributes_str = dom._format_attributes(classes, is_html=True)
             element_tag += f" {attributes_str}"
 
         if dom.children or dom.always_pair:
             children_str = dom._format_children()
@@ -279,15 +279,15 @@
 
 TChildrenArgs = TypeVarTuple("TChildrenArgs", default=Unpack[tuple[AnyChildren, ...]])
 """Type variable for strict elements representing type of children (the type of *args).
 
 See also: :class:`ludic.types.ComponentStrict`.
 """
 
-TAttrs = TypeVar("TAttrs", bound=Attrs, default=Attrs, covariant=True)
+TAttrs = TypeVar("TAttrs", bound=Attrs | NoAttrs, default=Attrs, covariant=True)
 """Type variable for elements representing type of attributes (the type of **kwargs)."""
 
 
 class Element(Generic[TChildren, TAttrs], BaseElement):
     """Base class for Ludic elements.
 
     Args:
```

### Comparing `ludic-0.3.1/ludic/components.py` & `ludic-0.4.0/ludic/components.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/format.py` & `ludic-0.4.0/ludic/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         str: The formatted HTML attribute.
     """
     if isinstance(value, dict):
         value = ";".join(
             f"{dict_key}:{html.escape(dict_value, False)}"
             for dict_key, dict_value in value.items()
         )
+    elif isinstance(value, list):
+        value = " ".join(html.escape(v, False) for v in value)
     elif isinstance(value, bool):
         if is_html and not key.startswith("hx"):
             value = html.escape(key, False) if value else ""
         else:
             value = "true" if value else "false"
     elif isinstance(value, str) and getattr(value, "escape", True):
         value = html.escape(value, False)
@@ -68,18 +70,22 @@
     def _get_key(key: str) -> str:
         if get_origin(hints[key]) is Annotated:
             args = get_args(hints[key])
             if len(args) > 1 and isinstance(args[1], str):
                 return args[1]
         return key
 
-    result = {}
+    result: dict[str, str] = {}
     for key, value in attrs.items():
         if formatted_value := format_attr_value(key, value, is_html=is_html):
-            result[_get_key(key)] = formatted_value
+            alias = _get_key(key)
+            if alias in result:
+                result[alias] += " " + formatted_value
+            else:
+                result[alias] = formatted_value
     return result
 
 
 def format_element(child: Any) -> str:
     """Default HTML formatter.
 
     Args:
```

### Comparing `ludic-0.3.1/ludic/html.py` & `ludic-0.4.0/ludic/html.py`

 * *Files identical despite different names*

```diff
@@ -329,18 +329,18 @@
     ) -> Self:
         return cls(from_components(*components, theme=theme), type="text/css")
 
     @classmethod
     def load(cls, cache: bool = False, theme: Theme | None = None) -> Self:
         return cls(from_loaded(cache=cache, theme=theme), type="text/css")
 
-    def __getitem__(self, key: str) -> CSSProperties | GlobalStyles:
+    def __getitem__(self, key: str | tuple[str, ...]) -> CSSProperties | GlobalStyles:
         return self.styles[key]
 
-    def __iter__(self) -> Iterator[str]:
+    def __iter__(self) -> Iterator[str | tuple[str, ...]]:
         return iter(self.styles.keys())
 
     def __len__(self) -> int:
         return len(self.styles)
 
     @property
     def styles(self) -> GlobalStyles:
```

### Comparing `ludic-0.3.1/ludic/types.py` & `ludic-0.4.0/ludic/types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/utils.py` & `ludic-0.4.0/ludic/utils.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/catalog/buttons.py` & `ludic-0.4.0/ludic/catalog/buttons.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,146 +2,147 @@
 from ludic.html import button, style
 from ludic.types import ComponentStrict, PrimitiveChildren
 
 
 class Button(ComponentStrict[PrimitiveChildren, ButtonAttrs]):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn`` class.
+    The component creates a button.
     """
 
     classes = ["btn"]
     styles = style.use(
         lambda theme: {
             "button.btn": {
                 "background-color": theme.colors.light,
                 "color": theme.colors.black,
-                "margin": "8px 10px 8px 0px",
-                "padding": "10px 17px",
+                "padding": f"{theme.sizes.xxs} {theme.sizes.s}",
                 "border": f"1px solid {theme.colors.light.darken(0.1)}",
-                "border-radius": "4px",
+                "border-radius": theme.rounding.normal,
                 "cursor": "pointer",
-                "font-size": theme.fonts.sizes.medium,
+                "font-size": theme.fonts.size,
                 "transition": "0.1s filter linear, 0.1s -webkit-filter linear",
             },
             "button.btn:hover": {
                 "filter": "brightness(85%)",
             },
             "button.btn.small": {
-                "font-size": theme.fonts.sizes.small,
+                "font-size": theme.fonts.size.scale(0.9),
+                "padding": f"{theme.sizes.xxxs} {theme.sizes.xs}",
             },
             "button.btn.large": {
-                "font-size": theme.fonts.sizes.large,
+                "font-size": theme.fonts.size.scale(1.2),
+                "padding": f"{theme.sizes.xs} {theme.sizes.m}",
             },
         }
     )
 
     def render(self) -> button:
         return button(self.children[0], **self.attrs)
 
 
 class ButtonPrimary(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-primary`` class.
+    The component creates a button with the ``primary`` class.
     """
 
-    classes = ["btn", "btn-primary"]
+    classes = ["btn", "primary"]
     styles = style.use(
         lambda theme: {
-            "button.btn-primary": {
+            "button.btn.primary": {
                 "color": theme.colors.primary.readable(),
                 "background-color": theme.colors.primary,
                 "border-color": theme.colors.primary.darken(0.05),
             }
         }
     )
 
 
 class ButtonSecondary(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-secondary`` class.
+    The component creates a button with the ``secondary`` class.
     """
 
-    classes = ["btn", "btn-secondary"]
+    classes = ["btn", "secondary"]
     styles = style.use(
         lambda theme: {
-            "button.btn-secondary": {
+            "button.btn.secondary": {
                 "color": theme.colors.secondary.readable(),
                 "background-color": theme.colors.secondary,
                 "border-color": theme.colors.secondary.darken(0.05),
             }
         }
     )
 
 
 class ButtonSuccess(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-success`` class.
+    The component creates a button with the ``success`` class.
     """
 
-    classes = ["btn", "btn-success"]
+    classes = ["btn", "success"]
     styles = style.use(
         lambda theme: {
-            "button.btn-success": {
+            "button.btn.success": {
                 "color": theme.colors.success.readable(),
                 "background-color": theme.colors.success,
                 "border-color": theme.colors.success.darken(0.05),
             }
         }
     )
 
 
 class ButtonDanger(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-danger`` class.
+    The component creates a button with the ``danger`` class.
     """
 
-    classes = ["btn", "btn-danger"]
+    classes = ["btn", "danger"]
     styles = style.use(
         lambda theme: {
-            "button.btn-danger": {
+            "button.btn.danger": {
                 "color": theme.colors.danger.readable(),
                 "background-color": theme.colors.danger,
                 "border-color": theme.colors.danger.darken(0.05),
             }
         }
     )
 
 
 class ButtonWarning(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-warning`` class.
+    The component creates a button with the ``warning`` class.
     """
 
-    classes = ["btn", "btn-warning"]
+    classes = ["btn", "warning"]
     styles = style.use(
         lambda theme: {
-            "button.btn-warning": {
+            "button.btn.warning": {
                 "color": theme.colors.warning.readable(),
                 "background-color": theme.colors.warning,
                 "border-color": theme.colors.warning.darken(0.05),
             }
         }
     )
 
 
 class ButtonInfo(Button):
     """Simple component creating an HTML button.
 
-    The component creates a button with the ``btn btn-info`` class.
+    The component creates a button with the ``info`` class.
     """
 
-    classes = ["btn", "btn-info"]
+    classes = ["btn", "info"]
     styles = style.use(
         lambda theme: {
-            "button.btn-info": {
+            "button.btn.info": {
                 "color": theme.colors.info.readable(),
                 "background-color": theme.colors.info,
                 "border-color": theme.colors.info.darken(0.05),
             }
         }
     )
```

### Comparing `ludic-0.3.1/ludic/catalog/forms.py` & `ludic-0.4.0/ludic/catalog/forms.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,26 +101,24 @@
 
     classes = ["form-field"]
     styles = style.use(
         lambda theme: {
             ".form-field": {
                 "label": {
                     "display": "block",
-                    "margin-top": "12px",
-                    "margin-bottom": "8px",
                     "font-weight": "bold",
+                    "margin": f"{theme.sizes.xxxs} 0 {theme.sizes.xxs}",
                 },
                 "input": {
                     "width": "100%",
-                    "padding": "10px",
-                    "margin": "5px 0",
+                    "padding": f"{theme.sizes.xs} {theme.sizes.xxxs}",
                     "border": f"1px solid {theme.colors.light.darken(0.2)}",
                     "border-radius": "4px",
                     "box-sizing": "border-box",
-                    "font-size": "1em",
+                    "font-size": theme.fonts.size,
                 },
             }
         }
     )
 
     def create_label(self, text: PrimitiveChildren, for_: str = "") -> label:
         if for_:
@@ -162,15 +160,15 @@
 
         return div(*elements)
 
 
 class Form(Component[ComplexChildren, FormAttrs]):
     """A component helper for creating HTML forms."""
 
-    classes = ["form"]
+    classes = ["form", "stack"]
 
     @override
     def render(self) -> form:
         return form(*self.children, **self.attrs)
 
 
 def create_fields(attrs: Any, spec: type[TAttrs]) -> tuple[ComplexChildren, ...]:
```

### Comparing `ludic-0.3.1/ludic/catalog/items.py` & `ludic-0.4.0/ludic/catalog/items.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 from collections.abc import Iterable
 from typing import override
 
 from ludic.attrs import GlobalAttrs
-from ludic.html import dd, dl, dt
+from ludic.html import dd, dl, dt, style
 from ludic.types import Component, PrimitiveChildren
 
 from .utils import attr_to_camel
 
 
 class Key(Component[PrimitiveChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``dt`` element."""
 
-    classes = ["key"]
-    styles = {
-        "dt.key": {
-            "font-weight": "bold",
-            "margin-bottom": "10px",
-        },
-    }
-
     @override
     def render(self) -> dt:
         return dt(*self.children, **self.attrs)
 
 
 class Value(Component[PrimitiveChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``dd`` element."""
 
-    classes = ["value"]
-    styles = {
-        "dd.value": {
-            "margin-left": "0",
-            "margin-bottom": "20px",
-        },
-    }
-
     @override
     def render(self) -> dd:
         return dd(*self.children, **self.attrs)
 
 
 class PairsAttrs(GlobalAttrs, total=False):
     """Attributes of the component ``Pairs``."""
@@ -67,21 +51,22 @@
     Or alternatively:
 
         Pairs(
             items={"name": "John", "age": 42}.items(),
         )
     """
 
-    classes = ["pairs"]
-    styles = {
-        "dl.pairs": {
-            "margin-top": "20px",
-            "margin-bottom": "20px",
-        },
-    }
+    classes = ["stack", "stack-small"]
+    styles = style.use(
+        lambda theme: {
+            ".stack.stack-small > dt + dd": {
+                "margin-block-start": theme.sizes.xxxxs,
+            },
+        }
+    )
 
     @override
     def render(self) -> dl:
         from_items: list[Key | Value] = []
 
         for key, value in self.attrs.get("items", ()):
             from_items.append(Key(attr_to_camel(key)))
```

### Comparing `ludic-0.3.1/ludic/catalog/lists.py` & `ludic-0.4.0/ludic/catalog/lists.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/catalog/loaders.py` & `ludic-0.4.0/ludic/catalog/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             },
         }
     )
 
     @override
     def render(self) -> div:
         return div(
-            div(div(""), div(""), div(""), div(""), class_="lds-ellipsis"),
+            div(div(""), div(""), div(""), div(""), classes=["lds-ellipsis"]),
         )
 
 
 class LazyLoaderAttrs(GlobalAttrs):
     load_url: str
     placeholder: NotRequired[AnyChildren]
```

### Comparing `ludic-0.3.1/ludic/catalog/navigation.py` & `ludic-0.4.0/ludic/catalog/navigation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import override
 
 from ludic.attrs import GlobalAttrs
-from ludic.html import li, ul
+from ludic.html import li, nav, ul
 from ludic.types import Component, PrimitiveChildren
 
 from .typography import Link
 
 
 class NavItemAttrs(GlobalAttrs):
     to: str
@@ -31,12 +31,10 @@
 
         Navigation(
             NavItem("Home", to="/"),
             NavItem("About", to="/about"),
         )
     """
 
-    classes = ["navigation"]
-
     @override
-    def render(self) -> ul:
-        return ul(*self.children, **self.attrs_for(ul))
+    def render(self) -> nav:
+        return nav(ul(*self.children), **self.attrs_for(nav))
```

### Comparing `ludic-0.3.1/ludic/catalog/quotes.py` & `ludic-0.4.0/ludic/catalog/quotes.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,29 +13,27 @@
 class Quote(ComponentStrict[str, QuoteAttrs]):
     """Simple component rendering as the HTML ``blockquote`` element."""
 
     classes = ["quote"]
     styles = style.use(
         lambda theme: {
             ".quote": {
-                "margin-bottom": "20px",  # type: ignore
                 "blockquote": {
                     "background-color": theme.colors.light,
-                    "border-left": f"8px solid {theme.colors.light.darken(0.1)}",
-                    "margin": "0",
-                    "margin-bottom": "10px",
-                    "padding": "15px",
+                    "border-left": (
+                        f"{theme.borders.thick} solid {theme.colors.light.darken(0.05)}"
+                    ),
+                    "margin-bottom": theme.sizes.xxs,
+                    "padding": f"{theme.sizes.l} {theme.sizes.m}",
                 },
                 "blockquote p": {
-                    "font-size": theme.fonts.sizes.medium,
-                    "margin-bottom": "10px",
+                    "font-size": theme.fonts.size,
                 },
                 "footer": {
-                    "font-size": theme.fonts.sizes.small,
-                    "margin-top": "10px",
+                    "font-size": theme.fonts.size.scale(0.9),
                     "color": theme.colors.dark.lighten(0.5),
                 },
                 "footer a": {
                     "text-decoration": "none",
                     "color": theme.colors.dark.darken(0.5),
                 },
                 "footer a:hover": {
```

### Comparing `ludic-0.3.1/ludic/catalog/tables.py` & `ludic-0.4.0/ludic/catalog/tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,25 +58,14 @@
     def __call__(self, value: Any) -> PrimitiveChildren:
         return self.parse(value)
 
 
 class TableRow(Component[AnyChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``tr`` element."""
 
-    classes = ["table-row"]
-    styles = style.use(
-        lambda theme: {
-            "tr.table-row td": {
-                "border": f"1px solid {theme.colors.light.darken(0.2)}",
-                "padding": "12px",
-                "font-size": theme.fonts.sizes.medium,
-            }
-        }
-    )
-
     def get_value(self, index: int) -> PrimitiveChildren | None:
         if len(self.children) > index:
             child = self.children[index]
             return child.text if isinstance(child, BaseElement) else child
         return None
 
     @override
@@ -86,25 +75,14 @@
             **self.attrs,
         )
 
 
 class TableHead(Component[AnyChildren, GlobalAttrs]):
     """Simple component rendering as the HTML ``tr`` element."""
 
-    classes = ["table-head"]
-    styles = style.use(
-        lambda theme: {
-            "tr.table-head th": {
-                "border": f"1px solid {theme.colors.light.darken(0.2)}",
-                "padding": "12px",
-                "font-size": theme.fonts.sizes.medium,
-            }
-        }
-    )
-
     @property
     def header(self) -> tuple[PrimitiveChildren, ...]:
         return tuple(
             child.text if isinstance(child, BaseElement) else str(child)
             for child in self.children
             if self.children
         )
@@ -149,22 +127,30 @@
 
     classes = ["table"]
     styles = style.use(
         lambda theme: {
             "table.table": {
                 "width": "100%",  # type: ignore
                 "border-collapse": "collapse",  # type: ignore
-                "margin-bottom": "15px",  # type: ignore
                 "thead": {
                     "background-color": theme.colors.light,
                 },
-                "button.btn": {
-                    "margin": "0 5px",
+                "tr th": {
+                    "border": (
+                        f"{theme.borders.thin} solid {theme.colors.light.darken(0.1)}"
+                    ),
+                    "padding": f"{theme.sizes.xxs} {theme.sizes.xxxs}",
+                },
+                "tr td": {
+                    "border": (
+                        f"{theme.borders.thin} solid {theme.colors.light.darken(0.1)}"
+                    ),
+                    "padding": f"{theme.sizes.xxs} {theme.sizes.xxxs}",
                 },
-            }
+            },
         }
     )
 
     @property
     def header(self) -> tuple[PrimitiveChildren, ...]:
         if isinstance(self.children[0], TableHead):
             return self.children[0].header
```

### Comparing `ludic-0.3.1/ludic/styles/collect.py` & `ludic-0.4.0/ludic/styles/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 def format_styles(styles: GlobalStyles, separator: str = "\n") -> str:
     """Format styles from all registered elements.
 
     Args:
         styles (GlobalStyles): Styles to format.
     """
     result: list[str] = []
-    nodes_to_parse: list[tuple[list[str], str | Mapping[str, Any]]] = [([], styles)]
+    nodes_to_parse: list[
+        tuple[list[str], str | Mapping[str | tuple[str, ...], Any]]
+    ] = [([], styles)]
 
     while nodes_to_parse:
         parents, node = nodes_to_parse.pop(0)
 
         content = []
         if isinstance(node, str):
             content.append(node)
         else:
             for key, value in node.items():
-                if isinstance(value, str):
+                if isinstance(value, str | int | float):
                     content.append(f"{key}: {value};")
                 elif isinstance(value, Mapping):
-                    if key.startswith("@"):
-                        value = format_styles(value, separator=" ")
-                    nodes_to_parse.append(([*parents, key], value))
+                    keys = (key,) if isinstance(key, str | int | float) else key
+                    for key in keys:
+                        if key.startswith("@"):
+                            value = format_styles(value, separator=" ")
+                        nodes_to_parse.append(([*parents, key], value))
 
         if content:
             result.append(f"{" ".join(parents)} {{ {" ".join(content)} }}")
 
     return separator.join(result)
 
 
@@ -60,16 +64,16 @@
                         *self.children,
                     ),
                 )
 
     This would render an HTML page containing the ``<style>`` element
     with the styles the given components.
     """
-    all_styles: dict[str, CSSProperties | GlobalStyles] = {}
     theme = theme or get_default_theme()
+    all_styles: dict[str | tuple[str, ...], CSSProperties | GlobalStyles] = {}
 
     for component in components:
         styles = getattr(component, "styles", {})
 
         if not isinstance(styles, Mapping):
             continue
         elif hasattr(styles, "context"):
```

### Comparing `ludic-0.3.1/ludic/styles/utils.py` & `ludic-0.4.0/ludic/styles/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,7 +94,15 @@
         color (str): Color to lighten.
         factor (float, optional): Lightening factor. Defaults to 0.5.
 
     Returns:
         : Lightened color.
     """
     return scale_color(color, max(1, min(2, 1 + factor)))
+
+
+def first_not_none(*values: float | int | None) -> float | int:
+    return next((value for value in values if value is not None), 0)
+
+
+def clamp(min: str, val: str, max: str) -> str:
+    return f"clamp({min}, {val}, {max})"
```

### Comparing `ludic-0.3.1/ludic/web/app.py` & `ludic-0.4.0/ludic/web/app.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/datastructures.py` & `ludic-0.4.0/ludic/web/datastructures.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/endpoints.py` & `ludic-0.4.0/ludic/web/endpoints.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/exceptions.py` & `ludic-0.4.0/ludic/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/parsers.py` & `ludic-0.4.0/ludic/web/parsers.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/requests.py` & `ludic-0.4.0/ludic/web/requests.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/responses.py` & `ludic-0.4.0/ludic/web/responses.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/ludic/web/routing.py` & `ludic-0.4.0/ludic/web/routing.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/tests/test_components.py` & `ludic-0.4.0/tests/test_components.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ludic.catalog.tables import Table, TableHead, TableRow
 from ludic.catalog.typography import Link, Paragraph
 from ludic.html import b
 
 
 def test_link() -> None:
     link = Link("A link!", to="https://example.com")
-    assert link.to_html() == '<a href="https://example.com" class="link">A link!</a>'
+    assert link.to_html() == '<a href="https://example.com">A link!</a>'
 
 
 def test_paragraph() -> None:
     paragraph = Paragraph(
         "Hello, how ",
         b("are you"),
         "? Click ",
@@ -23,48 +23,50 @@
     assert paragraph.children[3].attrs["to"] == "https://example.com"
     assert paragraph.to_string(pretty=False) == (
         "<Paragraph>"
           'Hello, how <b>are you</b>? Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
-        '<p class="paragraph">'
+        '<p>'
             'Hello, how <b>are you</b>? '
-            'Click <a href="https://example.com" class="link">here</a>.'
+            'Click <a href="https://example.com">here</a>.'
         '</p>'
     )  # fmt: skip
 
 
 def test_navigation() -> None:
     navigation = Navigation(
         NavItem("Home", to="/"),
         NavItem("About", to="/about"),
         id="nav",
     )
     assert navigation.to_html() == (
-        '<ul id="nav" class="navigation">'
-            '<li id="home"><a href="/" class="link">Home</a></li>'
-            '<li id="about"><a href="/about" class="link">About</a></li>'
-        "</ul>"
+        '<nav id="nav">'
+            "<ul>"
+                '<li id="home"><a href="/">Home</a></li>'
+                '<li id="about"><a href="/about">About</a></li>'
+            "</ul>"
+        "</nav>"
     )  # fmt: skip
 
 
 def test_pairs() -> None:
     pairs = Pairs(
         Key("Name"),
         Value("John"),
         Key("Age"),
         Value(42),
     )
     assert pairs.to_html() == (
-        '<dl class="pairs">'
-            '<dt class="key">Name</dt>'
-            '<dd class="value">John</dd>'
-            '<dt class="key">Age</dt>'
-            '<dd class="value">42</dd>'
+        '<dl class="stack stack-small">'
+            '<dt>Name</dt>'
+            '<dd>John</dd>'
+            '<dt>Age</dt>'
+            '<dd>42</dd>'
         "</dl>"
     )  # fmt: skip
 
 
 def test_tables() -> None:
     table = Table(
         TableHead("Name", "Age"),
@@ -79,32 +81,32 @@
 
     assert len(table.children) > 2
     assert table.children[2].get_value(123) is None
 
     assert table.to_html() == (
         '<table class="table">'
             "<thead>"
-                '<tr class="table-head"><th>Name</th><th>Age</th></tr>'
+                '<tr><th>Name</th><th>Age</th></tr>'
             "</thead>"
             "<tbody>"
-                '<tr class="table-row"><td>John</td><td>42</td></tr>'
-                '<tr class="table-row"><td>Jane</td><td>43</td></tr>'
+                '<tr><td>John</td><td>42</td></tr>'
+                '<tr><td>Jane</td><td>43</td></tr>'
             "</tbody>"
         "</table>"
     )  # fmt: skip
 
 
 def test_form_fields() -> None:
     form = Form(
         InputField(value="Name", name="name"),
         TextAreaField("Description", name="description"),
     )
 
     assert form.to_html() == (
-        '<form class="form">'
+        '<form class="form stack">'
             '<div class="form-field">'
                 '<input value="Name" name="name" id="name" />'
             "</div>"
             '<div class="form-field">'
                 '<textarea name="description" id="description">Description</textarea>'
             "</div>"
         "</form>"
@@ -112,15 +114,15 @@
 
     form = Form(
         InputField(value="Name", name="name", label="Foo"),
         TextAreaField("Description", name="description", label="Bar"),
     )
 
     assert form.to_html() == (
-        '<form class="form">'
+        '<form class="form stack">'
             '<div class="form-field">'
                 '<label for="name">Foo</label>'
                 '<input value="Name" name="name" id="name" />'
             "</div>"
             '<div class="form-field">'
                 '<label for="description">Bar</label>'
                 '<textarea name="description" id="description">Description</textarea>'
```

#### html2text {}

```diff
@@ -8,21 +8,21 @@
 to="https://example.com"), ".", ) assert isinstance(paragraph.children[3],
 Link) assert paragraph.children[3].attrs["to"] == "https://example.com" assert
 paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
 here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
 ' 'Hello, how aarree yyoouu? ' 'Click _h_e_r_e.' '
 ' ) # fmt: skip def test_navigation() -> None: navigation = Navigation( NavItem
 ("Home", to="/"), NavItem("About", to="/about"), id="nav", ) assert
-navigation.to_html() == ( '
-    * ' '
+navigation.to_html() == ( '' "
+    * " '
     * _H_o_m_e
     * ' '
     * _A_b_o_u_t
     * ' "
-" ) # fmt: skip def test_pairs() -> None: pairs = Pairs( Key("Name"), Value
+" "" ) # fmt: skip def test_pairs() -> None: pairs = Pairs( Key("Name"), Value
 ("John"), Key("Age"), Value(42), ) assert pairs.to_html() == ( '
 ' '
 " ) # fmt: skip def test_tables() -> None: table = Table( TableHead("Name",
 "Age"), TableRow("John", 42), TableRow("Jane", 43), ) assert table.header ==
 ("Name", "Age") assert table.getlist("Name") == ["John", "Jane"] assert
 table.getlist("Age") == [42, 43] assert table.getlist("NOT_FOUND") == [] assert
 len(table.children) > 2 assert table.children[2].get_value(123) is None assert
```

### Comparing `ludic-0.3.1/tests/test_elements.py` & `ludic-0.4.0/tests/test_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 def test_button_get() -> None:
     dom = div(
         div(label("First Name"), ": Joe"),
         div(label("Last Name"), ": Blow"),
         div(label("Email"), ": joe@blow.com"),
         button(
             "Click To Edit",
-            class_="btn btn-primary",
+            classes=["btn", "btn-primary"],
             hx_get="/contact/1/edit",
         ),
         hx_target="this",
         hx_swap="outerHTML",
     )
 
     assert isinstance(dom.children[3], button)
```

### Comparing `ludic-0.3.1/tests/test_examples.py` & `ludic-0.4.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/tests/test_exceptions.py` & `ludic-0.4.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/tests/test_formatting.py` & `ludic-0.4.0/tests/test_formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,15 @@
     assert paragraph.children[3].attrs["to"] == "https://example.com"
     assert paragraph.to_string(pretty=False) == (
         "<Paragraph>"
           'Hello, how <strong>are you</strong>? Click <Link to="https://example.com">here</Link>.'
         "</Paragraph>"
     )  # fmt: skip
     assert paragraph.to_html() == (
-        '<p class="paragraph">Hello, how <strong>are you</strong>? '
-        'Click <a href="https://example.com" class="link">here</a>.</p>'
+        '<p>Hello, how <strong>are you</strong>? Click <a href="https://example.com">here</a>.</p>'
     )
 
 
 def test_escaping_works() -> None:
     link = '<a href="https://example.com">test</a>'
     dom = p(f"Hello, how <b>are you</b>? Click {link}.")
     assert dom.to_html() == (
```

#### html2text {}

```diff
@@ -23,15 +23,15 @@
 {i("nested2")}")}") == div( "test ", div("foo ", b("nested"), ", ", i
 ("nested2")), ) assert context.get() == {} def test_component_with_f_string() -
 > None: paragraph = Paragraph( f"Hello, how {strong("are you")}? Click {Link
 ("here", to="https://example.com")}.", ) assert isinstance(paragraph.children
 [3], Link) assert paragraph.children[3].attrs["to"] == "https://example.com"
 assert paragraph.to_string(pretty=False) == ( "" 'Hello, how aarree yyoouu? Click
 here.' "" ) # fmt: skip assert paragraph.to_html() == ( '
-Hello, how aarree yyoouu? ' 'Click _h_e_r_e.
+Hello, how aarree yyoouu? Click _h_e_r_e.
 ' ) def test_escaping_works() -> None: link = '_t_e_s_t' dom = p(f"Hello, how aarree
 yyoouu? Click {link}.") assert dom.to_html() == ( "
 Hello, how <b>are you</b>? " 'Click <a href="https://example.com">test</a>.
 ' ) def test_quotes_not_escaped() -> None: dom = p("It's alive <3.") assert
 dom.to_html() == "
 It's alive <3.
 "
```

### Comparing `ludic-0.3.1/tests/test_styles.py` & `ludic-0.4.0/tests/styles/test_styles.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from ludic.html import style
 from ludic.types import AnyChildren, Attrs, Component
 
+from . import FooTheme
+
 
 class A(Component[AnyChildren, Attrs]):
     styles = {
         "a": {
             "color": "red",
         },
         ".content": {
@@ -103,15 +105,15 @@
         "@keyframes lds-ellipsis1 { 0% { transform: scale(0); color: red; } }\n"
         "@layer state { .alert { background-color: brown; } p { padding: 10px; } }\n"
         "</style>"
     )
 
 
 def test_styles_collection() -> None:
-    assert style.from_components(A, B).to_html() == (
+    assert style.from_components(A, B, theme=FooTheme()).to_html() == (
         '<style type="text/css">\n'
         "a { color: red; }\n"
         ".content { background: #ffe; padding: 10px; }\n"
         ".content > p { color: blue; font-size: 20px; }\n"
         "a.test { color: blue; }\n"
         "</style>"
     )
```

### Comparing `ludic-0.3.1/tests/test_themes.py` & `ludic-0.4.0/tests/styles/test_themes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from typing import override
 
 from ludic.attrs import GlobalAttrs
 from ludic.html import a, b, div, style
 from ludic.styles.themes import (
-    Color,
     Colors,
-    DarkTheme,
     Fonts,
-    FontSizes,
-    LightTheme,
-    Size,
     get_default_theme,
     set_default_theme,
 )
+from ludic.styles.types import Color, Size
 from ludic.types import Component
 
+from . import BarTheme, FooTheme
+
 
 def test_theme_colors() -> None:
-    theme = LightTheme(
+    theme = FooTheme(
         colors=Colors(
             primary=Color("#c2e7fd"),
             white=Color("#fff"),
             light=Color("#eee"),
             dark=Color("#333"),
             black=Color("#000"),
         )
@@ -41,37 +39,34 @@
     assert theme.colors.light.darken(0.5).rgb == (119, 119, 119)
     assert theme.colors.dark.lighten(0.5).rgb == (153, 153, 153)
 
     assert theme.colors.primary.darken(0.5).rgb == (97, 115, 126)
 
 
 def test_theme_font_sizes() -> None:
-    theme = LightTheme(
-        fonts=Fonts(sizes=FontSizes(small=Size(10, "px"), medium=Size(1.2, unit="em"))),
-    )
+    theme = FooTheme(fonts=Fonts(size=Size(10, "px")))
 
-    assert theme.fonts.sizes.small == "10px"
-    assert theme.fonts.sizes.medium == "1.2em"
+    assert theme.fonts.size == "10px"
+    assert theme.fonts.plain == "sans-serif"
 
 
 def test_themes_switching() -> None:
-    dark, light = DarkTheme(), LightTheme()
+    foo, bar = FooTheme(), BarTheme()
 
-    assert get_default_theme() == light
-    set_default_theme(dark)
-    assert get_default_theme() == dark
-    set_default_theme(light)
-    assert get_default_theme() == light
+    set_default_theme(foo)
+    assert get_default_theme() == foo
+    set_default_theme(bar)
+    assert get_default_theme() == bar
 
 
 def test_element_theme_switching() -> None:
-    dark = DarkTheme()
-    light = LightTheme()
+    foo = FooTheme()
+    bar = BarTheme()
 
-    set_default_theme(light)
+    set_default_theme(bar)
 
     class C1(Component[str, GlobalAttrs]):
         styles = style.use(
             lambda theme: {
                 "#c1 a": {"color": theme.colors.warning},
             }
         )
@@ -90,35 +85,35 @@
                 "#c2 a": {"color": theme.colors.danger},
             }
         )
 
         @override
         def render(self) -> div:
             return div(
-                dark.use(C1(*self.children)),
+                foo.use(C1(*self.children)),
                 id="c2",
                 style={"background-color": self.theme.colors.primary},
             )
 
     assert C2("World").to_html() == (
-        f'<div id="c2" style="background-color:{light.colors.primary}">'
+        f'<div id="c2" style="background-color:{bar.colors.primary}">'
           '<div id="c1">'
-            f'<b style="color:{dark.colors.secondary}">Hello, </b>'
+            f'<b style="color:{foo.colors.secondary}">Hello, </b>'
             '<a href="https://example.com">World</a>'
           "</div>"
         "</div>"
     )  # fmt: skip
     assert style.from_components(C1, C2).to_html() == (
         '<style type="text/css">\n'
-          f"#c1 a {{ color: {light.colors.warning}; }}\n"
-          f"#c2 a {{ color: {light.colors.danger}; }}\n"
+          f"#c1 a {{ color: {bar.colors.warning}; }}\n"
+          f"#c2 a {{ color: {bar.colors.danger}; }}\n"
         "</style>"
     )  # fmt: skip
 
-    set_default_theme(dark)
+    set_default_theme(foo)
 
     assert style.from_components(C1, C2).to_html() == (
         '<style type="text/css">\n'
-          f"#c1 a {{ color: {dark.colors.warning}; }}\n"
-          f"#c2 a {{ color: {dark.colors.danger}; }}\n"
+          f"#c1 a {{ color: {foo.colors.warning}; }}\n"
+          f"#c2 a {{ color: {foo.colors.danger}; }}\n"
         "</style>"
     )  # fmt: skip
```

#### html2text {}

```diff
@@ -1,39 +1,37 @@
 from typing import override from ludic.attrs import GlobalAttrs from ludic.html
-import a, b, div, style from ludic.styles.themes import ( Color, Colors,
-DarkTheme, Fonts, FontSizes, LightTheme, Size, get_default_theme,
-set_default_theme, ) from ludic.types import Component def test_theme_colors()
--> None: theme = LightTheme( colors=Colors( primary=Color("#c2e7fd"),
-white=Color("#fff"), light=Color("#eee"), dark=Color("#333"), black=Color
-("#000"), ) ) assert theme.colors.primary.rgb == (194, 231, 253) assert
-theme.colors.white.rgb == (255, 255, 255) assert theme.colors.light.rgb ==
-(238, 238, 238) assert theme.colors.dark.rgb == (51, 51, 51) assert
+import a, b, div, style from ludic.styles.themes import ( Colors, Fonts,
+get_default_theme, set_default_theme, ) from ludic.styles.types import Color,
+Size from ludic.types import Component from . import BarTheme, FooTheme def
+test_theme_colors() -> None: theme = FooTheme( colors=Colors( primary=Color
+("#c2e7fd"), white=Color("#fff"), light=Color("#eee"), dark=Color("#333"),
+black=Color("#000"), ) ) assert theme.colors.primary.rgb == (194, 231, 253)
+assert theme.colors.white.rgb == (255, 255, 255) assert theme.colors.light.rgb
+== (238, 238, 238) assert theme.colors.dark.rgb == (51, 51, 51) assert
 theme.colors.black.rgb == (0, 0, 0) assert theme.colors.white.darken(0.5).rgb
 == (127, 127, 127) assert theme.colors.white.darken(1).rgb == (1, 1, 1) assert
 theme.colors.black.lighten(0.5).rgb == (127, 127, 127) assert
 theme.colors.black.lighten(1).rgb == (255, 255, 255) assert
 theme.colors.light.darken(0.5).rgb == (119, 119, 119) assert
 theme.colors.dark.lighten(0.5).rgb == (153, 153, 153) assert
 theme.colors.primary.darken(0.5).rgb == (97, 115, 126) def
-test_theme_font_sizes() -> None: theme = LightTheme( fonts=Fonts
-(sizes=FontSizes(small=Size(10, "px"), medium=Size(1.2, unit="em"))), ) assert
-theme.fonts.sizes.small == "10px" assert theme.fonts.sizes.medium == "1.2em"
-def test_themes_switching() -> None: dark, light = DarkTheme(), LightTheme()
-assert get_default_theme() == light set_default_theme(dark) assert
-get_default_theme() == dark set_default_theme(light) assert get_default_theme()
-== light def test_element_theme_switching() -> None: dark = DarkTheme() light =
-LightTheme() set_default_theme(light) class C1(Component[str, GlobalAttrs]):
-styles = style.use( lambda theme: { "#c1 a": {"color": theme.colors.warning}, }
-) @override def render(self) -> div: return div( b("Hello, ", style={"color":
-self.theme.colors.secondary}), a(*self.children, href="https://example.com"),
-id="c1", ) class C2(Component[str, GlobalAttrs]): styles = style.use( lambda
-theme: { "#c2 a": {"color": theme.colors.danger}, } ) @override def render
-(self) -> div: return div( dark.use(C1(*self.children)), id="c2", style=
-{"background-color": self.theme.colors.primary}, ) assert C2("World").to_html()
-== ( f'
+test_theme_font_sizes() -> None: theme = FooTheme(fonts=Fonts(size=Size(10,
+"px"))) assert theme.fonts.size == "10px" assert theme.fonts.plain == "sans-
+serif" def test_themes_switching() -> None: foo, bar = FooTheme(), BarTheme()
+set_default_theme(foo) assert get_default_theme() == foo set_default_theme(bar)
+assert get_default_theme() == bar def test_element_theme_switching() -> None:
+foo = FooTheme() bar = BarTheme() set_default_theme(bar) class C1(Component
+[str, GlobalAttrs]): styles = style.use( lambda theme: { "#c1 a": {"color":
+theme.colors.warning}, } ) @override def render(self) -> div: return div( b
+("Hello, ", style={"color": self.theme.colors.secondary}), a(*self.children,
+href="https://example.com"), id="c1", ) class C2(Component[str, GlobalAttrs]):
+styles = style.use( lambda theme: { "#c2 a": {"color": theme.colors.danger}, }
+) @override def render(self) -> div: return div( foo.use(C1(*self.children)),
+id="c2", style={"background-color": self.theme.colors.primary}, ) assert C2
+("World").to_html() == ( f'
 ' '
 ' f'HHeelllloo,, ' '_W_o_r_l_d' "
 " "
 " ) # fmt: skip assert style.from_components(C1, C2).to_html() == ( '
-" ) # fmt: skip set_default_theme(dark) assert style.from_components(C1,
+" ) # fmt: skip set_default_theme(foo) assert style.from_components(C1,
 C2).to_html() == ( '
 " ) # fmt: skip
```

### Comparing `ludic-0.3.1/tests/test_types.py` & `ludic-0.4.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/.gitignore` & `ludic-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/LICENCE` & `ludic-0.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/README.md` & `ludic-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/pyproject.toml` & `ludic-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ludic-0.3.1/PKG-INFO` & `ludic-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ludic
-Version: 0.3.1
+Version: 0.4.0
 Summary: Lightweight framework for building dynamic HTML pages in pure Python.
 Author-email: Pavel Dedík <dedikx@gmail.com>
 Maintainer-email: Pavel Dedík <dedikx@gmail.com>
 License-Expression: MIT
 License-File: LICENCE
 Keywords: async,html,htmx,templating,web
 Classifier: Development Status :: 4 - Beta
```

