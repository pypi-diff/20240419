# Comparing `tmp/god-tool-0.8.1.tar.gz` & `tmp/god_tool-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "god-tool-0.8.1.tar", last modified: Fri Jan 12 07:12:47 2024, max compression
+gzip compressed data, was "god_tool-0.9.0.tar", last modified: Fri Apr 19 13:31:31 2024, max compression
```

## Comparing `god-tool-0.8.1.tar` & `god_tool-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-01-12 07:12:47.686427 god-tool-0.8.1/
--rw-r--r--   0 cjng96     (501) staff       (20)      664 2024-01-05 06:29:46.000000 god-tool-0.8.1/LICENSE.txt
--rw-r--r--   0 cjng96     (501) staff       (20)     1486 2024-01-12 07:12:47.686204 god-tool-0.8.1/PKG-INFO
--rw-r--r--   0 cjng96     (501) staff       (20)      594 2024-01-05 06:28:53.000000 god-tool-0.8.1/README.md
-drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-01-12 07:12:47.672760 god-tool-0.8.1/gat/
--rw-r--r--   0 cjng96     (501) staff       (20)       23 2024-01-12 07:12:38.000000 god-tool-0.8.1/gat/__init__.py
--rw-r--r--   0 cjng96     (501) staff       (20)     4212 2022-11-01 02:33:57.000000 god-tool-0.8.1/gat/coCollection.py
--rw-r--r--   0 cjng96     (501) staff       (20)      447 2022-11-01 02:33:57.000000 god-tool-0.8.1/gat/coPath.py
--rw-r--r--   0 cjng96     (501) staff       (20)     4711 2022-11-01 02:33:57.000000 god-tool-0.8.1/gat/coS3.py
--rw-r--r--   0 cjng96     (501) staff       (20)     7921 2024-01-10 01:16:56.000000 god-tool-0.8.1/gat/coSsh.py
--rw-r--r--   0 cjng96     (501) staff       (20)    62286 2024-01-10 11:10:58.000000 god-tool-0.8.1/gat/gat.py
--rw-r--r--   0 cjng96     (501) staff       (20)     7346 2024-01-05 06:28:53.000000 god-tool-0.8.1/gat/gatHelper.py
--rw-r--r--   0 cjng96     (501) staff       (20)     5402 2024-01-10 04:58:06.000000 god-tool-0.8.1/gat/myutil.py
--rw-r--r--   0 cjng96     (501) staff       (20)   111051 2024-01-12 06:34:36.000000 god-tool-0.8.1/gat/plugin.py
--rw-r--r--   0 cjng96     (501) staff       (20)    13131 2024-01-12 04:37:09.000000 god-tool-0.8.1/gat/sa.py
--rw-r--r--   0 cjng96     (501) staff       (20)     2064 2024-01-05 06:30:12.000000 god-tool-0.8.1/gat/sampleFiles.py
-drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-01-12 07:12:47.684694 god-tool-0.8.1/god_tool.egg-info/
--rw-r--r--   0 cjng96     (501) staff       (20)     1486 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/PKG-INFO
--rw-r--r--   0 cjng96     (501) staff       (20)      465 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/SOURCES.txt
--rw-r--r--   0 cjng96     (501) staff       (20)        1 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/dependency_links.txt
--rw-r--r--   0 cjng96     (501) staff       (20)       37 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/entry_points.txt
--rw-r--r--   0 cjng96     (501) staff       (20)        1 2024-01-02 06:02:02.000000 god-tool-0.8.1/god_tool.egg-info/not-zip-safe
--rw-r--r--   0 cjng96     (501) staff       (20)       25 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/requires.txt
--rw-r--r--   0 cjng96     (501) staff       (20)        9 2024-01-12 07:12:47.000000 god-tool-0.8.1/god_tool.egg-info/top_level.txt
--rw-r--r--   0 cjng96     (501) staff       (20)       79 2024-01-12 07:12:47.686899 god-tool-0.8.1/setup.cfg
--rw-r--r--   0 cjng96     (501) staff       (20)     1313 2024-01-05 06:29:46.000000 god-tool-0.8.1/setup.py
-drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-01-12 07:12:47.682426 god-tool-0.8.1/test/
--rw-r--r--   0 cjng96     (501) staff       (20)        0 2022-11-01 02:33:57.000000 god-tool-0.8.1/test/__init__.py
--rw-r--r--   0 cjng96     (501) staff       (20)     2409 2024-01-05 06:28:53.000000 god-tool-0.8.1/test/test_gatHelper.py
+drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-04-19 13:31:31.004447 god_tool-0.9.0/
+-rw-r--r--   0 cjng96     (501) staff       (20)      664 2024-03-31 01:10:10.000000 god_tool-0.9.0/LICENSE.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)     1486 2024-04-19 13:31:31.004385 god_tool-0.9.0/PKG-INFO
+-rw-r--r--   0 cjng96     (501) staff       (20)      594 2024-03-31 01:10:10.000000 god_tool-0.9.0/README.md
+drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-04-19 13:31:31.002345 god_tool-0.9.0/gat/
+-rw-r--r--   0 cjng96     (501) staff       (20)       23 2024-04-19 13:26:07.000000 god_tool-0.9.0/gat/__init__.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     4570 2024-03-31 01:10:10.000000 god_tool-0.9.0/gat/coCollection.py
+-rw-r--r--   0 cjng96     (501) staff       (20)      447 2024-01-03 02:36:13.000000 god_tool-0.9.0/gat/coPath.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     4711 2024-01-03 02:36:13.000000 god_tool-0.9.0/gat/coS3.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     7153 2024-03-31 01:10:10.000000 god_tool-0.9.0/gat/coSsh.py
+-rw-r--r--   0 cjng96     (501) staff       (20)    65678 2024-04-17 13:16:01.000000 god_tool-0.9.0/gat/gat.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     7346 2024-03-31 01:10:10.000000 god_tool-0.9.0/gat/gatHelper.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     5402 2024-03-31 01:10:10.000000 god_tool-0.9.0/gat/myutil.py
+-rw-r--r--   0 cjng96     (501) staff       (20)   113739 2024-04-19 13:20:44.000000 god_tool-0.9.0/gat/plugin.py
+-rw-r--r--   0 cjng96     (501) staff       (20)    13315 2024-03-31 01:10:10.000000 god_tool-0.9.0/gat/sa.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     2225 2024-04-06 12:19:51.000000 god_tool-0.9.0/gat/sampleFiles.py
+drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-04-19 13:31:31.004184 god_tool-0.9.0/god_tool.egg-info/
+-rw-r--r--   0 cjng96     (501) staff       (20)     1486 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/PKG-INFO
+-rw-r--r--   0 cjng96     (501) staff       (20)      465 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)        1 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)       37 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/entry_points.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)        1 2024-04-19 13:24:29.000000 god_tool-0.9.0/god_tool.egg-info/not-zip-safe
+-rw-r--r--   0 cjng96     (501) staff       (20)       25 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/requires.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)        9 2024-04-19 13:31:30.000000 god_tool-0.9.0/god_tool.egg-info/top_level.txt
+-rw-r--r--   0 cjng96     (501) staff       (20)       79 2024-04-19 13:31:31.004638 god_tool-0.9.0/setup.cfg
+-rw-r--r--   0 cjng96     (501) staff       (20)     1313 2024-03-31 01:10:10.000000 god_tool-0.9.0/setup.py
+drwxr-xr-x   0 cjng96     (501) staff       (20)        0 2024-04-19 13:31:31.003803 god_tool-0.9.0/test/
+-rw-r--r--   0 cjng96     (501) staff       (20)        0 2020-12-22 11:06:21.000000 god_tool-0.9.0/test/__init__.py
+-rw-r--r--   0 cjng96     (501) staff       (20)     2409 2024-03-31 01:10:10.000000 god_tool-0.9.0/test/test_gatHelper.py
```

### Comparing `god-tool-0.8.1/LICENSE.txt` & `god_tool-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/PKG-INFO` & `god_tool-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: god-tool
-Version: 0.8.1
+Version: 0.9.0
 Summary: Provisioning and App deployment tool.
 Home-page: https://github.com/cjng96/gat
 Author: Felix Choi
 Author-email: cjng96@gmail.com
 License: LGPL
 Keywords: auto restart,deployment
 Platform: Posix; MacOS X; Windows
```

### Comparing `god-tool-0.8.1/README.md` & `god_tool-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/gat/coCollection.py` & `god_tool-0.9.0/gat/coCollection.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,57 +27,70 @@
     assert dictGet(dic, "a", 99) == 1
     assert dictGet(dic, "b.A", 99) == 1
     assert dictGet(dic, "b.C", 99) == 99
 
 
 # dictGetTest()
 
+
 # https://gist.github.com/angstwad/bf22d1822c38a92ec0a9
 def dictMerge(dic, dic2):
     newDic = {}
 
     for k, v in dic.items():
         if k not in dic2:
             newDic[k] = deepcopy(v)
 
     for k, v in dic2.items():
-        if k in dic and isinstance(dic[k], dict) and isinstance(dic2[k], collectionsAbc.Mapping):
+        if (
+            k in dic
+            and isinstance(dic[k], dict)
+            and isinstance(dic2[k], collectionsAbc.Mapping)
+        ):
             # newDic[k] = mergeDict(dic[k], dic2[k])
             newDic[k] = dictMerge(dic[k], dic2[k])
         else:
             newDic[k] = deepcopy(dic2[k])
 
     return newDic
 
 
-def dictMerge2(dic, dic2):
-    newDic = Dict2()
-
+# supported Dict2
+def dict2Merge(dic, dic2):
     if isinstance(dic, Dict2):
         dic = dic.dic
 
     if isinstance(dic2, Dict2):
         dic2 = dic2.dic
 
+    newDic = Dict2()
     for k, v in dic.items():
         if k not in dic2:
             newDic[k] = deepcopy(v)
+
     for k, v in dic2.items():
-        if k in dic and isinstance(dic[k], (dict, Dict2)) and isinstance(dic2[k], (collectionsAbc.Mapping, Dict2)):
-            newDic[k] = dictMerge2(dic[k], dic2[k])
+        if (
+            k in dic
+            and isinstance(dic[k], (dict, Dict2))
+            and isinstance(dic2[k], (collectionsAbc.Mapping, Dict2))
+        ):
+            newDic[k] = dict2Merge(dic[k], dic2[k])
         else:
             newDic[k] = deepcopy(dic2[k])
 
     return newDic
 
 
 class Dict2:
     """
     dic["attr"] -> dic.attr
     dic.val = 1
+
+    # 단 새로운 멤버변수 생성은 안된다
+    dic.newV = 1
     """
 
     def __init__(self, dic=None):
         self.dic = dict()
         if dic is not None:
             self.fill(dic)
 
@@ -116,25 +129,27 @@
 
     def __keytransform__(self, key):
         return key
 
     def __contains__(self, key):
         return key in self.dic
 
+    # merge all attributes but array is replaced
     def fill(self, dic):
         if isinstance(dic, Dict2):
-            # self.fill(dic.dic)
-            # return
-            dic = dic.dic
+            dic = deepcopy(dic.dic)
 
         for key, value in dic.items():
-            tt = type(value)
-            if tt == dict:
-                self.dic[key] = Dict2(value)
-            elif tt == list:
+            valueType = type(value)
+            if valueType == dict:
+                if key in self.dic:
+                    self.dic[key] = dict2Merge(self.dic[key], value)
+                else:
+                    self.dic[key] = Dict2(value)
+            elif valueType == list:
                 for idx, vv in enumerate(value):
                     if type(vv) == dict:
                         value[idx] = Dict2(vv)
                 self.dic[key] = value
             else:
                 self.dic[key] = value
 
@@ -153,15 +168,15 @@
             print("%s is already defined. it will be overwritten." % name)
         self.dic[name] = value
 
 
 def dictMerge2Test():
     a = Dict2(dic={"a": 1, "d": {"a1": 1, "b1": 2}})
     b = Dict2(dic={"b": 1, "d": {"a1": 2, "c1": 3}})
-    c = dictMerge2(a, b)
+    c = dict2Merge(a, b)
     assert c.a == 1
     assert c.b == 1
     assert c.d.a1 == 2
     assert c.d.b1 == 2
     assert c.d.c1 == 3
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `god-tool-0.8.1/gat/coS3.py` & `god_tool-0.9.0/gat/coS3.py`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/gat/coSsh.py` & `god_tool-0.9.0/gat/coSsh.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
         self.uploadFilterFunc = falseFunc
 
     def close(self):
         if hasattr(self, "ssh"):
             self.ssh.close()
 
-    def _run(self, cmd, doOutput, arg):
+    def _run(self, cmd, doOutput, arg, log=False):
         s = time.time()
         chan = self.ssh.get_transport().open_session()
         # chan.get_pty()
         chan.exec_command(cmd)
         chan.setblocking(0)
         isLoop = True
         while isLoop:
