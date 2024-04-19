# Comparing `tmp/primerforge-1.0.0.tar.gz` & `tmp/primerforge-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerforge-1.0.0.tar", last modified: Thu Apr 18 18:10:50 2024, max compression
+gzip compressed data, was "primerforge-1.0.1.tar", last modified: Fri Apr 19 20:48:42 2024, max compression
```

## Comparing `primerforge-1.0.0.tar` & `primerforge-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-18 18:10:43.000000 primerforge-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-18 18:10:50.584383 primerforge-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-04-18 18:10:43.000000 primerforge-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/AnalysisData.py
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Log.py
--rw-r--r--   0 runner    (1001) docker     (127)    25046 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/Primer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/getCandidateKmers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/getPrimerPairs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18470 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-04-18 18:10:43.000000 primerforge-1.0.0/bin/removeOutgroupPrimers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 18:10:50.584383 primerforge-1.0.0/primerforge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-18 18:10:50.000000 primerforge-1.0.0/primerforge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 18:10:50.584383 primerforge-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-18 18:10:43.000000 primerforge-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:48:42.970077 primerforge-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 20:48:34.000000 primerforge-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-19 20:48:42.970077 primerforge-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-19 20:48:34.000000 primerforge-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:48:42.970077 primerforge-1.0.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/AnalysisData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/Clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28356 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/Parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/Primer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14444 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18304 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/getCandidateKmers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16993 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/getPrimerPairs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18470 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-04-19 20:48:34.000000 primerforge-1.0.1/bin/removeOutgroupPrimers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 20:48:42.970077 primerforge-1.0.1/primerforge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-19 20:48:42.000000 primerforge-1.0.1/primerforge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 20:48:42.970077 primerforge-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 20:48:34.000000 primerforge-1.0.1/setup.py
```

### Comparing `primerforge-1.0.0/LICENSE` & `primerforge-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/PKG-INFO` & `primerforge-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: primerforge
-Version: 1.0.0
+Version: 1.0.1
 Summary: software to identify primers that can be used to distinguish genomes
 Author: Joseph S. Wirth
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<img src="assets/logo.png" alt="Logo" width="250" height="250">
+
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
 ### `pip` installation
@@ -36,14 +38,28 @@
 conda activate primerforge
 ```
 
 ### Docker Installation
 
 A Docker image for the latest release is available at [DockerHub](https://hub.docker.com/r/jwirth/primerforge)
 
+### Checking installation
+
+If `primerForge` is installed correctly, then the following command should execute without errors:
+
+```shell
+primerForge --check_install
+```
+
+If you installed manually, you may need to use the following command instead
+
+```shell
+python primerforge.py --check_install
+```
+
 ## Usage
 
 ```text
 usage:
     primerForge [-ioaubfpgtrdnkvh]
 
 required arguments:
@@ -60,14 +76,15 @@
     -t, --tm_range       [float,float] a min and max melting temp (Tm) specified as a comma separated list (default: 55.0,68.0)
     -r, --pcr_prod       [int(s)] a single PCR product length or a range specified as 'min,max' (default: 120,2400)
     -d, --tm_diff        [float] the maximum allowable Tm difference between a pair of primers (default: 5.0)
     -n, --num_threads    [int] the number of threads for parallel processing (default: 1)
     -k, --keep           keep intermediate files (default: False)
     -v, --version        print the version
     -h, --help           print this message
+    --check_install      check installation
     --debug              run in debug mode (default: False)
 ```
 
 ## Workflow
 
 ```mermaid
 flowchart TB
```

### Comparing `primerforge-1.0.0/README.md` & `primerforge-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+<img src="assets/logo.png" alt="Logo" width="250" height="250">
+
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
 ### `pip` installation
@@ -25,14 +27,28 @@
 conda activate primerforge
 ```
 
 ### Docker Installation
 
 A Docker image for the latest release is available at [DockerHub](https://hub.docker.com/r/jwirth/primerforge)
 
+### Checking installation
+
+If `primerForge` is installed correctly, then the following command should execute without errors:
+
+```shell
+primerForge --check_install
+```
+
+If you installed manually, you may need to use the following command instead
+
+```shell
+python primerforge.py --check_install
+```
+
 ## Usage
 
 ```text
 usage:
     primerForge [-ioaubfpgtrdnkvh]
 
 required arguments:
