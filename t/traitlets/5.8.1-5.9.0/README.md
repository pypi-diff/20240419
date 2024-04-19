# Comparing `tmp/traitlets-5.8.1.tar.gz` & `tmp/traitlets-5.9.0.tar.gz`

## Comparing `traitlets-5.8.1.tar` & `traitlets-5.9.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 traitlets-5.8.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 traitlets-5.8.1/.mailmap
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 traitlets-5.8.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    28330 2020-02-02 00:00:00.000000 traitlets-5.8.1/CHANGELOG.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 traitlets-5.8.1/CHANGES.txt
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 traitlets-5.8.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 traitlets-5.8.1/RELEASE.md
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 traitlets-5.8.1/SECURITY.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 traitlets-5.8.1/codecov.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 traitlets-5.8.1/readthedocs.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/workflows/downstream.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 traitlets-5.8.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/Makefile
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/make.bat
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/readme-docs.md
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/api.rst
--rw-r--r--   0        0        0    10683 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/conf.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/config-api.rst
--rw-r--r--   0        0        0    36541 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/config.rst
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/defining_traits.rst
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/index.rst
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/migration.rst
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/trait_types.rst
--rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/using_traitlets.rst
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/source/utils.rst
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 traitlets-5.8.1/docs/sphinxext/github.py
--rwxr-xr-x   0        0        0     5346 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/argcomplete_app.py
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/myapp.py
--rwxr-xr-x   0        0        0     2239 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/subcommands_app.py
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/aliases.py
--rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/container.py
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/flags.py
--rwxr-xr-x   0        0        0      606 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/from_string.py
--rwxr-xr-x   0        0        0     1391 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/load_config_app.py
--rwxr-xr-x   0        0        0      577 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/multiple_apps.py
--rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/subcommands.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/configs/base_config.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 traitlets-5.8.1/examples/docs/configs/main_config.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/_version.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/py.typed
--rw-r--r--   0        0        0   126924 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/traitlets.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/__init__.py
--rw-r--r--   0        0        0    40429 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/application.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/argcomplete_config.py
--rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/configurable.py
--rw-r--r--   0        0        0    37692 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/loader.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/manager.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/sphinxdoc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/tests/__init__.py
--rw-r--r--   0        0        0    30674 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/tests/test_application.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/tests/test_argcomplete.py
--rw-r--r--   0        0        0    22464 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/tests/test_configurable.py
--rw-r--r--   0        0        0    22748 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/config/tests/test_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/tests/__init__.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/tests/_warnings.py
--rw-r--r--   0        0        0    80029 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/tests/test_traitlets.py
--rw-r--r--   0        0        0    13536 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/tests/test_traitlets_enum.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/tests/utils.py
--rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/bunch.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/decorators.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/descriptions.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/getargspec.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/importstring.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/nested_update.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/sentinel.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/text.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/tests/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/tests/test_bunch.py
--rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/tests/test_decorators.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 traitlets-5.8.1/traitlets/utils/tests/test_importstring.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 traitlets-5.8.1/.gitignore
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 traitlets-5.8.1/COPYING.md
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 traitlets-5.8.1/README.md
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 traitlets-5.8.1/pyproject.toml
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 traitlets-5.8.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 traitlets-5.9.0/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 traitlets-5.9.0/.mailmap
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 traitlets-5.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    29375 2020-02-02 00:00:00.000000 traitlets-5.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 traitlets-5.9.0/CHANGES.txt
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 traitlets-5.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 traitlets-5.9.0/RELEASE.md
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 traitlets-5.9.0/SECURITY.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 traitlets-5.9.0/codecov.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 traitlets-5.9.0/readthedocs.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2382 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/workflows/downstream.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 traitlets-5.9.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7449 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/Makefile
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/make.bat
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/readme-docs.md
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/api.rst
+-rw-r--r--   0        0        0    10683 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/conf.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/config-api.rst
+-rw-r--r--   0        0        0    36541 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/config.rst
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/defining_traits.rst
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/index.rst
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/migration.rst
+-rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/trait_types.rst
+-rw-r--r--   0        0        0     6033 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/using_traitlets.rst
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/source/utils.rst
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 traitlets-5.9.0/docs/sphinxext/github.py
+-rwxr-xr-x   0        0        0     5346 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/argcomplete_app.py
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/myapp.py
+-rwxr-xr-x   0        0        0     2239 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/subcommands_app.py
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/aliases.py
+-rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/container.py
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/flags.py
+-rwxr-xr-x   0        0        0      606 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/from_string.py
+-rwxr-xr-x   0        0        0     1391 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/load_config_app.py
+-rwxr-xr-x   0        0        0      577 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/multiple_apps.py
+-rwxr-xr-x   0        0        0      693 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/subcommands.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/configs/base_config.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 traitlets-5.9.0/examples/docs/configs/main_config.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/_version.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/py.typed
+-rw-r--r--   0        0        0   126924 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/traitlets.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/__init__.py
+-rw-r--r--   0        0        0    40479 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/application.py
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/argcomplete_config.py
+-rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/configurable.py
+-rw-r--r--   0        0        0    38313 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/loader.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/manager.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/sphinxdoc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/tests/__init__.py
+-rw-r--r--   0        0        0    30882 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/tests/test_application.py
+-rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/tests/test_argcomplete.py
+-rw-r--r--   0        0        0    22464 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/tests/test_configurable.py
+-rw-r--r--   0        0        0    22748 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/config/tests/test_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/tests/__init__.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/tests/_warnings.py
+-rw-r--r--   0        0        0    80029 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/tests/test_traitlets.py
+-rw-r--r--   0        0        0    13536 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/tests/test_traitlets_enum.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/tests/utils.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/__init__.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/bunch.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/decorators.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/descriptions.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/getargspec.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/importstring.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/nested_update.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/sentinel.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/text.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/tests/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/tests/test_bunch.py
+-rw-r--r--   0        0        0     4748 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/tests/test_decorators.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 traitlets-5.9.0/traitlets/utils/tests/test_importstring.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 traitlets-5.9.0/.gitignore
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 traitlets-5.9.0/COPYING.md
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 traitlets-5.9.0/README.md
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 traitlets-5.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 traitlets-5.9.0/PKG-INFO
```

### Comparing `traitlets-5.8.1/.mailmap` & `traitlets-5.9.0/.mailmap`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/.pre-commit-config.yaml` & `traitlets-5.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/CHANGELOG.md` & `traitlets-5.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 # Changes in Traitlets
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 5.9.0
+
+([Full Changelog](https://github.com/ipython/traitlets/compare/v5.8.1...c11a4d942b08df5c19be88b6cc81dfa8302fef9b))
+
+### Enhancements made
+
+- Polishing argcomplete support [#829](https://github.com/ipython/traitlets/pull/829) ([@azjps](https://github.com/azjps))
+
+### Maintenance and upkeep improvements
+
+- Test that name and description can be set via constructor. [#826](https://github.com/ipython/traitlets/pull/826) ([@Carreau](https://github.com/Carreau))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/ipython/traitlets/graphs/contributors?from=2023-01-09&to=2023-01-30&type=c))
+
+[@azjps](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Aazjps+updated%3A2023-01-09..2023-01-30&type=Issues) | [@blink1073](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Ablink1073+updated%3A2023-01-09..2023-01-30&type=Issues) | [@Carreau](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3ACarreau+updated%3A2023-01-09..2023-01-30&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 5.8.1
 
 ([Full Changelog](https://github.com/ipython/traitlets/compare/v5.8.0...18814204c7e7987851cc1836a36863b4fab60165))
 
 ### Bugs fixed
 
 - fix: mro_trait can be unbound when the class is not in mro [#824](https://github.com/ipython/traitlets/pull/824) ([@maartenbreddels](https://github.com/maartenbreddels))
@@ -18,16 +38,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/ipython/traitlets/graphs/contributors?from=2022-12-19&to=2023-01-09&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Ablink1073+updated%3A2022-12-19..2023-01-09&type=Issues) | [@maartenbreddels](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Amaartenbreddels+updated%3A2022-12-19..2023-01-09&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Apre-commit-ci+updated%3A2022-12-19..2023-01-09&type=Issues) | [@rmorshea](https://github.com/search?q=repo%3Aipython%2Ftraitlets+involves%3Armorshea+updated%3A2022-12-19..2023-01-09&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 5.8.0
 
 ([Full Changelog](https://github.com/ipython/traitlets/compare/v5.7.1...47e652f96aff54d1aa3b19337c9c8d80fe0fd4c4))
 
 ### Enhancements made
 
 -Shell command-line tab-completion via `argcomplete` [#811](https://github.com/ipython/traitlets/pull/811) ([@azjps](https://github.com/azjps))
```