@@ -94,65 +94,68 @@
                     doOutput(False, line.decode("utf-8"), arg)
 
             except socket.timeout as e:
                 pass
 
         ret = chan.recv_exit_status()
 
-        g = time.time() - s
-        g = int(g * 1000)
-        ss = f"{g}ms" if g < 10000 else f"{int(g/1000)}s"
+        if log:
+            g = time.time() - s
+            g = int(g * 1000)
+            ss = f"{g}ms" if g < 10000 else f"{int(g/1000)}s"
+            print(f"  -> ({ss}) ret:{ret} ")
 
-        print(f"  -> ({ss}) ret:{ret} ")
         chan.close()
         if ret != 0:
             # raise CalledProcessError("ssh command failed with ret:%d" % ret)
             ss = "" if arg is None else arg[0]
             raise MyCalledProcessError(ret, cmd, ss)
 
     # return: nothing
-    def run(self, cmd):
+    def run(self, cmd, log=False):
         """
         exception: output이 빈채로 온다
         """
 
         def doOutput(isStdout, ss, arg):
-            print(ss, end="")
+            if log:
+                print(ss, end="")
 
-        self._run(cmd, doOutput, None)
+        self._run(cmd, doOutput, None, log=log)
 
-    def runOutput(self, cmd):
+    def runOutput(self, cmd, log=False):
         """
         return: stdout result
         exception: output에 stdout만 포함
         """
         out = [""]
 
         def doOutput(isStdout, ss, arg):
             if isStdout:
                 arg[0] += ss
             else:
-                print(" stderr: ", ss)
+                if log:
+                    print(" stderr: ", ss)
 
-        self._run(cmd, doOutput, out)
-        print("  -> output:%s" % (out[0]))
+        self._run(cmd, doOutput, out, log=log)
+        # print("  -> output:%s" % (out[0]))
         return out[0]
 
-    def runOutputAll(self, cmd):
+    def runOutputAll(self, cmd, log=False):
         """
         return: stdout + stderr result
         exception: output에 stderr, stdout 모두 포함
         """
         out = [""]
 
         def doOutput(isStdout, ss, arg):
             arg[0] += ss
 
-        self._run(cmd, doOutput, out)
-        print("  -> output:%s" % (out[0]))
+        self._run(cmd, doOutput, out, log=log)
+        # print("  -> output:%s" % (out[0]))
         return out[0]
 
     # sftp 상에 경로를 생성한다.
     # remote 경로가 directory이면, is_dir에 True를 전달한다.
     def mkdirs(self, remote, isFolder=False):
         dirs = []
         if isFolder:
@@ -219,30 +222,7 @@
                 for pp in files:
                     src = os.path.join(folder, pp)
                     target = os.path.join(destPath, cutpath(srcPath, folder), pp)
                     self.uploadFile(src, target)
             except Exception as e:
                 print(e)
                 raise e
-            
-    # return os name of remote server
-    def getRemoteOS(self):
-        try:
-            stdin, stdout, stderr = self.ssh.exec_command('cat /etc/os-release')
-            osInfo = stdout.read().decode()
-
-            if 'ubuntu' in osInfo.lower():
-                print("========== remote os : ubuntu ==========")
-                return 'ubuntu'
-            elif 'centos' in osInfo.lower():
-                print("========== remote os : centos ==========")
-                return 'centos'
-        except Exception as e:
-            stdin, stdout, stderr = self.ssh.exec_command('sw_vers')
-            osInfo = stdout.read().decode()
-
-            osInfoStr = osInfo.lower()
-            if 'mac os' in osInfoStr or 'macos' in osInfoStr:
-                print("========== remote os : macos ==========")
-                return 'macos'
-            else:
-                raise Exception("Unknown OS")
```

### Comparing `god-tool-0.8.1/gat/gat.py` & `god_tool-0.9.0/gat/gat.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,25 @@
 
 # import inspect
 import fnmatch
 import traceback
 import importlib
 import importlib.util
 
+
 from copy import deepcopy
 
 # from io import StringIO
 from subprocess import Popen  # , PIPE
 
 import zipfile
 import tempfile
 
+from termcolor import colored, cprint
+
 from watchdog.observers import Observer
 from watchdog.events import PatternMatchingEventHandler
 
 from . import __version__
 from .coSsh import CoSsh
 from .coPath import cutpath
 from .sampleFiles import sampleApp, sampleSys
@@ -47,15 +50,15 @@
     cloneRepo,
     str2arg,
     envExpand,
     ObjectEncoder,
     pathRemove,
     pathIsChild,
 )  # NonBlockingStreamReader,
-from .coCollection import dictMerge, Dict2, dictMerge2
+from .coCollection import dictMerge, Dict2, dict2Merge
 
 g_cwd = ""
 g_scriptPath = ""
 
 # ##################### 나중에 사용될 여지가 있다. ###########################################
 
 # 우분투 명령어와 centos 명령어를 매핑
@@ -187,14 +190,33 @@
             g_options[optUbuntu][os] = opt
             print(f"{optUbuntu} for {os} has been successfully registered")
 
 
 # ######################################################################################3
 
 
+g_logLv = 0
+g_force = False
+
+g_connList = []
+
+
+def lld(ss):
+    if g_logLv >= 1:
+        print(ss)
+
+
+def llw(ss):
+    cprint(ss, "magenta", attrs=["bold"])
+
+
+def lle(ss):
+    cprint(ss, "red", attrs=["bold"])
+
+
 class Error(Exception):
     pass
 
 
 class ExcProgramExit(Exception):
     pass
 
@@ -207,23 +229,24 @@
         # self.config = None  # config object(g_config) -- 이건 전역 객체라 쓰면 안된다
 
     def str2arg(self, ss):
         return str2arg(ss)
 
     def deployFileListProd(self, env, func):
         include = env.config.deploy.include
-        exclude = env.config.get("deploy.exclude", [])
+        exclude = env.config.deploy.get("exclude", [])
+        # basePath = env.config.deploy.get("basePath", ".")
         followLinks = env.config.deploy.followLinks
         srcPath = env.config.srcPath
         g_main.targetFileListProd(
             include, exclude, func, followLinks=followLinks, localSrcPath=srcPath
         )
 
 
-class Tasks:
+class Conn:
     def __init__(self, server, config, dkTunnel=None, dkName=None, dkId=None):
         """
         server: can be none
         config = {name, host, port, id, pw}
         """
         self.proc = None
         self._uploadHelper = False
@@ -232,51 +255,100 @@
         self.ssh = None
         self.config = config
 
         # accessbility
         self.data = g_data
         self.util = g_util
 
-        # for log
-        self.name = "local" if server is None else server.host
+        self._os = None
 
-        # remote os
-        self.remoteOs = None
+        # for log
+        if server is None:
+            self.logName = "local"
+        else:
+            if dkTunnel is None:
+                self.logName = f"{server.host}:{server.port}"
+            else:
+                self.logName = f"{dkTunnel.logName}/{dkName}"
 
         if server is not None:
             if dkTunnel is None:
                 port = server.get("port", 22)
-                self.initSsh(
-                    server.host, port, server.id, keyFile=server.get("keyFile")
-                )
+                # port 0 is local conn
+                if port != 0:
+                    self.initSsh(
+                        server.host, port, server.id, keyFile=server.get("keyFile")
+                    )
 
             if "vars" not in server:
                 server.vars = {}
 
             self.vars = server.vars
 
         # docker일 경우 dkTunnel, dkName가 필수며, 부모의 server도 있어야 함
         self.dkTunnel = dkTunnel
         self.dkName = dkName
 
         if dkId is not None:
             dkId = strExpand(dkId, g_dic)
         self.dkId = dkId
 
+        self.tempPath = None
+
+        g_connList.append(self)
+
+    def clearConn(self):
+        self.tempPathClear()
+
+        if self._uploadHelper:
+            self.run("rm -f /tmp/gatHelper.py", printLog=False)
+            self._uploadHelper = False
+
+    def tempPathGet(self):
+        if self.tempPath is None:
+            pp = f"/tmp/gat-{self.config.name}"
+            ss = self.runOutput(f"test -d ${pp}; echo $?", printLog=False)
+            if ss == "0":
+                if not g_force:
+                    raise Exception(
+                        f"remote work path[{pp}] already exists. you can proceed with -f option."
+                    )
+
+                self.run(f"rm -rf {pp}")
+
+            self.tempPath = pp
+
+        return self.tempPath
+
+    def tempPathClear(self):
+        if self.tempPath is None:
+            try:
+                pp = self.tempPathGet()
+                self.run(f"rm -rf {pp}", printLog=False)
+                self.tempPath = None
+            except Exception as e:
+                if "No such container:" in str(e):
+                    # ignore it
+                    return
+
+        if self.dkTunnel is not None:
+            self.dkTunnel.tempPathClear()
+
+    def log(self, msg):
+        print(f"[{self.logName}]: {msg}")
+
     def initSsh(self, host, port, id, keyFile=None):
         self.ssh = CoSsh()
-        print(f"ssh: connecting to the server[{id}@{host}:{port}] with key:{keyFile}")
+        self.log(
+            f"ssh - connecting to the server[{id}@{host}:{port}] with key:{keyFile}"
+        )
         if keyFile is not None:
             with open(keyFile) as fp:
                 print("key - " + fp.read())
         self.ssh.init(host, port, id, keyFile=keyFile)
-        self.remoteOs = self.ssh.getRemoteOS()
-        print(
-            f"===================== remoteOs : {self.remoteOs} ========================="
-        )
 
     def __del__(self):
         if self.ssh is not None:
             self.ssh.close()
             self.ssh = None
 
     def str2arg(self, ss):
@@ -288,16 +360,15 @@
         return self.dkTunnel
 
     def dockerConn(self, name, dkId=None):
         if self.dkTunnel is not None:
             # raise Exception("dockerConn can be called only on remote connection.")
             return self.dkTunnel.dockerConn(name, dkId)
 
-        # dk = Tasks(self.server, g_config, self, name, dkId)
-        dk = Tasks(self.server, self.config, self, name, dkId)
+        dk = Conn(self.server, self.config, self, name, dkId)
         return dk
 
     def otherDockerConn(self, name, dkId=None):
         # if self.dkTunnel is None:
         #     raise Exception("otherDockerConn can be called on docker connection only.")
 
         # return self.dkTunnel.dockerConn(name, dkId)
