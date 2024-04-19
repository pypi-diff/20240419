# Comparing `tmp/wiremind-kubernetes-7.4.1.tar.gz` & `tmp/wiremind_kubernetes-7.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiremind-kubernetes-7.4.1.tar", last modified: Thu Nov 23 15:40:42 2023, max compression
+gzip compressed data, was "wiremind_kubernetes-7.4.2.tar", last modified: Fri Apr 19 13:58:01 2024, max compression
```

## Comparing `wiremind-kubernetes-7.4.1.tar` & `wiremind_kubernetes-7.4.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.538147 wiremind-kubernetes-7.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-11-23 15:40:42.538147 wiremind-kubernetes-7.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      489 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-11-23 15:40:42.538147 wiremind-kubernetes-7.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.526147 wiremind-kubernetes-7.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.530146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kube_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    20016 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kubernetes_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.530146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.534146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.534146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.534146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4348 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3887 2023-11-23 15:40:32.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 15:40:42.534146 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 15:40:42.000000 wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.697150 wiremind_kubernetes-7.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 13:58:01.697150 wiremind_kubernetes-7.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 13:58:01.697150 wiremind_kubernetes-7.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.685150 wiremind_kubernetes-7.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.689150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20036 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kubernetes_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.689150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.693150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.693150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.693150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3887 2024-04-19 13:57:57.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:58:01.693150 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:58:01.000000 wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/zip-safe
```

### Comparing `wiremind-kubernetes-7.4.1/LICENCE.md` & `wiremind_kubernetes-7.4.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/PKG-INFO` & `wiremind_kubernetes-7.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.4.1
+Version: 7.4.2
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.4.1/README.md` & `wiremind_kubernetes-7.4.2/README.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/setup.cfg` & `wiremind_kubernetes-7.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/setup.py` & `wiremind_kubernetes-7.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/exceptions.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kube_config.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/kubernetes_helper.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/kubernetes_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     A simple helper for Kubernetes manipulation.
     """
 
     SCALE_DOWN_MAX_WAIT_TIME = 3600
 
     def __init__(
         self,
-        use_kubeconfig: bool = False,
+        use_kubeconfig: Optional[bool] = False,
         dry_run: bool = False,
         pretty: bool = True,
         should_load_kubernetes_config: bool = True,
         context: Optional[str] = None,
     ):
         """
         :param use_kubeconfig:
@@ -82,15 +82,15 @@
 class NamespacedKubernetesHelper(KubernetesHelper):
     """
     A simple helper for Kubernetes manipulation.
     """
 
     def __init__(
         self,
-        use_kubeconfig: bool = False,
+        use_kubeconfig: Optional[bool] = False,
         namespace: Union[None, str] = None,
         dry_run: bool = False,
         should_load_kubernetes_config: bool = True,
         context: Optional[str] = None,
     ):
         """
         :param use_kubeconfig:
```

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/conftest.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/helpers.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes/utils.py` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/PKG-INFO` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.4.1
+Version: 7.4.2
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.4.1/src/wiremind_kubernetes.egg-info/SOURCES.txt` & `wiremind_kubernetes-7.4.2/src/wiremind_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

