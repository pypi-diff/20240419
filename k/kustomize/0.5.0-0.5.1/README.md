# Comparing `tmp/kustomize-0.5.0.tar.gz` & `tmp/kustomize-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp0hb69z12/tmppfv97vj0/kustomize-0.5.0.tar", last modified: Wed Dec  2 01:03:15 2020, max compression
+gzip compressed data, was "kustomize-0.5.1.tar", last modified: Fri Apr 19 02:47:36 2024, max compression
```

## Comparing `kustomize-0.5.0.tar` & `kustomize-0.5.1.tar`

### file list

```diff
@@ -1,278 +1,281 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-12-02 01:02:51.000000 kustomize-0.5.0/.coveragerc
--rw-rw-r--   0 travis    (2000) travis    (2000)      246 2020-12-02 01:02:51.000000 kustomize-0.5.0/.flake8
--rw-rw-r--   0 travis    (2000) travis    (2000)     1232 2020-12-02 01:02:51.000000 kustomize-0.5.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2020-12-02 01:02:51.000000 kustomize-0.5.0/.pre-commit-config.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2020-12-02 01:02:51.000000 kustomize-0.5.0/.readthedocs.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2020-12-02 01:02:51.000000 kustomize-0.5.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1090 2020-12-02 01:02:51.000000 kustomize-0.5.0/CHANGES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1063 2020-12-02 01:02:51.000000 kustomize-0.5.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     4337 2020-12-02 01:03:15.007484 kustomize-0.5.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3042 2020-12-02 01:02:51.000000 kustomize-0.5.0/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      435 2020-12-02 01:02:51.000000 kustomize-0.5.0/appveyor.yml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)      755 2020-12-02 01:02:51.000000 kustomize-0.5.0/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2020-12-02 01:02:51.000000 kustomize-0.5.0/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2020-12-02 01:02:51.000000 kustomize-0.5.0/docs/index.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/kustomize/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/kustomize/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6795 2020-12-02 01:02:51.000000 kustomize-0.5.0/kustomize/generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1481 2020-12-02 01:02:51.000000 kustomize-0.5.0/kustomize/main.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/kustomize.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4337 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     8988 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-12-02 01:03:14.000000 kustomize-0.5.0/kustomize.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      167 2020-12-02 01:02:51.000000 kustomize-0.5.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      148 2020-12-02 01:02:51.000000 kustomize-0.5.0/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)     1015 2020-12-02 01:03:15.007484 kustomize-0.5.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      112 2020-12-02 01:02:51.000000 kustomize-0.5.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8150 2020-12-02 01:02:51.000000 kustomize-0.5.0/skeleton.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      614 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      745 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      598 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.987494 kustomize-0.5.0/tests/fixtures/attrs/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/attrs/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      343 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/attrs/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/attrs/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/attrs/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/attrs/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/attrs/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/production/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/production/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/production/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      150 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/production/replica_count.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/staging/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/staging/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/staging/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/python/overlays/staging/special_labels.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.979498 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.979498 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.991492 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/production/
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/production/kustomization.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       92 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/production/replica_count.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/staging/
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/staging/kustomization.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/overlays/staging/special_labels.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      333 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/dataclasses_/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes11/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes11/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1513 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.995490 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/kubernetes11/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      124 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/add_init_container.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      406 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/add_init_container/
--rw-rw-r--   0 travis    (2000) travis    (2000)       53 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/add_init_container/add_init_container.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      339 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      203 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      209 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:14.999488 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/configmaps/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/configmaps/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      257 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/configmaps/configMap.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/deployments/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/deployments/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      235 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/kustomization.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/services/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      275 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/services/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/configmaps/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/configmaps/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/deployments/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/services/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/services/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      896 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2100 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      362 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      117 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/to_dict/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/to_dict/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.003486 kustomize-0.5.0/tests/fixtures/tuple_multiple/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      387 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/service/service.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      511 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/configMap.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1657 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/kustomization.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      272 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/configMap/
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/configMap/configMap.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/deployment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      697 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      199 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/kustomization.yaml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-12-02 01:03:15.007484 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/service/
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/service/service.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5342 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/test_generators.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1408 2020-12-02 01:02:51.000000 kustomize-0.5.0/tests/test_main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2020-12-02 01:02:51.000000 kustomize-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.204698 kustomize-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 02:47:17.000000 kustomize-0.5.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-19 02:47:17.000000 kustomize-0.5.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 02:47:17.000000 kustomize-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-19 02:47:17.000000 kustomize-0.5.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-19 02:47:17.000000 kustomize-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:47:17.000000 kustomize-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-19 02:47:17.000000 kustomize-0.5.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-19 02:47:17.000000 kustomize-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-19 02:47:17.000000 kustomize-0.5.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-19 02:47:36.200698 kustomize-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-19 02:47:17.000000 kustomize-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 02:47:17.000000 kustomize-0.5.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.168698 kustomize-0.5.1/kustomize/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 02:47:17.000000 kustomize-0.5.1/kustomize/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/kustomize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 02:47:36.000000 kustomize-0.5.1/kustomize.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 02:47:17.000000 kustomize-0.5.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-19 02:47:17.000000 kustomize-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-19 02:47:17.000000 kustomize-0.5.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-19 02:47:17.000000 kustomize-0.5.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 02:47:36.204698 kustomize-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.172698 kustomize-0.5.1/tests/fixtures/attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/attrs/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/attrs/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.176698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/production/replica_count.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/python/overlays/staging/special_labels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.156698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.156698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/kustomization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/production/replica_count.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/kustomization.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/overlays/staging/special_labels.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/dataclasses_/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.180698 kustomize-0.5.1/tests/fixtures/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/kubernetes11/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.184698 kustomize-0.5.1/tests/fixtures/patchesJson6902/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/add_init_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/add_init_container/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/add_init_container/add_init_container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.188698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/configmaps/configMap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/kustomization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/services/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/configmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/configmaps/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.192698 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/services/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/to_dict/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/to_dict/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.196698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/service/service.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/configMap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/kustomization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/configMap/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/configMap/configMap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/kustomization.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:47:36.200698 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/service/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-19 02:47:17.000000 kustomize-0.5.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 02:47:17.000000 kustomize-0.5.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-19 02:47:17.000000 kustomize-0.5.1/tox.ini
```

### Comparing `kustomize-0.5.0/.gitignore` & `kustomize-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/CHANGES.rst` & `kustomize-0.5.1/NEWS.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v0.5.1
+======
+
+Bugfixes
+--------
+
+- Refreshed the package metadata. (#1)
+- Require Python 3.8 or later.
+
+
 0.5.0
 =====
 
 * Separating generated modules by directories to avoid name clashes.
 
 0.4.1
 =====
```

### Comparing `kustomize-0.5.0/LICENSE` & `kustomize-0.5.1/LICENSE`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-MIT License
-
-Copyright (c) 2019 YouGov
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
+of this software and associated documentation files (the "Software"), to
+deal in the Software without restriction, including without limitation the
+rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
+sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
+IN THE SOFTWARE.
```

### Comparing `kustomize-0.5.0/README.rst` & `kustomize-0.5.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-python-kustomize
-================
-
-Build your Kubernetes manifests for Kustomize in Python!
-
 .. image:: https://img.shields.io/pypi/v/kustomize.svg
    :target: https://pypi.org/project/kustomize
 
 .. image:: https://img.shields.io/pypi/pyversions/kustomize.svg
 
-.. image:: https://img.shields.io/travis/yougov/python-kustomize/master.svg
-   :target: https://travis-ci.org/yougov/python-kustomize
+.. image:: https://github.com/coherent-oss/python-kustomize/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/coherent-oss/python-kustomize/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
-.. .. image:: https://img.shields.io/appveyor/ci/yougov/python-kustomize/master.svg
-..    :target: https://ci.appveyor.com/project/yougov/python-kustomize/branch/master
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. .. image:: https://readthedocs.org/projects/kustomize/badge/?version=latest
-..    :target: https://kustomize.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
+
+Build your Kubernetes manifests for Kustomize in Python!
 
 * PyPI: https://pypi.org/project/kustomize/
 * Repository: https://github.com/yougov/python-kustomize
 * Documentation: https://python-kustomize.readthedocs.io/en/latest/
 
 Overview
 --------
@@ -44,18 +46,21 @@
 
 In other words, the idea is to "compile" Python files into Kustomize files, then
 just use Kustomize for the rest of the deployment.
 
 Installing
 ----------
 
-The only mandatory dependency to this project is ``PyYAML``. Besides this, you
-can have ``attr`` installed if you want to use their classes, and, if you're
-running on Python 3.6, you can install ``dataclasses`` to use them - although
-this project is tested on Python 3.7 and 3.8 only, it probably runs fine on 3.6.
+The only mandatory dependency to this project is ``PyYAML``. This library
+supports a number of object definition types:
+
+* ``dict``
+* ``dataclasses``
+* ``attr`` (needs the library installed)
+* ``kubernetes`` (needs the library installed)
 
 This package will be available as ``kustomize``; you may install it with pip,
 for example::
 
     $ pip install kustomize
 
 This will also install ``PyYAML`` if it's not already installed.
```

### Comparing `kustomize-0.5.0/docs/conf.py` & `kustomize-0.5.1/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
-                pattern=r'^(?m)((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n',
+                pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `kustomize-0.5.0/kustomize/generators.py` & `kustomize-0.5.1/kustomize/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,34 +56,32 @@
     def build(self, dest_path: Path) -> Path:
         path = dest_path / self.build_path
         _dump_data(self.data, path)
 
         return self.build_path
 
 
-def generate(
-        source_path: Path, dest_path: Path, attr_name: str = 'kustomization'):
+def generate(source_path: Path, dest_path: Path, attr_name: str = 'kustomization'):
     source_path = source_path.absolute()
     dest_path = dest_path.absolute()
 
-    for (dirpath, dirnames, filenames) in os.walk(str(source_path)):
+    for dirpath, dirnames, filenames in os.walk(str(source_path)):
         for dirname in dirnames:
             down_source_path = source_path / dirname
             down_dest_path = dest_path / dirname
             generate(down_source_path, down_dest_path, attr_name)
 
     _generate_for_source(source_path, dest_path, attr_name)
 
 
 def _generate_for_source(source_path: Path, dest_path: Path, attr_name: str):
     if not (source_path / 'kustomization.py').is_file():
         return
 
-    logger.info(
-        'Generating kustomization from %s to %s', source_path, dest_path)
+    logger.info('Generating kustomization from %s to %s', source_path, dest_path)
 
     prepended = False
     source_path_str = str(source_path)
     if source_path_str not in sys.path:
         sys.path.insert(0, source_path_str)
         prepended = True
     try:
@@ -95,15 +93,15 @@
         if prepended:
             sys.path.pop(0)
 
 
 def _dump_data(data, path):
     logger.debug('Dumping data into %s', path)
     os.makedirs(os.path.dirname(path), mode=0o755, exist_ok=True)
-    with open(str(path), 'w') as f:
+    with open(str(path), 'w', encoding='utf-8') as f:
         if isinstance(data, tuple):
             yaml.safe_dump_all(clean_data(data), f)
         else:
             yaml.safe_dump(clean_data(data), f)
 
 
 def clean_data(data: Union[dict, list, tuple]):
@@ -134,16 +132,15 @@
         'patchesStrategicMerge',
     )
 
     for extension_name in extensions_names:
         if kustomization.get(extension_name) is None:
             continue
         extensions = [
-            Extension.from_reference(string)
-            for string in kustomization[extension_name]
+            Extension.from_reference(string) for string in kustomization[extension_name]
         ]
         kustomization[extension_name] = [
             str(resource.build(dest_path)) for resource in extensions
         ]
 
     if kustomization.get('patchesJson6902') is not None:
         patches = kustomization['patchesJson6902']
@@ -161,19 +158,20 @@
         return False
 
     return attr.has(type(obj))
 
 
 def _is_kubernetes(obj):
     return (
-        hasattr(obj, 'to_dict') and
-        hasattr(obj, 'attribute_map') and
-        (
+        hasattr(obj, 'to_dict')
+        and hasattr(obj, 'attribute_map')
+        and (
             # python-kubernetes<11
-            hasattr(obj, 'swagger_types') or
+            hasattr(obj, 'swagger_types')
+            or
             # python-kubernetes>=11
             hasattr(obj, 'openapi_types')
         )
     )
 
 
 def _k8s_to_serializable(obj):
@@ -208,30 +206,30 @@
             if getattr(obj, attr) is not None
         }
 
     return {key: _k8s_to_serializable(val) for key, val in obj_dict.items()}
 
 
 def to_dict_or_dicts(obj):
-    logger.debug(
-        'Transforming object of type %s into dict or dicts', type(obj))
+    logger.debug('Transforming object of type %s into dict or dicts', type(obj))
     if isinstance(obj, tuple):
         return tuple(to_dict_or_dicts(o) for o in obj)
     if _is_kubernetes(obj):
         logger.debug('Object is compatible with kubernetes models')
         return _k8s_to_serializable(obj)
     if hasattr(obj, 'to_dict'):
         logger.debug('Object has a simple to_dict, using it for conversion')
         obj = obj.to_dict()
     elif is_dataclass(obj):
         logger.debug('Object is dataclass, using it for conversion')
         obj = asdict(obj)
     elif is_attr_class(obj):
         logger.debug('Object is from attr class, using it for conversion')
         import attr
+
         obj = attr.asdict(obj, recurse=True)
     elif hasattr(obj, '__dict__'):
         obj = obj.__dict__
 
     obj = deepcopy(obj)
 
     return obj
```

### Comparing `kustomize-0.5.0/kustomize/main.py` & `kustomize-0.5.1/kustomize/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 import argparse
 import logging
 import sys
 from pathlib import Path
 
 
 def _get_options(args):
-    parser = argparse.ArgumentParser(description="""
+    parser = argparse.ArgumentParser(
+        description="""
         Generates a kustomization directory based on similar Python files.
         The generated directory can then be used by Kustomize.
-    """)
+    """
+    )
 
     parser.add_argument(
-        '--attr-name', '-a', default='kustomization', required=False,
-        help='Name of the attribute from the kustomization.py files.'
+        '--attr-name',
+        '-a',
+        default='kustomization',
+        required=False,
+        help='Name of the attribute from the kustomization.py files.',
     )
     parser.add_argument(
-        '--verbose', '-v', default=False, action='store_true',
-        help='Print debug logs to stdout.'
+        '--verbose',
+        '-v',
+        default=False,
+        action='store_true',
+        help='Print debug logs to stdout.',
     )
     parser.add_argument(
-        'source_path',
-        help='Source directory with Python kustomization files.'
+        'source_path', help='Source directory with Python kustomization files.'
     )
     parser.add_argument(
         'dest_path',
         help=(
-            'Destination directory where the Kustomize YAML files will be '
-            'put at.')
+            'Destination directory where the Kustomize YAML files will be ' 'put at.'
+        ),
     )
 
     return parser.parse_args(args)
 
 
 def run(args):
     options = _get_options(args)