@@ -310,15 +381,15 @@
         이건 util로 가는게 나을까
         """
         # dk = Tasks(Dict2(dict(name="remote", host=host, port=port, id=id)), g_config)  # no have owner
         serverCfg = Dict2(
             dict(name="remote", host=host, port=port, id=id, pw=pw, keyFile=keyFile)
         )
 
-        dk = Tasks(serverCfg, self.config)
+        dk = Conn(serverCfg, self.config)
         # no have owner
 
         # Tasks 생성자에서 접속하는듯...
         # dk.initSsh(host, port, id, keyFile=keyFile)
 
         if dkName is not None:
             dk = dk.dockerConn(dkName, dkId)
@@ -339,15 +410,15 @@
 
         path = os.path.expanduser(path)
         path = os.path.abspath(path)
 
         if not os.path.exists(path + ".py"):
             raise Exception(f"There is no target file[{path}] for deployApp")
 
-        print(f"\nsetupApp - path:{path}...")
+        self.log(f"setupApp - path:{path}...")
         dir = os.path.dirname(path)
         fn = os.path.basename(path)
 
         config = Config()
         helper = Helper(config)
 
         # sys.path.insert(0, dir)
@@ -381,31 +452,30 @@
         # remote = Tasks(server)
         # if "dkName" in server.dic:
         #     remote = remote.dockerConn(server.dkName, dkId=server.get("dkId"))
 
         pp = os.path.abspath(os.curdir)
         os.chdir(dir)
         try:
-            # g_main.taskDeploy(remote, server, mygat, config)
-            # g_main.taskSetup(remote, server, mygat, config)
             g_main.taskSetup(server, subCmd, mygat, config)
         finally:
             os.chdir(pp)
 
+    # 이제 이거 쓰는곳이 없다
     def deployApp(self, path, profile, serverOvr=None, varsOvr=None):
         if path.endswith(".py"):
             path = path[:-3]
 
         path = os.path.expanduser(path)
         path = os.path.abspath(path)
 
         if not os.path.exists(path + ".py"):
             raise Exception(f"There is no target file[{path}] for deployApp")
 
-        print(f"\ndeployApp - path:{path}, profile:{profile}")
+        self.log(f"deployApp - path:{path}, profile:{profile}")
         dir = os.path.dirname(path)
         fn = os.path.basename(path)
 
         config = Config()
         helper = Helper(config)
         # mymod = importlib.import_module(fn)
 
@@ -435,19 +505,19 @@
         # remote = Tasks(server)
         # if "dkName" in server.dic:
         #     remote = remote.dockerConn(server.dkName, dkId=server.get("dkId"))
 
         pp = os.path.abspath(os.curdir)
         os.chdir(dir)
         try:
-            # g_main.taskDeploy(remote, server, mygat, config)
             g_main.taskDeploy(server, mygat, config)
         finally:
             os.chdir(pp)
 
+    # 이거 좀 애매한데 uploadFile인데 사실상...
     def copyFile(self, srcPath, targetPath, sudo=False, mode=755, makeFolder=False):
         srcPath = os.path.expanduser(srcPath)
         srcPath = os.path.abspath(srcPath)
         with open(srcPath, "r") as fp:
             content = fp.read()
 
         self.makeFile(
@@ -475,64 +545,99 @@
         content = str2arg(content)
 
         self.run(
             f'echo "{content}" | {sudoCmd} tee {path} > /dev/null && {sudoCmd} chmod {mode} {path}'
         )
         # self.run(f'echo "{content}" > {path}')
 
-    def runOutput(self, cmd, expandVars=True):
+    def runOutput(self, cmd, expandVars=True, printLog=True):
         """
         cmd: string or array
         expandVars:
         return: stdout string
         exception: subprocess.CalledProcessError(returncode, output)
         """
-        print("executeOutput on %s[%s].." % (self._serverName(), cmd))
+        if printLog:
+            ss = cmd[:100] + "..." if g_logLv == 0 and len(cmd) > 100 else cmd
+            self.log(f"runOutput [{ss}]")
 
         # if expandVars:
         #     cmd = strExpand(cmd, g_dic)
 
+        log = g_logLv > 0 and printLog
+
+        out = ""
         if self.dkTunnel is not None:
             dkRunUser = "-u %s" % self.dkId if self.dkId is not None else ""
             cmd = str2arg(cmd)
             cmd = f'sudo docker exec -i {dkRunUser} {self.dkName} bash -c "{cmd}"'
             # alias defined in .bashrc is working but -l should be used for something in /etc/profile.d and .profile
-            return self.dkTunnel.ssh.runOutput(cmd)
+            out = self.dkTunnel.ssh.runOutput(cmd, log=log)
         elif self.ssh is not None:
-            return self.ssh.runOutput(cmd)
+            out = self.ssh.runOutput(cmd, log=log)
         else:
-            return subprocess.check_output(
+            out = subprocess.check_output(
                 cmd, shell=True, executable="/bin/bash"
             ).decode()
 
+        if log:
+            print("  -> output:%s" % (out))
+            
+        return out
+
+    # return os name of remote server
+    def getOS(self):
+        if self._os is None:
+            try:
+                osInfo = self.runOutput("cat /etc/os-release").lower()
+                if "ubuntu" in osInfo:
+                    self._os = "ubuntu"
+                elif "centos" in osInfo:
+                    self._os = "centos"
+                else:
+                    raise Exception("Unknown OS")
+
+            except Exception as e:
+                osInfo = self.runOutput("sw_vers")
+                osInfo = osInfo.lower()
+                if "mac os" in osInfo or "macos" in osInfo:
+                    self._os = "macos"
+                else:
+                    raise Exception("Unknown OS")
+
+            # print(f"========== remote os : {self._os} ==========")
+
+        return self._os
+
     # runOutput 래퍼 함수
     # os 별 ~/.profile 명령이 다르기 때문에 대응하기 위해
     def runOutputProf(self, cmd, expandVars=True):
-        os = self.remoteOs
-
-        tmpCmd = ". ~/."
+        os = self.getOS()
 
         if os == "ubuntu":
-            tmpCmd = tmpCmd + "profile"
+            profile = "profile"
         elif os == "centos":
-            tmpCmd = tmpCmd + "bash_profile"
-        tmpCmd = tmpCmd + " && "
-
-        cmd = tmpCmd + cmd
+            profile = "bash_profile"
+        elif os == "macos":
+            profile = "bash_profile"
+        else:
+            raise Exception(f"Unknown OS - {os}")
 
+        cmd = f". ~/.{profile} && " + cmd
         return self.runOutput(cmd, expandVars=expandVars)
 
     def runOutputAll(self, cmd, expandVars=True):
         """
         cmd: string or array
         expandVars:
         return: stdout and stderr string
         exception: subprocess.CalledProcessError(returncode, output)
         """
-        print("executeOutputAll on %s[%s].." % (self._serverName(), cmd))
+        ss = cmd[:100] + "..." if g_logLv == 0 and len(cmd) > 100 else cmd
+        self.log(f"runOutputAll [{ss}]")
 
         # if expandVars:
         #     cmd = strExpand(cmd, g_dic)
 
         if self.dkTunnel is not None:
             dkRunUser = "-u %s" % self.dkId if self.dkId is not None else ""
             cmd = str2arg(cmd)
@@ -541,25 +646,26 @@
         elif self.ssh is not None:
             return self.ssh.runOutputAll(cmd)
         else:
             return subprocess.check_output(
                 cmd, shell=True, stderr=subprocess.STDOUT, executable="/bin/bash"
             )
 
-    def _serverName(self):
-        if self.server is None:
-            return "local"
-        elif self.dkTunnel is None:
-            return f"{self.server.host}:{self.server.port}"
-        else:
-            return f"{self.dkName}[{self.server.host}:{self.server.port}]"
+    # def _serverName(self):
+    #     if self.server is None:
+    #         return "local"
+    #     elif self.dkTunnel is None:
+    #         return f"{self.server.host}:{self.server.port}"
+    #     else:
+    #         return f"{self.dkName}[{self.server.host}:{self.server.port}]"
 
     def run(self, cmd, expandVars=True, printLog=True):
         if printLog:
-            print(f"execute on {self._serverName()}[{cmd}]..")
+            ss = cmd[:100] + "..." if g_logLv == 0 and len(cmd) > 100 else cmd
+            self.log(f"run [{ss}]")
 
         # if expandVars:
         #     cmd = strExpand(cmd, g_dic)
 
         if self.dkTunnel is not None:
             # it하면 오류 난다
             dkRunUser = "-u %s" % self.dkId if self.dkId is not None else ""
@@ -599,52 +705,60 @@
                 p.communicate()
                 print("  -> ret:%d" % (p.returncode))
                 if p.returncode != 0:
                     raise subprocess.CalledProcessError(p.returncode, cmd)
 
     # runOutput 래퍼 함수
     # os 별 ~/.profile 명령이 다르기 때문에 대응하기 위해
-    def runProf(self, cmd, expandVars=True, printLog=True):
-        os = self.remoteOs
+    def runProf(self, cmd, expandVars=True):
+        os = self.getOS()
 
         tmpCmd = ". ~/."
 
         if os == "ubuntu":
             tmpCmd = tmpCmd + "profile"
         elif os == "centos":
             tmpCmd = tmpCmd + "bash_profile"
         tmpCmd = tmpCmd + " && "
 
         cmd = tmpCmd + cmd
-        self.run(cmd, expandVars=expandVars, printLog=printLog)
+        self.run(cmd, expandVars=expandVars)
 
     def runSafe(self, cmd):
         """
         return: success flag
         """
         try:
             self.run(cmd)
             return True
         except subprocess.CalledProcessError as e:
             print("run: failed %d\n -- %s\n" % (e.returncode, e.output))
             return False
 
     def uploadFile(self, src, dest):
-        self.onlyRemote()
+        """
+        support both local and remote
+        """
+        # self.onlyRemote()
         src = os.path.expanduser(src)
         dest = os.path.expanduser(dest)
-        pp = f"/tmp/upload-{g_main.uid}.tmp"
         if self.dkTunnel is not None:
+            # pp = f'/tmp/upload-{g_main.uid}.tmp'
+            pp = f"{self.tempPathGet()}/upload.tmp"
             self.dkTunnel.ssh.uploadFile(src, pp)
-            self.dkTunnel.ssh.run(f"sudo docker cp {pp} {self.dkName}:{dest}")
+            self.dkTunnel.ssh.run(
+                f"sudo docker cp {pp} {self.dkName}:{dest} && rm -f {pp}"
+            )
+        elif self.ssh is None:
+            self.run(f"cp {src} {dest}")
         else:
             self.ssh.uploadFile(src, dest)
 
     def uploadFileTo(self, src, dest):
-        self.onlyRemote()
+        # self.onlyRemote()
         src = os.path.expanduser(src)
         dest = os.path.expanduser(dest)
         pp = os.path.join(dest, os.path.basename(src))
         self.uploadFile(src, pp)
 
     def uploadFolder(self, src, dest):
         self.onlyRemote()
@@ -673,35 +787,41 @@
             self.ssh.uploadFolder(src, dest)
 
     def uploadFolderTo(self, src, dest):
         self.onlyRemote()
         self.ssh.uploadFolder(src, os.path.join(dest, os.path.basename(src)))
 
     def _helperRun(self, args, sudo=False):
-        pp2 = f"/tmp/gatHelper-{g_main.uid}.py"
+        # pp2 = f"{self.tempPathGet()}/gatHelper.py"
+        pp2 = f"/tmp/gatHelper.py"
         src = os.path.join(g_scriptPath, "gatHelper.py")
 
         if self.dkTunnel is None and self.ssh is None:
             shutil.copyfile(src, pp2)
         else:
             if not self._uploadHelper:
                 if self.dkTunnel is not None:
-                    self.dkTunnel.uploadFile(src, pp2)
-                    self.dkTunnel.ssh.run(f"sudo docker cp {pp2} {self.dkName}:{pp2}")
+                    pp3 = f"/tmp/gatHelperDk.py"
+                    self.dkTunnel.uploadFile(src, pp3)
+                    self.dkTunnel.ssh.run(
+                        f"sudo docker cp {pp3} {self.dkName}:{pp2} && rm -f {pp3}"
+                    )
                 else:
                     self.uploadFile(src, pp2)
 
                 self._uploadHelper = True
 
         # ss = str2arg(json.dumps(args, cls=ObjectEncoder))
         ss = json.dumps(args, cls=ObjectEncoder)
-        ss2 = zlib.compress(ss.encode())  # 1/3이나 절반 - 사이즈가 문제가 아니라 escape때문에
+        # 1/3이나 절반 - 사이즈가 문제가 아니라 escape때문에
+        ss2 = zlib.compress(ss.encode())
         ss = base64.b64encode(ss2).decode()
+        sudo = "sudo " if sudo else ""
         self.run(
-            '%spython3 %s runBin "%s"' % ("sudo " if sudo else "", pp2, ss),
+            f'{sudo}python3 {pp2} runBin "{ss}"',
             expandVars=False,
             printLog=False,
         )
 
     """ use myutil.makeUser
   def userNew(self, name, existOk=False, sshKey=False):
     print("task: userNew...")
