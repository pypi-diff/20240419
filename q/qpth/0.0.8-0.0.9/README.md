# Comparing `tmp/qpth-0.0.8.tar.gz` & `tmp/qpth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qpth-0.0.8.tar", last modified: Tue Mar 27 22:51:23 2018, max compression
+gzip compressed data, was "dist/qpth-0.0.9.tar", last modified: Sat Apr 14 18:24:42 2018, max compression
```

## Comparing `qpth-0.0.8.tar` & `qpth-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-03-27 22:51:23.000000 qpth-0.0.8/
--rw-r--r--   0 root         (0) root         (0)       38 2018-03-27 22:51:23.000000 qpth-0.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      363 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)      291 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)        5 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       11 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)      675 2017-04-07 18:08:43.000000 qpth-0.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)      291 2018-03-27 22:51:23.000000 qpth-0.0.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      398 2018-03-27 22:50:38.000000 qpth-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth/
--rw-rw-r--   0 root         (0) root         (0)     1358 2017-05-10 18:10:01.000000 qpth-0.0.8/qpth/util.py
--rw-r--r--   0 root         (0) root         (0)       76 2017-04-07 18:01:43.000000 qpth-0.0.8/qpth/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     8855 2017-11-09 20:35:14.000000 qpth-0.0.8/qpth/qp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth/solvers/
--rw-rw-r--   0 root         (0) root         (0)       50 2017-04-28 14:33:58.000000 qpth-0.0.8/qpth/solvers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1064 2017-05-16 15:00:50.000000 qpth-0.0.8/qpth/solvers/cvxpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-03-27 22:51:23.000000 qpth-0.0.8/qpth/solvers/pdipm/
--rw-rw-r--   0 root         (0) root         (0)        0 2017-04-07 18:01:45.000000 qpth-0.0.8/qpth/solvers/pdipm/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9134 2017-06-04 18:19:24.000000 qpth-0.0.8/qpth/solvers/pdipm/spbatch.py
--rw-rw-r--   0 root         (0) root         (0)    16124 2017-11-09 19:36:07.000000 qpth-0.0.8/qpth/solvers/pdipm/batch.py
--rw-rw-r--   0 root         (0) root         (0)     7226 2017-05-07 16:59:45.000000 qpth-0.0.8/qpth/solvers/pdipm/single.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-04-14 18:24:42.000000 qpth-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       38 2018-04-14 18:24:42.000000 qpth-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      363 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)      291 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        5 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       11 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)      675 2017-04-07 18:08:43.000000 qpth-0.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)      291 2018-04-14 18:24:42.000000 qpth-0.0.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      398 2018-04-14 18:23:24.000000 qpth-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth/
+-rw-rw-r--   0 root         (0) root         (0)     1358 2017-05-10 18:10:01.000000 qpth-0.0.9/qpth/util.py
+-rw-r--r--   0 root         (0) root         (0)       76 2017-04-07 18:01:43.000000 qpth-0.0.9/qpth/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     8912 2018-04-14 18:23:09.000000 qpth-0.0.9/qpth/qp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth/solvers/
+-rw-rw-r--   0 root         (0) root         (0)       50 2017-04-28 14:33:58.000000 qpth-0.0.9/qpth/solvers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1064 2017-05-16 15:00:50.000000 qpth-0.0.9/qpth/solvers/cvxpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-04-14 18:24:42.000000 qpth-0.0.9/qpth/solvers/pdipm/
+-rw-rw-r--   0 root         (0) root         (0)        0 2017-04-07 18:01:45.000000 qpth-0.0.9/qpth/solvers/pdipm/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9134 2017-06-04 18:19:24.000000 qpth-0.0.9/qpth/solvers/pdipm/spbatch.py
+-rw-rw-r--   0 root         (0) root         (0)    16124 2017-11-09 19:36:07.000000 qpth-0.0.9/qpth/solvers/pdipm/batch.py
+-rw-rw-r--   0 root         (0) root         (0)     7226 2017-05-07 16:59:45.000000 qpth-0.0.9/qpth/solvers/pdipm/single.py
```

### Comparing `qpth-0.0.8/README.md` & `qpth-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `qpth-0.0.8/qpth/util.py` & `qpth-0.0.9/qpth/util.py`

 * *Files identical despite different names*

### Comparing `qpth-0.0.8/qpth/qp.py` & `qpth-0.0.9/qpth/qp.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,14 +165,16 @@
             if b_e:
                 dbs = dbs.mean(0).squeeze(0)
         else:
             dAs, dbs = None, None
         dQs = 0.5 * (bger(dx, zhats) + bger(zhats, dx))
         if Q_e:
             dQs = dQs.mean(0).squeeze(0)
+        if p_e:
+            dps = dps.mean(0).squeeze(0)
 
         grads = (dQs, dps, dGs, dhs, dAs, dbs)
 
         return grads
 
 
 class SpQPFunction(Function):
```

### Comparing `qpth-0.0.8/qpth/solvers/cvxpy.py` & `qpth-0.0.9/qpth/solvers/cvxpy.py`

 * *Files identical despite different names*

### Comparing `qpth-0.0.8/qpth/solvers/pdipm/spbatch.py` & `qpth-0.0.9/qpth/solvers/pdipm/spbatch.py`

 * *Files identical despite different names*

### Comparing `qpth-0.0.8/qpth/solvers/pdipm/batch.py` & `qpth-0.0.9/qpth/solvers/pdipm/batch.py`

 * *Files identical despite different names*

### Comparing `qpth-0.0.8/qpth/solvers/pdipm/single.py` & `qpth-0.0.9/qpth/solvers/pdipm/single.py`

 * *Files identical despite different names*

