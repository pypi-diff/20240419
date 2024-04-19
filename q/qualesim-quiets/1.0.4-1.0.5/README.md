# Comparing `tmp/qualesim-quiets-1.0.4.tar.gz` & `tmp/qualesim-quiets-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-quiets-1.0.4.tar", last modified: Thu Apr 18 01:51:27 2024, max compression
+gzip compressed data, was "qualesim-quiets-1.0.5.tar", last modified: Fri Apr 19 03:18:40 2024, max compression
```

## Comparing `qualesim-quiets-1.0.4.tar` & `qualesim-quiets-1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.847695 qualesim-quiets-1.0.4/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.4/LICENSE
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-18 01:51:27.847695 qualesim-quiets-1.0.4/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      250 2024-01-02 01:13:56.000000 qualesim-quiets-1.0.4/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.843695 qualesim-quiets-1.0.4/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.843695 qualesim-quiets-1.0.4/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.4/data/bin/dqcsfeqi
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.843695 qualesim-quiets-1.0.4/qualesim_quiets/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.4/qualesim_quiets/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.4/qualesim_quiets/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    44819 2024-04-18 01:51:03.000000 qualesim-quiets-1.0.4/qualesim_quiets/frontend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.4/qualesim_quiets/utils.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.847695 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      852 2024-04-18 01:51:27.000000 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-18 01:51:27.000000 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-18 01:51:27.000000 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-18 01:51:27.000000 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/requires.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-18 01:51:27.000000 qualesim-quiets-1.0.4/qualesim_quiets.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-18 01:51:27.847695 qualesim-quiets-1.0.4/setup.cfg
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-18 01:51:12.000000 qualesim-quiets-1.0.4/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:51:27.847695 qualesim-quiets-1.0.4/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.4/tests/test_cls.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 08:24:10.000000 qualesim-quiets-1.0.4/tests/test_example_quiets_whitepaper.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.4/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.4/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.884014 qualesim-quiets-1.0.5/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    35149 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.5/LICENSE
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-19 03:18:40.884014 qualesim-quiets-1.0.5/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      289 2024-04-19 03:15:24.000000 qualesim-quiets-1.0.5/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.880014 qualesim-quiets-1.0.5/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.880014 qualesim-quiets-1.0.5/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:31:17.000000 qualesim-quiets-1.0.5/data/bin/dqcsfeqi
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.880014 qualesim-quiets-1.0.5/qualesim_quiets/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-09-28 06:57:55.000000 qualesim-quiets-1.0.5/qualesim_quiets/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      192 2024-01-02 01:17:17.000000 qualesim-quiets-1.0.5/qualesim_quiets/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    44768 2024-04-19 03:15:36.000000 qualesim-quiets-1.0.5/qualesim_quiets/frontend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    11426 2024-04-17 02:46:12.000000 qualesim-quiets-1.0.5/qualesim_quiets/utils.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.884014 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      891 2024-04-19 03:18:40.000000 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      445 2024-04-19 03:18:40.000000 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-19 03:18:40.000000 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       18 2024-04-19 03:18:40.000000 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/requires.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       16 2024-04-19 03:18:40.000000 qualesim-quiets-1.0.5/qualesim_quiets.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-19 03:18:40.884014 qualesim-quiets-1.0.5/setup.cfg
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     1086 2024-04-19 03:15:46.000000 qualesim-quiets-1.0.5/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-19 03:18:40.884014 qualesim-quiets-1.0.5/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     9572 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.5/tests/test_cls.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-18 01:57:47.000000 qualesim-quiets-1.0.5/tests/test_example_quiets_whitepaper.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     7477 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.5/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     6223 2024-03-29 08:02:16.000000 qualesim-quiets-1.0.5/tests/test_qifile.py
```

### Comparing `qualesim-quiets-1.0.4/LICENSE` & `qualesim-quiets-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.4/PKG-INFO` & `qualesim-quiets-1.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.4
+Version: 1.0.5
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
@@ -13,16 +13,17 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ply
 Requires-Dist: pyquiet
 
-# DQCSim-Quiets
+# QuaLeSim-QUIETs
 
 #### 介绍
-1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
+1. 本前端为QuaLeSim-QUIETs前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
 