@@ -709,38 +829,42 @@
     
     args = dict(cmd="userNew", dic=g_dic,
       name=name, existOk=existOk, sshKey=sshKey)
     self._helperRun(args, sudo=True)
   """
 
     def strLoad(self, path):
-        print("task: strLoad from[%s]..." % path)
+        self.log("task - strLoad from[%s]..." % path)
         self.onlyLocal()
 
         path = os.path.expanduser(path)
         with open(path, "rt") as fp:
             return fp.read()
 
     def strEnsure(self, path, str, sudo=False):
         """
         str이 없으면 추가한다
         """
-        print("task[%s]: strEnsure[%s] for %s..." % (self._serverName(), str, path))
+        self.log(f"task - strEnsure[{str}] for {path}...")
         self.onlyRemote()
 
         args = dict(cmd="strEnsure", dic=g_dic, path=path, str=str)
         self._helperRun(args, sudo)
 
     def configBlock(self, path, marker, block, insertAfter=None, sudo=False):
         """
         block이 보존한다(필요시 수정도)
         marker: ### {mark} TEST
         block: vv=1
         """
-        print(f"task: config block[{marker}] for {path}...\n[{block}]\n")
+
+        ss = f"task - config block[{marker}] for {path}...\n"
+        if g_logLv > 0:
+            ss += f"[{block}]\n"
+        self.log(ss)
         # self.onlyRemote()
 
         args = dict(
             cmd="configBlock",
             dic=g_dic,
             path=path,
             marker=marker,
@@ -749,75 +873,78 @@
         )
         self._helperRun(args, sudo)
 
     def configLine(self, path, regexp, line, items=None, sudo=False, append=False):
         """
         regexp에 부합되는 라인이 있을 경우 변경한다
         """
-        print("task: config line[%s] for %s..." % (line, path))
+        self.log("task - config line[%s] for %s..." % (line, path))
         # self.onlyRemote()
 
         args = dict(
             cmd="configLine",
             dic=g_dic,
             path=path,
             regexp=regexp,
             line=line,
             items=items,
             append=append,
         )
         self._helperRun(args, sudo)
 
     def s3List(self, env, bucket, prefix):
-        print("task: s3 list[%s/%s]..." % (bucket, prefix))
+        self.log("task - s3 list[%s/%s]..." % (bucket, prefix))
         self.onlyLocal()
 
         if not prefix.endswith("/"):
             prefix += "/"
 
         s3 = CoS3(env.config.get("s3.key", None), env.config.get("s3.secret", None))
         bb = s3.bucketGet(bucket)
         lst = bb.fileList(prefix)
         return lst
 
     def s3DownloadFiles(self, env, bucket, prefix, nameList, targetFolder):
-        print("task: s3 download files[%s/%s]..." % (bucket, prefix))
+        self.log("task - s3 download files[%s/%s]..." % (bucket, prefix))
         self.onlyLocal()
 
         if not targetFolder.endswith("/"):
             targetFolder += "/"
         if not prefix.endswith("/"):
             prefix += "/"
 
         s3 = CoS3(env.config.get("s3.key", None), env.config.get("s3.secret", None))
         bb = s3.bucketGet(bucket)
         for name in nameList:
             bb.downloadFile(prefix + name, targetFolder + name)
 
     def s3DownloadFile(self, env, bucket, key, dest=None):
-        print("task: s3 download file[%s -> %s]..." % (key, dest))
+        self.log("task - s3 download file[%s -> %s]..." % (key, dest))
         self.onlyLocal()
 
         s3 = CoS3(env.config.get("s3.key", None), env.config.get("s3.secret", None))
         bb = s3.bucketGet(bucket)
         return bb.downloadFile(key, dest)
 
     # ####################### 나중에 사용될 여지가 있다. ####################################
 
     # 패키지 install 함수 -> ubuntu, centos 지원
     def pkgInstall(self, sudo=False, options=[], packages=[]):
-        os = self.getOS()
         # sudo 권한 여부 확인 후 sudo 추가
         cmdSudo = "sudo " if sudo else ""
         # OS에 따라 패키지 매니저 추가
+        os = self.getOS()
         cmdPkgManager = None
         if os == "ubuntu":
             cmdPkgManager = "apt-get"
         elif os == "centos":
             cmdPkgManager = "yum"
+        else:
+            raise Exception(f"Unknown OS - {os}")
+
         # 해당 옵션을 운영체제에 알맞게 매핑
         optionList = self._mapOptionToOs(os=os, options=options)
         cmdOption = " ".join(optionList)
         # 해당 OS에 알맞게 패키지명 매핑
         packageList = self._mapPackageToOs(os=os, packages=packages)
         cmdPackage = " ".join(packageList)
         # 명령어 실행
@@ -870,31 +997,14 @@
         # 프로그램 정지 명령어
         cmdPkgStop = None
         pkg = self._mapPackageToOs(os=os, packages=package)
         cmdPkgStop = f"systemctl restart {pkg}"
         cmd = f"{cmdSudo}{cmdPkgStop}"
         self.run(cmd)
 
-    # Tasks 초기화는 보통 로컬에서 진행 -> 전역으로 두면 에러
-    # 매번 호출해주는게 바람직할듯
-    def getOS(self):
-        try:
-            with open("/etc/os-release") as file:
-                for line in file:
-                    if line.startswith("NAME="):
-                        os_name = line.strip().split("=")[1].replace('"', "")
-                        if "ubuntu" in os_name.lower():
-                            return "ubuntu"
-                        elif "centos" in os_name.lower():
-                            return "centos"
-                        else:
-                            raise Exception("Unknown OS")
-        except Exception as e:
-            print(f"Error detecting OS: {e}")
-
     # 옵션 인자를 OS에 맞춰서 매핑
     def _mapOptionToOs(self, os="", options=[]):
         global g_options
         optionList = []
         for option in options:
             if g_options.__contains__(option):
                 if os == "ubuntu":
@@ -998,15 +1108,17 @@
 
 
 import socket
 
 
 class Main:
     def __init__(self):
-        self.uid = socket.gethostname() + "-" + str(os.getpid())
+        # self.uid = socket.gethostname() + "-" + str(os.getpid())
+        # self.workPath = f"/tmp/"
+        pass
 
     # runTask와 doServerStep등은 Task말고 별도로 빼자 remote.runTask를 호출할일은 없으니까
     def runTask(self, mygat):
         # self.onlyLocal()
 
         if hasattr(mygat, "getRunCmd"):
             cmd = mygat.getRunCmd(util=g_util, local=g_local, remote=g_remote)
@@ -1095,72 +1207,48 @@
 
                 if g_util.isRestart:
                     g_util.isRestart = False
                     p.terminate()
                     break
 
     def buildTask(self, mygat):
-        print("run: building the app")
+        llw("buildTask: building the app")
         if hasattr(mygat, "buildTask"):
             return mygat.buildTask(util=g_util, local=g_local, remote=g_remote)
         else:
-            print("You should override buildTask method.")
+            lle("You should override buildTask method.")
 
-    # def taskSetup(self, target, serverName, subCmd):
     def taskSetup(self, server, subCmd, mygat, config):
-        # if not os.path.exists(target):
-        #     print("There is no target file[%s]" % target)
-        #     return
-
-        # server = g_config.configServerGet(serverName)
-        # if server is None:
-        #     return
+        llw("taskSetup: setting up the app...")
 
         # deprecated
-        # server["runImage"] = runImageFlag
         if subCmd not in ["run", "dev", "prod", "full", "init", ""]:
             raise Exception(f"Invalid sub command[{subCmd}] for setup task")
 
-        # global g_remote, g_data
-        # g_remote = Tasks(server)
-        # g_remote.runFlag = subCmd == "run"
-        # g_remote.runImageFlag = g_remote.runFlag  # deprecated
-        # g_remote.fullFlag = subCmd == "full"
-        # if "dkName" in server.dic:
-        #     g_remote = g_remote.dockerConn(server.dkName, dkId=server.get("dkId"))
-
-        env = Tasks(server, config)
+        env = Conn(server, config)
         if "dkName" in server.dic:
             env = env.dockerConn(server.dkName, dkId=server.get("dkId"))
 
-        # print("\n\n\n\nhahahaha")
         # print(env.config)
-        # print("\n\n\n\n")
 
         env.runFlag = False
         env.runProfile = None
         if subCmd in ["dev", "prod", "run"]:
             env.runFlag = True
             if subCmd != "run":
                 env.runProfile = subCmd
 
-        # env.runImageFlag = env.runFlag  # deprecated
-
         env.fullFlag = subCmd == "full"
         env.initFlag = subCmd == "init"
 
-        # g_remote.data = g_data
-        # g_remote.util = g_util
         dicInit(server)
-
-        # expand env and variables
         expandVar(config)
 
         if not hasattr(mygat, "setupTask"):
-            print("setup: You should override setupTask function in your myGat class")
+            lle("setup: You should override setupTask function in your myGat class")
             return
 
         # 1. 원격 repo에서 특정 브렌치의 최신 커밋 받기
         # 2. 기존 clone 이 최신인지 판단하고 최신이 아니면 삭제후 다시 클론
         # recentCommit = getRemoteRecentCommit(config=config)
         # directory = os.getcwd() + "/clone"
         # print(directory)
@@ -1224,55 +1312,55 @@
     # localSrcPath 를 뒤에 둔 이유는 기본 값이 필요해서 + 이 함수를 사용하는 다른 곳에서 인자 위치로 인한 에러
     def targetFileListProd(
         self, include, exclude, func, localSrcPath="", followLinks=True
     ):
         for pp in include:
             if type(pp) == str:
                 if pp == "*":
-                    pp = ""
+                    pp = "."
 
                 # daemon
                 pp = _pathExpand(pp)
                 pp = os.path.join(localSrcPath, pp)
 
                 p = pathlib.Path(pp)
                 if not p.exists():
-                    print(f"target: not exists - {pp}")
+                    llw(f"targetList: not exists - {pp}")
                     continue
 
                 if p.is_dir():
                     if _excludeFilter(exclude, pp):
-                        print(f"target: skip - {pp}")
+                        lld(f"targetList: skip - {pp}")
                         continue
 
                     for folder, dirs, files in os.walk(pp, followlinks=followLinks):
                         # filtering dirs too
                         dirs2 = []
                         for d in dirs:
                             dd = os.path.join(folder, d)
                             if _excludeFilter(exclude, dd):
-                                print(f"target: skip - {dd}")
+                                lld(f"targetList: skip - {dd}")
                                 continue
 
                             dirs2.append(d)
 
                         dirs[:] = dirs2  # 이걸 변경하면 다음 files가 바뀌나?
 
                         for ff in files:
                             # _zipAdd(os.path.join(folder, ff), os.path.join(folder, ff))
                             full = os.path.join(folder, ff)
                             if _excludeFilter(exclude, full):
-                                print(f"target: skip - {full}")
+                                lld(f"targetList: skip - {full}")
                                 continue
 
                             func(full, None)
                 else:
                     # _zipAdd(pp, pp)
                     if _excludeFilter(exclude, pp):
-                        print(f"target: skip - {pp}")
+                        lld(f"targetList: skip - {pp}")
                         continue
 
                     func(pp, None)
 
             else:
                 src = pp["src"]
                 src = _pathExpand(src)
@@ -1283,26 +1371,27 @@
                     exclude2 = pp["exclude"]
 
                 for folder, dirs, files in os.walk(src):
                     for ff in files:
                         localPath = os.path.join(folder, ff)
                         localPath = pathRemove(localPath, src)
                         if _excludeFilter(exclude2, localPath):
-                            print(f"target: skip - {os.path.join(folder, ff)}")
+                            lld(f"targetList: skip - {os.path.join(folder, ff)}")
                             continue
 
                         # _zipAdd(os.path.join(folder, ff), os.path.join(dest, cutpath(src, folder), ff))
                         func(
                             os.path.join(folder, ff),
                             os.path.join(dest, cutpath(src, folder), ff),
                         )
 
-    # def taskDeploy(self, env, server, mygat, config):
     def taskDeploy(self, server, mygat, config):
-        env = Tasks(server, config)
+        llw("taskDeploy: deploy the app...")
+
+        env = Conn(server, config)
         if "dkName" in server.dic:
             env = env.dockerConn(server.dkName, dkId=server.get("dkId"))
 
         self.buildTask(mygat)
 
         dicInit(server)
         # expand env and variables
@@ -1310,14 +1399,15 @@
 
         sudoCmd = ""
         if "owner" in server:
             sudoCmd = "sudo"
 
         # name = config.name
         deployRoot = server.deployRoot
+        env.run(f"mkdir -p {deployRoot}")
         realTarget = env.runOutput("realpath %s" % deployRoot)
         realTarget = realTarget.strip("\r\n")  # for sftp
         todayName = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")[2:]
 
         # pre task
         deployPath = os.path.join(realTarget, "releases", todayName)
         g_dic.dic["deployRoot"] = deployRoot
@@ -1337,32 +1427,27 @@
         releases = list(
             filter(lambda x: re.match("\d{6}_\d{6}", x) is not None, res.split())
         )
         releases.sort()
 
         max = config.deploy.maxRelease - 1
         cnt = len(releases)
-        print(f"deploy: releases folders count is {cnt}")
+        llw(f"taskDeploy: releases folders count is {cnt}")
         if cnt > max:
-            print(f"deploy: remove old {cnt - max} folders")
+            llw(f"taskDeploy: remove old {cnt - max} folders")
             removeList = releases[: cnt - max]
             for ff in removeList:
                 env.runOutput(f"{sudoCmd} rm -rf {deployRoot}/releases/{ff}")
 
         # if deploy / owner is defined,
         # create release folder as ssh user, upload, extract then change release folder to deploy / owner
-        res = env.runOutput(
-            f"cd {deployRoot}/releases"
-            + f"&& {sudoCmd} mkdir {todayName}"
-            + (
-                f"&& sudo chown {server.owner}: {todayName}"
-                if "owner" in server
-                else ""
-            )
-        )
+        cmd = f"cd {deployRoot}/releases && {sudoCmd} mkdir {todayName}"
+        if "owner" in server:
+            cmd += f" && {sudoCmd} chown {server.owner}: {todayName}"
+        res = env.runOutput(cmd)
 
         # upload files
         include = config.deploy.include
         exclude = config.get("deploy.exclude", [])
         sharedLinks = config.get("deploy.sharedLinks", [])
 
         def zipProcess(env, include, exclude, localSrcPath):
@@ -1373,15 +1458,15 @@
                     # if _filterFunc(srcP, exclude):
                     #     print(f"deploy: skip - {srcP}")
                     #     return
 
                     # make "./aaa" -> "aaa"
                     targetP = os.path.normpath(targetP)
 
-                    print(f"zipping {srcP} -> {targetP}")
+                    lld(f"zipping {srcP} -> {targetP}")
                     zipWork.write(srcP, targetP, compress_type=zipfile.ZIP_DEFLATED)
 
                 # dic = dict(name=config.name)
                 # def _pathExpand(pp):
                 #     pp = os.path.expanduser(pp)
                 #     return strExpand(pp, dic)
 
@@ -1395,79 +1480,87 @@
                     include,
                     exclude,
                     _fileProc,
                     localSrcPath=localSrcPath,
                     followLinks=config.deploy.followLinks,
                 )
 
-            env.uploadFile(
-                zipPath, "/tmp/gatUploadPkg.zip"
-            )  # we don't include it by default
+            # we don't include it by default
+            env.uploadFile(zipPath, "/tmp/gatUploadPkg.zip")
+            os.remove(zipPath)
             env.run(
                 f"cd {deployRoot}/releases/{todayName} "
                 + f"&& {sudoCmd} unzip /tmp/gatUploadPkg.zip && {sudoCmd} rm /tmp/gatUploadPkg.zip"
             )
-            os.remove(zipPath)
 
         strategy = g_config.deploy.strategy
         # workPath = env.config.srcPath
-        workPath = g_config.srcPath  # deployApp으로 온 경우 env.config가 새로 만들어진다
-        if strategy == "zip":
-            zipProcess(env, include, exclude, workPath)
-
-        elif strategy == "git":
-            # 여기 path는 git clone을 받을 주소
-            # 나중에 따로 god_app.py에서 설정하도록 하면 코드가 더욱 좋아질거라 예상
-            cloneRepo(g_config.deploy.gitRepo, server.gitBranch, workPath)
-            zipProcess(env, include, exclude, workPath)
-
-            """	no use copy strategy anymore
-      elif strategy == "copy":
-        ssh.uploadFile(config.name, os.path.join(realTargetFull, config.name))	# we don't include it by default
-        ssh.run("chmod 755 %s/%s" % (realTargetFull, config.name))
+        workPath = g_config.srcPath
 