@@ -49,14 +65,15 @@
     -t, --tm_range       [float,float] a min and max melting temp (Tm) specified as a comma separated list (default: 55.0,68.0)
     -r, --pcr_prod       [int(s)] a single PCR product length or a range specified as 'min,max' (default: 120,2400)
     -d, --tm_diff        [float] the maximum allowable Tm difference between a pair of primers (default: 5.0)
     -n, --num_threads    [int] the number of threads for parallel processing (default: 1)
     -k, --keep           keep intermediate files (default: False)
     -v, --version        print the version
     -h, --help           print this message
+    --check_install      check installation
     --debug              run in debug mode (default: False)
 ```
 
 ## Workflow
 
 ```mermaid
 flowchart TB
```

### Comparing `primerforge-1.0.0/bin/AnalysisData.py` & `primerforge-1.0.1/bin/AnalysisData.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/Clock.py` & `primerforge-1.0.1/bin/Clock.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/Log.py` & `primerforge-1.0.1/bin/Log.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/Parameters.py` & `primerforge-1.0.1/bin/Parameters.py`

 * *Files 19% similar despite different names*

```diff
@@ -148,14 +148,101 @@
                 except StopIteration:
                     fail = True
             
             # raise an error only after the file is closed
             if fail:
                 raise ValueError(f"{fn}{ERR_MSG}")
     