```

### Comparing `kustomize-0.5.0/kustomize.egg-info/SOURCES.txt` & `kustomize-0.5.1/kustomize.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 .coveragerc
-.flake8
+.editorconfig
 .gitignore
 .pre-commit-config.yaml
-.readthedocs.yml
-.travis.yml
-CHANGES.rst
+.readthedocs.yaml
 LICENSE
+NEWS.rst
 README.rst
-appveyor.yml
+mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
-setup.py
-skeleton.md
+ruff.toml
+towncrier.toml
 tox.ini
+.github/dependabot.yml
+.github/workflows/main.yml
 docs/conf.py
 docs/history.rst
 docs/index.rst
 kustomize/__init__.py
 kustomize/generators.py
 kustomize/main.py
 kustomize.egg-info/PKG-INFO
```

### Comparing `kustomize-0.5.0/tests/conftest.py` & `kustomize-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/configMap.py` & `kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/configMap.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 class ConfigMap:
     metadata: dict
     data: dict
     apiVersion: str = 'v1'
     kind: str = 'ConfigMap'
 
     def __init__(
-            self, metadata: Metadata, data: dict,
-            apiVersion: str = 'v1', kind: str = 'ConfigMap',
+        self,
+        metadata: Metadata,
+        data: dict,
+        apiVersion: str = 'v1',
+        kind: str = 'ConfigMap',
     ):
         self.metadata = metadata.__dict__
         self.data = data
         self.apiVersion = apiVersion
         self.kind = kind