-        ssh.uploadFilterFunc = _filterFunc
+        old = os.path.abspath(os.curdir)
+        try:
+            # 아예 해당 폴더로 가서 생성한다
+            os.chdir(workPath)
+            workPath = ""
+
+            # deployApp으로 온 경우 env.config가 새로 만들어진다
+            if strategy == "zip":
+                zipProcess(env, include, exclude, workPath)
+
+            elif strategy == "git":
+                # 여기 path는 git clone을 받을 주소
+                # 나중에 따로 god_app.py에서 설정하도록 하면 코드가 더욱 좋아질거라 예상
+                cloneRepo(g_config.deploy.gitRepo, server.gitBranch, workPath)
+                zipProcess(env, include, exclude, workPath)
+
+                """	no use copy strategy anymore
+        elif strategy == "copy":
+            ssh.uploadFile(config.name, os.path.join(realTargetFull, config.name))	# we don't include it by default
+            ssh.run("chmod 755 %s/%s" % (realTargetFull, config.name))
 
-        for pp in include:
-          if type(pp) == str:
-            if pp == "*":
-              pp = "."
-            
-            # daemon
-            pp = pp.replace("${name}", config.name)
-                        
-            p = pathlib.Path(pp)
-            if not p.exists():
-              print("deploy: not exists - %s" % pp)
-              continue
-            
-            if p.is_dir():
-              tt = os.path.join(realTargetFull, pp)
-              ssh.uploadFolder(pp, tt)
-            else: 
-              ssh.uploadFileTo(pp, realTargetFull)
-          else:
-            src = pp["src"]
-            target = pp["target"]
-            tt = os.path.join(realTargetFull, target)
-            ssh.uploadFolder(src, tt)
-      """
-        else:
-            raise Exception(f"unknown strategy[{strategy}]")
+            ssh.uploadFilterFunc = _filterFunc
+
+            for pp in include:
+            if type(pp) == str:
+                if pp == "*":
+                  pp = "."
+                
+                # daemon
+                pp = pp.replace("${name}", config.name)
+                            
+                p = pathlib.Path(pp)
+                if not p.exists():
+                print("deploy: not exists - %s" % pp)
+                continue
+                
+                if p.is_dir():
+                tt = os.path.join(realTargetFull, pp)
+                ssh.uploadFolder(pp, tt)
+                else: 
+                ssh.uploadFileTo(pp, realTargetFull)
+            else:
+                src = pp["src"]
+                target = pp["target"]
+                tt = os.path.join(realTargetFull, target)
+                ssh.uploadFolder(src, tt)
+        """
+            else:
+                raise Exception(f"unknown strategy[{strategy}]")
+        finally:
+            os.chdir(old)
 
         # shared links
         for pp in sharedLinks:
-            print(f"deploy: sharedLinks - {pp}")
+            lld(f"taskDeploy: sharedLinks - {pp}")
             if pp.endswith("/"):
                 env.run(f"cd {deployRoot} && {sudoCmd} mkdir -p shared/{pp} ")
                 pp = pp[:-1]
 
             env.run(
-                "%s ln -rsf %s/shared/%s %s/releases/%s/%s"
-                % (sudoCmd, deployRoot, pp, deployRoot, todayName, pp)
+                f"{sudoCmd} ln -rsf {deployRoot}/shared/{pp} {deployRoot}/releases/{todayName}/{pp}"
             )
 
             # ssh user용으로 변경해놔야 post process에서 쉽게 접근 가능
             if "owner" in server:
                 env.run(
                     f"cd {deployRoot} && sudo chown {server.get('dkId', server.id)}: releases/{todayName} shared -R"
                 )
@@ -1496,15 +1589,15 @@
 def initSamples(type, fn):
     with open(fn, "w") as fp:
         if type == "app":
             fp.write(sampleApp)
         else:
             fp.write(sampleSys)
 
-    print(
+    llw(
         "init: %s file generated. You should modify that file for your environment before service or deployment."
         % (fn)
     )
 
 
 def expandVar(dic):
     dicType = type(dic)
@@ -1533,41 +1626,36 @@
             elif tt == list:
                 expandVar(value)
 
 
 class Config(Dict2):
     def __init__(self):
         super().__init__()
+        self.dic["srcPath"] = "."
 
     def configStr(self, cfgType, ss):
         """
         type: yaml
         """
         if cfgType == "yaml":
             try:
-                # self.cfg = Dict2()
                 self.fill(yaml.safe_load(ss))
-                # g_util.config = g_config
 
                 if "defaultVars" in self:
                     for server in self.servers:
-                        # vars2 = Dict2()
-                        # vars2.fill(self.defaultVars)
-                        # vars2.fill(server.vars)
-                        # server.vars = vars2
-                        server.vars = dictMerge2(self.defaultVars, server.vars)
+                        server.vars = dict2Merge(self.defaultVars, server.vars)
 
                 if self.type == "app":
                     if "followLinks" not in self.deploy:
                         self.deploy["followLinks"] = False
 
             except yaml.YAMLError as e:
                 raise e
         else:
-            raise Exception("unknown config type[%s]" % cfgType)
+            raise Exception(f"unknown config type[{cfgType}]")
 
     def configFile(self, cfgType, pp):
         """
         type: yaml
         """
         with open(pp, "r") as fp:
             self.configStr(cfgType, fp.read())
@@ -1600,19 +1688,19 @@
     def configGet(self):
         return self.config.configGet()
 
     def loadData(self, pp):
         if not os.path.exists(pp):
             raise Exception(f"there is no data file[{pp}]")
 
-        print(f"load data from {pp}...")
+        print(f"init: load data from {pp}...")
         # TODO: encrypt with input key when changed
         with open(pp, "r") as fp:
             dd = Dict2(yaml.safe_load(fp.read()))
-            print("data -", dd)
+            # print("data -", dd)
             return dd
 
 
 # g_helper = Helper()
 g_config = Config()
 g_main = Main()
 # g_config = Dict2()	# py코드에서는 util.cfg로 접근 가능
@@ -1632,282 +1720,358 @@
     print(
         """\
 Usage.
 gat init app - Generates gat_app.py file for application.
 gat init sys SYSTEM_NAME - Generates the file for system.
   the SYSTEM_NAME.py file will be generated.
 
-For application(There should be gat_app.py file.),
+For application(a gat_app.py file should be exist),
 gat - Serves application.
-gat test - running automatic test.
-gat PROFILE_NAME deploy - Deploy the application to the server.
+gat test - Runs automatic test.
+
+For deployment(a gat_app.py file should be exist),
+gat SERVER_NAME deploy - Deploy the application to the server.
 
-gat PROFILE_NAME setup - Setup task.
-gat PROFILE_NAME run - Run system.
+For setup task(a gat_app.py file should be exist),
+gat SERVER_NAME setup - Setups environment.
+gat SERVER_NAME run - Setup and Run the system.
 