### Comparing `traitlets-5.8.1/RELEASE.md` & `traitlets-5.9.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/.github/workflows/downstream.yml` & `traitlets-5.9.0/.github/workflows/downstream.yml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/.github/workflows/prep-release.yml` & `traitlets-5.9.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/.github/workflows/publish-release.yml` & `traitlets-5.9.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/.github/workflows/tests.yml` & `traitlets-5.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/Makefile` & `traitlets-5.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/make.bat` & `traitlets-5.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/readme-docs.md` & `traitlets-5.9.0/docs/readme-docs.md`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/api.rst` & `traitlets-5.9.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/conf.py` & `traitlets-5.9.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/config-api.rst` & `traitlets-5.9.0/docs/source/config-api.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/config.rst` & `traitlets-5.9.0/docs/source/config.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/defining_traits.rst` & `traitlets-5.9.0/docs/source/defining_traits.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/index.rst` & `traitlets-5.9.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/migration.rst` & `traitlets-5.9.0/docs/source/migration.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/trait_types.rst` & `traitlets-5.9.0/docs/source/trait_types.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/using_traitlets.rst` & `traitlets-5.9.0/docs/source/using_traitlets.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/source/utils.rst` & `traitlets-5.9.0/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/docs/sphinxext/github.py` & `traitlets-5.9.0/docs/sphinxext/github.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/argcomplete_app.py` & `traitlets-5.9.0/examples/argcomplete_app.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/myapp.py` & `traitlets-5.9.0/examples/myapp.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/subcommands_app.py` & `traitlets-5.9.0/examples/subcommands_app.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/aliases.py` & `traitlets-5.9.0/examples/docs/aliases.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/flags.py` & `traitlets-5.9.0/examples/docs/flags.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/from_string.py` & `traitlets-5.9.0/examples/docs/from_string.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/load_config_app.py` & `traitlets-5.9.0/examples/docs/load_config_app.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/multiple_apps.py` & `traitlets-5.9.0/examples/docs/multiple_apps.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/examples/docs/subcommands.py` & `traitlets-5.9.0/examples/docs/subcommands.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/__init__.py` & `traitlets-5.9.0/traitlets/__init__.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/_version.py` & `traitlets-5.9.0/traitlets/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 handle the current version info of traitlets.
 """
 import re
 from typing import List
 
 # Version string must appear intact for hatch versioning
-__version__ = "5.8.1"
+__version__ = "5.9.0"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r"(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)"
 match = re.match(pattern, __version__)
 assert match is not None
 parts: List[object] = [int(match[part]) for part in ["major", "minor", "patch"]]
 if match["rest"]:
```

### Comparing `traitlets-5.8.1/traitlets/log.py` & `traitlets-5.9.0/traitlets/log.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/traitlets.py` & `traitlets-5.9.0/traitlets/traitlets.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/config/application.py` & `traitlets-5.9.0/traitlets/config/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -727,15 +727,15 @@
 
     def flatten_flags(self):
         """Flatten flags and aliases for loaders, so cl-args override as expected.
 
         This prevents issues such as an alias pointing to InteractiveShell,
         but a config file setting the same trait in TerminalInteraciveShell
         getting inappropriate priority over the command-line arg.
