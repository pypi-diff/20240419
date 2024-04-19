# Comparing `tmp/pySuperfish-0.1.1.tar.gz` & `tmp/pySuperfish-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PySuperfish/PySuperfish/dist/.tmp-gvnjo5_h/pySuperfish-0.1.1.tar", last modified: Thu Mar 16 16:39:40 2023, max compression
+gzip compressed data, was "/home/runner/work/PySuperfish/PySuperfish/dist/.tmp-01g43w6_/pySuperfish-0.1.2.tar", last modified: Fri Apr 19 02:50:23 2024, max compression
```

## Comparing `pySuperfish-0.1.1.tar` & `pySuperfish-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/pySuperfish.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/superfish/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-16 16:39:40.000000 pySuperfish-0.1.1/superfish/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16112 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10198 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/superfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/superfish/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-16 16:39:30.000000 pySuperfish-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/pySuperfish.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/superfish/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-19 02:50:23.000000 pySuperfish-0.1.2/superfish/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16112 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10184 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/superfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/superfish/writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-19 02:50:16.000000 pySuperfish-0.1.2/versioneer.py
```

### Comparing `pySuperfish-0.1.1/LICENSE` & `pySuperfish-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pySuperfish-0.1.1/PKG-INFO` & `pySuperfish-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: pySuperfish
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/ChristopherMayes/PySuperfish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySuperfish
 Python tools for Poisson Superfish calculations
 
 https://laacg.lanl.gov
 