```

### Comparing `kustomize-0.5.0/tests/fixtures/attributes_as_dict/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/base_and_overlays/python/base/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-class CustomDeployment:
-    def to_dict(self) -> dict:
-        return {
-            'apiVersion': 'apps/v1',
-            'kind': 'Deployment',
-            'metadata': {'name': 'the-deployment'},
+deployment = {
+    'apiVersion': 'apps/v1',
+    'kind': 'Deployment',
+    'metadata': {'name': 'the-deployment'},
+    'spec': {
+        'replicas': 3,
+        'template': {
+            'metadata': {'labels': {'deployment': 'hello'}},
             'spec': {
-                'replicas': 3,
-                'template': {
-                    'metadata': {'labels': {'deployment': 'hello'}},
-                    'spec': {
-                        'containers': [
+                'containers': [
+                    {
+                        'name': 'the-container',
+                        'image': 'monopole/hello:1',
+                        'command': [
+                            '/hello',
+                            '--port=8080',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                        ],
+                        'ports': [{'containerPort': 8080}],
+                        'env': [
                             {
-                                'name': 'the-container',
-                                'image': 'monopole/hello:1',
-                                'command': [
-                                    '/hello',
-                                    '--port=8080',
-                                    '--enableRiskyFeature=$('
-                                    'ENABLE_RISKY)',
-                                ],
-                                'ports': [{'containerPort': 8080}],
-                                'env': [
-                                    {
-                                        'name': 'ALT_GREETING',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'altGreeting'
-                                            }
-                                        }
-                                    },
-                                    {
-                                        'name': 'ENABLE_RISKY',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'enableRisky'
-                                            }
-                                        }
-                                    },
-                                ],
-                            }]
+                                'name': 'ALT_GREETING',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'altGreeting',
+                                    }
+                                },
+                            },
+                            {
+                                'name': 'ENABLE_RISKY',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'enableRisky',
+                                    }
+                                },
+                            },
+                        ],
                     }
