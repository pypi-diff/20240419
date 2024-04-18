# Comparing `tmp/qwrapper-0.1.14.tar.gz` & `tmp/qwrapper-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwrapper-0.1.14.tar", last modified: Thu Apr 18 17:31:18 2024, max compression
+gzip compressed data, was "qwrapper-0.1.15.tar", last modified: Thu Apr 18 22:03:57 2024, max compression
```

## Comparing `qwrapper-0.1.14.tar` & `qwrapper-0.1.15.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:18.908493 qwrapper-0.1.14/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:14.000000 qwrapper-0.1.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 17:31:18.908493 qwrapper-0.1.14/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      792 2024-04-18 17:31:14.000000 qwrapper-0.1.14/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-04-18 17:31:14.000000 qwrapper-0.1.14/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:18.904493 qwrapper-0.1.14/qwrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/qemumachine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:18.908493 qwrapper-0.1.14/qwrapper/x86/
--rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:18.908493 qwrapper-0.1.14/qwrapper/x86/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/utils/debugging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/utils/machinestate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/utils/memory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/utils/registers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3642 2024-04-18 17:31:14.000000 qwrapper-0.1.14/qwrapper/x86/x86machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 17:31:18.908493 qwrapper-0.1.14/qwrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-18 17:31:18.000000 qwrapper-0.1.14/qwrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 17:31:18.000000 qwrapper-0.1.14/qwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 17:31:18.000000 qwrapper-0.1.14/qwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 17:31:18.000000 qwrapper-0.1.14/qwrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 17:31:18.908493 qwrapper-0.1.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:57.596451 qwrapper-0.1.15/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1130 2024-04-18 22:03:53.000000 qwrapper-0.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 22:03:57.596451 qwrapper-0.1.15/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-04-18 22:03:53.000000 qwrapper-0.1.15/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      586 2024-04-18 22:03:53.000000 qwrapper-0.1.15/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:57.592451 qwrapper-0.1.15/qwrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       38 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/qemumachine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:57.596451 qwrapper-0.1.15/qwrapper/x86/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       34 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:57.596451 qwrapper-0.1.15/qwrapper/x86/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/utils/debugging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1041 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/utils/machinestate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/utils/memory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2432 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/utils/registers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3976 2024-04-18 22:03:53.000000 qwrapper-0.1.15/qwrapper/x86/x86machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 22:03:57.596451 qwrapper-0.1.15/qwrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-18 22:03:57.000000 qwrapper-0.1.15/qwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-18 22:03:57.000000 qwrapper-0.1.15/qwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 22:03:57.000000 qwrapper-0.1.15/qwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 22:03:57.000000 qwrapper-0.1.15/qwrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 22:03:57.596451 qwrapper-0.1.15/setup.cfg
```

### Comparing `qwrapper-0.1.14/pyproject.toml` & `qwrapper-0.1.15/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 [project]
 license = { file = "LICENSE" }
 name = "qwrapper"
-version = "0.1.14"
+version = "0.1.15"
 description = "A QEMU wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [{ name = "Daniel Dybing", email = "danieldy@uia.no" },
            { name = "Ali Sirvanovitsj Ismailov", email = "alisi18@uia.no"},
            { name = "Sirén Elise Lund Lohre", email = "selohre@uia.no"}]
 classifiers = [
```

### Comparing `qwrapper-0.1.14/qwrapper/qemumachine.py` & `qwrapper-0.1.15/qwrapper/qemumachine.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.14/qwrapper/x86/utils/machinestate.py` & `qwrapper-0.1.15/qwrapper/x86/utils/machinestate.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.14/qwrapper/x86/utils/memory.py` & `qwrapper-0.1.15/qwrapper/x86/utils/memory.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.14/qwrapper/x86/utils/registers.py` & `qwrapper-0.1.15/qwrapper/x86/utils/registers.py`

 * *Files identical despite different names*

### Comparing `qwrapper-0.1.14/qwrapper/x86/x86machine.py` & `qwrapper-0.1.15/qwrapper/x86/x86machine.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,20 +11,32 @@
 import asyncio
 
 class X86Machine(QemuMachine):
         gdbControl = gdbcontroller.GdbController()
         gdbConnected = False
         qemuCmd = []
 
-        def __init__(self, qmpwait):
+        def __init__(self, disk_images, qmpwait=False,):
             super().__init__()
+
+            self.disk_counter = ord('a') # Initial disk value
+
             if qmpwait == True:
-                self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=on', '-hda', 'kernel.iso', '-hdb', 'disk.iso']
+                self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=on']
             if qmpwait == False:
-                self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=off', '-hda', 'kernel.iso', '-hdb', 'disk.iso']
+                self.qemuCmd = ['qemu-system-i386', '-display', 'none', '-S', '-s', '-qmp', 'unix:/tmp/qmp.socket,server=on,wait=off']
+
+            for image in disk_images:
+                if self.disk_counter > ord('z'):
+                    print("Error: Too many disk images")
+                    break
+                self.qemuCmd.append('-hd' + chr(self.disk_counter))
+                self.qemuCmd.append(image)
+                self.disk_counter += 1
+            
 
             print("Setting up virtual machine...")
             # Start Qemu with gdb stub and QMP Server. Add the kernel and disk images.
             # Virtual machine starts in "wait" mode. Waits for user to start VM execution.
             self.QemuProcess = subprocess.Popen(self.qemuCmd, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 
             # Wait 2 seconds to allow QEMU to create the socket file
```