-For system,
-gat SYSTEM_NAME PROFILE_NAME - Setup server defined in GAT_FILE.
+For system(GAT_FILE_NAME.py file should be exist),
+gat GAT_FILE_NAME SERVER_NAME - Setup server defined in GAT_FILE.
 """
     )
     if target is not None:
         print(f"\nThere is no {target} script file.")
 
 
-def main():
-    global g_cwd, g_scriptPath, g_mygat
-    g_cwd = os.getcwd()
-    g_scriptPath = os.path.dirname(os.path.realpath(__file__))
-    target = "gat_app.py"
+class MyArgv:
+    def __init__(self, argv, fileExists=None):
+        self.gatName = "gat_app.py"
+        self.serverName = ""
+        self.opts = []  # -v, --git, --zip
+        self.cmd = ""  # help, init | deploy, setup, run
+        self.args = []  # arguments
+
+        if fileExists is None:
+            fileExists = os.path.exists
+
+        removeIdxs = []
+        for i in range(len(argv)):
+            arg = argv[i]
+            if arg.startswith("-"):
+                self.opts.append(arg)
+                removeIdxs.append(i)
+        for i in reversed(removeIdxs):
+            argv.pop(i)
+
+        if "--help" in self.opts:
+            self.opts.remove("--help")
+            self.cmd = "help"
+            return
 
-    cnt = len(sys.argv)
-    cmd = None
-    # setup or run의 argv를 받기 위한 변수
-    manualStrategyValue = None
-    if cnt > 1:
-        cmd = sys.argv[1]
+        if len(argv) == 0:
+            raise Exception("missing gat command")
 
-        if cmd == "help" or cmd == "--help":
-            help(None)
+        self.cmd = argv[0]
+        if self.cmd == "help":
             return
+        elif self.cmd == "init":
+            if len(argv) < 2:
+                raise Exception("gat init app OR gat init sys FILE_NAME.")
+            self.args.append(argv[1])
+            if self.args[-1] == "sys":
+                if len(argv) < 3:
+                    raise Exception(
+                        "Please specify target file name to be generated.\n$ gat init sys FILE_NAME"
+                    )
 
-        elif cmd == "init":
-            if cnt < 3:
-                print("gat init app OR gat init sys NAME.")
-                return
+                self.args.append(argv[2])
+            return
+        # elif self.cmd == "test":
+        #     return
+        # elif self.cmd == "serve":
+        #     return
 
-            type = sys.argv[2]
-            if type != "app" and type != "sys":
-                print("app or sys can be used for gat init command.")
-                return
+        # 이제 용법은
+        # gat SERVER_NAME CMD - gat파일은 gat_app.py로 고정
 
-            if type == "app":
-                initSamples(type, "gat_app.py")
+        # gat파일 명시
+        # gat GAT_FILE SERVER_NAME CMD
+        # gat GAT_FILE SERVER_NAME - cmd는 setup
+        # gat GAT_FILE CMD - server 하나
+        # gat GAT_FILE - server하나, CMD는 setup -- 시스템용
+
+        # xxx gat CMD - gat_app.py, server 하나
+
+        # SERVER_NAME에는 아래 예약된 명령어는 못쓴다
+        cmds = ["deploy", "setup", "run"]
+
+        pt = 0
+        name = argv[pt]
+        if not name.endswith(".py"):
+            name += ".py"
+        if fileExists(name):
+            self.gatName = name
+            pt += 1
+
+        # if pt >= len(argv):
+        #     raise Exception("Please specify SERVER_NAME")
+        if pt == len(argv):
+            self.cmd = "setup"
+            return
 
-            elif type == "sys":
-                if cnt < 4:
-                    print("Please specify Target file name to be generated.")
-                    return
+        arg1 = argv[pt]
+        if arg1 in cmds:
+            self.cmd = arg1
+            pt += 1
+            # if pt >= len(argv):
+            #     raise Exception("No more arguments")
+            return
 
-                target = sys.argv[3]
-                if not target.endswith(".py"):
-                    target += ".py"
-                initSamples(type, target)
+        self.serverName = arg1
+        pt += 1
 
-            else:
-                print("unknown init type[%s]" % type)
+        if pt >= len(argv):
+            self.cmd = "setup"
+            # raise Exception("Please specify CMD")
+        else:
+            self.cmd = argv[pt]
 
-            return
+        return
 
-        elif cmd == "test":
-            pass
 
-        elif cmd == "serve":
-            pass
+def testMyArgv():
+    argv = ["help"]
+    aa = MyArgv(argv)
+    assert aa.cmd == "help"
+
+    argv = ["init", "app"]
+    aa = MyArgv(argv)
+    assert aa.cmd == "init"
+    assert aa.args == ["app"]
+
+    argv = ["init", "sys", "test"]
+    aa = MyArgv(argv)
+    assert aa.cmd == "init"
+    assert aa.args == ["sys", "test"]
+
+    try:
+        argv = ["init", "sys"]
+        aa = MyArgv(argv)
+        assert False
+    except Exception as e:
+        pass
+
+    # gat GAT_FILE [SERVER_NAME] [CMD]
+    argv = ["gat2", "ser1", "run"]
+    aa = MyArgv(argv, fileExists=lambda x: x == "gat2.py")
+    assert aa.gatName == "gat2.py"
+    assert aa.serverName == "ser1"
+    assert aa.cmd == "run"
+
+    argv = ["gat2", "ser1"]
+    aa = MyArgv(argv, fileExists=lambda x: x == "gat2.py")
+    assert aa.gatName == "gat2.py"
+    assert aa.serverName == "ser1"
+    assert aa.cmd == "setup"
+
+    argv = ["gat2", "run"]
+    aa = MyArgv(argv, fileExists=lambda x: x == "gat2.py")
+    assert aa.gatName == "gat2.py"
+    assert aa.serverName == ""
+    assert aa.cmd == "run"
+
+    argv = ["gat2.py", "deploy"]
+    aa = MyArgv(argv, fileExists=lambda x: x == "gat2.py")
+    assert aa.gatName == "gat2.py"
+    assert aa.serverName == ""
+    assert aa.cmd == "deploy"
+
+    argv = ["gat2"]
+    aa = MyArgv(argv, fileExists=lambda x: x == "gat2.py")
+    assert aa.gatName == "gat2.py"
+    assert aa.serverName == ""
+    assert aa.cmd == "setup"
+
+    # gat SERVER_NAME CMD
+    argv = ["prod", "run"]
+    aa = MyArgv(argv)
+    assert aa.gatName == "gat_app.py"
+    assert aa.serverName == "prod"
+    assert aa.cmd == "run"
 
-        # deploy도 아래 system 문법으로
-        # elif cmd == "deploy":
-        #     pass
+    print("test ok")
 
-        else:
-            # 로칼에 gat_app.py가 있으면 configName생략 모드
-            if not os.path.exists(target):
-                target = None
-
-            # setup server system or deploy
-            cmd = "system"
-            if cnt < 2:
-                # can skip SERVER_NAME(if there is only one target), cmd(default setup)
-                print("gat [CONFIG_NAME] [SERVER_NAME] [run|deploy|init|SETUP]")
-                return
 
-            p = 1
-            if target is None:
-                target = sys.argv[p]
-                if not target.endswith(".py"):
-                    target += ".py"
-                p += 1
-
-            runCmd = None
-            serverName = None
-            if cnt > p:
-                second = sys.argv[p]
-                # print(f"second:{second}")
-                if second in ["run", "deploy", "init", "setup"]:
-                    runCmd = second
-                else:
-                    # 아니면 Server이름
-                    serverName = second
-                p += 1
-
-                # print(f"cnt:{cnt}, p:{p}")
-                if cnt > p:
-                    if runCmd is not None:
-                        serverName = runCmd
-                    runCmd = sys.argv[p]
-                else:
-                    runCmd = "setup"
+def main():
+    mainDo()
 
-                print(f"target2 -- {runCmd}, {serverName}")
+    for conn in reversed(g_connList):
+        conn.clearConn()
 
-            else:
-                runCmd = "setup"
 
-            # strategy 분기
-            p += 1
-            if (runCmd == "setup" or runCmd == "run") and cnt - 1 == p:
-                print(f"========== 명령어 확인 : {sys.argv[p]} ==========")
-                if sys.argv[p] == "--git":
-                    manualStrategyValue = "git"
-                    # g_config.deploy.strategy = argv
-                elif sys.argv[p] == "--zip":
-                    manualStrategyValue = "zip"
-                    # g_config.deploy.strategy = argv
-                else:
-                    raise Exception(f"{manualStrategyValue}는 올바르지 않은 명령어입니다.")
+def mainDo():
+    # testMyArgv()
+    # return
 
-    else:
-        print("missing gat command")
+    ma = MyArgv(sys.argv[1:])
+    if ma.cmd == "help":
+        help(None)
         return
+    elif ma.cmd == "init":
+        if len(ma.args) == 0:
+            lle("gat init app OR gat init sys FILE_NAME.")
+            return
+
+        type = ma.args[0]
+        if type != "app" and type != "sys":
+            lle("app or sys can be used for gat init command.")
+            return
+
+        if type == "app":
+            initSamples(type, "gat_app.py")
+        else:
+            if len(ma.args) < 2:
+                lle("Please specify target file name to be generated.")
+                return
+
+            target = ma.args[1]
+            if not target.endswith(".py"):
+                target += ".py"
+            initSamples(type, target)
 
-    # check first
-    if not os.path.exists(target):  # or not os.path.exists("gat.yml"):
-        help(target)
         return
 
+    global g_cwd, g_scriptPath, g_mygat
+    g_cwd = os.getcwd()
+    g_scriptPath = os.path.dirname(os.path.realpath(__file__))
+    deployStrategy = None
+
     global g_config
     helper = Helper(g_config)
     sys.path.append(g_cwd)
-    mymod = __import__(target[:-3], fromlist=[""])
+    pyFileName = ma.gatName[:-3]
+    mymod = __import__(pyFileName, fromlist=[""])
     g_mygat = mymod.myGat(helper=helper)
     # g_config 객체 생성 지점 -> 여기부터 설정 객체 사용 가능
-    if manualStrategyValue is not None:
-        g_config.deploy.strategy = manualStrategyValue
 
-    print("gat-tool V%s" % __version__)
+    cprint(f"gat-tool V{__version__}", "green")
     name = g_config.name
     type = g_config.get("type", "app")
-
-    print("** config[type:%s, name:%s]" % (type, name))
+    srcPath = g_config.srcPath
 
     # load secret - 이걸 mygat init하는데서 수동으로 하게해놨는데..
     # 무조건 로드하게하고 추가 로드를 할수 있게할까? - 좀 애매하다
     global g_data
-    # secretPath = os.path.join(g_cwd, ".data.yml")
-    # if os.path.exists(secretPath):
-    #     print("load data...")
-    #     # TODO: encrypt with input key when changed
-    #     with open(secretPath, "r") as fp:
-    #         ss = fp.read()
-    #         g_data = Dict2(yaml.safe_load(ss))
-    #         print("data - ", g_data)
-    # if g_mygat.data is not None:
     if hasattr(g_mygat, "data"):
         g_data = g_mygat.data
 
     global g_local
-    g_local = Tasks(None, g_config)
-    # g_local.util = g_util
+    g_local = Conn(None, g_config)
+    if not os.path.exists(ma.gatName):  # or not os.path.exists("gat.yml"):
+        help(ma.gatName)
+        return
 
-    g_config.srcPath = "."
-    if cmd != "system":
-        strategy = g_config.deploy.strategy
-        if strategy == "git":
-            g_config.srcPath = "./clone"
+    print(f"** config[type:{type} name:{name} srcPath:{srcPath} cmd:{ma.cmd}]")
 
-    def checkServerName(serverName):
-        """
-        return: none(error), str(new serverName)
-        """
-        if serverName is None:
-            if len(g_config.servers) == 0:
-                print("\nThere is no server definition.")
-                return
+    if ma.cmd == "test":
+        # serve
+        if type != "app":
+            lle("just gat command can be used for application type only.")
+            return
+        g_main.taskTest()
 
-            if len(g_config.servers) == 1:
-                serverName = g_config.servers[0].name
+    elif ma.cmd == "serve":
+        # serve
+        if type != "app":
+            lle("just gat command can be used for application type only.")
+            return
+        g_main.taskServe()
 
+    else:
+        if ma.cmd not in ["run", "setup", "deploy"]:
+            raise Exception(f"Invalid command[{ma.cmd}]")
+
+        for opt in ma.opts:
+            if opt == "-v":
+                global g_logLv
+                g_logLv = 1
+            elif opt == "-f":
+                global g_force
+                g_force = True
+            elif opt == "--git":
+                deployStrategy = "git"
+            elif opt == "--zip":
+                deployStrategy = "zip"
             else:
-                ss = ""
-                for it in g_config.servers:
-                    ss += it["name"] + "|"
-                print(
-                    f"\nPlease specify the sever name is no server definition.[{ss[:-1]}]"
-                )
-                return
+                raise Exception(f"unknown option[{opt}]")
 
-        else:
-            serverFound = False
-            for it in g_config.servers:
-                if it.name == serverName:
-                    serverFound = True
-            if not serverFound:
-                ss = ""
+        def checkServerName(serverName):
+            """
+            return: none(error), str(new serverName)
+            """
+            if serverName == "":
+                if len(g_config.servers) == 0:
+                    lle("\nThere is no server definition.")
+                    return
+
+                if len(g_config.servers) == 1:
+                    serverName = g_config.servers[0].name
+
+                else:
+                    ss = ""
+                    for it in g_config.servers:
+                        ss += it["name"] + "|"
+                    s2 = ss[:-1]
+                    lle(
+                        f"\nPlease specify the sever name is no server definition.[{s2}]"
+                    )
+                    return
+
+            else:
+                serverFound = False
                 for it in g_config.servers:
-                    ss += it.name + "|"
+                    if it.name == serverName:
+                        serverFound = True
+                if not serverFound:
+                    ss = ""
+                    for it in g_config.servers:
+                        ss += it.name + "|"
 
-                print(f"There is no server[{serverName}] in {ss[:-1]}")
-                return
-        return serverName
+                    lle(f"There is no server[{serverName}] in {ss[:-1]}")
+                    return
+            return serverName
+
+        if deployStrategy is not None:
+            g_config.deploy.strategy = deployStrategy
 
-    if cmd == "system":
-        if runCmd == "deploy":
-            # g_util.deployOwner = g_config.get("deploy.owner", None)	# replaced by server.owner
-            # serverName = sys.argv[2] if cnt > 2 else None
-            # if serverName is None:
-            #     if len(g_config.servers) == 1:
-            #         serverName = g_config.servers[0]["name"]
-            #     else:
-            #         ss = ""
-            #         for it in g_config.servers:
-            #             ss += it["name"] + "|"
-            #         print(f"\nPlease specify server name.[{ss[:-1]}]")
-            #         return
-            serverName = checkServerName(serverName)
+        # g_config.srcPath = "."
+        # if cmd != "system":
+        #     strategy = g_config.deploy.strategy
+        #     if strategy == "git":
+        #         g_config.srcPath = "./clone"
+        if "deploy" in g_config and g_config.deploy.strategy == "git":
+            g_config.srcPath = "./clone"
+
+        if ma.cmd == "deploy":
+            serverName = checkServerName(ma.serverName)
             if serverName is None:
                 return
 
             server = g_config.configServerGet(serverName)
-
-            # env = Tasks(server)
-            # if "dkName" in server.dic:
-            #     env = env.dockerConn(server.dkName, dkId=server.get("dkId"))
-
-            # g_main.taskDeploy(env, server, g_mygat, g_config)
             g_main.taskDeploy(server, g_mygat, g_config)
             return
 
-        subCmd = ""
-        if runCmd in ["run", "full", "init"]:
-            subCmd = runCmd
+        subCmd = "run" if ma.cmd == "run" else ""
 
-        serverName = checkServerName(serverName)
+        serverName = checkServerName(ma.serverName)
         if serverName is None:
             return
 
-        print(f"systemSetup - target:{target}, server:{serverName}, subCmd:{subCmd}")
+        llw(f"systemSetup - target:{ma.gatName}, server:{serverName}, subCmd:{subCmd}")
         server = g_config.configServerGet(serverName)
 
         g_main.taskSetup(server, subCmd, g_mygat, g_config)
-        return
-
-    elif cmd == "test":
-        # serve
-        if type != "app":
-            print("just gat command can be used for application type only.")
-            return
-
-        g_main.taskTest()
-
-    elif cmd == "serve":
-        # serve
-        if type != "app":
-            print("just gat command can be used for application type only.")
-            return
-
-        g_main.taskServe()
-
-    else:
-        print("unknown command mode[%s]" % cmd)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `god-tool-0.8.1/gat/gatHelper.py` & `god_tool-0.9.0/gat/gatHelper.py`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/gat/myutil.py` & `god_tool-0.9.0/gat/myutil.py`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/gat/plugin.py` & `god_tool-0.9.0/gat/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,29 +354,56 @@
     domain,
     prot="https",
     port=80,
     name="next",
     proxy="next:9000",
     nginxCfgPath="/data/nginx",
     localBind=False,
+    selfSign=False,  # true: 사설 인증서 사용
+    selfSignPort=443,
 ):
     # https://www.reddit.com/r/selfhosted/comments/rvqv3l/nextcloud_behind_nginx_proxy_manager_nextcloud
     # https://github.com/nextcloud/docker/blob/master/.examples/docker-compose/insecure/mariadb/fpm/web/nginx.conf
 
     listen = port
     # if localBind:
     #     listen = f'127.0.0.1:{port}'
+    extra1 = ""
+    extra2 = ""
+
+    if selfSign:
+        env.run("apt install -y openssl")
+        env.run("mkdir -p /data/ssl")
+        if not env.runSafe("test -f /data/ssl/nginx.key"):
+            env.run(
+                "openssl req -x509 -nodes -days 3650 -newkey rsa:2048 -keyout /data/ssl/nginx.key -out /data/ssl/nginx.crt  -subj '/C=KR'"
+            )
+
+        listen = f"{selfSignPort} ssl"
+        extra1 = """
+ssl_certificate /data/ssl/nginx.crt;
+ssl_certificate_key /data/ssl/nginx.key;
+"""
+        extra2 = f"""
+server {{
+    listen 80;
+    server_name {domain};
+    return 301 https://$host$request_uri;
+}}
+"""
 
     env.makeFile(
         f"""\
 server {{
 	listen			{listen};
 	server_name		{domain};
 	root			/data/{name};
 
+    {extra1}
+
 	#access_log		/var/log/nginx/{name}.log;
 	error_log		/var/log/nginx/error.log;
 
 	# index			index.php index.html index.htm;
     index           index.php index.html /index.php$request_uri;
 	# fastcgi_index	index.php;
 	# fastcgi_param	SCRIPT_FILENAME $document_root$fastcgi_script_name;
@@ -428,37 +455,38 @@
         return 301 /remote.php$request_uri;
     }}
 
     location / {{
         try_files $uri $uri/ /index.php$request_uri;
     }}
 }}