-                }
-            }
-        }
-
-
-deployment = CustomDeployment()
+                ]
+            },
+        },
+    },
+}
```

### Comparing `kustomize-0.5.0/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/attributes_as_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/attrs/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/dataclasses_/python/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-class CustomDeployment:
-    def to_dict(self) -> dict:
-        return {
-            'apiVersion': 'apps/v1',
-            'kind': 'Deployment',
-            'metadata': {'name': 'the-deployment'},
+deployment = {
+    'apiVersion': 'apps/v1',
+    'kind': 'Deployment',
+    'metadata': {'name': 'the-deployment'},
+    'spec': {
+        'replicas': 3,
+        'template': {
+            'metadata': {'labels': {'deployment': 'hello'}},
             'spec': {
-                'replicas': 3,
-                'template': {
-                    'metadata': {'labels': {'deployment': 'hello'}},
-                    'spec': {
-                        'containers': [
+                'containers': [
+                    {
+                        'name': 'the-container',
+                        'image': 'monopole/hello:1',
+                        'command': [
+                            '/hello',
+                            '--port=8080',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                        ],
+                        'ports': [{'containerPort': 8080}],
+                        'env': [
                             {
-                                'name': 'the-container',
-                                'image': 'monopole/hello:1',
-                                'command': [
-                                    '/hello',
-                                    '--port=8080',
-                                    '--enableRiskyFeature=$('
-                                    'ENABLE_RISKY)',
-                                ],
-                                'ports': [{'containerPort': 8080}],
-                                'env': [
-                                    {
-                                        'name': 'ALT_GREETING',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'altGreeting'
-                                            }
-                                        }
-                                    },
-                                    {
-                                        'name': 'ENABLE_RISKY',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'enableRisky'
-                                            }
-                                        }
-                                    },
-                                ],
-                            }]
+                                'name': 'ALT_GREETING',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'altGreeting',
+                                    }
+                                },
+                            },
+                            {
+                                'name': 'ENABLE_RISKY',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'enableRisky',
+                                    }
+                                },
+                            },
+                        ],
                     }
-                }
-            }
-        }
-
-
-deployment = CustomDeployment()
+                ]
+            },
+        },
+    },
+}
```

### Comparing `kustomize-0.5.0/tests/fixtures/attrs/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/attrs/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/base_and_overlays/python/base/deployment.py` & `kustomize-0.5.1/tests/fixtures/simple_dict/python/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-deployment = {
+my_deployment = {
     'apiVersion': 'apps/v1',
     'kind': 'Deployment',
     'metadata': {'name': 'the-deployment'},
     'spec': {
         'replicas': 3,
         'template': {
             'metadata': {'labels': {'deployment': 'hello'}},
@@ -10,36 +10,36 @@
                 'containers': [
                     {
                         'name': 'the-container',
                         'image': 'monopole/hello:1',
                         'command': [
                             '/hello',
                             '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
                         ],
                         'ports': [{'containerPort': 8080}],
                         'env': [
                             {
                                 'name': 'ALT_GREETING',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'altGreeting'
+                                        'key': 'altGreeting',
                                     }
-                                }
+                                },
                             },
                             {
                                 'name': 'ENABLE_RISKY',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'enableRisky'
+                                        'key': 'enableRisky',
                                     }
-                                }
+                                },
                             },
                         ],
-                    }]
-            }
-        }
-    }
+                    }
+                ]
+            },
+        },
+    },
 }
```

### Comparing `kustomize-0.5.0/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/base_and_overlays/reference/base/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/dataclasses_/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-deployment = {
+my_deployment = {
     'apiVersion': 'apps/v1',
     'kind': 'Deployment',
     'metadata': {'name': 'the-deployment'},
     'spec': {
         'replicas': 3,
         'template': {
             'metadata': {'labels': {'deployment': 'hello'}},
@@ -10,36 +10,36 @@
                 'containers': [
                     {
                         'name': 'the-container',
                         'image': 'monopole/hello:1',
                         'command': [
                             '/hello',
                             '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
                         ],
                         'ports': [{'containerPort': 8080}],
                         'env': [
                             {
                                 'name': 'ALT_GREETING',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'altGreeting'
+                                        'key': 'altGreeting',
                                     }
-                                }
+                                },
                             },
                             {
                                 'name': 'ENABLE_RISKY',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'enableRisky'
+                                        'key': 'enableRisky',
                                     }
-                                }
+                                },
                             },
                         ],