-        Also, loaders expect ``(key: longname)`` and not ````key: (longname, help)`` items.
+        Also, loaders expect ``(key: longname)`` and not ``key: (longname, help)`` items.
 
         Only aliases with exactly one descendent in the class list
         will be promoted.
 
         """
         # build a tree of classes in our list that inherit from a particular
         # it will be a dict by parent classname of classes in our list
@@ -781,15 +781,17 @@
             if not isinstance(key, tuple):
                 key = (key,)
             for k in key:
                 flags[k] = (newflag, help)
         return flags, aliases
 
     def _create_loader(self, argv, aliases, flags, classes):
-        return KVArgParseConfigLoader(argv, aliases, flags, classes=classes, log=self.log)
+        return KVArgParseConfigLoader(
+            argv, aliases, flags, classes=classes, log=self.log, subcommands=self.subcommands
+        )
 
     @classmethod
     def _get_sys_argv(cls, check_argcomplete: bool = False) -> t.List[str]:
         """Get `sys.argv` or equivalent from `argcomplete`
 
         `argcomplete`'s strategy is to call the python script with no arguments,
         so ``len(sys.argv) == 1``, and run until the `ArgumentParser` is constructed
```

### Comparing `traitlets-5.8.1/traitlets/config/argcomplete_config.py` & `traitlets-5.9.0/traitlets/config/argcomplete_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 """Helper utilities for integrating argcomplete with traitlets"""
+
+# Copyright (c) IPython Development Team.
+# Distributed under the terms of the Modified BSD License.
+
+
 import argparse
 import os
 import typing as t
 
 try:
     import argcomplete  # type: ignore[import]
     from argcomplete import CompletionFinder
