# Comparing `tmp/pulumi_libvirt-0.4.6a1713332971.tar.gz` & `tmp/pulumi_libvirt-0.4.6a1713561081.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.4.6a1713332971.tar", last modified: Wed Apr 17 06:04:41 2024, max compression
+gzip compressed data, was "pulumi_libvirt-0.4.6a1713561081.tar", last modified: Fri Apr 19 21:14:00 2024, max compression
```

## Comparing `pulumi_libvirt-0.4.6a1713332971.tar` & `pulumi_libvirt-0.4.6a1713561081.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:04:41.015758 pulumi_libvirt-0.4.6a1713332971/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-17 06:04:41.015758 pulumi_libvirt-0.4.6a1713332971/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:04:41.011758 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51051 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:04:41.011758 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    89116 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)    34091 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    44490 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16188 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28668 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:04:41.015758 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-17 06:04:40.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-17 06:04:41.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:04:40.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-17 06:04:41.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-17 06:04:41.000000 pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-17 06:04:33.000000 pulumi_libvirt-0.4.6a1713332971/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 06:04:41.015758 pulumi_libvirt-0.4.6a1713332971/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50939 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89513 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34091 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44378 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28986 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/setup.cfg
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/PKG-INFO` & `pulumi_libvirt-0.4.6a1713561081/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.6a1713332971
+Version: 0.4.6a1713561081
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/README.md` & `pulumi_libvirt-0.4.6a1713561081/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,31 +216,37 @@
                
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
-               leap = libvirt.Volume("leap", source="http://someurl/openSUSE_Leap-42.1.qcow2")
-               mydisk = libvirt.Volume("mydisk", base_volume_id=leap.id)
-               domain1 = libvirt.Domain("domain1", disks=[
-                   libvirt.DomainDiskArgs(
-                       volume_id=mydisk.id,
-                       scsi=True,
-                   ),
-                   libvirt.DomainDiskArgs(
-                       url="http://foo.com/install.iso",
-                   ),
-                   libvirt.DomainDiskArgs(
-                       file="/absolute/path/to/disk.iso",
-                   ),
-                   libvirt.DomainDiskArgs(
-                       block_device="/dev/mapper/36005076802810e55400000000000145f",
-                   ),
-               ])
+               leap = libvirt.Volume("leap",
+                   name="leap",
+                   source="http://someurl/openSUSE_Leap-42.1.qcow2")
+               mydisk = libvirt.Volume("mydisk",
+                   name="mydisk",
+                   base_volume_id=leap.id)
+               domain1 = libvirt.Domain("domain1",
+                   name="domain1",
+                   disks=[
+                       libvirt.DomainDiskArgs(
+                           volume_id=mydisk.id,
+                           scsi=True,
+                       ),
+                       libvirt.DomainDiskArgs(
+                           url="http://foo.com/install.iso",
+                       ),
+                       libvirt.DomainDiskArgs(
+                           file="/absolute/path/to/disk.iso",
+                       ),
+                       libvirt.DomainDiskArgs(
+                           block_device="/dev/mapper/36005076802810e55400000000000145f",
+                       ),
+                   ])
                ```
                <!--End PulumiCodeChooser -->
                
                Also note that the `disk` block is actually a list of maps, so it is possible to
                declare several of them by using either the literal list and map syntax as in
                the following examples:
         """
@@ -329,31 +335,37 @@
 
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
-        leap = libvirt.Volume("leap", source="http://someurl/openSUSE_Leap-42.1.qcow2")
-        mydisk = libvirt.Volume("mydisk", base_volume_id=leap.id)
-        domain1 = libvirt.Domain("domain1", disks=[
-            libvirt.DomainDiskArgs(
-                volume_id=mydisk.id,
-                scsi=True,
-            ),
-            libvirt.DomainDiskArgs(
-                url="http://foo.com/install.iso",
-            ),
-            libvirt.DomainDiskArgs(
-                file="/absolute/path/to/disk.iso",
-            ),
-            libvirt.DomainDiskArgs(
-                block_device="/dev/mapper/36005076802810e55400000000000145f",
-            ),
-        ])
+        leap = libvirt.Volume("leap",
+            name="leap",
+            source="http://someurl/openSUSE_Leap-42.1.qcow2")
+        mydisk = libvirt.Volume("mydisk",
+            name="mydisk",
+            base_volume_id=leap.id)
+        domain1 = libvirt.Domain("domain1",
+            name="domain1",
+            disks=[
+                libvirt.DomainDiskArgs(
+                    volume_id=mydisk.id,
+                    scsi=True,
+                ),
+                libvirt.DomainDiskArgs(
+                    url="http://foo.com/install.iso",
+                ),
+                libvirt.DomainDiskArgs(
+                    file="/absolute/path/to/disk.iso",
+                ),
+                libvirt.DomainDiskArgs(
+                    block_device="/dev/mapper/36005076802810e55400000000000145f",
+                ),
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         Also note that the `disk` block is actually a list of maps, so it is possible to
         declare several of them by using either the literal list and map syntax as in
         the following examples:
         """
@@ -377,22 +389,14 @@
                where to mount the source.
         :param pulumi.Input[str] accessmode: specifies the security mode for accessing the source. By default
                the `mapped` mode is chosen.
         :param pulumi.Input[bool] readonly: enables exporting filesystem as a readonly mount for guest, by
                default read-only access is given.
                
                Example:
-               
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
-               ```
-               <!--End PulumiCodeChooser -->
-               
-               The exported filesystems can be mounted inside of the guest in this way:
         """
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "target", target)
         if accessmode is not None:
             pulumi.set(__self__, "accessmode", accessmode)
         if readonly is not None:
             pulumi.set(__self__, "readonly", readonly)
@@ -439,22 +443,14 @@
     @pulumi.getter
     def readonly(self) -> Optional[pulumi.Input[bool]]:
         """
         enables exporting filesystem as a readonly mount for guest, by
         default read-only access is given.
 
         Example:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