-                    }]
-            }
-        }
-    }
+                    }
+                ]
+            },
+        },
+    },
 }
```

### Comparing `kustomize-0.5.0/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/dataclasses_/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes/python/configMap.py` & `kustomize-0.5.1/tests/fixtures/kubernetes11/python/configMap.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime as dt
 
 
 class Metadata:
-    swagger_types = {
+    openapi_types = {
         'name': 'str',
         'labels': 'dict',
     }
 
     attribute_map = {
         'name': 'name',
         'labels': 'labels',
@@ -20,31 +20,34 @@
         return {
             'name': self.name,
             'labels': self.labels,
         }
 
 
 class ConfigMap:
-    swagger_types = {
+    openapi_types = {
         'metadata': 'Metadata',
         'data': 'dict',
         'api_version': 'str',
         'kind': 'str',
     }
 
     attribute_map = {
         'metadata': 'metadata',
         'data': 'data',
         'api_version': 'apiVersion',
         'kind': 'kind',
     }
 
     def __init__(
-            self, metadata: Metadata, data: dict,
-            api_version: str = 'v1', kind: str = 'ConfigMap',
+        self,
+        metadata: Metadata,
+        data: dict,
+        api_version: str = 'v1',
+        kind: str = 'ConfigMap',
     ):
         self.metadata = metadata
         self.data = data
         self.api_version = api_version
         self.kind = kind
 
     def to_dict(self) -> dict:
@@ -60,11 +63,11 @@
     metadata=Metadata(
         name='the-map',
         labels={
             'when': dt.datetime(2019, 1, 1),
             'ignore': None,
             'numbers': [1, 2],
             'others': (3, 4),
-        }
+        },
     ),
     data={'altGreeting': 'Good Morning!', 'enableRisky': 'false'},
 )
```

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/patchesJson6902/python/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-class CustomDeployment:
-    def to_dict(self) -> dict:
-        return {
-            'apiVersion': 'apps/v1',
-            'kind': 'Deployment',
-            'metadata': {'name': 'the-deployment'},
+deployment = {
+    'apiVersion': 'apps/v1',
+    'kind': 'Deployment',
+    'metadata': {'name': 'the-deployment'},
+    'spec': {
+        'replicas': 3,
+        'template': {
+            'metadata': {'labels': {'deployment': 'hello'}},
             'spec': {
-                'replicas': 3,
-                'template': {
-                    'metadata': {'labels': {'deployment': 'hello'}},
-                    'spec': {
-                        'containers': [
+                'containers': [
+                    {
+                        'name': 'the-container',
+                        'image': 'monopole/hello:1',
+                        'command': [
+                            '/hello',
+                            '--port=8080',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                        ],
+                        'ports': [{'containerPort': 8080}],
+                        'env': [
                             {
-                                'name': 'the-container',
-                                'image': 'monopole/hello:1',
-                                'command': [
-                                    '/hello',
-                                    '--port=8080',
-                                    '--enableRiskyFeature=$('
-                                    'ENABLE_RISKY)',
-                                ],
-                                'ports': [{'containerPort': 8080}],
-                                'env': [
-                                    {
-                                        'name': 'ALT_GREETING',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'altGreeting'
-                                            }
-                                        }
-                                    },
-                                    {
-                                        'name': 'ENABLE_RISKY',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'enableRisky'
-                                            }
-                                        }
-                                    },
-                                ],
-                            }]
+                                'name': 'ALT_GREETING',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'altGreeting',
+                                    }
+                                },
+                            },
+                            {
+                                'name': 'ENABLE_RISKY',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'enableRisky',
+                                    }
+                                },
+                            },
+                        ],
                     }
-                }
-            }
-        }
-
-
-deployment = CustomDeployment()
+                ]
+            },
+        },
+    },
+}
```

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/kubernetes/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes11/python/configMap.py` & `kustomize-0.5.1/tests/fixtures/kubernetes/python/configMap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime as dt
 
 
 class Metadata:
-    openapi_types = {
+    swagger_types = {
         'name': 'str',
         'labels': 'dict',
     }
 
     attribute_map = {
         'name': 'name',
         'labels': 'labels',
@@ -20,31 +20,34 @@
         return {
             'name': self.name,
             'labels': self.labels,
         }
 
 
 class ConfigMap:
-    openapi_types = {
+    swagger_types = {
         'metadata': 'Metadata',
         'data': 'dict',
         'api_version': 'str',
         'kind': 'str',
     }
 
     attribute_map = {
         'metadata': 'metadata',
         'data': 'data',
         'api_version': 'apiVersion',
         'kind': 'kind',
     }
 
     def __init__(
-            self, metadata: Metadata, data: dict,
-            api_version: str = 'v1', kind: str = 'ConfigMap',
+        self,
+        metadata: Metadata,
+        data: dict,
+        api_version: str = 'v1',
+        kind: str = 'ConfigMap',
     ):
         self.metadata = metadata
         self.data = data
         self.api_version = api_version
         self.kind = kind
 
     def to_dict(self) -> dict:
@@ -60,11 +63,11 @@
     metadata=Metadata(
         name='the-map',
         labels={
             'when': dt.datetime(2019, 1, 1),
             'ignore': None,
             'numbers': [1, 2],
             'others': (3, 4),
-        }
+        },
     ),
     data={'altGreeting': 'Good Morning!', 'enableRisky': 'false'},
 )
```

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes11/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/simple_dict_defaults/python/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,45 @@
-class CustomDeployment:
-    def to_dict(self) -> dict:
-        return {
-            'apiVersion': 'apps/v1',
-            'kind': 'Deployment',
-            'metadata': {'name': 'the-deployment'},
+deployment = {
+    'apiVersion': 'apps/v1',
+    'kind': 'Deployment',
+    'metadata': {'name': 'the-deployment'},
+    'spec': {
+        'replicas': 3,
+        'template': {
+            'metadata': {'labels': {'deployment': 'hello'}},
             'spec': {
-                'replicas': 3,
-                'template': {
-                    'metadata': {'labels': {'deployment': 'hello'}},
-                    'spec': {
-                        'containers': [
+                'containers': [
+                    {
+                        'name': 'the-container',
+                        'image': 'monopole/hello:1',
+                        'command': [
+                            '/hello',
+                            '--port=8080',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                        ],
+                        'ports': [{'containerPort': 8080}],
+                        'env': [
                             {
-                                'name': 'the-container',
-                                'image': 'monopole/hello:1',
-                                'command': [
-                                    '/hello',
-                                    '--port=8080',
-                                    '--enableRiskyFeature=$('
-                                    'ENABLE_RISKY)',
-                                ],
-                                'ports': [{'containerPort': 8080}],
-                                'env': [
-                                    {
-                                        'name': 'ALT_GREETING',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'altGreeting'
-                                            }
-                                        }
-                                    },
-                                    {
-                                        'name': 'ENABLE_RISKY',
-                                        'valueFrom': {
-                                            'configMapKeyRef': {
-                                                'name': 'the-map',
-                                                'key': 'enableRisky'
-                                            }
-                                        }
-                                    },
-                                ],
-                            }]
+                                'name': 'ALT_GREETING',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'altGreeting',
+                                    }
+                                },
+                            },
+                            {
+                                'name': 'ENABLE_RISKY',
+                                'valueFrom': {
+                                    'configMapKeyRef': {
+                                        'name': 'the-map',
+                                        'key': 'enableRisky',
+                                    }
+                                },
+                            },
+                        ],
                     }
-                }
-            }
-        }
-
-
-deployment = CustomDeployment()
+                ]
+            },
+        },
+    },
+}
```

### Comparing `kustomize-0.5.0/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/kubernetes11/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/patchesJson6902/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/tuple_multiple/python/deployment.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,36 +10,36 @@
                 'containers': [
                     {
                         'name': 'the-container',
                         'image': 'monopole/hello:1',
                         'command': [
                             '/hello',
                             '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
                         ],
                         'ports': [{'containerPort': 8080}],
                         'env': [
                             {
                                 'name': 'ALT_GREETING',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'altGreeting'
+                                        'key': 'altGreeting',
                                     }
-                                }
+                                },
                             },
                             {
                                 'name': 'ENABLE_RISKY',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'enableRisky'
+                                        'key': 'enableRisky',
                                     }
-                                }
+                                },
                             },
                         ],
