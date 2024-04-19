# Comparing `tmp/paka-0.1.3.tar.gz` & `tmp/paka-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.3.tar", max compression
+gzip compressed data, was "paka-0.1.4.tar", max compression
```

## Comparing `paka-0.1.3.tar` & `paka-0.1.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1072 2024-04-18 06:53:43.507527 paka-0.1.3/LICENSE
--rw-r--r--   0        0        0     4570 2024-04-18 06:53:43.507527 paka-0.1.3/README.md
--rw-r--r--   0        0        0      153 2024-04-18 06:53:43.511527 paka-0.1.3/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/build.py
--rw-r--r--   0        0        0     3263 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/cluster.py
--rw-r--r--   0        0        0     6726 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/function.py
--rw-r--r--   0        0        0     5910 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2233 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/run.py
--rw-r--r--   0        0        0     8815 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    12154 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1468 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1874 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/keda.py
--rw-r--r--   0        0        0     4956 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2773 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/namespace.py
--rw-r--r--   0        0        0     3414 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/nvidia_device_plugin.py
--rw-r--r--   0        0        0     4273 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-18 06:53:43.511527 paka-0.1.3/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    15395 2024-04-18 06:53:43.511527 paka-0.1.3/paka/config.py
--rw-r--r--   0        0        0      115 2024-04-18 06:53:43.511527 paka-0.1.3/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-04-18 06:53:43.511527 paka-0.1.3/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-04-18 06:53:43.511527 paka-0.1.3/paka/container/pack.py
--rw-r--r--   0        0        0    19188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5742 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     2048 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0    10074 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/model.py
--rw-r--r--   0        0        0    17498 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0     1105 2024-04-18 06:53:43.511527 paka-0.1.3/paka/kube_resources/model_group/supported_models.py
--rw-r--r--   0        0        0      761 2024-04-18 06:53:43.511527 paka-0.1.3/paka/logger.py
--rw-r--r--   0        0        0        0 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/__init__.py
--rw-r--r--   0        0        0     3188 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/base_model.py
--rw-r--r--   0        0        0     2473 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/hf_model.py
--rw-r--r--   0        0        0     1485 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/http_model.py
--rw-r--r--   0        0        0     1648 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/manifest.py
--rw-r--r--   0        0        0     2374 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/progress_bar.py
--rw-r--r--   0        0        0     2671 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/settings.py
--rw-r--r--   0        0        0     9467 2024-04-18 06:53:43.511527 paka-0.1.3/paka/model/store.py
--rw-r--r--   0        0        0     9786 2024-04-18 06:53:43.511527 paka-0.1.3/paka/utils.py
--rw-r--r--   0        0        0     1459 2024-04-18 06:53:43.511527 paka-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5830 1970-01-01 00:00:00.000000 paka-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-19 04:36:42.330546 paka-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4570 2024-04-19 04:36:42.330546 paka-0.1.4/README.md
+-rw-r--r--   0        0        0      153 2024-04-19 04:36:42.334546 paka-0.1.4/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/build.py
+-rw-r--r--   0        0        0     3891 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6726 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/function.py
+-rw-r--r--   0        0        0     5910 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/job.py
+-rw-r--r--   0        0        0      427 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2233 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/run.py
+-rw-r--r--   0        0        0     8815 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12154 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1468 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1932 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4956 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2773 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3414 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4273 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     4000 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-19 04:36:42.334546 paka-0.1.4/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    15395 2024-04-19 04:36:42.334546 paka-0.1.4/paka/config.py
+-rw-r--r--   0        0        0      115 2024-04-19 04:36:42.334546 paka-0.1.4/paka/constants.py
+-rw-r--r--   0        0        0     3015 2024-04-19 04:36:42.334546 paka-0.1.4/paka/container/ecr.py
+-rw-r--r--   0        0        0     2374 2024-04-19 04:36:42.334546 paka-0.1.4/paka/container/pack.py
+-rw-r--r--   0        0        0    19188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/k8s.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/function/__init__.py
+-rw-r--r--   0        0        0     5742 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/autoscaler.py
+-rw-r--r--   0        0        0     4142 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/__init__.py
+-rw-r--r--   0        0        0     2048 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/manifest.py
+-rw-r--r--   0        0        0    10074 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/model.py
+-rw-r--r--   0        0        0    17498 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/service.py
+-rw-r--r--   0        0        0     1105 2024-04-19 04:36:42.334546 paka-0.1.4/paka/kube_resources/model_group/supported_models.py
+-rw-r--r--   0        0        0      761 2024-04-19 04:36:42.334546 paka-0.1.4/paka/logger.py
+-rw-r--r--   0        0        0        0 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/__init__.py
+-rw-r--r--   0        0        0     3188 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/base_model.py
+-rw-r--r--   0        0        0     2473 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/hf_model.py
+-rw-r--r--   0        0        0     1485 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/http_model.py
+-rw-r--r--   0        0        0     1648 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/manifest.py
+-rw-r--r--   0        0        0     2565 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/progress_bar.py
+-rw-r--r--   0        0        0     2671 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/settings.py
+-rw-r--r--   0        0        0     9467 2024-04-19 04:36:42.334546 paka-0.1.4/paka/model/store.py
+-rw-r--r--   0        0        0     9786 2024-04-19 04:36:42.334546 paka-0.1.4/paka/utils.py
+-rw-r--r--   0        0        0     1456 2024-04-19 04:36:42.334546 paka-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5816 1970-01-01 00:00:00.000000 paka-0.1.4/PKG-INFO
```

### Comparing `paka-0.1.3/LICENSE` & `paka-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/README.md` & `paka-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/__main__.py` & `paka-0.1.4/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/build.py` & `paka-0.1.4/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/cluster.py` & `paka-0.1.4/paka/cli/cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,25 +63,29 @@
     Tears down the Kubernetes cluster, removing all associated resources and data.
     """
     if yes or click.confirm(
         f"Are you sure you want to proceed with the operation? Please note that "
         "all resources and data will be permanently deleted.",
         default=False,
     ):
-        # Sometime finalizers might block CRD deletion, so we need to force delete those
-        # TODO: better way to handle this
-        remove_crd_finalizers(
-            "scaledobjects.keda.sh",
-        )
-        remove_crd_finalizers(
-            "routes.serving.knative.dev",
-        )
-        remove_crd_finalizers(
-            "ingresses.networking.internal.knative.dev",
-        )
+        try:
+            # Sometime finalizers might block CRD deletion, so we need to force delete those.
+            # This is best effort and might not work in all cases.
+            # TODO: better way to handle this
+            remove_crd_finalizers(
+                "scaledobjects.keda.sh",
+            )
+            remove_crd_finalizers(
+                "routes.serving.knative.dev",
+            )
+            remove_crd_finalizers(
+                "ingresses.networking.internal.knative.dev",
+            )
+        except Exception:
+            pass
 
         cluster_manager = load_cluster_manager(cluster_config)
         cluster_manager.destroy()
 
 
 @cluster_app.command()
 def preview(
@@ -103,7 +107,24 @@
     Previews the changes that will be applied to the cloud resources.
     """
     cluster_manager = load_cluster_manager(cluster_config)
     if policy_packs:
         cluster_manager.preview(policy_packs=policy_packs)
     else:
         cluster_manager.preview()