+{extra2}
 """,
         path=f"{nginxCfgPath}/{name}",
         sudo=True,
         mode=664,
     )
 
-    if prot == "https":
+    if prot == "https" and not selfSign:
         certbotSetup(
             env,
             domainStr=domain,
             email="cjng96@gmail.com",
             name=name,
             nginxCfgPath=nginxCfgPath,
             localBind=localBind,
         )
 
 
 def dockerNextcloudFpm(
     env,
-    srcPath,
-    domain,
+    dataPath,
     name="next",
-    prot="https",
+    overwriteProt="https",
+    overwriteDomain=None,  # None이면 overwrite안한다
     dbHost="sql",
     dbName="next",
     dbId="next",
     dbPw="1234",
     publishPort=0,
     restart="unless-stopped",
 ):
@@ -486,47 +514,56 @@
         # TODO: next가 만들다 실패했을도 있으니 더 검사해야 한다
         return
 
     # bind mount도 안먹힌다
     # env.run(f'sudo mount --bind {srcPath} /data/web/{name}')
     env.run(f"sudo mkdir -p /data/web/{name}")
 
+    # 어차피 web통해서 접근해서 이거 필요없는거 같은데..
     publishPortCmd = "" if publishPort == 0 else f"-p {publishPort}:9000"
+    # publishPortCmd = ""
 
     # web쪽에 /data/next로 별도로 마운팅하지 않으려면 web쪽꺼를 가져다 쓸수밖에 없다
+    overwrite = ""
+    if overwriteDomain is not None:
+        overwrite = f"""\
+  -e OVERWRITEPROTOCOL={overwriteProt} \
+  -e OVERWRITEHOST={overwriteDomain} \
+  -e OVERWRITECLIURL={overwriteProt}://{overwriteDomain} \
+  """
+
     env.run(
         f"""\
 sudo docker run -d --name {name} \
   --restart {restart} \
   {publishPortCmd} \
   -e MYSQL_DATABASE={dbName} \
   -e MYSQL_HOST={dbHost} \
   -e MYSQL_USER={dbId} \
   -e MYSQL_PASSWORD={dbPw} \
-  -e OVERWRITEPROTOCOL={prot} \
-  -e OVERWRITEHOST={domain} \
-  -e OVERWRITECLIURL={prot}://{domain} \
+  {overwrite} \
   -v /data/web/{name}:/var/www/html \
-  -v {srcPath}:/var/www/html/data \
+  -v {dataPath}:/var/www/html/data \
   nextcloud:fpm
 """
     )
     env.run(f"docker network connect net {name}")
 
+    env.runSafe(f"sudo docker rm -f {name}Cron")
     env.run(
         f"""\
 sudo docker run -d --name {name}Cron \
   --restart {restart} \
   --entrypoint /cron.sh \
   -e MYSQL_DATABASE={dbName} \
   -e MYSQL_HOST={dbHost} \
   -e MYSQL_USER={dbId} \
   -e MYSQL_PASSWORD={dbPw} \
   -v /data/web/{name}:/var/www/html \
-  -v {srcPath}:/var/www/html/data \
+  -v {dataPath}:/var/www/html/data \
   nextcloud:fpm
 """
     )
     env.run(f"docker network connect net {name}Cron")
 
 
 def dockerNextcloud(
@@ -891,19 +928,19 @@
     또 문제가, internal-sftp는 /media/ssd1/users/b_test2를 쓰려고 하면 /media/ssd1..등의 부모 폴더도
     다 root owned and 755여야 한다. mount bind할수 있지만 치명적
     """
     # https://www.cyberciti.biz/tips/howto-linux-unix-rssh-chroot-jail-setup.html"
     if env.runSafe(f"test -f {home}/ok"):
         return
 
-    print(f"========== install rssh on {env.remoteOs} ==========")
-
-    if env.remoteOs == "ubuntu":
+    os = env.getOS()
+    print(f"========== install rssh on {os} ==========")
+    if os == "ubuntu":
         env.run("sudo apt install --no-install-recommends -y rssh")
-    elif env.remoteOs == "centos":
+    elif os == "centos":
         env.run("sudo yum install -y rssh")
 
     env.run(f"mkdir -p {home}/{{dev,etc,lib,usr,bin}}")
     env.run(f"mkdir -p {home}/usr/bin")
     # env.run(f'mkdir -p {home}/usr/libexec/openssh'.format(home))
     env.run(f"mkdir -p {home}/usr/lib/openssh")
     env.run(f"mkdir -p {home}/usr/lib/rssh")
@@ -986,15 +1023,15 @@
 
 
 def makeRsshUser(env, id, rootPath, authPubs):
     makeUser(env, id, home=f"{rootPath}/{id}", shell="/usr/bin/rssh", authPubs=authPubs)
 
 
 def registerAuthPubs(env, authPubs, id=None):
-    print(f">> [{env.name}] registerAuthPubs - id:{id} pubs:{authPubs}")
+    env.log(f">> registerAuthPubs - id:{id} pubs:{authPubs}")
     if id is None:
         home = "~"
     else:
         home = env.runOutput(f"echo ~{id}").strip()
         if home == "":
             raise Exception(f"registerAuthPubs: failed to get home folder for {id}")
 
@@ -1006,16 +1043,16 @@
 def registerAuthPub(env, pub, id=None):
     registerAuthPubs(env, [pub], id)
 
 
 def makeUser(
     env, id, home=None, shell=None, genSshKey=True, grantSudo=False, authPubs=None
 ):
-    print(
-        f">> [{env.name}] makeUser - id:{id} home:{home} shell:{shell} genKey:{genSshKey} grantSudo:{grantSudo} authPubs:{authPubs}"
+    env.log(
+        f">> makeUser - id:{id} home:{home} shell:{shell} genKey:{genSshKey} grantSudo:{grantSudo} authPubs:{authPubs}"
     )
 
     # if env.runSafe('cat /etc/passwd | grep -e "^%s:"' % id):
     if env.runSafe(f'grep -c "^{id}:" /etc/passwd'):
         # 이 경우도 등록은 갱신한다.
         print(f"  -> makeUser - exist user[{id}]")
         if authPubs is not None:
@@ -1189,15 +1226,15 @@
 
     #     print(f"{fn}/{component}: {ver} version exists...")
 
     # if not okFlag:
     #     raise Exception(f"Failed to found next new version - {imgName}:{prefix}{infoVer}")
     ver = _skipSameVersion(env, f"{imgName}:{prefix}", infoVer)
 
-    print(f"{fn}/{component}: new ver - {ver}")
+    print(f"{fn}/{component}: new version - {ver}")
     info["version"] = ver
     info["hash"] = hash
     info["date"] = nowStr
     with open(fn2, "w") as fp:
         fp.write(yaml.dump(infos))
 
     return ver
@@ -1237,15 +1274,15 @@
 
 def dockerUpdateImage(
     env, baseName, baseVer, newName, newVer, hash, func, net=None, userId=None
 ):
     """
     return: true(created new one), false(already exists)
     """
-    print(f"dockerUpdateImage - {newName}:{newVer} from {baseName}:{baseVer}")
+    print(f"dockerUpdateImage: {newName}:{newVer} from {baseName}:{baseVer}")
     # baseVer = verStr(baseVer)
     # newVer = verStr(newVer)
 
     # 해당 버젼이 이미 있으면 생략
     ret = env.runOutputProf(f"sudo docker images -q {newName}:{newVer}").strip()
     if ret != "":
         # 해당부모가 동일한지 확인
@@ -1279,14 +1316,15 @@
     if net is not None:
         extra = f"--network {net}"
 
     env.run(f"sudo docker run -itd {extra} --name {newName}-con {baseName}:{baseVer}")
     dk = env.dockerConn(f"{newName}-con", dkId=userId)
 
     func(dk)
+    dk.clearConn()
 
     # 이미지 생성 및 리소스 제거
     extra = ""
     if hash is not None:
         extra = f"""-c 'LABEL hash="{hash}"'"""
 
     env.run(f"""sudo docker commit {extra} {newName}-con {newName}:{newVer}""")
@@ -1546,15 +1584,15 @@
     awsLogsGroup=None,
     awsLogsStream=None,
     awsLogsRegion=None,
 ):
     """
     port: "3306:3306", "9018-9019:9018-9019", ["9018-9019:9018-9019"]
     """
-    print("port", port)
+    # print("port", port)
 
     # if portCnt != 1:
     # 	portCmd = '-p {0}-{1}:{0}-{1}'.format(port, port+portCnt-1)
     # else:
     # 	portCmd = '-p {0}:{0}'.format(port)
 
     cmd = (
@@ -1656,43 +1694,48 @@
 #LABEL maintainer="cjng96@gmail.com"
 RUN echo "#!/bin/bash\\\\nexec /bin/bash" > /start && chmod 755 /start
 RUN mkdir -p /data && mkdir -p /work/log && ln -sf /work/log /var/log
 CMD ["/start"]
 """,
             "/tmp/docker-sv/Dockerfile",
         )
-        env.run(
-            f". ~/.profile && sudo docker build -t {image} /tmp/docker-sv && rm -rf /tmp/docker-sv"
+        env.runProf(
+            f"sudo docker build -t {image} /tmp/docker-sv && rm -rf /tmp/docker-sv"
         )  # --no-cache
 
     cmd = dockerRunCmd(name, image, port, mountBase)
-    env.run(". ~/.profile && " + cmd)
+    env.runProf(cmd)
 
     # leave cmd as a file
     env.makeFile(cmd, "/tmp/dockerCmd")
-    env.run(f". ~/.profile && sudo docker cp /tmp/dockerCmd {name}:/cmd")
+    env.runProf(f"sudo docker cp /tmp/dockerCmd {name}:/cmd")
+
 
+def writeRunScript(env, cmd, targetPath="/app/current"):
+    env.log(f">> writeRunScript: {cmd}")
 
-def writeRunScript(env, cmd):
-    print(f">> [{env.name}] writeRunScript: {cmd}")
+    pp = "/etc/service/app" if targetPath is None else targetPath
 
+    env.run("mkdir -p /etc/service/app")
     env.makeFile(
         f"""\
 #!/bin/sh
 {upcntRunStr()}
 {cmd}
 """,
-        "/app/current/run",
+        f"{pp}/run",
     )
-    env.run("mkdir -p /etc/service/app && ln -sf /app/current/run /etc/service/app/run")
+    if targetPath is not None:
+        env.run(f"ln -sf {pp}/run /etc/service/app/run")
+
     writeSvHelper(env)
 
 
 def writeSvHelper(env):
-    print(f">> [{env.name}] writeSvHelper")
+    env.log(f">> writeSvHelper")
 
     help = "shortcuts - c(app),s(status),r(run),d(stop),re(restart),e(exit)"
     env.configBlock(
         path="~/.bashrc",
         marker="# {mark} alias",
         block=f"""
 function readlinks() {{ readlink "$@" || echo "$@"; }}
@@ -1894,14 +1937,16 @@
 
     env.run('''sudo mysql -e "DROP USER '%s'@'%s';"''' % (id, host))
 
 
 def mysqlUserGen(env, id, pw, host, priv, unixSocket=False):
     """
     priv: "*.*:ALL,GRANT", "*.*:RELOAD,PROCESS,LOCK TABLES,REPLICATION CLIENT"
+    앞에께 ON 대상, 뒤에껀 권한인데 - ALL PRIVILEGES를 주면 전체 권한이 된다
+
     """
     # pw = str2arg(pw).replace(';', '\\;').replace('`', '``').replace("'", "\\'")
     pw = env.str2arg(pw).replace("'", "''")
     # 이게 좀 웃긴데, mysql 통해서 실행하는거기 때문에 \\는 \\\\로 바꿔야한다.
     pw = pw.replace("\\\\", "\\\\\\\\")
     host = env.str2arg(host)
     if unixSocket:
@@ -1918,15 +1963,15 @@
         priv2, oper = priv.split(":")
 
         grantOper = ""
         lst = list(map(lambda x: x.strip().upper(), oper.split(",")))
         if "GRANT" in lst:
             lst.remove("GRANT")
             grantOper = "WITH GRANT OPTION"
-            oper = ",".join(lst)
+        oper = ",".join(lst)
 
         env.run(
             f'''sudo mysql -e "GRANT {oper} ON {priv2} TO '{id}'@'{host}' {grantOper};"'''
         )
 
 
 def goBuild(env, targetOs="", targetArch=""):
@@ -2112,14 +2157,39 @@
         regexp="^#security:",
         line="security:\n  authorization: enabled",
         sudo=True,
     )
     env.run("sudo supervisorctl restart mongodb")
 
 