-                    }]
-            }
-        }
-    }
+                    }
+                ]
+            },
+        },
+    },
 }
```

### Comparing `kustomize-0.5.0/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/patchesJson6902/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/python/deployment.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-my_deployment = {
+deployment = {
     'apiVersion': 'apps/v1',
     'kind': 'Deployment',
     'metadata': {'name': 'the-deployment'},
     'spec': {
         'replicas': 3,
         'template': {
             'metadata': {'labels': {'deployment': 'hello'}},
@@ -10,36 +10,36 @@
                 'containers': [
                     {
                         'name': 'the-container',
                         'image': 'monopole/hello:1',
                         'command': [
                             '/hello',
                             '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
+                            '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
                         ],
                         'ports': [{'containerPort': 8080}],
                         'env': [
                             {
                                 'name': 'ALT_GREETING',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'altGreeting'
+                                        'key': 'altGreeting',
                                     }
-                                }
+                                },
                             },
                             {
                                 'name': 'ENABLE_RISKY',
                                 'valueFrom': {
                                     'configMapKeyRef': {
                                         'name': 'the-map',
-                                        'key': 'enableRisky'
+                                        'key': 'enableRisky',
                                     }
-                                }
+                                },
                             },
                         ],
-                    }]
-            }
-        }
-    }
+                    }
+                ]
+            },
+        },
+    },
 }