+    def __checkInstallation(self) -> None:
+        """checks the installation of all primerforge dependencies
+
+        Raises:
+            BaseException: incompatible python version
+            BaseException: biopython version is bad
+            BaseException: biopython not installed
+            BaseException: matplotlib version is bad
+            BaseException: matplotlib not installed
+            BaseException: numpy not installed
+            BaseException: primer3-py version is bad
+            BaseException: primer3-py not installed
+            BaseException: scipy version is bad
+            BaseException: scipy not installed
+        """
+        # constants
+        PY_MAJOR = 3
+        PY_MINOR = 11
+        BIO_VER = "1.81"
+        MPL_VER = "3.7.2"
+        P3_VER = 2
+        SCI_VER = (1, 10)
+        
+        # messages
+        BAD_VER = ' version is incompatible (requires '
+        NOT_INS = ' package is not installed'
+        SUCCESS = f'primerForge v{self.__version} is properly installed'
+        
+        # check python version
+        if sys.version_info.major != PY_MAJOR or not sys.version_info.minor >= PY_MINOR:
+            raise BaseException(f'incompatible python version (requires {PY_MAJOR}.{PY_MINOR} or above)')
+    
+        # check that all dependencies exist
+        # check Bio installation
+        try:
+            import Bio
+            
+            # check bio version
+            if Bio.__version__ != BIO_VER:
+                raise BaseException(f"'Bio'{BAD_VER}{BIO_VER})")
+        
+        except:
+            raise BaseException(f"'Bio'{NOT_INS}")
+
+        # check matplotlib installation
+        try:
+            import matplotlib
+            
+            # check matplotlib version
+            if matplotlib.__version__ != MPL_VER:
+                raise BaseException(f"'matplotlib{BAD_VER}{MPL_VER})")
+        
+        except:
+            raise BaseException(f"'matplotlib'{NOT_INS}")
+        
+        # check numpy installation
+        try:
+            import numpy
+        except:
+            raise BaseException(f"'numpy'{NOT_INS}")
+        
+        # check primer3-py installation
+        try:
+            import primer3
+            
+            # check primer3-py version
+            if int(primer3.__version__.split('.')[0]) < P3_VER:
+                raise BaseException(f"'primer3-py'{BAD_VER}{P3_VER} or above)")
+        
+        except:
+            raise BaseException(f"'primer3-py'{NOT_INS}")
+        
+        # check scipy installation
+        try:
+            import scipy
+            
+            # check scipy version
+            vers = tuple(map(int, scipy.__version__.split('.')))
+            if vers[0] < SCI_VER[0] or (vers[0] >= SCI_VER[0] and vers[1] < SCI_VER[1]):
+                raise BaseException(f"'scipy'{BAD_VER}{'.'.join(map(str,SCI_VER))} or above)")
+        
+        except:
+            raise BaseException(f"'scipy'{NOT_INS}")
+
+        # print success message
+        print(SUCCESS)
+    
     def __parseArgs(self) -> None:
         """parses command line arguments
 
         Raises:
             ValueError: invalid/missing ingroup files
             ValueError: invalid/missing ingroup files
             ValueError: invalid/missing outgroup files
@@ -190,14 +277,15 @@
         TM_FLAGS = ('-t', '--tm_range')
         THREADS_FLAGS = ('-n', '--num_threads')
         PCR_LEN_FLAGS = ('-r', '--pcr_prod')
         TM_DIFF_FLAGS = ('-d', '--tm_diff')
         KEEP_FLAGS = ('-k', '--keep')
         VERSION_FLAGS = ('-v', '--version')
         HELP_FLAGS = ('-h', '--help')
+        CHECK_FLAGS = ('--check_install',)
         DEBUG_FLAGS = ("--debug",)
         SHORT_OPTS = INGROUP_FLAGS[0][-1] + ":" + \
                      OUT_FLAGS[0][-1] + ":" + \
                      ANAL_FLAGS[0][1] + ":" + \
                      OUTGROUP_FLAGS[0][-1] + ":" + \
                      DISALLOW_FLAGS[0][-1] + ":" + \
                      FMT_FLAGS[0][-1] + ":" + \
@@ -221,14 +309,15 @@
                      TM_FLAGS[1][2:] + "=",
                      PCR_LEN_FLAGS[1][2:] + "=",
                      TM_DIFF_FLAGS[1][2:] + "=",
                      KEEP_FLAGS[1][2:],
                      THREADS_FLAGS[1][2:] + "=",
                      VERSION_FLAGS[1][2:],
                      HELP_FLAGS[1][2:],
+                     CHECK_FLAGS[0][2:],
                      DEBUG_FLAGS[0][2:])
 
         # messages
         ERR_MSG_1  = 'invalid or missing ingroup file(s)'
         ERR_MSG_2  = 'invalid or missing outgroup file(s)'
         ERR_MSG_3  = 'must specify exactly two integers for bad outgroup PCR product length'
         ERR_MSG_4  = 'bad outgroup PCR product lengths are not integers'
@@ -271,14 +360,15 @@
                        f"{GAP}{TM_FLAGS[0] + SEP_1 + TM_FLAGS[1]:<{WIDTH}}[float,float] a min and max melting temp (Tm) specified as a comma separated list{DEF_OPEN}{Parameters._DEF_MIN_TM}{SEP_3}{Parameters._DEF_MAX_TM}{CLOSE}{EOL}" + \
                        f"{GAP}{PCR_LEN_FLAGS[0] + SEP_1 + PCR_LEN_FLAGS[1]:<{WIDTH}}[int(s)] a single PCR product length or a range specified as 'min,max'{DEF_OPEN}{Parameters._DEF_MIN_PCR}{SEP_3}{Parameters._DEF_MAX_PCR}{CLOSE}{EOL}" + \
                        f"{GAP}{TM_DIFF_FLAGS[0] + SEP_1 + TM_DIFF_FLAGS[1]:<{WIDTH}}[float] the maximum allowable Tm difference between a pair of primers{DEF_OPEN}{Parameters._DEF_MAX_TM_DIFF}{CLOSE}{EOL}" + \
                        f"{GAP}{THREADS_FLAGS[0] + SEP_1 + THREADS_FLAGS[1]:<{WIDTH}}[int] the number of threads for parallel processing{DEF_OPEN}{Parameters._DEF_NUM_THREADS}{CLOSE}{EOL}" + \
                        f"{GAP}{KEEP_FLAGS[0] + SEP_1 + KEEP_FLAGS[1]:<{WIDTH}}keep intermediate files{DEF_OPEN}{Parameters._DEF_KEEP}{CLOSE}{EOL}" + \
                        f"{GAP}{VERSION_FLAGS[0] + SEP_1 + VERSION_FLAGS[1]:<{WIDTH}}print the version{EOL}" + \
                        f"{GAP}{HELP_FLAGS[0] + SEP_1 + HELP_FLAGS[1]:<{WIDTH}}print this message{EOL}" + \
+                       f"{GAP}{CHECK_FLAGS[0]:<{WIDTH}}check installation{EOL}" + \
                        f"{GAP}{DEBUG_FLAGS[0]:<{WIDTH}}run in debug mode{DEF_OPEN}{Parameters._DEF_DEBUG}{CLOSE}{EOL*2}"
             
             print(HELP_MSG)
             
         # set default values
         self.ingroupFns = None
         self.resultsFn = os.path.join(os.getcwd(), Parameters._DEF_RESULTS_FN)
@@ -307,14 +397,19 @@
             printHelp()
         
         # print the version if requested
         elif VERSION_FLAGS[0] in sys.argv or VERSION_FLAGS[1] in sys.argv:
             self.helpRequested = True
             print(self.__version)
         
+        # check the installation if requested
+        elif CHECK_FLAGS[0] in sys.argv:
+            self.helpRequested = True
+            self.__checkInstallation()
+        
         # parse command line arguments
         else:
             opts,args = getopt.getopt(sys.argv[1:], SHORT_OPTS, LONG_OPTS)
             for opt,arg in opts:
                 # get the ingroup filenames
                 if opt in INGROUP_FLAGS:
                     self.ingroupFns = glob.glob(arg)
```

### Comparing `primerforge-1.0.0/bin/Primer.py` & `primerforge-1.0.1/bin/Primer.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/analysis.py` & `primerforge-1.0.1/bin/analysis.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/getCandidateKmers.py` & `primerforge-1.0.1/bin/getCandidateKmers.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/getPrimerPairs.py` & `primerforge-1.0.1/bin/getPrimerPairs.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/bin/main.py` & `primerforge-1.0.1/bin/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bin.AnalysisData import AnalysisData
 from bin.getCandidateKmers import _getAllCandidateKmers
 from bin.removeOutgroupPrimers import _removeOutgroupPrimers
 from bin.getPrimerPairs import _getPrimerPairs, _keepOnePairPerBinPair
 from bin.analysis import _initializeAnalysisData, _updateAnalysisData, _plotAnalysisData
 
 # global constants
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __author__ = "Joseph S. Wirth"
 __SHARED_NUM = 0
 __CAND_NUM   = 1
 __PAIR_1_NUM = 2
 __PAIR_2_NUM = 3
 __PAIR_3_NUM = 4
 __ANAL_NUM   = 5
```

### Comparing `primerforge-1.0.0/bin/removeOutgroupPrimers.py` & `primerforge-1.0.1/bin/removeOutgroupPrimers.py`

 * *Files identical despite different names*

### Comparing `primerforge-1.0.0/primerforge.egg-info/PKG-INFO` & `primerforge-1.0.1/primerforge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: primerforge
-Version: 1.0.0
+Version: 1.0.1
 Summary: software to identify primers that can be used to distinguish genomes
 Author: Joseph S. Wirth
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+<img src="assets/logo.png" alt="Logo" width="250" height="250">
+
 # primerForge
 
 software to identify primers that can be used to distinguish genomes
 
 ## Installation
 
 ### `pip` installation
@@ -36,14 +38,28 @@
 conda activate primerforge
 ```
 
 ### Docker Installation
 
 A Docker image for the latest release is available at [DockerHub](https://hub.docker.com/r/jwirth/primerforge)
 
+### Checking installation
+
+If `primerForge` is installed correctly, then the following command should execute without errors:
+
+```shell
+primerForge --check_install
+```
+
+If you installed manually, you may need to use the following command instead
+
+```shell
+python primerforge.py --check_install
+```
+
 ## Usage
 
 ```text
 usage:
     primerForge [-ioaubfpgtrdnkvh]
 
 required arguments:
@@ -60,14 +76,15 @@
     -t, --tm_range       [float,float] a min and max melting temp (Tm) specified as a comma separated list (default: 55.0,68.0)
     -r, --pcr_prod       [int(s)] a single PCR product length or a range specified as 'min,max' (default: 120,2400)
     -d, --tm_diff        [float] the maximum allowable Tm difference between a pair of primers (default: 5.0)
     -n, --num_threads    [int] the number of threads for parallel processing (default: 1)
     -k, --keep           keep intermediate files (default: False)
     -v, --version        print the version
     -h, --help           print this message
+    --check_install      check installation
     --debug              run in debug mode (default: False)
 ```
 
 ## Workflow
 
 ```mermaid
 flowchart TB
```

### Comparing `primerforge-1.0.0/setup.py` & `primerforge-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='primerforge',
-    version='1.0.0',
+    version='1.0.1',
     author='Joseph S. Wirth',
     packages=find_packages(),
     description='software to identify primers that can be used to distinguish genomes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         'biopython==1.81',
```

