# Comparing `tmp/pulumi_kubernetes_cert_manager-0.0.5.tar.gz` & `tmp/pulumi_kubernetes_cert_manager-0.0.7a1713477261.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_cert_manager-0.0.5.tar", last modified: Wed Nov 23 23:58:41 2022, max compression
+gzip compressed data, was "pulumi_kubernetes_cert_manager-0.0.7a1713477261.tar", last modified: Thu Apr 18 22:00:11 2024, max compression
```

## Comparing `pulumi_kubernetes_cert_manager-0.0.5.tar` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 23:58:41.725685 pulumi_kubernetes_cert_manager-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-11-23 23:58:41.725685 pulumi_kubernetes_cert_manager-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1541 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 23:58:41.725685 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/
--rw-------   0 runner    (1001) docker     (121)      782 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/__init__.py
--rw-------   0 runner    (1001) docker     (121)    90881 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/_inputs.py
--rw-------   0 runner    (1001) docker     (121)     7647 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/_utilities.py
--rw-------   0 runner    (1001) docker     (121)    37571 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/cert_manager.py
--rw-------   0 runner    (1001) docker     (121)     3371 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/outputs.py
--rw-------   0 runner    (1001) docker     (121)     2832 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/provider.py
--rw-------   0 runner    (1001) docker     (121)       60 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (121)        0 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 23:58:41.725685 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 23:58:41.725685 pulumi_kubernetes_cert_manager-0.0.5/setup.cfg
--rw-------   0 runner    (1001) docker     (121)     2027 2022-11-23 23:58:41.000000 pulumi_kubernetes_cert_manager-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-18 22:00:11.605262 pulumi_kubernetes_cert_manager-0.0.7a1713477261/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-18 22:00:11.605262 pulumi_kubernetes_cert_manager-0.0.7a1713477261/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1541 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-18 22:00:11.605262 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/
+-rw-------   0 runner    (1000) runner    (1000)      782 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/__init__.py
+-rw-------   0 runner    (1000) runner    (1000)    90893 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/_inputs.py
+-rw-------   0 runner    (1000) runner    (1000)     9228 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/_utilities.py
+-rw-------   0 runner    (1000) runner    (1000)    37520 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/cert_manager.py
+-rw-------   0 runner    (1000) runner    (1000)     3383 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/outputs.py
+-rw-------   0 runner    (1000) runner    (1000)     2781 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/provider.py
+-rw-------   0 runner    (1000) runner    (1000)       60 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/pulumi-plugin.json
+-rw-------   0 runner    (1000) runner    (1000)        0 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/py.typed
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-04-18 22:00:11.605262 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1951 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      692 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1000) runner    (1000)       81 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       31 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-04-18 22:00:11.605262 pulumi_kubernetes_cert_manager-0.0.7a1713477261/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)     1427 2024-04-18 22:00:11.000000 pulumi_kubernetes_cert_manager-0.0.7a1713477261/setup.py
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_cert_manager
-Version: 0.0.5
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
+Version: 0.0.7a1713477261
+Summary: Strongly-typed Cert Manager installation
+Home-page: https://pulumi.io
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
 Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
-Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Pulumi Cert Manager Component
 
 This repo contains the Pulumi Cert Manager component for Kubernetes. This add-on automates the
 management and issuance of TLS certificates from various issuing sources. It ensures certificates
 are valid and up to date periodically, and attempts to renew certificates at an appropriate time
@@ -35,9 +36,7 @@
 
 The Helm deployment uses reasonable defaults, including the chart name and repo URL, however,
 if you need to override them, you may do so using the `helmOptions` parameter. Refer to
 [the API docs for the `kubernetes:helm/v3:Release` Pulumi type](
 https://www.pulumi.com/docs/reference/pkg/kubernetes/helm/v3/release/#inputs) for a full set of choices.
 
 For complete details, refer to the Pulumi Package details within the Pulumi Registry.
-
-
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/README.md` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/__init__.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/_inputs.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 import pulumi_kubernetes
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/_utilities.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/_utilities.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 
+import asyncio
+import importlib.metadata
 import importlib.util
 import inspect
 import json
 import os
