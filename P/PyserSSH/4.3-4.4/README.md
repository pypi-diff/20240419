# Comparing `tmp/PyserSSH-4.3.tar.gz` & `tmp/PyserSSH-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyserSSH-4.3.tar", last modified: Sun Apr  7 10:07:53 2024, max compression
+gzip compressed data, was "PyserSSH-4.4.tar", last modified: Fri Apr 19 08:27:49 2024, max compression
```

## Comparing `PyserSSH-4.3.tar` & `PyserSSH-4.4.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.672365 PyserSSH-4.3/
--rw-rw-rw-   0        0        0     2157 2024-04-07 10:07:53.672365 PyserSSH-4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1852 2024-03-31 07:02:15.000000 PyserSSH-4.3/README.md
--rw-rw-rw-   0        0        0      115 2024-04-07 10:07:53.679882 PyserSSH-4.3/setup.cfg
--rw-rw-rw-   0        0        0      607 2024-04-07 10:07:23.000000 PyserSSH-4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.471907 PyserSSH-4.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.508903 PyserSSH-4.3/src/PyserSSH/
--rw-rw-rw-   0        0        0     2067 2024-04-07 09:53:16.000000 PyserSSH-4.3/src/PyserSSH/__init__.py
--rw-rw-rw-   0        0        0     8384 2024-04-07 10:00:41.000000 PyserSSH-4.3/src/PyserSSH/account.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.609790 PyserSSH-4.3/src/PyserSSH/extensions/
--rw-rw-rw-   0        0        0     9258 2024-04-06 10:27:06.000000 PyserSSH-4.3/src/PyserSSH/extensions/XHandler.py
--rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:52.000000 PyserSSH-4.3/src/PyserSSH/extensions/__init__.py
--rw-rw-rw-   0        0        0     7072 2024-04-06 10:26:37.000000 PyserSSH-4.3/src/PyserSSH/extensions/dialog.py
--rw-rw-rw-   0        0        0     3582 2024-04-06 10:26:40.000000 PyserSSH-4.3/src/PyserSSH/extensions/moredisplay.py
--rw-rw-rw-   0        0        0    13483 2024-04-06 10:26:49.000000 PyserSSH-4.3/src/PyserSSH/extensions/processbar.py
--rw-rw-rw-   0        0        0     1332 2024-04-06 10:26:53.000000 PyserSSH-4.3/src/PyserSSH/extensions/ptop.py
--rw-rw-rw-   0        0        0     7095 2024-04-07 08:41:56.000000 PyserSSH-4.3/src/PyserSSH/interactive.py
--rw-rw-rw-   0        0        0    13692 2024-04-07 09:57:13.000000 PyserSSH-4.3/src/PyserSSH/server.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.669376 PyserSSH-4.3/src/PyserSSH/system/
--rw-rw-rw-   0        0        0     7265 2024-04-06 10:26:25.000000 PyserSSH-4.3/src/PyserSSH/system/SFTP.py
--rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:54.000000 PyserSSH-4.3/src/PyserSSH/system/__init__.py
--rw-rw-rw-   0        0        0     1492 2024-04-06 10:26:13.000000 PyserSSH-4.3/src/PyserSSH/system/info.py
--rw-rw-rw-   0        0        0     8771 2024-04-07 08:44:26.000000 PyserSSH-4.3/src/PyserSSH/system/inputsystem.py
--rw-rw-rw-   0        0        0     4277 2024-04-06 10:26:21.000000 PyserSSH-4.3/src/PyserSSH/system/interface.py
--rw-rw-rw-   0        0        0     1799 2024-04-06 10:26:29.000000 PyserSSH-4.3/src/PyserSSH/system/syscom.py
--rw-rw-rw-   0        0        0     2282 2024-04-06 10:26:32.000000 PyserSSH-4.3/src/PyserSSH/system/sysfunc.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:07:53.670365 PyserSSH-4.3/src/PyserSSH.egg-info/
--rw-rw-rw-   0        0        0     2157 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      739 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-07 10:07:53.000000 PyserSSH-4.3/src/PyserSSH.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.966670 PyserSSH-4.4/
+-rw-rw-rw-   0        0        0     2812 2024-04-19 08:27:49.966670 PyserSSH-4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2505 2024-04-19 08:22:38.000000 PyserSSH-4.4/README.md
+-rw-rw-rw-   0        0        0      115 2024-04-19 08:27:49.968674 PyserSSH-4.4/setup.cfg
+-rw-rw-rw-   0        0        0      607 2024-04-19 07:57:28.000000 PyserSSH-4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.829586 PyserSSH-4.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.846988 PyserSSH-4.4/src/PyserSSH/
+-rw-rw-rw-   0        0        0     2253 2024-04-19 07:59:50.000000 PyserSSH-4.4/src/PyserSSH/__init__.py
+-rw-rw-rw-   0        0        0     8763 2024-04-18 07:11:53.000000 PyserSSH-4.4/src/PyserSSH/account.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.877523 PyserSSH-4.4/src/PyserSSH/demo/
+-rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:52.000000 PyserSSH-4.4/src/PyserSSH/demo/__init__.py
+-rw-rw-rw-   0        0        0     7476 2024-04-19 08:17:13.000000 PyserSSH-4.4/src/PyserSSH/demo/demo1.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.909567 PyserSSH-4.4/src/PyserSSH/extensions/
+-rw-rw-rw-   0        0        0     9258 2024-04-06 10:27:06.000000 PyserSSH-4.4/src/PyserSSH/extensions/XHandler.py
+-rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:52.000000 PyserSSH-4.4/src/PyserSSH/extensions/__init__.py
+-rw-rw-rw-   0        0        0     7072 2024-04-18 06:56:32.000000 PyserSSH-4.4/src/PyserSSH/extensions/dialog.py
+-rw-rw-rw-   0        0        0     3582 2024-04-06 10:26:40.000000 PyserSSH-4.4/src/PyserSSH/extensions/moredisplay.py
+-rw-rw-rw-   0        0        0    13483 2024-04-06 10:26:49.000000 PyserSSH-4.4/src/PyserSSH/extensions/processbar.py
+-rw-rw-rw-   0        0        0     1332 2024-04-06 10:26:53.000000 PyserSSH-4.4/src/PyserSSH/extensions/ptop.py
+-rw-rw-rw-   0        0        0     7208 2024-04-18 06:56:24.000000 PyserSSH-4.4/src/PyserSSH/interactive.py
+-rw-rw-rw-   0        0        0    14510 2024-04-18 07:09:03.000000 PyserSSH-4.4/src/PyserSSH/server.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.962505 PyserSSH-4.4/src/PyserSSH/system/
+-rw-rw-rw-   0        0        0     7265 2024-04-06 10:26:25.000000 PyserSSH-4.4/src/PyserSSH/system/SFTP.py
+-rw-rw-rw-   0        0        0     1396 2024-04-07 10:05:54.000000 PyserSSH-4.4/src/PyserSSH/system/__init__.py
+-rw-rw-rw-   0        0        0     1492 2024-04-14 08:20:10.000000 PyserSSH-4.4/src/PyserSSH/system/info.py
+-rw-rw-rw-   0        0        0     9149 2024-04-14 08:44:42.000000 PyserSSH-4.4/src/PyserSSH/system/inputsystem.py
+-rw-rw-rw-   0        0        0     4277 2024-04-06 10:26:21.000000 PyserSSH-4.4/src/PyserSSH/system/interface.py
+-rw-rw-rw-   0        0        0     1790 2024-04-14 14:28:38.000000 PyserSSH-4.4/src/PyserSSH/system/syscom.py
+-rw-rw-rw-   0        0        0     2282 2024-04-06 10:26:32.000000 PyserSSH-4.4/src/PyserSSH/system/sysfunc.py
+drwxrwxrwx   0        0        0        0 2024-04-19 08:27:49.965672 PyserSSH-4.4/src/PyserSSH.egg-info/
+-rw-rw-rw-   0        0        0     2812 2024-04-19 08:27:49.000000 PyserSSH-4.4/src/PyserSSH.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      796 2024-04-19 08:27:49.000000 PyserSSH-4.4/src/PyserSSH.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 08:27:49.000000 PyserSSH-4.4/src/PyserSSH.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 08:27:49.000000 PyserSSH-4.4/src/PyserSSH.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-19 08:27:49.000000 PyserSSH-4.4/src/PyserSSH.egg-info/top_level.txt
```

### Comparing `PyserSSH-4.3/PKG-INFO` & `PyserSSH-4.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyserSSH
-Version: 4.3
+Version: 4.4
 Summary: python scriptable ssh server library. based on Paramiko
 Home-page: https://github.com/damp11113/PyserSSH
 Author: damp11113
 Author-email: damp51252@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: paramiko