+> :warning: As of April 2024, and since at least May 2023, the download site for
+Poisson/Superfish is unavailable. Unfortunately, we do not have any information
+about when or if it will be made available again. (see https://github.com/ChristopherMayes/PySuperfish/issues/2)
+
 ## Native Windows
 
 Download and install Poisson Supefish from:
 
 https://laacg.lanl.gov
 
+*see note above about availability of Poisson/Superfish files.
+
 ## Docker 
 
 Public (you must provide the executables)
 
 https://github.com/hhslepicka/docker-poisson-superfish-nobin
 
 (Private)
```

### Comparing `pySuperfish-0.1.1/README.md` & `pySuperfish-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # PySuperfish
 Python tools for Poisson Superfish calculations
 
 https://laacg.lanl.gov
 
+> :warning: As of April 2024, and since at least May 2023, the download site for
+Poisson/Superfish is unavailable. Unfortunately, we do not have any information
+about when or if it will be made available again. (see https://github.com/ChristopherMayes/PySuperfish/issues/2)
+
 ## Native Windows
 
 Download and install Poisson Supefish from:
 
 https://laacg.lanl.gov
 
+*see note above about availability of Poisson/Superfish files.
+
 ## Docker 
 
 Public (you must provide the executables)
 
 https://github.com/hhslepicka/docker-poisson-superfish-nobin
 
 (Private)
```

### Comparing `pySuperfish-0.1.1/pySuperfish.egg-info/PKG-INFO` & `pySuperfish-0.1.2/pySuperfish.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: pySuperfish
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/ChristopherMayes/PySuperfish
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PySuperfish
 Python tools for Poisson Superfish calculations
 
 https://laacg.lanl.gov
 
+> :warning: As of April 2024, and since at least May 2023, the download site for
+Poisson/Superfish is unavailable. Unfortunately, we do not have any information
+about when or if it will be made available again. (see https://github.com/ChristopherMayes/PySuperfish/issues/2)
+
 ## Native Windows
 
 Download and install Poisson Supefish from:
 
 https://laacg.lanl.gov
 
+*see note above about availability of Poisson/Superfish files.
+
 ## Docker 
 
 Public (you must provide the executables)
 
 https://github.com/hhslepicka/docker-poisson-superfish-nobin
 
 (Private)
```

### Comparing `pySuperfish-0.1.1/setup.py` & `pySuperfish-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pySuperfish-0.1.1/superfish/interpolate.py` & `pySuperfish-0.1.2/superfish/interpolate.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,17 +72,21 @@
         f.write(F)
     
     # Needed so that the fields aren't normalized to 1 MV/m average
     inifile = os.path.join(sf.path, 'SF.INI')
     with open(inifile, 'w') as f:
         f.write("""[global]
 Force1MVperMeter=No""")
+
+    # Needed on WSL, otherwise optional
+    t35file = sf.basename+'.T35'
     
+        
     # Run
-    sf.run_cmd('sf7', ifile)
+    sf.run_cmd('sf7', ifile, t35file)
     
     # Get the filename
     t7file = get_t7(sf.path)
     assert len(t7file) == 1, f'T7 file is missing.'
     t7file = t7file[0]
     
     
@@ -108,8 +112,8 @@
     else:
         if sf.output['sfo']['header']['variable']['XJFACT'] == 0:
             type = 'electric'
         else:
             type = 'magnetic'
         d =  parse_poisson_t7(t7file, type=type)
     
-    return d
+    return d
```

### Comparing `pySuperfish-0.1.1/superfish/parsers.py` & `pySuperfish-0.1.2/superfish/parsers.py`

 * *Files identical despite different names*

### Comparing `pySuperfish-0.1.1/superfish/plot.py` & `pySuperfish-0.1.2/superfish/plot.py`

 * *Files identical despite different names*

### Comparing `pySuperfish-0.1.1/superfish/superfish.py` & `pySuperfish-0.1.2/superfish/superfish.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,25 +239,25 @@
         
         if len(args) > 1:
             cmd = cmd + ' ' + ' '.join(args[1:])
        
         return cmd
         
     def run_cmd(self, *cmds, **kwargs):
-        """
-        Runs a command in in self.
+        r"""
+        Runs a command in self.
         
         Example:
             .run_cmd(['C:\LANL\AUTOMESH.EXE', 'TEST.AM'], timeout=1)
         
         """
-        if platform.system() == 'Windows':
-            cmds = self.windows_run_cmd(*cmds)
-        else:
+        if self.use_container:
             cmds = self.container_run_cmd(*cmds)
+        else:
+            cmds = self.windows_run_cmd(*cmds)
         
         self.vprint(f'Running: {cmds}')
     
         logfile = os.path.join(self.path, 'output.log')
     
         if self.use_container:
```

### Comparing `pySuperfish-0.1.1/superfish/writers.py` & `pySuperfish-0.1.2/superfish/writers.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     # Normalize on-axis field
     if normalize_by_Ez0:
         Ez0_max = 1e6*np.abs(t7data['Ez'][0,:]).max() # V/m
     else:
         Ez0_max = 1
         
     components = {}
-    components['electricField/r'] = t7data['Er'].reshape(nr, 1, nz).astype(np.complex) * 1e6/Ez0_max
-    components['electricField/z'] = t7data['Ez'].reshape(nr, 1, nz).astype(np.complex) * 1e6/Ez0_max
+    components['electricField/r'] = t7data['Er'].reshape(nr, 1, nz).astype(complex) * 1e6/Ez0_max
+    components['electricField/z'] = t7data['Ez'].reshape(nr, 1, nz).astype(complex) * 1e6/Ez0_max
     components['magneticField/theta'] = t7data['Hphi'].reshape(nr, 1, nz) * -1j*mu_0/Ez0_max # -i * mu_0
     
     
     
     return dict(attrs=attrs, components=components)
 
 
@@ -242,8 +242,8 @@
         keys = ['Br', 'Bz']
     
     # Unroll the arrays
     dat = np.array([t7data[f].reshape(nx*ny, order='F').T for f in keys]).T
     
     np.savetxt(filename, dat, header=header, comments='',  fmt = fmt)
     
-    return filename
+    return filename
```

### Comparing `pySuperfish-0.1.1/versioneer.py` & `pySuperfish-0.1.2/versioneer.py`

 * *Files identical despite different names*