-import pkg_resources
 import sys
 import typing
 
 import pulumi
 import pulumi.runtime
+from pulumi.runtime.sync_await import _sync_await
 
 from semver import VersionInfo as SemverVersion
 from parver import Version as PEP440Version
 
 
 def get_env(*args):
     for v in args:
@@ -66,15 +68,15 @@
     # pkg_resources uses setuptools to inspect the set of installed packages. We use it here to ask
     # for the currently installed version of the root package (i.e. us) and get its version.
 
     # Unfortunately, PEP440 and semver differ slightly in incompatible ways. The Pulumi engine expects
     # to receive a valid semver string when receiving requests from the language host, so it's our
     # responsibility as the library to convert our own PEP440 version into a valid semver string.
 
-    pep440_version_string = pkg_resources.require(root_package)[0].version
+    pep440_version_string = importlib.metadata.version(root_package)
     pep440_version = PEP440Version.parse(pep440_version_string)
     (major, minor, patch) = pep440_version.release
     prerelease = None
     if pep440_version.pre_tag == 'a':
         prerelease = f"alpha.{pep440_version.pre}"
     elif pep440_version.pre_tag == 'b':
         prerelease = f"beta.{pep440_version.pre}"
@@ -94,14 +96,25 @@
 _version = _get_semver_version()
 _version_str = str(_version)
 
 
 def get_version():
     return _version_str
 
+def get_resource_opts_defaults() -> pulumi.ResourceOptions:
+    return pulumi.ResourceOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
+
+def get_invoke_opts_defaults() -> pulumi.InvokeOptions:
+    return pulumi.InvokeOptions(
+        version=get_version(),
+        plugin_download_url=get_plugin_download_url(),
+    )
 
 def get_resource_args_opts(resource_args_type, resource_options_type, *args, **kwargs):
     """
     Return the resource args and options given the *args and **kwargs of a resource's
     __init__ method.
     """
 
@@ -230,7 +243,49 @@
             'args': args_list,
             'kwargs': bound_args.kwargs
         }).apply(lambda resolved_args: func(*resolved_args['args'],
                                             opts=opts,
                                             **resolved_args['kwargs']))
 
     return (lambda _: lifted_func)
+
+
+def call_plain(
+    tok: str,
+    props: pulumi.Inputs,
+    res: typing.Optional[pulumi.Resource] = None,
+    typ: typing.Optional[type] = None,
+) -> typing.Any:
+    """
+    Wraps pulumi.runtime.plain to force the output and return it plainly.
+    """
+
+    output = pulumi.runtime.call(tok, props, res, typ)
+
+    # Ingoring deps silently. They are typically non-empty, r.f() calls include r as a dependency.
+    result, known, secret, _ = _sync_await(asyncio.ensure_future(_await_output(output)))
+
+    problem = None
+    if not known:
+        problem = ' an unknown value'
+    elif secret:
+        problem = ' a secret value'
+
+    if problem:
+        raise AssertionError(
+            f"Plain resource method '{tok}' incorrectly returned {problem}. "
+            + "This is an error in the provider, please report this to the provider developer."
+        )
+
+    return result
+
+
+async def _await_output(o: pulumi.Output[typing.Any]) -> typing.Tuple[object, bool, bool, set]:
+    return (
+        await o._future,
+        await o._is_known,
+        await o._is_secret,
+        await o._resources,
+    )
+
+def get_plugin_download_url():
+	return None
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/cert_manager.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/cert_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 from ._inputs import *
@@ -585,20 +586,17 @@
                  service_annotations: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  service_labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  startupapicheck: Optional[pulumi.Input[pulumi.InputType['CertManagerStartupAPICheckArgs']]] = None,
                  strategy: Optional[pulumi.Input[pulumi.InputType['pulumi_kubernetes.apps.v1.DeploymentStrategyArgs']]] = None,
                  tolerations: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_kubernetes.core.v1.TolerationArgs']]]]] = None,
                  webhook: Optional[pulumi.Input[pulumi.InputType['CertManagerWebhookArgs']]] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CertManagerArgs.__new__(CertManagerArgs)
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/outputs.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager/provider.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding=utf-8
 # *** WARNING: this file was generated by Pulumi SDK Generator. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