```

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/simple_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict_defaults/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/attributes_as_dict/python/deployment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-deployment = {
-    'apiVersion': 'apps/v1',
-    'kind': 'Deployment',
-    'metadata': {'name': 'the-deployment'},
-    'spec': {
-        'replicas': 3,
-        'template': {
-            'metadata': {'labels': {'deployment': 'hello'}},
+class CustomDeployment:
+    def to_dict(self) -> dict:
+        return {
+            'apiVersion': 'apps/v1',
+            'kind': 'Deployment',
+            'metadata': {'name': 'the-deployment'},
             'spec': {
-                'containers': [
-                    {
-                        'name': 'the-container',
-                        'image': 'monopole/hello:1',
-                        'command': [
-                            '/hello',
-                            '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
-                        ],
-                        'ports': [{'containerPort': 8080}],
-                        'env': [
+                'replicas': 3,
+                'template': {
+                    'metadata': {'labels': {'deployment': 'hello'}},
+                    'spec': {
+                        'containers': [
                             {
-                                'name': 'ALT_GREETING',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'altGreeting'
-                                    }
-                                }
-                            },
-                            {
-                                'name': 'ENABLE_RISKY',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'enableRisky'
-                                    }
-                                }
-                            },
-                        ],
-                    }]
-            }
+                                'name': 'the-container',
+                                'image': 'monopole/hello:1',
+                                'command': [
+                                    '/hello',
+                                    '--port=8080',
+                                    '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                                ],
+                                'ports': [{'containerPort': 8080}],
+                                'env': [
+                                    {
+                                        'name': 'ALT_GREETING',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'altGreeting',
+                                            }
+                                        },
+                                    },
+                                    {
+                                        'name': 'ENABLE_RISKY',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'enableRisky',
+                                            }
+                                        },
+                                    },
+                                ],
+                            }
+                        ]
+                    },
+                },
+            },
         }
-    }
-}
+
+
+deployment = CustomDeployment()
```

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/simple_dict_defaults/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/python/deployments/deployment.py` & `kustomize-0.5.1/tests/fixtures/attrs/python/deployment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-my_deployment = {
-    'apiVersion': 'apps/v1',
-    'kind': 'Deployment',
-    'metadata': {'name': 'the-deployment'},
-    'spec': {
-        'replicas': 3,
-        'template': {
-            'metadata': {'labels': {'deployment': 'hello'}},
+class CustomDeployment:
+    def to_dict(self) -> dict:
+        return {
+            'apiVersion': 'apps/v1',
+            'kind': 'Deployment',
+            'metadata': {'name': 'the-deployment'},
             'spec': {
-                'containers': [
-                    {
-                        'name': 'the-container',
-                        'image': 'monopole/hello:1',
-                        'command': [
-                            '/hello',
-                            '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
-                        ],
-                        'ports': [{'containerPort': 8080}],
-                        'env': [
+                'replicas': 3,
+                'template': {
+                    'metadata': {'labels': {'deployment': 'hello'}},
+                    'spec': {
+                        'containers': [
                             {
-                                'name': 'ALT_GREETING',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'altGreeting'
-                                    }
-                                }
-                            },
-                            {
-                                'name': 'ENABLE_RISKY',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'enableRisky'
-                                    }
-                                }
-                            },
-                        ],
-                    }]
-            }
+                                'name': 'the-container',
+                                'image': 'monopole/hello:1',
+                                'command': [
+                                    '/hello',
+                                    '--port=8080',
+                                    '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                                ],
+                                'ports': [{'containerPort': 8080}],
+                                'env': [
+                                    {
+                                        'name': 'ALT_GREETING',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'altGreeting',
+                                            }
+                                        },
+                                    },
+                                    {
+                                        'name': 'ENABLE_RISKY',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'enableRisky',
+                                            }
+                                        },
+                                    },
+                                ],
+                            }
+                        ]
+                    },
+                },
+            },
         }
-    }
-}
+
+
+deployment = CustomDeployment()
```

### Comparing `kustomize-0.5.0/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/simple_dict_subdirs/reference/deployments/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/to_dict/python/configMap.py` & `kustomize-0.5.1/tests/fixtures/to_dict/python/configMap.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,16 +13,19 @@
 class ConfigMap:
     metadata: Metadata
     data: dict
     apiVersion: str = 'v1'
     kind: str = 'ConfigMap'
 
     def __init__(
-            self, metadata: Metadata, data: dict,
-            apiVersion: str = 'v1', kind: str = 'ConfigMap',
+        self,
+        metadata: Metadata,
+        data: dict,
+        apiVersion: str = 'v1',
+        kind: str = 'ConfigMap',
     ):
         self.metadata = metadata
         self.data = data
         self.apiVersion = apiVersion
         self.kind = kind
 
     def to_dict(self) -> dict:
```

### Comparing `kustomize-0.5.0/tests/fixtures/to_dict/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/kubernetes/python/deployment.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,39 +12,39 @@
                         'containers': [
                             {
                                 'name': 'the-container',
                                 'image': 'monopole/hello:1',
                                 'command': [
                                     '/hello',
                                     '--port=8080',
-                                    '--enableRiskyFeature=$('
-                                    'ENABLE_RISKY)',
+                                    '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
                                 ],
                                 'ports': [{'containerPort': 8080}],
                                 'env': [
                                     {
                                         'name': 'ALT_GREETING',
                                         'valueFrom': {
                                             'configMapKeyRef': {
                                                 'name': 'the-map',
-                                                'key': 'altGreeting'
+                                                'key': 'altGreeting',
                                             }
-                                        }
+                                        },
                                     },
                                     {
                                         'name': 'ENABLE_RISKY',
                                         'valueFrom': {
                                             'configMapKeyRef': {
                                                 'name': 'the-map',
-                                                'key': 'enableRisky'
+                                                'key': 'enableRisky',
                                             }
-                                        }
+                                        },
                                     },
                                 ],
-                            }]
-                    }
-                }
-            }
+                            }
+                        ]
+                    },
+                },
+            },
         }
 
 
 deployment = CustomDeployment()