@@ -72,31 +77,33 @@
         except (KeyError, ModuleNotFoundError):
             pass
 
 
 class ExtendedCompletionFinder(CompletionFinder):
     """An extension of CompletionFinder which dynamically completes class-trait based options
 
-    This finder mainly adds 2 functionalities:
+    This finder adds a few functionalities:
 
-    1. When completing options, it will add --Class. to the list of completions, for each
-    class in Application.classes that could complete the current option.
-    2. If it detects that we are currently trying to complete an option related to --Class.,
-    it will add the corresponding config traits of Class to the ArgumentParser instance,
+    1. When completing options, it will add ``--Class.`` to the list of completions, for each
+    class in `Application.classes` that could complete the current option.
+    2. If it detects that we are currently trying to complete an option related to ``--Class.``,
+    it will add the corresponding config traits of Class to the `ArgumentParser` instance,
     so that the traits' completers can be used.
+    3. If there are any subcommands, they are added as completions for the first word
 
-    Note that we are avoiding adding all config traits of all classes to the ArgumentParser,
+    Note that we are avoiding adding all config traits of all classes to the `ArgumentParser`,
     which would be easier but would add more runtime overhead and would also make completions
     appear more spammy.
 
-    These changes do require using the internals of argcomplete.CompletionFinder.
+    These changes do require using the internals of `argcomplete.CompletionFinder`.
     """
 
     _parser: argparse.ArgumentParser
-    config_classes: t.List[t.Any]  # Configurables
+    config_classes: t.List[t.Any] = []  # Configurables
+    subcommands: t.List[str] = []
 
     def match_class_completions(self, cword_prefix: str) -> t.List[t.Tuple[t.Any, str]]:
         """Match the word to be completed against our Configurable classes
 
         Check if cword_prefix could potentially match against --{class}. for any class
         in Application.classes.
         """
@@ -178,14 +185,24 @@
                     if matched_completions:
                         matched_cls = matched_completions[0][0]
                         self.inject_class_to_parser(matched_cls)
                     break
 
         completions: t.List[str]
         completions = super()._get_completions(comp_words, cword_prefix, *args)
+
+        # For subcommand-handling: it is difficult to get this to work
+        # using argparse subparsers, because the ArgumentParser accepts
+        # arbitrary extra_args, which ends up masking subparsers.
+        # Instead, check if comp_words only consists of the script,
+        # if so check if any subcommands start with cword_prefix.
+        if self.subcommands and len(comp_words) == 1:
+            argcomplete.debug("Adding subcommands for", cword_prefix)
+            completions.extend(subc for subc in self.subcommands if subc.startswith(cword_prefix))
+
         return completions
 
     def _get_option_completions(
         self, parser: argparse.ArgumentParser, cword_prefix: str
     ) -> t.List[str]:
         """Overriden to add --Class. completions when appropriate"""
         completions: t.List[str]
```

### Comparing `traitlets-5.8.1/traitlets/config/configurable.py` & `traitlets-5.9.0/traitlets/config/configurable.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/config/loader.py` & `traitlets-5.9.0/traitlets/config/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -780,27 +780,32 @@
         # must be done immediately prior to parsing because if we do it in init,
         # registration of explicit actions via parser.add_option will fail during setup
         for container in (self, self._optionals):
             container._option_string_actions = _DefaultOptionDict(container._option_string_actions)
         return super().parse_known_args(args, namespace)
 
 