-1. 与QuaLeSim协同安装
-    - `pip install qualesim[PLUGINS]`
+1. 直接从 pypi 上安装
+    - `pip install qualesim-quiets`
+    - 其中依赖 `pyquiet == 0.0.3`
```

### Comparing `qualesim-quiets-1.0.4/qualesim_quiets/frontend.py` & `qualesim-quiets-1.0.5/qualesim_quiets/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,37 +320,37 @@
                         if len(func_data.func_qubit[ii]) == 1:
                             func_data.res_qubit.append(ii)
                         else:
                             func_data.res_qubit.append(str(ii) + "[" + str(jj) + "]")
             res_state_vector["classical"] = res_cls
             if measure_mod == "state_vector":
                 if measure_flag == 1:
-                    res_state_vector["quantum"] = (
-                        func_data.res_qubit,
-                        eval(func_data.state_vector)[1],
-                    )
+                    if len(func_data.res_qubit) == 0:
+                        res_state_vector["quantum"] = (
+                            func_data.res_qubit,
+                            [],
+                        )
+                    else:
+                        res_state_vector["quantum"] = (
+                            func_data.res_qubit,
+                            eval(func_data.state_vector)[1],
+                        )
                 else:
                     if len(func_data.free_list) == 0:
                         res_state_vector["quantum"] = [1]
                     else:
                         tar = func_data.func_qubit[func_data.free_list[0]][0]
                         self.measure(
                             tar,
                             arb=ArbData(measure_mod="measureforres"),
                         )
                         res_state_vector["quantum"] = (
                             func_data.res_qubit,
                             eval(self.get_measurement(tar)["state_vector"])[1],
                         )
-                if 2 ** len(res_state_vector["quantum"][0]) != len(
-                    res_state_vector["quantum"][1]
-                ):
-                    self.info(
-                        "here is untraced qubit, and may rise a bug when exemod is statevector in quantumsim backend!"
-                    )
             func_data.state_vector = str(res_state_vector)
             for i in func_data.free_list:
                 self.free(func_data.func_qubit[i])
             return func_data, ret
 
         for i in func_data.free_list:
             self.free(func_data.func_qubit[i])
```

### Comparing `qualesim-quiets-1.0.4/qualesim_quiets/utils.py` & `qualesim-quiets-1.0.5/qualesim_quiets/utils.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.4/qualesim_quiets.egg-info/PKG-INFO` & `qualesim-quiets-1.0.5/qualesim_quiets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualesim-quiets
-Version: 1.0.4
+Version: 1.0.5
 Summary: QuaLeSim frontend for QUIET-S.
 Home-page: https://gitee.com/hpcl_quanta/dqcsim-quiets.git
 Author: Dingdong Liu
 Author-email: dingdongliu@quanta.org.cn
 License: GPLv3
 Keywords: qualesim quiets
 Classifier: Development Status :: 3 - Alpha
@@ -13,16 +13,17 @@
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ply
 Requires-Dist: pyquiet
 
-# DQCSim-Quiets
+# QuaLeSim-QUIETs
 
 #### 介绍
-1. 本前端为QuaLeSim-QUIETS前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
+1. 本前端为QuaLeSim-QUIETs前端，为QuaLeSim框架提供了一个可以识别QUIET-S量子-经典混合指令集的前端插件。
 
 #### 安装教程
 
-1. 与QuaLeSim协同安装
-    - `pip install qualesim[PLUGINS]`
+1. 直接从 pypi 上安装
+    - `pip install qualesim-quiets`
+    - 其中依赖 `pyquiet == 0.0.3`
```

### Comparing `qualesim-quiets-1.0.4/setup.py` & `qualesim-quiets-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-quiets",
-    version="1.0.4",
+    version="1.0.5",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="QuaLeSim frontend for QUIET-S.",
     license="GPLv3",
     keywords="qualesim quiets",
     url="https://gitee.com/hpcl_quanta/dqcsim-quiets.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-quiets-1.0.4/tests/test_cls.py` & `qualesim-quiets-1.0.5/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.4/tests/test_gate.py` & `qualesim-quiets-1.0.5/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-quiets-1.0.4/tests/test_qifile.py` & `qualesim-quiets-1.0.5/tests/test_qifile.py`

 * *Files identical despite different names*