-        The exported filesystems can be mounted inside of the guest in this way:
         """
         return pulumi.get(self, "readonly")
 
     @readonly.setter
     def readonly(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "readonly", value)
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,17 +62,18 @@
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
-                   kernel=libvirt_volume["kernel"]["id"],
+                   kernel=kernel["id"],
                    cmdlines=[{
                        "arg1": "value1",
                        "arg2": "value2",
                        "_": "rw nosplash",
                    }])
                ```
                <!--End PulumiCodeChooser -->
@@ -116,21 +117,22 @@
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                kernel = libvirt.Volume("kernel",
                    source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+                   name="kernel",
                    pool="default",
                    format="raw")
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
                    kernel=kernel.id)
-               # ...
                ```
                <!--End PulumiCodeChooser -->
         :param pulumi.Input[str] machine: The machine type,
                you normally won't need to set this unless you are running on a platform that
                defaults to the wrong machine type for your template
         :param pulumi.Input[int] memory: The amount of memory in MiB. If not specified the domain
                will be created with 512 MiB of memory be used.
@@ -271,17 +273,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
-            kernel=libvirt_volume["kernel"]["id"],
+            kernel=kernel["id"],
             cmdlines=[{
                 "arg1": "value1",
                 "arg2": "value2",
                 "_": "rw nosplash",
             }])
         ```
         <!--End PulumiCodeChooser -->
@@ -453,21 +456,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         kernel = libvirt.Volume("kernel",
             source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+            name="kernel",
             pool="default",
             format="raw")
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
             kernel=kernel.id)
-        # ...
         ```
         <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "kernel")
 
     @kernel.setter
     def kernel(self, value: Optional[pulumi.Input[str]]):
@@ -678,17 +682,18 @@
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
-                   kernel=libvirt_volume["kernel"]["id"],
+                   kernel=kernel["id"],
                    cmdlines=[{
                        "arg1": "value1",
                        "arg2": "value2",
                        "_": "rw nosplash",
                    }])
                ```
                <!--End PulumiCodeChooser -->
@@ -732,21 +737,22 @@
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                kernel = libvirt.Volume("kernel",
                    source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+                   name="kernel",
                    pool="default",
                    format="raw")
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
                    kernel=kernel.id)
-               # ...
                ```
                <!--End PulumiCodeChooser -->
         :param pulumi.Input[str] machine: The machine type,
                you normally won't need to set this unless you are running on a platform that
                defaults to the wrong machine type for your template
         :param pulumi.Input[int] memory: The amount of memory in MiB. If not specified the domain
                will be created with 512 MiB of memory be used.
@@ -887,17 +893,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
-            kernel=libvirt_volume["kernel"]["id"],
+            kernel=kernel["id"],
             cmdlines=[{
                 "arg1": "value1",
                 "arg2": "value2",
                 "_": "rw nosplash",
             }])
         ```
         <!--End PulumiCodeChooser -->
@@ -1069,21 +1076,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         kernel = libvirt.Volume("kernel",
             source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+            name="kernel",
             pool="default",
             format="raw")
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
             kernel=kernel.id)
-        # ...
         ```
         <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "kernel")
 
     @kernel.setter
     def kernel(self, value: Optional[pulumi.Input[str]]):
@@ -1288,15 +1296,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
-        default = libvirt.Domain("default")
+        default = libvirt.Domain("default", name="test")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] arch: The architecture for the VM (probably x86_64 or i686),
                you normally won't need to set this unless you are building a special VM
@@ -1312,17 +1320,18 @@
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
-                   kernel=libvirt_volume["kernel"]["id"],
+                   kernel=kernel["id"],
                    cmdlines=[{
                        "arg1": "value1",
                        "arg2": "value2",
                        "_": "rw nosplash",
                    }])
                ```
                <!--End PulumiCodeChooser -->
@@ -1366,21 +1375,22 @@
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                kernel = libvirt.Volume("kernel",
                    source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+                   name="kernel",
                    pool="default",
                    format="raw")
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
                    kernel=kernel.id)
-               # ...
                ```
                <!--End PulumiCodeChooser -->
         :param pulumi.Input[str] machine: The machine type,
                you normally won't need to set this unless you are running on a platform that
                defaults to the wrong machine type for your template
         :param pulumi.Input[int] memory: The amount of memory in MiB. If not specified the domain
                will be created with 512 MiB of memory be used.
@@ -1411,15 +1421,15 @@
         ## Example Usage
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
-        default = libvirt.Domain("default")
+        default = libvirt.Domain("default", name="test")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param DomainArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
@@ -1564,17 +1574,18 @@
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
-                   kernel=libvirt_volume["kernel"]["id"],
+                   kernel=kernel["id"],
                    cmdlines=[{
                        "arg1": "value1",
                        "arg2": "value2",
                        "_": "rw nosplash",
                    }])
                ```
                <!--End PulumiCodeChooser -->
@@ -1618,21 +1629,22 @@
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                kernel = libvirt.Volume("kernel",
                    source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+                   name="kernel",
                    pool="default",
                    format="raw")
                domain_suse = libvirt.Domain("domain-suse",
+                   name="suse",
                    memory=1024,
                    vcpu=1,
                    kernel=kernel.id)
-               # ...
                ```
                <!--End PulumiCodeChooser -->
         :param pulumi.Input[str] machine: The machine type,
                you normally won't need to set this unless you are running on a platform that
                defaults to the wrong machine type for your template
         :param pulumi.Input[int] memory: The amount of memory in MiB. If not specified the domain
                will be created with 512 MiB of memory be used.
@@ -1732,17 +1744,18 @@
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
-            kernel=libvirt_volume["kernel"]["id"],
+            kernel=kernel["id"],
             cmdlines=[{
                 "arg1": "value1",
                 "arg2": "value2",
                 "_": "rw nosplash",
             }])
         ```
         <!--End PulumiCodeChooser -->
@@ -1866,21 +1879,22 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         kernel = libvirt.Volume("kernel",
             source="http://download.opensuse.org/tumbleweed/repo/oss/boot/x86_64/loader/linux",
+            name="kernel",
             pool="default",
             format="raw")
         domain_suse = libvirt.Domain("domain-suse",
+            name="suse",
             memory=1024,
             vcpu=1,
             kernel=kernel.id)
-        # ...
         ```
         <!--End PulumiCodeChooser -->
         """
         return pulumi.get(self, "kernel")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/network.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,31 +229,37 @@
                
                
                <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
