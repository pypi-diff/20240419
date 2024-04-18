# Comparing `tmp/zetaforge-0.1.1.tar.gz` & `tmp/zetaforge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zetaforge-0.1.1.tar", last modified: Mon Apr  8 19:11:46 2024, max compression
+gzip compressed data, was "zetaforge-0.1.2.tar", last modified: Thu Apr 18 21:39:05 2024, max compression
```

## Comparing `zetaforge-0.1.1.tar` & `zetaforge-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 19:11:46.793562 zetaforge-0.1.1/
--rw-r--r--   0 jon        (501) staff       (20)    34523 2024-04-08 18:07:53.000000 zetaforge-0.1.1/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-08 19:11:46.793425 zetaforge-0.1.1/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     4843 2024-04-08 18:10:41.000000 zetaforge-0.1.1/README.md
--rw-r--r--   0 jon        (501) staff       (20)      104 2024-04-08 18:08:45.000000 zetaforge-0.1.1/pyproject.toml
--rw-r--r--   0 jon        (501) staff       (20)       38 2024-04-08 19:11:46.793605 zetaforge-0.1.1/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)     1805 2024-04-08 18:44:22.000000 zetaforge-0.1.1/setup.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 19:11:46.791773 zetaforge-0.1.1/zetaforge/
--rw-r--r--   0 jon        (501) staff       (20)       22 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)     1617 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/check_forge_dependencies.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 19:11:46.792677 zetaforge-0.1.1/zetaforge/executables/
--rw-r--r--   0 jon        (501) staff       (20)      122 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/executables/README.md
--rw-r--r--   0 jon        (501) staff       (20)     3391 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/forge_cli.py
--rw-r--r--   0 jon        (501) staff       (20)    14283 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/forge_runner.py
--rw-r--r--   0 jon        (501) staff       (20)    11862 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/install_forge_dependencies.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 19:11:46.792962 zetaforge-0.1.1/zetaforge/utils/
--rw-r--r--   0 jon        (501) staff       (20)     2959 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/utils/build.yaml
--rw-r--r--   0 jon        (501) staff       (20)    37294 2024-04-08 18:08:45.000000 zetaforge-0.1.1/zetaforge/utils/install.yaml
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-08 19:11:46.792569 zetaforge-0.1.1/zetaforge.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      478 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       55 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/entry_points.txt
--rw-r--r--   0 jon        (501) staff       (20)       76 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       10 2024-04-08 19:11:46.000000 zetaforge-0.1.1/zetaforge.egg-info/top_level.txt
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.144678 zetaforge-0.1.2/
+-rw-r--r--   0 jon        (501) staff       (20)    34523 2024-04-08 18:07:53.000000 zetaforge-0.1.2/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-18 21:39:05.144558 zetaforge-0.1.2/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     5695 2024-04-10 16:47:21.000000 zetaforge-0.1.2/README.md
+-rw-r--r--   0 jon        (501) staff       (20)      104 2024-04-08 19:29:07.000000 zetaforge-0.1.2/pyproject.toml
+-rw-r--r--   0 jon        (501) staff       (20)       38 2024-04-18 21:39:05.144725 zetaforge-0.1.2/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)     1844 2024-04-18 20:56:32.000000 zetaforge-0.1.2/setup.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.142507 zetaforge-0.1.2/zetaforge/
+-rw-r--r--   0 jon        (501) staff       (20)       22 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge/__init__.py
+-rw-r--r--   0 jon        (501) staff       (20)     1657 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/check_forge_dependencies.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143305 zetaforge-0.1.2/zetaforge/executables/
+-rw-r--r--   0 jon        (501) staff       (20)      122 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/executables/README.md
+-rw-r--r--   0 jon        (501) staff       (20)     3389 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/forge_cli.py
+-rw-r--r--   0 jon        (501) staff       (20)    13795 2024-04-18 20:56:35.000000 zetaforge-0.1.2/zetaforge/forge_runner.py
+-rw-r--r--   0 jon        (501) staff       (20)    11862 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/install_forge_dependencies.py
+-rw-r--r--   0 jon        (501) staff       (20)     1504 2024-04-18 20:56:32.000000 zetaforge-0.1.2/zetaforge/mixpanel_client.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143840 zetaforge-0.1.2/zetaforge/utils/
+-rw-r--r--   0 jon        (501) staff       (20)     3003 2024-04-10 16:47:21.000000 zetaforge-0.1.2/zetaforge/utils/build.yaml
+-rw-r--r--   0 jon        (501) staff       (20)    37294 2024-04-08 19:29:07.000000 zetaforge-0.1.2/zetaforge/utils/install.yaml
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2024-04-18 21:39:05.143174 zetaforge-0.1.2/zetaforge.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)      212 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)      507 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)       55 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (501) staff       (20)      126 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       10 2024-04-18 21:39:05.000000 zetaforge-0.1.2/zetaforge.egg-info/top_level.txt
```

### Comparing `zetaforge-0.1.1/LICENSE` & `zetaforge-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zetaforge-0.1.1/README.md` & `zetaforge-0.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -64,25 +64,48 @@
 
 You need to install Docker Desktop or any other container runtime that includes Kubernetes integration.
 Follow the instructions to [install Docker Desktop](https://docs.docker.com/desktop/) from their official website.
 You will need to [enable Kubernetes](https://docs.docker.com/desktop/kubernetes/) to use ZetaForge.
 
 > Note: We recommend [OrbStack](https://orbstack.dev/download) to macOS users for efficiency and performance reasons.
 
+## Launch ZetaForge
+
+To launch ZetaForge, run the following command after installing via pip:
+```
+zetaforge launch
+```
+
+This will set up the correct services in Kubernetes, check that they are running, and then launch ZetaForge. 
+
+If something goes wrong, you can run:
+
+```
+zetaforge setup
+```
+
+to reconfigure the container services. 
+
+To teardown and remove the Kubernetes services, you can run:
+
+```
+zetaforge teardown
+```
+
 
 ## Run your First Pipeline
 
 ![Demo Pipeline](assets/quick-start.gif)
 
 To experience ZetaForge in action, start by dragging and dropping a core pipeline, such as the "Canny Edge Pipeline," from the Core Pipelines Library into your workspace. Once the pipeline is loaded, click the "Run" button to see the magic happen!
 
 
 ## Documentation
 
-Explore our [official documentation](https://zetane.com/docs) for a guide on using ZetaForge. Learn how to create your own ZetaForge blocks, assemble custom pipelines, and more. You'll also find tutorials and best practices to enhance your ZetaForge experience.
+Explore our [official documentation](https://zetane.com/docs/) for a guide on using ZetaForge. Learn how to create your own ZetaForge blocks, assemble custom pipelines, and more. You'll also find tutorials and best practices to enhance your ZetaForge experience.
 
 
 ## Pipeline Gallery
 
 **Visualize Multidimensional Numpy Arrays**
 
 ![Pipeline Screenshot Numpy](assets/numpy-visualization.png)
@@ -103,14 +126,23 @@
 
 1. **Save:** Go to `File` -> `Save` or `Save As`, choose a target folder, and name your pipeline.
 2. **Package and Send:** Zip the saved folder, which contains all necessary files, and share it with your team.
 3. **Load and Run:** Team members can unzip the folder, load the pipeline via `File` -> `Load` -> `Pipeline`, and click `Run` to replicate the results.
 
 This streamlined process ensures easy sharing and consistent results across your team.
 
+
+## Contributing
+
+ZetaForge is under active development. We welcome contributions from the community to make our project even better! 
+
+Before contributing, please take a moment to review our [Contribution Guide](CONTRIBUTING.md) to see our guidelines.
+Whether it's improving documentations, reporting bugs, suggesting new features, or submitting code changes, 
+your contributions help us improve the project for everyone. 
+
 ## License
 
 - **[AGPL license](https://opensource.org/license/agpl-v3/)**
 - If you need another type of license please contact us [here](https://zetane.com/contact-us).
 
 ## Contact
```

### Comparing `zetaforge-0.1.1/setup.py` & `zetaforge-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from setuptools import setup, find_packages
-import os
 import json
+import os
+
+from setuptools import find_packages, setup
 
 version = {}
 with open("zetaforge/__init__.py") as fp:
     exec(fp.read(), version)
 
 def get_package_version():
     # Specify the path to the package.json file
@@ -43,17 +44,16 @@
         'console_scripts': [
             'zetaforge = zetaforge.forge_cli:main'
         ]
     },
     packages=find_packages(include=('zetaforge',)),
     python_requires='>=3.7',
     install_requires = [
-        'setuptools',
-        'requests', 
-        'boto3', 
-        'colorama', 
+        'setuptools==69.0.2',
+        'requests==2.31.0', 
+        'boto3==1.34.79', 
+        'colorama==0.4.6', 
         'mixpanel==4.10.1', 
-        "langchain", 
-        "openai", 
-        "pyyaml"],
+        "langchain==0.1.15", 
+        "langchain-openai==0.1.2"],
     include_package_data=True,
     package_data={'zetaforge': ['utils/*.yaml', 'executables/*'],},)
```

### Comparing `zetaforge-0.1.1/zetaforge/check_forge_dependencies.py` & `zetaforge-0.1.2/zetaforge/check_forge_dependencies.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 def check_kubectl():
     check_ctl = subprocess.run(["kubectl", "version", "--client"], capture_output=True, text=True)
     return check_ctl.returncode == 0
 
 def check_running_kube(context):
     check_kube = subprocess.run(["kubectl", f"--context={context}", "get", "pods"], capture_output=True, text=True)
     if check_kube.returncode == 0:
-        print("Kube check pods: ", check_kube.stdout)
+        print("Kubernetes is running, continuing..")
         return True
     else:
-        print("Kube check pods: ", check_kube.stderr)
+        print("Kubernetes is not running!  ", check_kube.returncode)
+        print(check_kube.stderr)
         return False
 
 def check_kube_pod(name):
     check_kube = subprocess.run(["kubectl", "get", "pods"], capture_output=True, text=True)
     lines = check_kube.stdout.strip().split("\n")[1:]  # Skip the header line
     for line in lines:
         parts = line.split("-")
@@ -38,10 +39,8 @@
         if platform.system() == 'Windows':
             print("https://docs.docker.com/desktop/install/windows-install/")
         elif platform.system() == 'Darwin':
             print("https://docs.docker.com/desktop/install/mac-install/")
         else:
             print("https://docs.docker.com/desktop/install/linux-install/")
         return -1
-    return 0
-    
-
+    return 0
```

### Comparing `zetaforge-0.1.1/zetaforge/forge_cli.py` & `zetaforge-0.1.2/zetaforge/forge_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,9 +61,8 @@
                 config = json.load(file)
                 return config
         except (IOError, json.JSONDecodeError) as e:
             print("Error loading configuration file:", str(e))
     return None
 
 if __name__ == "__main__":
-    main()
-
+    main()
```

### Comparing `zetaforge-0.1.1/zetaforge/forge_runner.py` & `zetaforge-0.1.2/zetaforge/forge_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 import json
 from pkg_resources import resource_filename
 from .check_forge_dependencies import check_dependencies, check_running_kube, check_kube_pod
 from .install_forge_dependencies import *
 from pathlib import Path
 from colorama import init, Fore
 from datetime import datetime
-import mixpanel
 import socket, errno
-import uuid
-from hashlib import sha256
 import json
 import shutil
 import yaml 
 import threading
+from .mixpanel_client import MixpanelClient
+
+
+mixpanel_client = MixpanelClient('4c09914a48f08de1dbe3dc4dd2dcf90d')
 
-mixpanel_token = '4c09914a48f08de1dbe3dc4dd2dcf90d'
-mixpanel_instance = mixpanel.Mixpanel(mixpanel_token)
 
 BUILD_YAML = resource_filename("zetaforge", os.path.join('utils', 'build.yaml'))
 INSTALL_YAML = resource_filename("zetaforge", os.path.join('utils', 'install.yaml'))
 
 EXECUTABLES_PATH = os.path.join(Path(__file__).parent, 'executables')
 FRONT_END = os.path.join(EXECUTABLES_PATH, "frontend")
 
@@ -225,18 +224,15 @@
         print("Registry container not found, restarting..")
         setup(server_version, client_version)
         raise Exception("Container registry is not running, please ensure kubernetes is running or re-run `zetaforge setup`.")
     weed = check_kube_pod("weed")
     if not weed:
         raise Exception("SeaweedFS is not running, please ensure kubernetes is running or re-run `zetaforge setup`.")
 
-    #mixpanel_instance.track(distinct_id,'Initial Launch')
-    distinct_id = generate_distinct_id()
-    #added this for funnel reviews(for e.g., user Launched and after created a run, loaded a pipeline etc.)
-    mixpanel_instance.track(distinct_id, "Initial Launch", {})
+    mixpanel_client.track_event('Initial Launch')
 
     if server_path is None:
         _, server_path = get_launch_paths(server_version, client_version)
 
     if client_path is None:
         client_path, _ = get_launch_paths(server_version, client_version)
 
@@ -245,23 +241,23 @@
         client = None
         print(f"Launching execution server {server_path}..")
         server_executable = os.path.basename(server_path)
         if platform.system() != 'Windows':
             server_executable = f"./{server_executable}"
         else:
             server_executable = server_path
-
+        
         server = subprocess.Popen([server_executable],stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(server_path))
 
         print(f"Launching client {client_path}..")
         client_executable = os.path.basename(client_path)
         if platform.system() == 'Darwin':
             client_executable = [f"./{client_executable}"]
         elif platform.system() == 'Windows':
-            client_executable = [client_path]
+            client_executable = [client_path, '--no-sandbox']
         else: 
             client_executable = [f"./{client_executable}"]
 
         client = subprocess.Popen(client_executable, stdout=subprocess.PIPE, stderr=subprocess.PIPE, cwd=os.path.dirname(client_path))
 
         def read_output(process, name):
             for line in process.stdout:
@@ -290,18 +286,18 @@
         client_stderr_thread.join()
 
     except KeyboardInterrupt: 
         print("Terminating servers..")
 
     finally:
         total_time = (datetime.now() - time_start).total_seconds()
-        distinct_id = generate_distinct_id()
+       
 
         try:
-            mixpanel_instance.track(distinct_id,'Full Launch', {'Duration(seconds)': total_time})
+            mixpanel_client.track_event('Full Launch', props={'Duration(seconds)': total_time})
             time.sleep(2) # mixpanel instance is asynch, so making sure that it completes the call before tear down
         except:
             print("Mixpanel cannot track")
 
         server.kill()
         client.kill()
 
@@ -371,18 +367,8 @@
         }
     } 
 
     file_path = os.path.join(s2_path, "config.json")
     with open(file_path, "w") as outfile: 
         json.dump(config, outfile)
 
-    return file_path
-
-def generate_distinct_id():
-    seed = 0
-    try:
-        seed = uuid.getnode()
-    except:
-        seed = 0
-        
-    distinct_id = sha256(str(seed).encode('utf-8')).hexdigest()
-    return distinct_id
+    return file_path
```

### Comparing `zetaforge-0.1.1/zetaforge/install_forge_dependencies.py` & `zetaforge-0.1.2/zetaforge/install_forge_dependencies.py`

 * *Files identical despite different names*

### Comparing `zetaforge-0.1.1/zetaforge/utils/build.yaml` & `zetaforge-0.1.2/zetaforge/utils/build.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -128,12 +128,14 @@
         - containerPort: 5000
 ---
 apiVersion: v1
 kind: Service
 metadata:
   name: registry
 spec:
+  loadBalancerIP: null
   ports:
   - port: 5000
     targetPort: 5000
   selector:
     app.kubernetes.io/name: registry
+  type: LoadBalancer
```

### Comparing `zetaforge-0.1.1/zetaforge/utils/install.yaml` & `zetaforge-0.1.2/zetaforge/utils/install.yaml`

 * *Files identical despite different names*