@@ -13,25 +13,26 @@
 
 PyserSSH is a library for remote control your code with ssh client. The aim is to provide a scriptable SSH server which can be made to behave like any SSH-enabled device.
 
 This project is part from [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 This Server use port **2222** for default port
 
+> [!WARNING]  
+> For use in product please **generate new private key**! If you still use this demo private key maybe your product getting **hacked**! up to 90%. Please don't use this demo private key for real product.
+
 # Install
 Install from pypi
 ```bash
 pip install PyserSSH
 ```
 Install from github
 ```bash
 pip install git+https://github.com/damp11113/PyserSSH.git
 ```
-## Optional Packages
- - [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 # Quick Example
 ```py
 import os
 
 from PyserSSH import Server, Send, AccountManager
 
@@ -49,15 +50,29 @@
 ```
 This example you can connect with `ssh admin@localhost -p 2222` and press enter on login
 If you input `hello` the response is `world`
 
 # Demo
 https://github.com/damp11113/PyserSSH/assets/64675096/49bef3e2-3b15-4b64-b88e-3ca84a955de7
 
-See [server.py](https://github.com/damp11113/PyserSSH/blob/main/demo/server.py)
+For run this demo you can use this command
+```
+$ python -m PyserSSH
+```
+then
+```
+Do you want to run demo? (y/n): y
+```
+But if no [damp11113-library](https://github.com/damp11113/damp11113-library)
+```
+No 'damp11113-library'
+This demo is require 'damp11113-library' for run
+```
+you need to install [damp11113-library](https://github.com/damp11113/damp11113-library) for run this demo by choose `y` or `yes` in lowercase or uppercase
+```
+Do you want to install 'damp11113-library'? (y/n): y
+```
+For exit demo you can use `ctrl+c` or use `shutdown now` in PyserSSH shell **(not in real terminal)**
 
 I intend to leaked private key because that key i generated new. I recommend to generate new key if you want to use on your host because that key is for demo only.
 why i talk about this? because when i push private key into this repo in next 5 min++ i getting new email from GitGuardian. in that email say "
 GitGuardian has detected the following RSA Private Key exposed within your GitHub account" i dont knows what is GitGuardian and i not install this app into my account.
-
-
-
```

### Comparing `PyserSSH-4.3/README.md` & `PyserSSH-4.4/src/PyserSSH.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,38 @@
+Metadata-Version: 2.1
+Name: PyserSSH
+Version: 4.4
+Summary: python scriptable ssh server library. based on Paramiko
+Home-page: https://github.com/damp11113/PyserSSH
+Author: damp11113
+Author-email: damp51252@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+Requires-Dist: paramiko
+
 # What is PyserSSH
 
 PyserSSH is a library for remote control your code with ssh client. The aim is to provide a scriptable SSH server which can be made to behave like any SSH-enabled device.
 
 This project is part from [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 This Server use port **2222** for default port
 
+> [!WARNING]  
+> For use in product please **generate new private key**! If you still use this demo private key maybe your product getting **hacked**! up to 90%. Please don't use this demo private key for real product.
+
 # Install
 Install from pypi
 ```bash
 pip install PyserSSH
 ```
 Install from github
 ```bash
 pip install git+https://github.com/damp11113/PyserSSH.git
 ```
-## Optional Packages
- - [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 # Quick Example
 ```py
 import os
 
 from PyserSSH import Server, Send, AccountManager
 
@@ -38,15 +50,29 @@
 ```
 This example you can connect with `ssh admin@localhost -p 2222` and press enter on login
 If you input `hello` the response is `world`
 
 # Demo
 https://github.com/damp11113/PyserSSH/assets/64675096/49bef3e2-3b15-4b64-b88e-3ca84a955de7
 
-See [server.py](https://github.com/damp11113/PyserSSH/blob/main/demo/server.py)
+For run this demo you can use this command
+```
+$ python -m PyserSSH
+```
+then
+```
+Do you want to run demo? (y/n): y
+```
+But if no [damp11113-library](https://github.com/damp11113/damp11113-library)
+```
+No 'damp11113-library'
+This demo is require 'damp11113-library' for run
+```
+you need to install [damp11113-library](https://github.com/damp11113/damp11113-library) for run this demo by choose `y` or `yes` in lowercase or uppercase
+```
+Do you want to install 'damp11113-library'? (y/n): y
+```
+For exit demo you can use `ctrl+c` or use `shutdown now` in PyserSSH shell **(not in real terminal)**
 
 I intend to leaked private key because that key i generated new. I recommend to generate new key if you want to use on your host because that key is for demo only.
 why i talk about this? because when i push private key into this repo in next 5 min++ i getting new email from GitGuardian. in that email say "
 GitGuardian has detected the following RSA Private Key exposed within your GitHub account" i dont knows what is GitGuardian and i not install this app into my account.
-
-
-
```

### Comparing `PyserSSH-4.3/setup.py` & `PyserSSH-4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PyserSSH',
-    version='4.3',
+    version='4.4',
     license='MIT',
     author='damp11113',
     author_email='damp51252@gmail.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     url='https://github.com/damp11113/PyserSSH',
     description="python scriptable ssh server library. based on Paramiko",
```

### Comparing `PyserSSH-4.3/src/PyserSSH/__init__.py` & `PyserSSH-4.4/src/PyserSSH/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 """
 import os
 import logging
 
 from .interactive import *
 from .server import Server
 from .account import AccountManager
-from .system.info import system_banner
 
 
+from .system.info import system_banner
+
 try:
     os.environ["pyserssh_systemmessage"]
 except:
     os.environ["pyserssh_systemmessage"] = "YES"
 
 try:
     os.environ["pyserssh_enable_damp11113"]
@@ -62,7 +63,14 @@
 
 if os.environ["pyserssh_log"] == "NO":
     logger = logging.getLogger("PyserSSH")
     logger.disabled = True
 
 if os.environ["pyserssh_systemmessage"] == "YES":
     print(system_banner)
+
+if __name__ == "__main__":
+    stadem = input("Do you want to run demo? (y/n): ")
+    if stadem.upper() in ["Y", "YES"]:
+        from .demo import demo1
+    else:
+        exit()
```

### Comparing `PyserSSH-4.3/src/PyserSSH/account.py` & `PyserSSH-4.4/src/PyserSSH/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         self.__autosaveworknexttime = time.time() + self.autosavedelay
         self.__autosavework = True
         while self.__autosavework:
             if int(self.__autosaveworknexttime) == int(time.time()):
                 self.save("autosave_session.ses")
                 self.__autosaveworknexttime = time.time() + self.autosavedelay
 
+            time.sleep(1) # fix cpu load
+
     def __saveexit(self):
         self.__autosavework = False
         self.save("autosave_session.ses")
         self.__autosavethread.join()
 
     def validate_credentials(self, username, password):
         if username in self.accounts and self.accounts[username]["password"] == password or self.anyuser:
@@ -136,14 +138,23 @@
                 self.accounts[username]["sftp_path"] = path
 
     def get_user_sftp_path(self, username):
         if username in self.accounts and "sftp_path" in self.accounts[username]:
             return self.accounts[username]["sftp_path"]
         return ""
 
+    def set_banner(self, username, banner):
+        if username in self.accounts:
+            self.accounts[username]["banner"] = banner
+
+    def get_banner(self, username):
+        if username in self.accounts and "banner" in self.accounts[username]:
+            return self.accounts[username]["banner"]
+        return None
+
     def get_user_timeout(self, username):
         if username in self.accounts and "timeout" in self.accounts[username]:
             return self.accounts[username]["timeout"]
         return None
 
     def set_user_timeout(self, username, timeout=None):
         if username in self.accounts:
```

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/XHandler.py` & `PyserSSH-4.4/src/PyserSSH/extensions/XHandler.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/__init__.py` & `PyserSSH-4.4/src/PyserSSH/demo/__init__.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/dialog.py` & `PyserSSH-4.4/src/PyserSSH/extensions/dialog.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/moredisplay.py` & `PyserSSH-4.4/src/PyserSSH/extensions/moredisplay.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/processbar.py` & `PyserSSH-4.4/src/PyserSSH/extensions/processbar.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/extensions/ptop.py` & `PyserSSH-4.4/src/PyserSSH/extensions/ptop.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/interactive.py` & `PyserSSH-4.4/src/PyserSSH/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,20 +32,23 @@
 def Send(client, string, ln=True):
     channel = client["channel"]
     if ln:
         channel.send(replace_enter_with_crlf(str(string) + "\n"))
     else:
         channel.send(replace_enter_with_crlf(str(string)))
 
-def Clear(client, oldclear=False):
+def Clear(client, oldclear=False, keep=False):
     sx, sy = client["windowsize"]["width"], client["windowsize"]["height"]
 
     if oldclear:
         for x in range(sy):
             Send(client, '\b \b' * sx, ln=False)  # Send newline after each line
+    elif keep:
+        Send(client, "\033[2J", ln=False)
+        Send(client, "\033[H", ln=False)
     else:
         Send(client, "\033[3J", ln=False)
         Send(client, "\033[1J", ln=False)
         Send(client, "\033[H", ln=False)
 
 def Title(client, title):
     Send(client, f"\033]0;{title}\007", ln=False)
```

### Comparing `PyserSSH-4.3/src/PyserSSH/server.py` & `PyserSSH-4.4/src/PyserSSH/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,45 +32,46 @@
 from functools import wraps
 import logging
 
 from .system.SFTP import SSHSFTPServer
 from .system.interface import Sinterface
 from .interactive import *
 from .system.inputsystem import expect
-from .system.info import system_banner, __version__
+from .system.info import __version__
 
-#paramiko.sftp_file.SFTPFile.MAX_REQUEST_SIZE = pow(2, 22)
+# paramiko.sftp_file.SFTPFile.MAX_REQUEST_SIZE = pow(2, 22)
 
 sftpclient = ["WinSCP", "Xplore"]
 
 logger = logging.getLogger("PyserSSH")
 
 class Server:
-    def __init__(self, accounts, system_message=True, disable_scroll_with_arrow=True, sftp=True, sftproot=os.getcwd(), system_commands=True, compression=True, usexternalauth=False, history=True, inputsystem=True, XHandler=None, title=f"PyserSSH v{__version__}", inspeed=32768):
+    def __init__(self, accounts, system_message=True, disable_scroll_with_arrow=True, sftp=False, sftproot=os.getcwd(), system_commands=True, compression=True, usexternalauth=False, history=True, inputsystem=True, XHandler=None, title=f"PyserSSH v{__version__}", inspeed=32768):
         """
          A simple SSH server
         """
         self._event_handlers = {}
         self.sysmess = system_message
         self.client_handlers = {}  # Dictionary to store event handlers for each client
-        self.current_users = {}  # Dictionary to store current_user for each connected client
         self.accounts = accounts
         self.disable_scroll_with_arrow = disable_scroll_with_arrow
         self.sftproot = sftproot
         self.sftpena = sftp
         self.enasyscom = system_commands
         self.compressena = compression
         self.usexternalauth = usexternalauth
         self.history = history
         self.enainputsystem = inputsystem
         self.XHandler = XHandler
         self.title = title
         self.inspeed = inspeed
 
-        self.system_banner = system_banner
+        self.__processmode = None
+        self.__serverisrunning = False
+        self.__server_stopped = threading.Event()  # Event to signal server stop
 
         if self.enasyscom:
             print("\033[33m!!Warning!! System commands is enable! \033[0m")
 
     def on_user(self, event_name):
         def decorator(func):
             @wraps(func)
@@ -100,15 +101,14 @@
 
         if self.sftpena:
             SSHSFTPServer.ROOT = self.sftproot
             SSHSFTPServer.ACCOUNT = self.accounts
             SSHSFTPServer.CLIENTHANDELES = self.client_handlers
             bh_session.set_subsystem_handler('sftp', paramiko.SFTPServer, SSHSFTPServer)
 
-
         if self.compressena:
             bh_session.use_compression(True)
         else:
             bh_session.use_compression(False)
 
         bh_session.default_window_size = 2147483647
         bh_session.packetizer.REKEY_BYTES = pow(2, 40)
@@ -135,50 +135,55 @@
                     "event_handlers": {},
                     "current_user": None,
                     "channel": channel,  # Associate the channel with the client handler,
                     "last_activity_time": None,
                     "connecttype": None,
                     "last_login_time": None,
                     "windowsize": {},
-                    "x11": {}
+                    "x11": {},
+                    "prompt": None,
+                    "inputbuffer": None,
+                    "peername": peername
                 }
             client_handler = self.client_handlers[peername]
             client_handler["current_user"] = server.current_user
             client_handler["channel"] = channel  # Update the channel attribute for the client handler
             client_handler["last_activity_time"] = time.time()
             client_handler["last_login_time"] = time.time()
+            client_handler["prompt"] = self.accounts.get_prompt(server.current_user)
 
             self.accounts.set_user_last_login(self.client_handlers[channel.getpeername()]["current_user"], peername[0])
 
             #if not any(bh_session.remote_version.split("-")[2].startswith(prefix) for prefix in sftpclient):
             if not channel.out_window_size == bh_session.default_window_size:
                 while self.client_handlers[channel.getpeername()]["windowsize"] == {}:
                     pass
 
-                channel.send(f"\033]0;{self.title}\007".encode())
+                userbanner = self.accounts.get_banner(self.client_handlers[channel.getpeername()]["current_user"])
 
-                if self.sysmess:
-                    channel.sendall(replace_enter_with_crlf(self.system_banner))
+                if self.sysmess or userbanner != None:
+                    channel.send(f"\033]0;{self.title}\007".encode())
+                    channel.sendall(replace_enter_with_crlf(userbanner))
                     channel.sendall(replace_enter_with_crlf("\n"))
 
                 try:
                     self._handle_event("connect", self.client_handlers[channel.getpeername()])
                 except Exception as e:
                     self._handle_event("error", self.client_handlers[channel.getpeername()], e)
 
                 client_handler["connecttype"] = "ssh"
                 if self.enainputsystem:
                     try:
                         if self.accounts.get_user_timeout(self.client_handlers[channel.getpeername()]["current_user"]) != None:
                             channel.setblocking(False)
                             channel.settimeout(self.accounts.get_user_timeout(self.client_handlers[channel.getpeername()]["current_user"]))
 
-                        channel.send(replace_enter_with_crlf(self.accounts.get_prompt(self.client_handlers[channel.getpeername()]["current_user"]) + " ").encode('utf-8'))
+                        channel.send(replace_enter_with_crlf(self.client_handlers[channel.getpeername()]["prompt"] + " ").encode('utf-8'))
                         while True:
-                            expect(self, channel, peername)
+                            expect(self, self.client_handlers[channel.getpeername()])
                     except KeyboardInterrupt:
                         self._handle_event("disconnected", self.client_handlers[peername]["current_user"])
                         channel.close()
                         bh_session.close()
                     except Exception as e:
                         self._handle_event("syserror", client_handler, e)
                         logger.error(e)
@@ -202,38 +207,50 @@
     def stop_server(self):
         logger.info("Stopping the server...")
         try:
             for client_handler in self.client_handlers.values():
                 channel = client_handler.get("channel")
                 if channel:
                     channel.close()
+            self.__serverisrunning = True
             self.server.close()
             logger.info("Server stopped.")
         except Exception as e:
             logger.error(f"Error occurred while stopping the server: {e}")
 
     def _start_listening_thread(self):
         try:
-            self.server.listen(10)
             logger.info("Start Listening for connections...")
-            while True:
+            while self.__serverisrunning:
                 client, addr = self.server.accept()
-                client_thread = threading.Thread(target=self.handle_client, args=(client, addr))
-                client_thread.start()
+                if self.__processmode == "thread":
+                    client_thread = threading.Thread(target=self.handle_client, args=(client, addr))
+                    client_thread.start()
+                else:
+                    self.handle_client(client, addr)
 
         except Exception as e:
             logger.error(e)
 
-    def run(self, private_key_path, host="0.0.0.0", port=2222):
+    def run(self, private_key_path, host="0.0.0.0", port=2222, mode="thread", maxuser=0, daemon=False):
+        """mode: single, thread"""
         self.server = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, True)
         self.server.bind((host, port))
         self.private_key = paramiko.RSAKey(filename=private_key_path)
+        if maxuser == 0:
+            self.server.listen()
+        else:
+            self.server.listen(maxuser)
+
+        self.__processmode = mode.lower()
+        self.__serverisrunning = True
 
         client_thread = threading.Thread(target=self._start_listening_thread)
+        client_thread.daemon = daemon
         client_thread.start()
 
     def kickbyusername(self, username, reason=None):
         for peername, client_handler in list(self.client_handlers.items()):
             if client_handler["current_user"] == username:
                 channel = client_handler.get("channel")
                 self._handle_event("disconnected", channel.getpeername(), self.client_handlers[channel.getpeername()]["current_user"])
@@ -300,8 +317,8 @@
                     try:
                         # Send the message to the specific client
                         Send(channel, message)
                     except Exception as e:
                         logger.error(f"Error occurred while sending message to {username}: {e}")
                     break
         else:
-            logger.warning(f"User '{username}' not found.")
+            logger.warning(f"User '{username}' not found.")
```

### Comparing `PyserSSH-4.3/src/PyserSSH/system/SFTP.py` & `PyserSSH-4.4/src/PyserSSH/system/SFTP.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/system/__init__.py` & `PyserSSH-4.4/src/PyserSSH/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/system/info.py` & `PyserSSH-4.4/src/PyserSSH/system/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,14 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = "4.2"
+__version__ = "4.4"
 
 system_banner = (
     f"\033[36mPyserSSH V{__version__} \033[0m\n"
     #"\033[33m!!Warning!! This is Testing Version of PyserSSH \033[0m\n"
     "\033[35mUse Putty and WinSCP (SFTP) for best experience \033[0m"
 )
```

### Comparing `PyserSSH-4.3/src/PyserSSH/system/inputsystem.py` & `PyserSSH-4.4/src/PyserSSH/system/inputsystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,20 +31,22 @@
 import traceback
 
 from .sysfunc import replace_enter_with_crlf
 from .syscom import systemcommand
 
 logger = logging.getLogger("PyserSSH")
 
-def expect(self, chan, peername, echo=True):
+def expect(self, client, echo=True):
     buffer = bytearray()
     cursor_position = 0
     outindexall = 0
     history_index_position = 0  # Initialize history index position outside the loop
-    currentuser = self.client_handlers[chan.getpeername()]
+    chan = client["channel"]
+    peername = client["peername"]
+
     try:
         while True:
             try:
                 byte = chan.recv(1)
             except socket.timeout:
                 chan.setblocking(False)
                 chan.settimeout(None)
@@ -62,36 +64,44 @@
             elif byte == b'\t':
                 pass
             elif byte == b'\x7f' or byte == b'\x08':
                 if cursor_position > 0:
                     buffer = buffer[:cursor_position - 1] + buffer[cursor_position:]
                     cursor_position -= 1
                     outindexall -= 1
-                    chan.sendall(b"\b \b")
+                    if cursor_position != outindexall:
+                        chan.sendall(b"\b \b")
+                        chan.sendall(buffer[cursor_position:])
+                    else:
+                        chan.sendall(b"\b \b")
                 else:
                     chan.sendall(b"\x07")
             elif byte == b"\x1b" and chan.recv(1) == b'[':
                 arrow_key = chan.recv(1)
                 if not self.disable_scroll_with_arrow:
                     if arrow_key == b'C':
                         # Right arrow key, move cursor right if not at the end
                         if cursor_position < len(buffer):
                             chan.sendall(b'\x1b[C')
-                            cursor_position += 1
+                        #    cursor_position += 1
+                            cursor_position = min(len(buffer), cursor_position + 1)
+
                     elif arrow_key == b'D':
                         # Left arrow key, move cursor left if not at the beginning
                         if cursor_position > 0:
                             chan.sendall(b'\x1b[D')
-                            cursor_position -= 1
-                elif self.history:
+                        #    cursor_position -= 1
+                            cursor_position = max(0, cursor_position - 1)
+
+                if self.history:
                     if arrow_key == b'A':
                         if history_index_position == 0:
-                            command = self.accounts.get_lastcommand(currentuser["current_user"])
+                            command = self.accounts.get_lastcommand(client["current_user"])
                         else:
-                            command = self.accounts.get_history(currentuser["current_user"], history_index_position)
+                            command = self.accounts.get_history(client["current_user"], history_index_position)
 
                         # Clear the buffer
                         for i in range(cursor_position):
                             chan.send(b"\b \b")
 
                         # Update buffer and cursor position with the new command
                         buffer = bytearray(command.encode('utf-8'))
@@ -101,17 +111,17 @@
                         # Print the updated buffer
                         chan.sendall(buffer)
 
                         history_index_position += 1
                     elif arrow_key == b'B':
                         if history_index_position != -1:
                             if history_index_position == 0:
-                                command = self.accounts.get_lastcommand(currentuser["current_user"])
+                                command = self.accounts.get_lastcommand(client["current_user"])
                             else:
-                                command = self.accounts.get_history(currentuser["current_user"], history_index_position)
+                                command = self.accounts.get_history(client["current_user"], history_index_position)
 
                             # Clear the buffer
                             for i in range(cursor_position):
                                 chan.send(b"\b \b")
 
                             # Update buffer and cursor position with the new command
                             buffer = bytearray(command.encode('utf-8'))
@@ -135,58 +145,62 @@
                 break
             else:
                 history_index_position = -1
 
                 self._handle_event("ontype", self.client_handlers[chan.getpeername()], byte)
                 if echo:
                     if outindexall != cursor_position:
+                        chan.sendall(b" ")
+                        chan.sendall(b'\033[s')
                         chan.sendall(byte + buffer[cursor_position:])
-                        chan.sendall(f"\033[{cursor_position}G".encode())
+                        chan.sendall(b'\033[u')
                     else:
                         chan.sendall(byte)
 
                 #print(buffer[:cursor_position], byte, buffer[cursor_position:])
                 buffer = buffer[:cursor_position] + byte + buffer[cursor_position:]
                 cursor_position += 1
                 outindexall += 1
 
+            client["inputbuffer"] = buffer
+
         if echo:
             chan.sendall(b'\r\n')
 
         command = str(buffer.decode('utf-8')).strip()
 
-        if self.history and command.strip() != "" and self.accounts.get_lastcommand(currentuser["current_user"]) != command:
-            self.accounts.add_history(currentuser["current_user"], command)
+        if self.history and command.strip() != "" and self.accounts.get_lastcommand(client["current_user"]) != command:
+            self.accounts.add_history(client["current_user"], command)
 
         if command.strip() != "":
             if self.accounts.get_user_timeout(self.client_handlers[chan.getpeername()]["current_user"]) != None:
                 chan.setblocking(False)
                 chan.settimeout(None)
 
             try:
                 if self.enasyscom:
-                    sct = systemcommand(currentuser, command)
+                    sct = systemcommand(client, command)
                 else:
                     sct = False
 
                 if not sct:
                     if self.XHandler != None:
-                        self._handle_event("beforexhandler", currentuser, command)
+                        self._handle_event("beforexhandler", client, command)
 
-                        self.XHandler.call(currentuser, command)
+                        self.XHandler.call(client, command)
 
-                        self._handle_event("afterxhandler", currentuser, command)
+                        self._handle_event("afterxhandler", client, command)
                     else:
-                        self._handle_event("command", currentuser, command)
+                        self._handle_event("command", client, command)
 
             except Exception as e:
-                self._handle_event("error", currentuser, e)
+                self._handle_event("error", client, e)
 
         try:
-            chan.send(replace_enter_with_crlf(self.accounts.get_prompt(currentuser["current_user"]) + " ").encode('utf-8'))
+            chan.send(replace_enter_with_crlf(client["prompt"] + " ").encode('utf-8'))
         except:
             logger.error("Send error")
 
         chan.setblocking(False)
         chan.settimeout(None)
 
         if self.accounts.get_user_timeout(self.client_handlers[chan.getpeername()]["current_user"]) != None:
```

### Comparing `PyserSSH-4.3/src/PyserSSH/system/interface.py` & `PyserSSH-4.4/src/PyserSSH/system/interface.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH/system/syscom.py` & `PyserSSH-4.4/src/PyserSSH/system/syscom.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,26 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 import shlex
 
-from ..interactive import *
+from ..interactive import Send, Clear, Title
 
 def systemcommand(client, command):
-    channel = client["channel"]
-
     if command == "whoami":
-        Send(channel, client["current_user"])
+        Send(client, client["current_user"])
         return True
     elif command.startswith("title"):
         args = shlex.split(command)
         title = args[1]
         Title(client, title)
         return True
     elif command == "exit":
-        channel.close()
+        client["channel"].close()
         return True
     elif command == "clear":
         Clear(client)
         return True
     else:
         return False
```

### Comparing `PyserSSH-4.3/src/PyserSSH/system/sysfunc.py` & `PyserSSH-4.4/src/PyserSSH/system/sysfunc.py`

 * *Files identical despite different names*

### Comparing `PyserSSH-4.3/src/PyserSSH.egg-info/PKG-INFO` & `PyserSSH-4.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,27 @@
-Metadata-Version: 2.1
-Name: PyserSSH
-Version: 4.3
-Summary: python scriptable ssh server library. based on Paramiko
-Home-page: https://github.com/damp11113/PyserSSH
-Author: damp11113
-Author-email: damp51252@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-Requires-Dist: paramiko
-
 # What is PyserSSH
 
 PyserSSH is a library for remote control your code with ssh client. The aim is to provide a scriptable SSH server which can be made to behave like any SSH-enabled device.
 
 This project is part from [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 This Server use port **2222** for default port
 
+> [!WARNING]  
+> For use in product please **generate new private key**! If you still use this demo private key maybe your product getting **hacked**! up to 90%. Please don't use this demo private key for real product.
+
 # Install
 Install from pypi
 ```bash
 pip install PyserSSH
 ```
 Install from github
 ```bash
 pip install git+https://github.com/damp11113/PyserSSH.git
 ```
-## Optional Packages
- - [damp11113-library](https://github.com/damp11113/damp11113-library)
 
 # Quick Example
 ```py
 import os
 
 from PyserSSH import Server, Send, AccountManager
 
@@ -49,15 +39,29 @@
 ```
 This example you can connect with `ssh admin@localhost -p 2222` and press enter on login
 If you input `hello` the response is `world`
 
 # Demo
 https://github.com/damp11113/PyserSSH/assets/64675096/49bef3e2-3b15-4b64-b88e-3ca84a955de7
 
-See [server.py](https://github.com/damp11113/PyserSSH/blob/main/demo/server.py)
+For run this demo you can use this command
+```
+$ python -m PyserSSH
+```
+then
+```
+Do you want to run demo? (y/n): y
+```
+But if no [damp11113-library](https://github.com/damp11113/damp11113-library)
+```
+No 'damp11113-library'
+This demo is require 'damp11113-library' for run
+```
+you need to install [damp11113-library](https://github.com/damp11113/damp11113-library) for run this demo by choose `y` or `yes` in lowercase or uppercase
+```
+Do you want to install 'damp11113-library'? (y/n): y
+```
+For exit demo you can use `ctrl+c` or use `shutdown now` in PyserSSH shell **(not in real terminal)**
 
 I intend to leaked private key because that key i generated new. I recommend to generate new key if you want to use on your host because that key is for demo only.
 why i talk about this? because when i push private key into this repo in next 5 min++ i getting new email from GitGuardian. in that email say "
-GitGuardian has detected the following RSA Private Key exposed within your GitHub account" i dont knows what is GitGuardian and i not install this app into my account.
-
-
-
+GitGuardian has detected the following RSA Private Key exposed within your GitHub account" i dont knows what is GitGuardian and i not install this app into my account.
```

### Comparing `PyserSSH-4.3/src/PyserSSH.egg-info/SOURCES.txt` & `PyserSSH-4.4/src/PyserSSH.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/PyserSSH/interactive.py
 src/PyserSSH/server.py
 src/PyserSSH.egg-info/PKG-INFO
 src/PyserSSH.egg-info/SOURCES.txt
 src/PyserSSH.egg-info/dependency_links.txt
 src/PyserSSH.egg-info/requires.txt
 src/PyserSSH.egg-info/top_level.txt
+src/PyserSSH/demo/__init__.py
+src/PyserSSH/demo/demo1.py
 src/PyserSSH/extensions/XHandler.py
 src/PyserSSH/extensions/__init__.py
 src/PyserSSH/extensions/dialog.py
 src/PyserSSH/extensions/moredisplay.py
 src/PyserSSH/extensions/processbar.py
 src/PyserSSH/extensions/ptop.py
 src/PyserSSH/system/SFTP.py
```