+# type aliases
+Flags = t.Union[str, t.Tuple[str, ...]]
+SubcommandsDict = t.Dict[str, t.Any]
+
+
 class ArgParseConfigLoader(CommandLineConfigLoader):
     """A loader that uses the argparse module to load from the command line."""
 
     parser_class = ArgumentParser
-    Flags = t.Union[str, t.Tuple[str, ...]]
 
     def __init__(
         self,
         argv: t.Optional[t.List[str]] = None,
         aliases: t.Optional[t.Dict[Flags, str]] = None,
         flags: t.Optional[t.Dict[Flags, str]] = None,
         log: t.Any = None,
         classes: t.Optional[t.List[t.Type[t.Any]]] = None,
+        subcommands: t.Optional[SubcommandsDict] = None,
         *parser_args: t.Any,
         **parser_kw: t.Any,
     ) -> None:
         """Create a config loader for use with argparse.
 
         Parameters
         ----------
@@ -833,14 +838,15 @@
         self.clear()
         if argv is None:
             argv = sys.argv[1:]
         self.argv = argv
         self.aliases = aliases or {}
         self.flags = flags or {}
         self.classes = classes
+        self.subcommands = subcommands  # only used for argcomplete currently
 
         self.parser_args = parser_args
         self.version = parser_kw.pop("version", None)
         kwargs = dict(argument_default=argparse.SUPPRESS)
         kwargs.update(parser_kw)
         self.parser_kw = kwargs
 
@@ -870,14 +876,15 @@
         if argv is None:
             argv = self.argv
         if aliases is not None:
             self.aliases = aliases
         if classes is not None:
             self.classes = classes
         self._create_parser()
+        self._argcomplete(self.classes, self.subcommands)
         self._parse_args(argv)
         self._convert_to_config()
         return self.config
 
     def get_extra_args(self):
         if hasattr(self, "extra_args"):
             return self.extra_args
@@ -889,14 +896,20 @@
             *self.parser_args, **self.parser_kw  # type:ignore[arg-type]
         )
         self._add_arguments(self.aliases, self.flags, self.classes)
 
     def _add_arguments(self, aliases, flags, classes):
         raise NotImplementedError("subclasses must implement _add_arguments")
 
+    def _argcomplete(
+        self, classes: t.List[t.Any], subcommands: t.Optional[SubcommandsDict]
+    ) -> None:
+        """If argcomplete is enabled, allow triggering command-line autocompletion"""
+        pass
+
     def _parse_args(self, args):
         """self.parser->self.parsed_data"""
         uargs = [cast_unicode(a) for a in args]
 
         unpacked_aliases: t.Dict[str, str] = {}
         if self.aliases:
             unpacked_aliases = {}
@@ -1043,15 +1056,14 @@
                     argparse_kwds["flag"] = alias_flags[traitname]
                     argparse_kwds["alias"] = traitname
                 keys = ("-" + key, "--" + key) if len(key) == 1 else ("--" + key,)
                 action = paa(*keys, **argparse_kwds)
                 if argcompleter is not None:
                     # argcomplete's completers are callables returning list of completion strings
                     action.completer = functools.partial(argcompleter, key=key)  # type: ignore
-        self.argcomplete(classes)
 
     def _convert_to_config(self):
         """self.parsed_data->self.config, parse unrecognized extra args via KVLoader."""
         extra_args = self.extra_args
 
         for lhs, rhs in vars(self.parsed_data).items():
             if lhs == "extra_args":
@@ -1093,24 +1105,28 @@
 
         Probably a mistyped alias. By default just log a warning,
         but users can override this to raise an error instead, e.g.
         self.parser.error("Unrecognized alias: '%s'" % arg)
         """
         self.log.warning("Unrecognized alias: '%s', it will have no effect.", arg)
 
-    def argcomplete(self, classes: t.List[t.Any]) -> None:
+    def _argcomplete(
+        self, classes: t.List[t.Any], subcommands: t.Optional[SubcommandsDict]
+    ) -> None:
+        """If argcomplete is enabled, allow triggering command-line autocompletion"""
         try:
             import argcomplete  # type: ignore[import]  # noqa
         except ImportError:
             return
 
         from . import argcomplete_config
 
         finder = argcomplete_config.ExtendedCompletionFinder()
         finder.config_classes = classes