-               leap = libvirt.Volume("leap", source="http://someurl/openSUSE_Leap-42.1.qcow2")
-               mydisk = libvirt.Volume("mydisk", base_volume_id=leap.id)
-               domain1 = libvirt.Domain("domain1", disks=[
-                   libvirt.DomainDiskArgs(
-                       volume_id=mydisk.id,
-                       scsi=True,
-                   ),
-                   libvirt.DomainDiskArgs(
-                       url="http://foo.com/install.iso",
-                   ),
-                   libvirt.DomainDiskArgs(
-                       file="/absolute/path/to/disk.iso",
-                   ),
-                   libvirt.DomainDiskArgs(
-                       block_device="/dev/mapper/36005076802810e55400000000000145f",
-                   ),
-               ])
+               leap = libvirt.Volume("leap",
+                   name="leap",
+                   source="http://someurl/openSUSE_Leap-42.1.qcow2")
+               mydisk = libvirt.Volume("mydisk",
+                   name="mydisk",
+                   base_volume_id=leap.id)
+               domain1 = libvirt.Domain("domain1",
+                   name="domain1",
+                   disks=[
+                       libvirt.DomainDiskArgs(
+                           volume_id=mydisk.id,
+                           scsi=True,
+                       ),
+                       libvirt.DomainDiskArgs(
+                           url="http://foo.com/install.iso",
+                       ),
+                       libvirt.DomainDiskArgs(
+                           file="/absolute/path/to/disk.iso",
+                       ),
+                       libvirt.DomainDiskArgs(
+                           block_device="/dev/mapper/36005076802810e55400000000000145f",
+                       ),
+                   ])
                ```
                <!--End PulumiCodeChooser -->
                
                Also note that the `disk` block is actually a list of maps, so it is possible to
                declare several of them by using either the literal list and map syntax as in
                the following examples:
         """
@@ -322,31 +328,37 @@
 
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
-        leap = libvirt.Volume("leap", source="http://someurl/openSUSE_Leap-42.1.qcow2")
-        mydisk = libvirt.Volume("mydisk", base_volume_id=leap.id)
-        domain1 = libvirt.Domain("domain1", disks=[
-            libvirt.DomainDiskArgs(
-                volume_id=mydisk.id,
-                scsi=True,
-            ),
-            libvirt.DomainDiskArgs(
-                url="http://foo.com/install.iso",
-            ),
-            libvirt.DomainDiskArgs(
-                file="/absolute/path/to/disk.iso",
-            ),
-            libvirt.DomainDiskArgs(
-                block_device="/dev/mapper/36005076802810e55400000000000145f",
-            ),
-        ])
+        leap = libvirt.Volume("leap",
+            name="leap",
+            source="http://someurl/openSUSE_Leap-42.1.qcow2")
+        mydisk = libvirt.Volume("mydisk",
+            name="mydisk",
+            base_volume_id=leap.id)
+        domain1 = libvirt.Domain("domain1",
+            name="domain1",
+            disks=[
+                libvirt.DomainDiskArgs(
+                    volume_id=mydisk.id,
+                    scsi=True,
+                ),
+                libvirt.DomainDiskArgs(
+                    url="http://foo.com/install.iso",
+                ),
+                libvirt.DomainDiskArgs(
+                    file="/absolute/path/to/disk.iso",
+                ),
+                libvirt.DomainDiskArgs(
+                    block_device="/dev/mapper/36005076802810e55400000000000145f",
+                ),
+            ])
         ```
         <!--End PulumiCodeChooser -->
 
         Also note that the `disk` block is actually a list of maps, so it is possible to
         declare several of them by using either the literal list and map syntax as in
         the following examples:
         """
@@ -366,22 +378,14 @@
                where to mount the source.
         :param str accessmode: specifies the security mode for accessing the source. By default
                the `mapped` mode is chosen.
         :param bool readonly: enables exporting filesystem as a readonly mount for guest, by
                default read-only access is given.
                
                Example:
-               
-               <!--Start PulumiCodeChooser -->
-               ```python
-               import pulumi
-               ```
-               <!--End PulumiCodeChooser -->
-               
-               The exported filesystems can be mounted inside of the guest in this way:
         """
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "target", target)
         if accessmode is not None:
             pulumi.set(__self__, "accessmode", accessmode)
         if readonly is not None:
             pulumi.set(__self__, "readonly", readonly)