+def installGitea(env):
+    # cmd = "sudo apt install git"
+    # env.run(cmd)
+
+    # https://docs.gitea.com/installation/install-from-binary
+    # cmd = "wget -O gitea https://dl.gitea.com/gitea/1.21.7/gitea-1.21.7-linux-amd64 && chmod +x gitea"
+    if not env.runSafe("command -v gitea"):
+        cmd = "curl -L -o gitea https://dl.gitea.com/gitea/1.21.7/gitea-1.21.7-linux-amd64 && chmod +x gitea"
+        env.run(cmd)
+        env.run("mv gitea /usr/local/bin/gitea")
+
+
+def initGitea(env, dataDir="/var/lib/gitea"):
+    env.run(f"mkdir -p {dataDir}/{{custom,data,log}}")
+    env.run(f"chown -R git:git {dataDir}/")
+    env.run(f"chmod -R 750 {dataDir}/")
+
+    env.run("mkdir -p /etc/gitea")
+    env.run("chown root:git /etc/gitea")
+    env.run("chmod 770 /etc/gitea")
+
+    # env.run('chmod 750 /etc/gitea')
+    # env.run('chmod 640 /etc/gitea/app.ini')
+
+
 def installMariaDb(env, dataDir="/var/lib/mysql", port=3306, repo=None):
     """
     repo = "deb [arch=amd64,arm64,ppc64el,s390x] https://mirror.yongbok.net/mariadb/repo/10.5/ubuntu focal main"
     """
     # hr = env.runOutput('pidof mysqld; echo').strip()
     # if len(hr) > 0:
     if env.runSafe("command -v mysqld"):
@@ -2402,30 +2472,42 @@
 
 def dockerForceNetwork(env, name):
     env.run(f"docker network inspect {name} || docker network create {name}")
     # -f {{.Name}}
 
 
 def getArch(env):
-    arch = env.runOutput("dpkg --print-architecture").strip()
+    os = env.getOS()
+    arch = None
+
+    if os == "ubuntu":
+        arch = env.runOutput("dpkg --print-architecture").strip()
+    elif os == "centos":
+        arch = env.runOutput("uname -m").strip()
+    else:
+        raise Exception("Unsupported Operating System")
+
     return arch
 
 
 def installDocker(env, arch=None):
     """
     arch: amd64 | arm64
     """
     if arch is None:
         arch = getArch(env)
 
     # if env.runRet('which docker > /dev/null') != 0:
     if env.runSafe("command -v docker"):
         return
 
-    if env.remoteOs == "ubuntu":
+    os = env.getOS()
+
+    if os == "ubuntu":
+        # docker.io로 설치가 더 편한데, 좀 애매하다...
         env.run(
             "sudo apt install --no-install-recommends -y apt-transport-https ca-certificates curl gnupg-agent software-properties-common"
         )
         env.run(
             "curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -"
         )
         # sudo apt-key fingerprint 0EBFCD88
@@ -2435,26 +2517,29 @@
         env.run("sudo apt update")
         env.run("apt-cache policy docker-ce")
         env.run("sudo apt install --no-install-recommends -y docker-ce")
 
         env.run("sudo usermod -aG docker $USER")
         # env.run("sudo adduser {{server.id}} docker")	# remote.server.id
         # env.run("sudo service docker restart")	# /etc/init.d/docker restart
-    elif env.remoteOs == "centos":
+    elif os == "centos":
         env.run("sudo yum install -y yum-utils device-mapper-persistent-data lvm2")
         env.run(
             "sudo yum-config-manager --add-repo https://download.docker.com/linux/centos/docker-ce.repo"
         )
-        env.run("sudo yum makecache fast")
+        # env.run("sudo yum makecache fast")
+        env.run("sudo yum makecache")
         env.run("yum list docker-ce --showduplicates | sort -r")
         env.run("sudo yum install -y docker-ce docker-ce-cli containerd.io")
         env.run("sudo systemctl start docker")
         env.run("sudo systemctl enable docker")
         # 여기 명령어가 이상한것 같은데?
         env.run("sudo usermod -aG docker $USER")
+    else:
+        raise Exception(f"Unsupported Operating System - {os}")
 
     time.sleep(3)  # boot up
 
 
 def installRestic(env, version, arch=None):
     """
     version: 0.12.1
@@ -2886,15 +2971,16 @@
 
     if certSetup:
         certbotSetup(env, domainStr=domain, email=certAdminEmail, name=name)
     else:
         env.run("sudo nginx -s reload")
 
 
-#
+# 단순 proxy로 쓰려면 privateApi, root없이 쓰자. publicApi는 '/'
+# proxyUrl: http://192.168.1.105
 def setupWebApp(
     env,
     name,
     domain,
     proxyUrl,
     publicApi,
     root=None,
@@ -2915,14 +3001,15 @@
     apiPath -> publicApi
 
     privateContent=
     allow 172.0.0.0/8; # docker
     allow 45.77.21.99; # tk1
     allow 115.178.67.152; # rt
     """
+
     privPath = f"/data/nginx/{name}.priv"
     if privateFilter is not None:
         env.makeFile(privateFilter, privPath, sudo=True, mode=664)
 
     extra = (
         ""
         if buffering
```

### Comparing `god-tool-0.8.1/gat/sa.py` & `god_tool-0.9.0/gat/sa.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,29 +136,37 @@
         img = con["img"]
 
         cmd = f"{dkCmd} image history -q {img}"
         ss = subprocess.check_output(cmd, shell=True).decode("utf-8").strip()
         qs = ss.splitlines()
         ids = ids + qs
 
-    cmd = """{dkCmd} images --format '{"id":"{{.ID}}", "img":"{{.Repository}}:{{.Tag}}"}' """
+    cmd = (
+        dkCmd
+        + """ images --format '{"id":"{{.ID}}", "img":"{{.Repository}}:{{.Tag}}"}' """
+    )
 
     ss = subprocess.check_output(cmd, shell=True).decode("utf-8").strip()
     images = ss.splitlines()
     for node in images:
         img = json.loads(node)
         # print(f'img {img}')
         imgName = img["img"].split(":")[0]
         if img["id"] not in ids:
             print(f"\n{img['img']}({img['id']}) is not used...")
             if imgName in deleteTargets:
                 cmd = f"{dkCmd} rmi {img['id']}"
                 # print(cmd)
-                ss = subprocess.check_output(cmd, shell=True).decode("utf-8").strip()
-                print(ss)
+                try:
+                    ss = (
+                        subprocess.check_output(cmd, shell=True).decode("utf-8").strip()
+                    )
+                    print(ss)
+                except Exception as e:
+                    print(f"  err -> {e}")
             else:
                 print("  -> but don't delete it which is not in deleteTarget list")
 
 
 def parsePs(ss):
     lines = ss.splitlines()
     upcnt = lines[0].strip()
```

### Comparing `god-tool-0.8.1/gat/sampleFiles.py` & `god_tool-0.9.0/gat/sampleFiles.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,93 +1,90 @@
-sampleApp = """
-# https://
-config='''
-type: app	# it's default
+sampleApp = '''
+config="""
 name: sample
+type: app	
 #cmd: [ python3, sample.py ]
 
 serve:
-  patterns: [ "*.go", "*.json", "*.graphql" ]
+    patterns: [ "*.go", "*.json", "*.graphql" ]
 
 deploy:
-  strategy: zip
-  maxRelease: 3
-  include:
-    #- "*"
-    - "{{name}}"
-    - config
-    - pm2.json
-    - src: ../build
-      target: build
-  exclude:
-    - config/my.json
-  sharedLinks:
-    - config/my.json
-  gitRepo: <your remote repo>
+    strategy: zip
+    maxRelease: 3
+    include:
+        #- "*"
+        - "{{name}}"
+        - config
+        - pm2.json
+        - src: ../build
+          target: build
+    exclude:
+        - config/my.json
+    sharedLinks:
+        - config/my.json
+    gitRepo: <your remote repo>
 
 servers:
-  - name: test
-    host: test.com
-    port: 22
-    id: test      # ssh worker user id
-    #dkName: con  #
-    #dkId: test
-    owner: engt   # opt, generated files owner
+    - name: test
+      host: test.com
+      port: 22
+      id: test      # ssh worker user id
+      #dkName: con
+      #dkId: test
+      owner: engt   # opt, generated files owner
       # you don't need sudo right if it's not specified.
       # if you need the operation needed sudo right, should specify it.
-    deployRoot: ~/test  # deployment target path
-    gitBranch: <your remote repo branch>
-'''
+      deployRoot: ~/test  # deployment target path
+      gitBranch: <your remote repo branch>
+"""
 
 class myGat:
-	def __init__(self, helper, **_):
-		helper.configStr("yaml", config)	# helper.configFile("yaml", "gat.yaml")
-
-	def buildTask(self, util, local, **_):
-		#local.gqlGen()
-		local.goBuild()
-
-	# it's default operation and you can override running cmd
-	#def getRunCmd(self, util, local, **_):
-	#	return [util.config.config.name]
-
-	def deployPreTask(self, util, remote, local, **_):
-		#print('deploy to {{server.name}}) # remote.server.name
-		#local.run("npm run build")
-		pass
-
-	def deployPostTask(self, util, remote, local, **_):
-		#remote.pm2Register():
-		#local.run("cd {{deployRoot}}/current && echo 'finish'") # util.dic.deployRoot
-		pass
+    def __init__(self, helper, **_):
+        helper.configStr("yaml", config)	# helper.configFile("yaml", "gat.yaml")
 
-"""
+    def buildTask(self, util, local, **_):
+        #local.gqlGen()
+        local.goBuild()
+
+    # it's default operation and you can override running cmd
+    #def getRunCmd(self, util, local, **_):
+    #	return [util.config.config.name]
+
+    def deployPreTask(self, util, remote, local, **_):
+        #print('deploy to {{server.name}}) # remote.server.name
+        #local.run("npm run build")
+        pass
+
+    def deployPostTask(self, util, remote, local, **_):
+        #remote.pm2Register():
+        #local.run("cd {{deployRoot}}/current && echo 'finish'") # util.dic.deployRoot
+        pass
+'''
 
-sampleSys = """
-# https://
-config='''
+sampleSys = '''
+config="""
+name: sample
 type: sys
-name: test	# hostname
 
-s3:
-  key: ${aws_key}
-  secret: ${aws_secret}
+# s3:
+#   key: ${aws_key}
+#   secret: ${aws_secret}
 
 servers:
-  - name: test
-    host: test.com
-    port: 22
-		#dkName: name
-    id: test
-	vars:
-	  hello: test
-'''
+    - name: test
+      host: test.com
+      port: 22
+      id: test  # ssh worker user id
+      #dkName: name
+      vars:
+        hello: test
+"""
 
 class myGat:
-	def __init__(self, helper, **_):
-		helper.configStr("yaml", config)	# helper.configFile("yaml", "gat.yaml")
+    def __init__(self, helper, **_):
+        helper.configStr("yaml", config)	# helper.configFile("yaml", "gat.yaml")
 
-	def setupTask(self, util, local, remote, **_):
-		#remote.pm2Register():
-		#remote.run("cd %%s/current && echo 'finish'" %% remote.vars.deployRoot)
+    def setupTask(self, util, local, remote, **_):
+        #remote.pm2Register():
+        #remote.run("cd %%s/current && echo 'finish'" %% remote.vars.deployRoot)
 
-"""
+'''
```

### Comparing `god-tool-0.8.1/god_tool.egg-info/PKG-INFO` & `god_tool-0.9.0/god_tool.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: god-tool
-Version: 0.8.1
+Version: 0.9.0
 Summary: Provisioning and App deployment tool.
 Home-page: https://github.com/cjng96/gat
 Author: Felix Choi
 Author-email: cjng96@gmail.com
 License: LGPL
 Keywords: auto restart,deployment
 Platform: Posix; MacOS X; Windows
```

### Comparing `god-tool-0.8.1/setup.py` & `god_tool-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `god-tool-0.8.1/test/test_gatHelper.py` & `god_tool-0.9.0/test/test_gatHelper.py`

 * *Files identical despite different names*