+import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = ['ProviderArgs', 'Provider']
@@ -50,20 +51,17 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  __props__=None):
-        if opts is None:
-            opts = pulumi.ResourceOptions()
+        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.version is None:
-            opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ProviderArgs.__new__(ProviderArgs)
 
         super(Provider, __self__).__init__(
             'kubernetes-cert-manager',
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pulumi-kubernetes-cert-manager
-Version: 0.0.5
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
+Version: 0.0.7a1713477261
+Summary: Strongly-typed Cert Manager installation
+Home-page: https://pulumi.io
+License: Apache-2.0
+Project-URL: Repository, https://github.com/pulumi/pulumi-kubernetes-cert-manager
 Keywords: pulumi kubernetes cert-manager kind/component category/infrastructure
-Platform: UNKNOWN
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Pulumi Cert Manager Component
 
 This repo contains the Pulumi Cert Manager component for Kubernetes. This add-on automates the
 management and issuance of TLS certificates from various issuing sources. It ensures certificates
 are valid and up to date periodically, and attempts to renew certificates at an appropriate time
@@ -35,9 +36,7 @@
 
 The Helm deployment uses reasonable defaults, including the chart name and repo URL, however,
 if you need to override them, you may do so using the `helmOptions` parameter. Refer to
 [the API docs for the `kubernetes:helm/v3:Release` Pulumi type](
 https://www.pulumi.com/docs/reference/pkg/kubernetes/helm/v3/release/#inputs) for a full set of choices.
 
 For complete details, refer to the Pulumi Package details within the Pulumi Registry.
-
-
```

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/pulumi_kubernetes_cert_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_cert_manager-0.0.5/setup.py` & `pulumi_kubernetes_cert_manager-0.0.7a1713477261/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,58 +4,42 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.0.5"
-PLUGIN_VERSION = "0.0.5"
-
-class InstallPluginCommand(install):
-    def run(self):
-        install.run(self)
-        try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'kubernetes-cert-manager', PLUGIN_VERSION])
-        except OSError as error:
-            if error.errno == errno.ENOENT:
-                print(f"""
-                There was an error installing the kubernetes-cert-manager resource provider plugin.
-                It looks like `pulumi` is not installed on your system.
-                Please visit https://pulumi.com/ to install the Pulumi CLI.
-                You may try manually installing the plugin by running
-                `pulumi plugin install resource kubernetes-cert-manager {PLUGIN_VERSION}`
-                """)
-            else:
-                raise
-
-
+VERSION = "0.0.7a1713477261"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "kubernetes-cert-manager Pulumi Package - Development Version"
 
 
 setup(name='pulumi_kubernetes_cert_manager',
+      python_requires='>=3.8',
       version=VERSION,
+      description="Strongly-typed Cert Manager installation",
       long_description=readme(),
       long_description_content_type='text/markdown',
-      cmdclass={
-          'install': InstallPluginCommand,
-      },
       keywords='pulumi kubernetes cert-manager kind/component category/infrastructure',
+      url='https://pulumi.io',
+      project_urls={
+          'Repository': 'https://github.com/pulumi/pulumi-kubernetes-cert-manager'
+      },
+      license='Apache-2.0',
       packages=find_packages(),
       package_data={
           'pulumi_kubernetes_cert_manager': [
               'py.typed',
               'pulumi-plugin.json',
           ]
       },
       install_requires=[
           'parver>=0.2.1',
           'pulumi>=3.0.0,<4.0.0',
-          'pulumi-kubernetes>=3.7.1,<4.0.0',
+          'pulumi-kubernetes>=3.7.1,<5.0.0',
           'semver>=2.8.1'
       ],
       zip_safe=False)
```