@@ -416,22 +420,14 @@
     @pulumi.getter
     def readonly(self) -> Optional[bool]:
         """
         enables exporting filesystem as a readonly mount for guest, by
         default read-only access is given.
 
         Example:
-
-        <!--Start PulumiCodeChooser -->
-        ```python
-        import pulumi
-        ```
-        <!--End PulumiCodeChooser -->
-
-        The exported filesystems can be mounted inside of the guest in this way:
         """
         return pulumi.get(self, "readonly")
 
 
 @pulumi.output_type
 class DomainGraphics(dict):
     @staticmethod
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,17 +248,19 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # A pool for all cluster volumes
         cluster = libvirt.Pool("cluster",
+            name="cluster",
             type="dir",
             path="/home/user/cluster_storage")
-        opensuse_leap = libvirt.Volume("opensuseLeap",
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
             pool=cluster.name,
             source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
@@ -284,17 +286,19 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # A pool for all cluster volumes
         cluster = libvirt.Pool("cluster",
+            name="cluster",
             type="dir",
             path="/home/user/cluster_storage")
-        opensuse_leap = libvirt.Volume("opensuseLeap",
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
             pool=cluster.name,
             source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         ```
         <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param PoolArgs args: The arguments to use to populate this resource's properties.
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -357,21 +357,27 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # Base OS image to use to create a cluster of different
         # nodes
-        opensuse_leap = libvirt.Volume("opensuseLeap", source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
+            source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         # volume to attach to the "master" domain as main disk
-        master = libvirt.Volume("master", base_volume_id=opensuse_leap.id)
+        master = libvirt.Volume("master",
+            name="master.qcow2",
+            base_volume_id=opensuse_leap.id)
         # volumes to attach to the "workers" domains as main disk
         worker = []
-        for range in [{"value": i} for i in range(0, var.workers_count)]:
-            worker.append(libvirt.Volume(f"worker-{range['value']}", base_volume_id=opensuse_leap.id))
+        for range in [{"value": i} for i in range(0, workers_count)]:
+            worker.append(libvirt.Volume(f"worker-{range['value']}",
+                name=f"worker_{range['value']}.qcow2",
+                base_volume_id=opensuse_leap.id))
         ```
         <!--End PulumiCodeChooser -->
 
         > **Tip:** when provisioning multiple domains using the same base image, create
         a `Volume` for the base image and then define the domain specific ones
         as based on it. This way the image will not be modified and no extra disk space
         is going to be used for the base image.
@@ -410,21 +416,27 @@
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # Base OS image to use to create a cluster of different
         # nodes
-        opensuse_leap = libvirt.Volume("opensuseLeap", source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
+        opensuse_leap = libvirt.Volume("opensuse_leap",
+            name="opensuse_leap",
+            source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         # volume to attach to the "master" domain as main disk
-        master = libvirt.Volume("master", base_volume_id=opensuse_leap.id)
+        master = libvirt.Volume("master",
+            name="master.qcow2",
+            base_volume_id=opensuse_leap.id)
         # volumes to attach to the "workers" domains as main disk
         worker = []
-        for range in [{"value": i} for i in range(0, var.workers_count)]:
-            worker.append(libvirt.Volume(f"worker-{range['value']}", base_volume_id=opensuse_leap.id))
+        for range in [{"value": i} for i in range(0, workers_count)]:
+            worker.append(libvirt.Volume(f"worker-{range['value']}",
+                name=f"worker_{range['value']}.qcow2",
+                base_volume_id=opensuse_leap.id))
         ```
         <!--End PulumiCodeChooser -->
 
         > **Tip:** when provisioning multiple domains using the same base image, create
         a `Volume` for the base image and then define the domain specific ones
         as based on it. This way the image will not be modified and no extra disk space
         is going to be used for the base image.
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.6a1713332971
+Version: 0.4.6a1713561081
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.4.6a1713332971/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713332971/pyproject.toml` & `pulumi_libvirt-0.4.6a1713561081/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_libvirt"
   description = "A Pulumi package for creating and managing libvirt cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "libvirt"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.4.6a1713332971"
+  version = "0.4.6a1713561081"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-libvirt"
 
 [build-system]
```