```

### Comparing `kustomize-0.5.0/tests/fixtures/to_dict/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/to_dict/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/tuple_multiple/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/kubernetes11/python/deployment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-deployment = {
-    'apiVersion': 'apps/v1',
-    'kind': 'Deployment',
-    'metadata': {'name': 'the-deployment'},
-    'spec': {
-        'replicas': 3,
-        'template': {
-            'metadata': {'labels': {'deployment': 'hello'}},
+class CustomDeployment:
+    def to_dict(self) -> dict:
+        return {
+            'apiVersion': 'apps/v1',
+            'kind': 'Deployment',
+            'metadata': {'name': 'the-deployment'},
             'spec': {
-                'containers': [
-                    {
-                        'name': 'the-container',
-                        'image': 'monopole/hello:1',
-                        'command': [
-                            '/hello',
-                            '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
-                        ],
-                        'ports': [{'containerPort': 8080}],
-                        'env': [
+                'replicas': 3,
+                'template': {
+                    'metadata': {'labels': {'deployment': 'hello'}},
+                    'spec': {
+                        'containers': [
                             {
-                                'name': 'ALT_GREETING',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'altGreeting'
-                                    }
-                                }
-                            },
-                            {
-                                'name': 'ENABLE_RISKY',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'enableRisky'
-                                    }
-                                }
-                            },
-                        ],
-                    }]
-            }
+                                'name': 'the-container',
+                                'image': 'monopole/hello:1',
+                                'command': [
+                                    '/hello',
+                                    '--port=8080',
+                                    '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                                ],
+                                'ports': [{'containerPort': 8080}],
+                                'env': [
+                                    {
+                                        'name': 'ALT_GREETING',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'altGreeting',
+                                            }
+                                        },
+                                    },
+                                    {
+                                        'name': 'ENABLE_RISKY',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'enableRisky',
+                                            }
+                                        },
+                                    },
+                                ],
+                            }
+                        ]
+                    },
+                },
+            },
         }
-    }
-}
+
+
+deployment = CustomDeployment()
```

### Comparing `kustomize-0.5.0/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/tuple_multiple/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/python/deployment.py` & `kustomize-0.5.1/tests/fixtures/to_dict/python/deployment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-deployment = {
-    'apiVersion': 'apps/v1',
-    'kind': 'Deployment',
-    'metadata': {'name': 'the-deployment'},
-    'spec': {
-        'replicas': 3,
-        'template': {
-            'metadata': {'labels': {'deployment': 'hello'}},
+class CustomDeployment:
+    def to_dict(self) -> dict:
+        return {
+            'apiVersion': 'apps/v1',
+            'kind': 'Deployment',
+            'metadata': {'name': 'the-deployment'},
             'spec': {
-                'containers': [
-                    {
-                        'name': 'the-container',
-                        'image': 'monopole/hello:1',
-                        'command': [
-                            '/hello',
-                            '--port=8080',
-                            '--enableRiskyFeature=$('
-                            'ENABLE_RISKY)',
-                        ],
-                        'ports': [{'containerPort': 8080}],
-                        'env': [
+                'replicas': 3,
+                'template': {
+                    'metadata': {'labels': {'deployment': 'hello'}},
+                    'spec': {
+                        'containers': [
                             {
-                                'name': 'ALT_GREETING',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'altGreeting'
-                                    }
-                                }
-                            },
-                            {
-                                'name': 'ENABLE_RISKY',
-                                'valueFrom': {
-                                    'configMapKeyRef': {
-                                        'name': 'the-map',
-                                        'key': 'enableRisky'
-                                    }
-                                }
-                            },
-                        ],
-                    }]
-            }
+                                'name': 'the-container',
+                                'image': 'monopole/hello:1',
+                                'command': [
+                                    '/hello',
+                                    '--port=8080',
+                                    '--enableRiskyFeature=$(' 'ENABLE_RISKY)',
+                                ],
+                                'ports': [{'containerPort': 8080}],
+                                'env': [
+                                    {
+                                        'name': 'ALT_GREETING',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'altGreeting',
+                                            }
+                                        },
+                                    },
+                                    {
+                                        'name': 'ENABLE_RISKY',
+                                        'valueFrom': {
+                                            'configMapKeyRef': {
+                                                'name': 'the-map',
+                                                'key': 'enableRisky',
+                                            }
+                                        },
+                                    },
+                                ],
+                            }
+                        ]
+                    },
+                },
+            },
         }
-    }
-}
+
+
+deployment = CustomDeployment()
```

### Comparing `kustomize-0.5.0/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml` & `kustomize-0.5.1/tests/fixtures/tuple_multiple_attr/reference/deployment/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/test_generators.py` & `kustomize-0.5.1/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `kustomize-0.5.0/tests/test_main.py` & `kustomize-0.5.1/tests/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 def test_generates_simple_dict(cd_fixtures, create_build_path):
     fixtures_path = cd_fixtures('simple_dict')
     build_path = create_build_path()
     python_path = fixtures_path / 'python'
     reference_path = fixtures_path / 'reference'
 
     args = [
-        '--attr-name', 'my_kustomization',
+        '--attr-name',
+        'my_kustomization',
         str(python_path),
         str(build_path),
     ]
 
     run(args)
 
     assert_yaml_dirs_equal(build_path, reference_path)
@@ -22,15 +23,16 @@
 def test_generates_simple_dict_verbose(cd_fixtures, create_build_path):
     fixtures_path = cd_fixtures('simple_dict')
     build_path = create_build_path()
     python_path = fixtures_path / 'python'
     reference_path = fixtures_path / 'reference'
 
     args = [
-        '--attr-name', 'my_kustomization',
+        '--attr-name',
+        'my_kustomization',
         '--verbose',
         str(python_path),
         str(build_path),
     ]
 
     run(args)
 
@@ -40,15 +42,16 @@
 def test_generates_simple_dict_with_subdirs(cd_fixtures, create_build_path):
     fixtures_path = cd_fixtures('simple_dict_subdirs')
     build_path = create_build_path()
     python_path = fixtures_path / 'python'
     reference_path = fixtures_path / 'reference'
 
     args = [
-        '--attr-name', 'my_kustomization',
+        '--attr-name',
+        'my_kustomization',
         str(python_path),
         str(build_path),
     ]
 
     run(args)
 
     assert_yaml_dirs_equal(build_path, reference_path)
```

