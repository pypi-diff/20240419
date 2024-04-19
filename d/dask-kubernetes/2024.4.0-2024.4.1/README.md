# Comparing `tmp/dask-kubernetes-2024.4.0.tar.gz` & `tmp/dask-kubernetes-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2024.4.0.tar", last modified: Tue Apr  2 13:09:22 2024, max compression
+gzip compressed data, was "dask-kubernetes-2024.4.1.tar", last modified: Fri Apr 19 12:37:21 2024, max compression
```

## Comparing `dask-kubernetes-2024.4.0.tar` & `dask-kubernetes-2024.4.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:21.996817 dask-kubernetes-2024.4.0/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29927 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:21.996817 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.004818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.008818 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/dask_kubernetes/operator/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:09:22.000818 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 13:09:21.000000 dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-02 13:09:22.012817 dask-kubernetes-2024.4.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-02 13:09:11.000000 dask-kubernetes-2024.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.277413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/versioneer.py
```

### Comparing `dask-kubernetes-2024.4.0/LICENSE` & `dask-kubernetes-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/PKG-INFO` & `dask-kubernetes-2024.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
@@ -37,15 +37,15 @@
    :target: https://pypi.org/project/dask-kubernetes/
    :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
    :target: https://anaconda.org/conda-forge/dask-kubernetes
    :alt: Conda Forge
 
-.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11-blue
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11%7C3.12-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Python Support
 
 .. image:: https://img.shields.io/badge/Kubernetes%20support-1.26%7C1.27%7C1.28%7C1.29-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Kubernetes Support
```

### Comparing `dask-kubernetes-2024.4.0/README.rst` & `dask-kubernetes-2024.4.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    :target: https://pypi.org/project/dask-kubernetes/
    :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
    :target: https://anaconda.org/conda-forge/dask-kubernetes
    :alt: Conda Forge
 
-.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11-blue
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11%7C3.12-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Python Support
 
 .. image:: https://img.shields.io/badge/Kubernetes%20support-1.26%7C1.27%7C1.28%7C1.29-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Kubernetes Support
```

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/__init__.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/auth.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/networking.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/objects.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/common/utils.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/conftest.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 ),
                 namespace=self.namespace,
             )
         assert len(services) == 1
         return services[0]
 
     async def ready(self) -> bool:
-        await self._refresh()
+        await self.async_refresh()
         return (
             "status" in self.raw
             and "phase" in self.status
             and self.status.phase == "Running"
         )
```

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from datetime import datetime
 from uuid import uuid4
 
 import aiohttp
 import dask.config
 import kopf
 import kr8s
+import pkg_resources
 from distributed.core import clean_exception, rpc
 from distributed.protocol.pickle import dumps
-from importlib_metadata import entry_points
 from kr8s.asyncio.objects import Deployment, Pod, Service
 
 from dask_kubernetes.common.objects import validate_cluster_name
 from dask_kubernetes.constants import SCHEDULER_NAME_TEMPLATE
 from dask_kubernetes.exceptions import ValidationError
 from dask_kubernetes.operator._objects import (
     DaskAutoscaler,
@@ -34,15 +34,15 @@
 
 KUBERNETES_DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 DASK_AUTOSCALER_COOLDOWN_UNTIL_ANNOTATION = "kubernetes.dask.org/cooldown-until"
 
 # Load operator plugins from other packages
 PLUGINS = []
-for ep in entry_points(group="dask_operator_plugin"):
+for ep in pkg_resources.iter_entry_points(group="dask_operator_plugin"):
     with suppress(AttributeError, ImportError):
         PLUGINS.append(ep.load())
 
 
 class SchedulerCommError(Exception):
     """Raised when unable to communicate with a scheduler."""
 
@@ -193,25 +193,27 @@
         "metadata": {
             "name": get_job_runner_pod_name(job_name),
             "labels": labels,
             "annotations": annotations,
         },
         "spec": copy.deepcopy(spec),
     }
-    env = [
-        {
-            "name": "DASK_SCHEDULER_ADDRESS",
-            "value": f"tcp://{cluster_name}-scheduler.{namespace}.svc.cluster.local:8786",
-        },
-    ]
+    scheduler_env = {
+        "name": "DASK_SCHEDULER_ADDRESS",
+        "value": f"tcp://{cluster_name}-scheduler.{namespace}.svc.cluster.local:8786",
+    }
     for container in pod_spec["spec"]["containers"]:
-        if "env" in container:
-            container["env"].extend(env)
-        else:
-            container["env"] = env
+        if "env" not in container:
+            container["env"] = [scheduler_env]
+            continue
+
+        container_env_names = [env_item["name"] for env_item in container["env"]]
+
+        if "DASK_SCHEDULER_ADDRESS" not in container_env_names:
+            container["env"].append(scheduler_env)
     return pod_spec
 
 
 def build_default_worker_group_spec(cluster_name, spec, annotations, labels):
     labels.update(
         **{
             "dask.org/cluster-name": cluster_name,
@@ -845,20 +847,21 @@
         logger.debug(
             "Not autoscaling %s with %d workers", spec["cluster"], current_replicas
         )
 
 
 @kopf.timer("daskcluster.kubernetes.dask.org", interval=5.0)
 async def daskcluster_autoshutdown(spec, name, namespace, logger, **kwargs):
-    if spec["idleTimeout"]:
+    idle_timeout = spec.get("idleTimeout", 0)
+    if idle_timeout:
         try:
             idle_since = await check_scheduler_idle(
                 scheduler_service_name=f"{name}-scheduler",
                 namespace=namespace,
                 logger=logger,
             )
         except Exception:
             logger.warn("Unable to connect to scheduler, skipping autoshutdown check.")
             return
-        if idle_since and time.time() > idle_since + spec["idleTimeout"]:
+        if idle_since and time.time() > idle_since + idle_timeout:
             cluster = await DaskCluster.get(name, namespace=namespace)
             await cluster.delete()
```

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes/operator/networking.py` & `dask-kubernetes-2024.4.1/dask_kubernetes/operator/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
@@ -37,15 +37,15 @@
    :target: https://pypi.org/project/dask-kubernetes/
    :alt: PyPI
 
 .. image:: https://img.shields.io/conda/vn/conda-forge/dask-kubernetes
    :target: https://anaconda.org/conda-forge/dask-kubernetes
    :alt: Conda Forge
 
-.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11-blue
+.. image:: https://img.shields.io/badge/python%20support-3.9%7C3.10%7C3.11%7C3.12-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Python Support
 
 .. image:: https://img.shields.io/badge/Kubernetes%20support-1.26%7C1.27%7C1.28%7C1.29-blue
    :target: https://kubernetes.dask.org/en/latest/installing.html#supported-versions
    :alt: Kubernetes Support
```

### Comparing `dask-kubernetes-2024.4.0/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/pyproject.toml` & `dask-kubernetes-2024.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/setup.cfg` & `dask-kubernetes-2024.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/setup.py` & `dask-kubernetes-2024.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.0/versioneer.py` & `dask-kubernetes-2024.4.1/versioneer.py`

 * *Files identical despite different names*

