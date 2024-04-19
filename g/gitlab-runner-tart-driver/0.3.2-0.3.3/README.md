# Comparing `tmp/gitlab-runner-tart-driver-0.3.2.tar.gz` & `tmp/gitlab-runner-tart-driver-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-runner-tart-driver-0.3.2.tar", last modified: Wed Mar 27 21:25:28 2024, max compression
+gzip compressed data, was "gitlab-runner-tart-driver-0.3.3.tar", last modified: Fri Apr 19 07:03:59 2024, max compression
```

## Comparing `gitlab-runner-tart-driver-0.3.2.tar` & `gitlab-runner-tart-driver-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.427528 gitlab-runner-tart-driver-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)     3303 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    20705 2024-03-27 21:25:28.427528 gitlab-runner-tart-driver-0.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    20007 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.422528 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.425528 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1422 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/config.py
--rw-rw-rw-   0 root         (0) root         (0)    10487 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/prepare.py
--rw-rw-rw-   0 root         (0) root         (0)     2235 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.426528 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3086 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9677 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/tart.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.426528 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     2533 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 21:25:28.426528 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/
--rw-r--r--   0 root         (0) root         (0)    20705 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       72 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-27 21:25:28.000000 gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 21:25:28.427528 gitlab-runner-tart-driver-0.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-27 21:25:19.000000 gitlab-runner-tart-driver-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.376450 gitlab-runner-tart-driver-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)     3303 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    20705 2024-04-19 07:03:59.375450 gitlab-runner-tart-driver-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    20007 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.371450 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.373450 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1422 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10487 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/prepare.py
+-rw-rw-rw-   0 root         (0) root         (0)     2235 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.374450 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3086 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/gitlab_custom_driver_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9914 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/tart.py
+-rw-rw-rw-   0 root         (0) root         (0)      923 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.375450 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     2533 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-19 07:03:59.375450 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    20705 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       72 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-19 07:03:59.000000 gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       31 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-19 07:03:59.376450 gitlab-runner-tart-driver-0.3.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-04-19 07:03:50.000000 gitlab-runner-tart-driver-0.3.3/setup.py
```

### Comparing `gitlab-runner-tart-driver-0.3.2/LICENSE.txt` & `gitlab-runner-tart-driver-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/PKG-INFO` & `gitlab-runner-tart-driver-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.3.2/README.md` & `gitlab-runner-tart-driver-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/cli.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/cli.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/cleanup.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/cleanup.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/config.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/prepare.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/commands/run.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/commands/run.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/gitlab_custom_command_config.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/tart.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/tart.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 class TartVmSpec(BaseModel):
     cpu_count: int
     memory: int
     disk: int
     display: str
     running: bool
     ip_address: str
+    os: str
+    size: str
 
 
 class TartVolume(BaseModel):
     name: str
     source: str
     dest: str
     ro: bool = Field(default=False)
@@ -122,51 +124,61 @@
 
     def get(self, name) -> TartVmSpec:
         specs = self.exec(["get", name])
 
         # 'spec' will look like this:
         #
         # tart version < 2.7
-        #    CPU Memory Disk Display  Running
-        #    4   8192   46   1024x768 true
+        # CPU Memory Disk Display  Running
+        # 4   8192   46   1024x768 true
         #
         # tart version > 2.6
         # CPU Memory Disk Size   Display  State
         # 4   8192   50   20.794 1024x768 running
+        #
+        # tart version > 2.8
+        # OS     CPU Memory Disk Size   Display  State
+        # darwin 4   8192   50   22.294 1024x768 stopped
+
+        # Read headers
+        headers = specs.split("\n")[0]
+        header_elements = headers.split(" ")
+        header_elements = [s.strip().lower() for s in header_elements if s]
 
-        spec_line = specs.split("\n")[1]
-        spec_elements = spec_line.split(" ")
+        spec = specs.split("\n")[1]
+        spec_elements = spec.split(" ")
         spec_elements = [s.strip() for s in spec_elements if s]
 
-        # old version
-        if len(spec_elements) == 5:
-            spec = TartVmSpec(
-                cpu_count=int(spec_elements[0]),
-                memory=int(spec_elements[1]),
-                disk=int(spec_elements[2]),
-                display=spec_elements[3],
-                running=True if spec_elements[4].lower() == "true" else False,
-                ip_address="n/a",
-            )
-        elif len(spec_elements) == 6:
-            spec = TartVmSpec(
-                cpu_count=int(spec_elements[0]),
-                memory=int(spec_elements[1]),
-                disk=int(spec_elements[2]),
-                display=spec_elements[4],
-                running=True if spec_elements[5].lower() == "running" else False,
-                ip_address="n/a",
-            )
+        specs = {}
+        for i, spec_element in enumerate(spec_elements):
+            specs[header_elements[i]] = spec_element
+
+        # check the state of the machine
+        vm_state = specs.get("state", "n/a")
+        running = True
+        if vm_state == "running" or vm_state == "true":
+            running = True
         else:
-            raise ValueError("cloud not determine vm specs")
+            running = False
+
+        vm_spec = TartVmSpec(
+            cpu_count=int(specs.get("cpu", 0)),
+            memory=int(specs.get("memory", 0)),
+            disk=int(specs.get("disk", 0)),
+            display=specs.get("display", "n/a"),
+            running=running,
+            ip_address="n/a",
+            os=specs.get("os", "n/a"),
+            size=specs.get("size", "n/a"),
+        )
 
-        if spec.running:
-            spec.ip_address = self.ip(name)
+        if vm_spec.running:
+            vm_spec.ip_address = self.ip(name)
 
-        return spec
+        return vm_spec
 
     def print_spec(self, name, tablefmt="fancy_grid"):
         spec = self.get(name)
         data = [
             (str(spec.cpu_count), str(spec.memory), str(spec.disk), spec.display, str(spec.running), spec.ip_address)
         ]
         print(tabulate(data, headers=["CPU", "Memory", "Disk", "Display", "Running", "IP Address"], tablefmt=tablefmt))
```

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/modules/utils.py` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/modules/utils.py`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver/scripts/install-gitlab-runner.sh.j2`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/PKG-INFO` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-runner-tart-driver
-Version: 0.3.2
+Version: 0.3.3
 Home-page: https://gitlab.com/schmieder.matthias/gitlab-runner-tart-driver
 Author: Matthias Schmieder
 Author-email: schmieder.matthias@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
```

### Comparing `gitlab-runner-tart-driver-0.3.2/gitlab_runner_tart_driver.egg-info/SOURCES.txt` & `gitlab-runner-tart-driver-0.3.3/gitlab_runner_tart_driver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlab-runner-tart-driver-0.3.2/setup.py` & `gitlab-runner-tart-driver-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 
 # read the long description from README.md
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-version = "0.3.2"
+version = "0.3.3"
 
 version = f"{version}{os.environ.get('PIP_VERSION_POSTFIX','')}"
 
 # read the requirements from requirements.txt
 requirements = []
 with pathlib.Path("requirements.txt").open() as requirements_txt:
     requirements = [str(requirement) for requirement in pkg_resources.parse_requirements(requirements_txt)]
```