+
+
+@cluster_app.command()
+def refresh(
+    cluster_config: str = typer.Option(
+        "",
+        "--file",
+        "-f",
+        help="Path to the cluster config file. The cluster config file is a "
+        "YAML file that contains the configuration of the cluster",
+    ),
+) -> None:
+    """
+    Synchronize the local cluster state with the state in the cloud.
+    """
+    cluster_manager = load_cluster_manager(cluster_config)
+    cluster_manager.refresh()
```

### Comparing `paka-0.1.3/paka/cli/function.py` & `paka-0.1.4/paka/cli/function.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/job.py` & `paka-0.1.4/paka/cli/job.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/model_group.py` & `paka-0.1.4/paka/cli/model_group.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/run.py` & `paka-0.1.4/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cli/utils.py` & `paka-0.1.4/paka/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/cloudwatch.py` & `paka-0.1.4/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.4/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/container_registry.py` & `paka-0.1.4/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.4/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/eks.py` & `paka-0.1.4/paka/cluster/aws/eks.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/elb.py` & `paka-0.1.4/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/object_store.py` & `paka-0.1.4/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/service_account.py` & `paka-0.1.4/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/aws/utils.py` & `paka-0.1.4/paka/cluster/aws/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import pulumi
 import pulumi_aws as aws
 import pulumi_eks as eks
 
 from paka.config import CloudConfig
 
 
 def odic_role_for_sa(
@@ -20,35 +21,40 @@
         ns_service_account (str): The name of the service account. e.g. "default:sa", "kube-system:auto-scaler"
 
     Returns:
         aws.iam.Role: The IAM role for the service account.
     """
     project = config.cluster.name
 
+    oidc_url = cluster.core.oidc_provider.url
+    oidc_arn = cluster.core.oidc_provider.arn
+
+    assume_role_policy = pulumi.Output.all(oidc_url, oidc_arn).apply(
+        lambda args: aws.iam.get_policy_document(
+            statements=[
+                aws.iam.GetPolicyDocumentStatementArgs(
+                    effect="Allow",
+                    principals=[
+                        aws.iam.GetPolicyDocumentStatementPrincipalArgs(
+                            type="Federated",
+                            identifiers=[str(args[1])],
+                        )
+                    ],
+                    actions=["sts:AssumeRoleWithWebIdentity"],
+                    conditions=[
+                        aws.iam.GetPolicyDocumentStatementConditionArgs(
+                            test="StringEquals",
+                            variable=f"{args[0]}:sub",
+                            values=[f"system:serviceaccount:{ns_service_account}"],
+                        )
+                    ],
+                )
+            ],
+        ).json
+    )
+
     role = aws.iam.Role(
         f"{project}-{role_name}-role",
-        assume_role_policy=cluster.core.oidc_provider.url.apply(
-            lambda url: aws.iam.get_policy_document(
-                statements=[
-                    aws.iam.GetPolicyDocumentStatementArgs(
-                        effect="Allow",
-                        principals=[
-                            aws.iam.GetPolicyDocumentStatementPrincipalArgs(
-                                type="Federated",
-                                identifiers=[cluster.core.oidc_provider.arn],
-                            )
-                        ],
-                        actions=["sts:AssumeRoleWithWebIdentity"],
-                        conditions=[
-                            aws.iam.GetPolicyDocumentStatementConditionArgs(
-                                test="StringEquals",
-                                variable=f"{url}:sub",
-                                values=[f"system:serviceaccount:{ns_service_account}"],
-                            )
-                        ],
-                    )
-                ],
-            ).json
-        ),
+        assume_role_policy=assume_role_policy,
     )
 
     return role
```

### Comparing `paka-0.1.3/paka/cluster/fluentbit.py` & `paka-0.1.4/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/keda.py` & `paka-0.1.4/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/knative.py` & `paka-0.1.4/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/manager/aws.py` & `paka-0.1.4/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/manager/base.py` & `paka-0.1.4/paka/cluster/manager/base.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/namespace.py` & `paka-0.1.4/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/nvidia_device_plugin.py` & `paka-0.1.4/paka/cluster/nvidia_device_plugin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/prometheus.py` & `paka-0.1.4/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/qdrant.py` & `paka-0.1.4/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/redis.py` & `paka-0.1.4/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/cluster/zipkin.py` & `paka-0.1.4/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/config.py` & `paka-0.1.4/paka/config.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/container/ecr.py` & `paka-0.1.4/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/container/pack.py` & `paka-0.1.4/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/k8s.py` & `paka-0.1.4/paka/k8s.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/function/service.py` & `paka-0.1.4/paka/kube_resources/function/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/job/autoscaler.py` & `paka-0.1.4/paka/kube_resources/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/job/worker.py` & `paka-0.1.4/paka/kube_resources/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/model_group/ingress.py` & `paka-0.1.4/paka/kube_resources/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/model_group/model.py` & `paka-0.1.4/paka/kube_resources/model_group/model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/model_group/service.py` & `paka-0.1.4/paka/kube_resources/model_group/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/kube_resources/model_group/supported_models.py` & `paka-0.1.4/paka/kube_resources/model_group/supported_models.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/logger.py` & `paka-0.1.4/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/base_model.py` & `paka-0.1.4/paka/model/base_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/hf_model.py` & `paka-0.1.4/paka/model/hf_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/http_model.py` & `paka-0.1.4/paka/model/http_model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/manifest.py` & `paka-0.1.4/paka/model/manifest.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/progress_bar.py` & `paka-0.1.4/paka/model/progress_bar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 from threading import Lock
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
 from tqdm import tqdm
 
 
 class ProgressBar:
     def __init__(self, message: str = "Downloading") -> None:
         self.counter: Dict[str, int] = {}
         self.lock = Lock()
-        self.progress_bar: tqdm = None
+        self.progress_bar: Optional[tqdm] = None
         self.completed_files: List[Tuple[str, str]] = []
         self.message = message
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self.progress_bar, name)
 
     def set_postfix_str(self, *args: Any, **kwargs: Any) -> None:
+        if self.progress_bar is None:
+            return
         self.progress_bar.set_postfix_str(*args, **kwargs)
 
     def clear_counter(self) -> None:
         with self.lock:
             self.counter = {}
 
     def create_progress_bar(self, total_size: int) -> None:
@@ -41,20 +43,24 @@
             if self.progress_bar is not None:
                 # Increase the total count of the progress bar by the provided value
                 self.progress_bar.total += value
                 # Refresh the progress bar to reflect the new total
                 self.progress_bar.refresh()
 
     def close_progress_bar(self) -> None:
+        if self.progress_bar is None:
+            return
         with self.lock:
             self.counter = {}
             self.progress_bar.close()
             self.progress_bar = None
 
     def advance_progress_bar(self, key: str = "", value: int = 0) -> None:
+        if self.progress_bar is None:
+            return
         with self.lock:
             if key:
                 self.counter[key] = value
             # Calculate the total progress by summing the progress of all tasks
             total_progress = sum(self.counter.values())
             # Update the progress bar by the amount of progress made since the last update
             self.progress_bar.update(total_progress - self.progress_bar.n)
```

### Comparing `paka-0.1.3/paka/model/settings.py` & `paka-0.1.4/paka/model/settings.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/model/store.py` & `paka-0.1.4/paka/model/store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/paka/utils.py` & `paka-0.1.4/paka/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.3/pyproject.toml` & `paka-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.3"
+version = "0.1.4"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
 
@@ -24,22 +24,22 @@
 ]
 
 [tool.poetry.scripts]
 paka = "paka.cli.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = { extras = ["mypy"], version = "^2.7.0" }
+pydantic = "^2.7.0"
 ruamel-yaml = "^0.18.6"
-pulumi = "^3.113.0"
+pulumi = "3.105.0"
 pulumi-aws = "^6.31.0"
 typer = "^0.12.3"
 pulumi-eks = "^2.3.0"
 pulumi-awsx = "^2.7.0"
-pulumi-kubernetes = "^4.10.0"
+pulumi-kubernetes = "^4.8.1"
 pathspec = "^0.12.1"
 requests = "^2.31.0"
 kubernetes = "^29.0.0"
 boto3 = "^1.34.86"
 tabulate = "^0.9.0"
 huggingface-hub = "^0.22.2"
 tqdm = "^4.66.2"
@@ -52,12 +52,13 @@
 pytest = "^8.1.1"
 pytest-snapshot = "^0.9.0"
 types-requests = "2.31.0.6"
 isort = "^5.13.2"
 types-tabulate = "^0.9.0.20240106"
 pulumi-policy = "^1.11.0"
 moto = "^5.0.5"
-boto3-stubs = { extras = ["s3"], version = "^1.34.86" }
+boto3-stubs = { extras = ["s3"], version = "^1.34.87" }
+types-tqdm = "^4.66.0.20240417"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `paka-0.1.3/PKG-INFO` & `paka-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.3
+Version: 0.1.4
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.86,<2.0.0)
 Requires-Dist: huggingface-hub (>=0.22.2,<0.23.0)
 Requires-Dist: kubernetes (>=29.0.0,<30.0.0)
 Requires-Dist: pathspec (>=0.12.1,<0.13.0)
-Requires-Dist: pulumi (>=3.113.0,<4.0.0)
+Requires-Dist: pulumi (==3.105.0)
 Requires-Dist: pulumi-aws (>=6.31.0,<7.0.0)
 Requires-Dist: pulumi-awsx (>=2.7.0,<3.0.0)
 Requires-Dist: pulumi-eks (>=2.3.0,<3.0.0)
-Requires-Dist: pulumi-kubernetes (>=4.10.0,<5.0.0)
-Requires-Dist: pydantic[mypy] (>=2.7.0,<3.0.0)
+Requires-Dist: pulumi-kubernetes (>=4.8.1,<5.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruamel-yaml (>=0.18.6,<0.19.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: typer (>=0.12.3,<0.13.0)
 Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
```