+        finder.subcommands = list(subcommands or [])
         # for ease of testing, pass through self._argcomplete_kwargs if set
         finder(self.parser, **getattr(self, "_argcomplete_kwargs", {}))
 
 
 class KeyValueConfigLoader(KVArgParseConfigLoader):
     """Deprecated in traitlets 5.0
```

### Comparing `traitlets-5.8.1/traitlets/config/manager.py` & `traitlets-5.9.0/traitlets/config/manager.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/config/sphinxdoc.py` & `traitlets-5.9.0/traitlets/config/sphinxdoc.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/config/tests/test_application.py` & `traitlets-5.9.0/traitlets/config/tests/test_application.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,18 @@
     def test_basic(self):
         app = MyApp()
         self.assertEqual(app.name, "myapp")
         self.assertEqual(app.running, False)
         self.assertEqual(app.classes, [MyApp, Bar, Foo])  # type:ignore
         self.assertEqual(app.config_file, "")
 
+    def test_app_name_set_via_constructor(self):
+        app = MyApp(name='set_via_constructor')
+        assert app.name == "set_via_constructor"
+
     def test_mro_discovery(self):
         app = MyApp()
 
         self.assertSequenceEqual(
             class_to_names(app._classes_with_config_traits()),
             ["Application", "MyApp", "Bar", "Foo"],
         )
@@ -629,14 +633,17 @@
         self.assertIsInstance(app.subapp, Sub1)
         self.assertIsInstance(app.subapp.subapp, Sub3)
         self.assertTrue(app.subapp.subapp.flag)  # Set by factory.
         # Check parent hierarchy.
         self.assertIs(app.subapp.parent, app)
         self.assertIs(app.subapp.subapp.parent, app.subapp)  # Set by factory.
 
+        Root.clear_instance()
+        Sub1.clear_instance()
+
     def test_loaded_config_files(self):
         app = MyApp()
         app.log = logging.getLogger()
         name = "config.py"
         with TemporaryDirectory("_1") as td1:
             config_file = pjoin(td1, name)
             with open(config_file, "w") as f:
```

### Comparing `traitlets-5.8.1/traitlets/config/tests/test_argcomplete.py` & `traitlets-5.9.0/traitlets/config/tests/test_argcomplete.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """
 Tests for argcomplete handling by traitlets.config.application.Application
 """
 
+# Copyright (c) IPython Development Team.
+# Distributed under the terms of the Modified BSD License.
+
 import io
 import os
 import typing as t
 
 import pytest
 
 argcomplete = pytest.importorskip("argcomplete")
@@ -17,16 +20,27 @@
 
 
 class ArgcompleteApp(Application):
     """Override loader to pass through kwargs for argcomplete testing"""
 
     argcomplete_kwargs: t.Dict[str, t.Any]
 
+    def __init__(self, *args, **kwargs):
+        # For subcommands, inherit argcomplete_kwargs from parent app
+        parent = kwargs.get("parent")
+        super().__init__(*args, **kwargs)
+        if parent:
+            argcomplete_kwargs = getattr(parent, "argcomplete_kwargs", None)
+            if argcomplete_kwargs:
+                self.argcomplete_kwargs = argcomplete_kwargs
+
     def _create_loader(self, argv, aliases, flags, classes):
-        loader = KVArgParseConfigLoader(argv, aliases, flags, classes=classes, log=self.log)
+        loader = KVArgParseConfigLoader(
+            argv, aliases, flags, classes=classes, log=self.log, subcommands=self.subcommands
+        )
         loader._argcomplete_kwargs = self.argcomplete_kwargs  # type: ignore[attr-defined]
         return loader
 
 
 class SubApp1(ArgcompleteApp):
     pass
 
@@ -165,31 +179,41 @@
         assert self.run_completer(app, "app --CustomCls.val  ") == ["foo", "bar"]
         assert self.run_completer(app, "app --CustomCls.val=") == ["foo", "bar"]
         completions = self.run_completer(app, "app --val= abc xyz", point=10)
         # fixed in argcomplete >= 2.0 to return latter below
         assert completions == ["--val=foo", "--val=bar"] or completions == ["foo", "bar"]
         assert self.run_completer(app, "app --val  --log-level=", point=10) == ["foo", "bar"]
 
-    # TODO: don't have easy way of testing subcommands yet, since we want
-    # to inject _argcomplete_kwargs to subapp. Could use mocking for this
-    # def test_complete_subcommands_subapp1(self, argcomplete_on):
-    #     # subcommand handling modifies _ARGCOMPLETE env var global state, so
-    #     # only can test one completion per unit test
-    #     app = MainApp()
-    #     assert set(self.run_completer(app, "app subapp1 --Sub")) > {
-    #         '--SubApp1.show_config',
-    #         '--SubApp1.log_level',
-    #         '--SubApp1.log_format',
-    #     }
-    #
-    # def test_complete_subcommands_subapp2(self, argcomplete_on):
-    #     app = MainApp()
-    #     assert set(self.run_completer(app, "app subapp2 --")) > {
-    #         '--Application.',
-    #         '--SubApp2.',
-    #     }
+    def test_complete_subcommands(self, argcomplete_on):
+        app = MainApp()
+        assert set(self.run_completer(app, "app ")) >= {"subapp1", "subapp2"}
+        assert set(self.run_completer(app, "app sub")) == {"subapp1", "subapp2"}
+        assert set(self.run_completer(app, "app subapp1")) == {"subapp1"}
+
+    def test_complete_subcommands_subapp1(self, argcomplete_on):
+        # subcommand handling modifies _ARGCOMPLETE env var global state, so
+        # only can test one completion per unit test
+        app = MainApp()
+        try:
+            assert set(self.run_completer(app, "app subapp1 --Sub")) > {
+                '--SubApp1.show_config',
+                '--SubApp1.log_level',
+                '--SubApp1.log_format',
+            }
+        finally:
+            SubApp1.clear_instance()
+
+    def test_complete_subcommands_subapp2(self, argcomplete_on):
+        app = MainApp()
+        try:
+            assert set(self.run_completer(app, "app subapp2 --")) > {
+                '--Application.',
+                '--SubApp2.',
+            }
+        finally:
+            SubApp2.clear_instance()
 
     def test_complete_subcommands_main(self, argcomplete_on):
         app = MainApp()
         completions = set(self.run_completer(app, "app --"))
         assert completions > {'--Application.', '--MainApp.'}
         assert "--SubApp1." not in completions and "--SubApp2." not in completions
```

### Comparing `traitlets-5.8.1/traitlets/config/tests/test_configurable.py` & `traitlets-5.9.0/traitlets/config/tests/test_configurable.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/config/tests/test_loader.py` & `traitlets-5.9.0/traitlets/config/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/tests/_warnings.py` & `traitlets-5.9.0/traitlets/tests/_warnings.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/tests/test_traitlets.py` & `traitlets-5.9.0/traitlets/tests/test_traitlets.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/tests/test_traitlets_enum.py` & `traitlets-5.9.0/traitlets/tests/test_traitlets_enum.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/tests/utils.py` & `traitlets-5.9.0/traitlets/tests/utils.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/__init__.py` & `traitlets-5.9.0/traitlets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/bunch.py` & `traitlets-5.9.0/traitlets/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/decorators.py` & `traitlets-5.9.0/traitlets/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/descriptions.py` & `traitlets-5.9.0/traitlets/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/getargspec.py` & `traitlets-5.9.0/traitlets/utils/getargspec.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/importstring.py` & `traitlets-5.9.0/traitlets/utils/importstring.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/nested_update.py` & `traitlets-5.9.0/traitlets/utils/nested_update.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/sentinel.py` & `traitlets-5.9.0/traitlets/utils/sentinel.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/text.py` & `traitlets-5.9.0/traitlets/utils/text.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/tests/test_decorators.py` & `traitlets-5.9.0/traitlets/utils/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/traitlets/utils/tests/test_importstring.py` & `traitlets-5.9.0/traitlets/utils/tests/test_importstring.py`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/COPYING.md` & `traitlets-5.9.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/README.md` & `traitlets-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/pyproject.toml` & `traitlets-5.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `traitlets-5.8.1/PKG-INFO` & `traitlets-5.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traitlets
-Version: 5.8.1
+Version: 5.9.0
 Summary: Traitlets Python configuration system
 Project-URL: Homepage, https://github.com/ipython/traitlets
 Author-email: IPython Development Team <ipython-dev@python.org>
 License: # Licensing terms
         
         Traitlets is adapted from enthought.traits, Copyright (c) Enthought, Inc.,
         under the terms of the Modified BSD License.
```

