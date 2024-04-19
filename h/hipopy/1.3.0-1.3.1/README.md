# Comparing `tmp/hipopy-1.3.0.tar.gz` & `tmp/hipopy-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hipopy-1.3.0.tar", max compression
+gzip compressed data, was "hipopy-1.3.1.tar", max compression
```

## Comparing `hipopy-1.3.0.tar` & `hipopy-1.3.1.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1098 2024-04-11 20:15:48.863986 hipopy-1.3.0/LICENSE
--rw-r--r--   0        0        0     1001 2024-04-11 20:15:48.864143 hipopy-1.3.0/README.md
--rw-r--r--   0        0        0      108 2024-04-18 20:16:20.203572 hipopy-1.3.0/hipopy/__init__.py
--rw-r--r--   0        0        0    30484 2024-04-17 18:03:08.077803 hipopy-1.3.0/hipopy/hipopy.py
--rw-r--r--   0        0        0      513 2024-04-18 20:15:36.420722 hipopy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 hipopy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-11 20:15:48.863986 hipopy-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1001 2024-04-18 20:43:32.190734 hipopy-1.3.1/README.md
+-rw-r--r--   0        0        0      108 2024-04-19 15:57:00.912124 hipopy-1.3.1/hipopy/__init__.py
+-rw-r--r--   0        0        0    35709 2024-04-19 15:50:27.709925 hipopy-1.3.1/hipopy/hipopy.py
+-rw-r--r--   0        0        0    35778 2024-04-18 20:43:27.454609 hipopy-1.3.1/hipopy/hipopy__BACKUP.py
+-rw-r--r--   0        0        0     5594 2024-04-18 21:19:07.532207 hipopy-1.3.1/hipopy/test1.py
+-rw-r--r--   0        0        0     3317 2024-04-18 21:19:05.507302 hipopy-1.3.1/hipopy/test2.py
+-rw-r--r--   0        0        0      513 2024-04-19 15:57:50.383260 hipopy-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 hipopy-1.3.1/PKG-INFO
```

### Comparing `hipopy-1.3.0/LICENSE` & `hipopy-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.0/README.md` & `hipopy-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hipopy-1.3.0/hipopy/hipopy.py` & `hipopy-1.3.1/hipopy/hipopy.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     -----------
     Open a HIPO file to read.
     """
     f = hipofile(filename,mode=mode,tags=tags)
     f.open()
     return f
 
-def iterate(files,banks=None,step=100,tags=None):
+def iterate(files,banks=None,step=100,tags=None,experimental=False):
     """
     Parameters
     ----------
     files : list, required
         List of file names
     banks : list, optional
         List of bank names to read
@@ -48,21 +48,25 @@
     step : int, optional
         Batch size for iterating through file events
         Default : 100
     tags : int or list of ints, optional
         Set bank tags for reader to use.  0 works for most banks.
         1 is needed for scaler banks.
         Default : None
+    experimental : bool, optional
+        Whether to use experimental hipopybind.HipoFileIterator to iterate files
+        Default : False
 
     Description
     -----------
     Iterate through a list of hipofiles reading all banks unless specific banks are specified.
     Iteration is broken into batches of step events.
     """
-    f = hipochain(files,banks,step=step,tags=tags)
+    if tags is None and experimental: tags = []
+    f = hipochain(files,banks,step=step,tags=tags,experimental=experimental)
     return f
 
 def create(filename):
     """
     Parameters
     ----------
     filename : string, required
@@ -120,14 +124,15 @@
         Name of buffer file
     banklist : dict
         Dictionary to hipopybind.Bank objects
     """
 
     # Methods
     # -------
+    # __len__
     # open
     # flush
     # close
     # goToEvent
     # nextEvent
     # addSchema
     # addEvent
@@ -174,14 +179,22 @@
         self.group      = 0
         self.item       = 1
         self.dtypes     = {}
         self.buffext    = "~"
         self.buffname   = None
         self.banklist   = {}
         self.tags       = tags
+
+    def __len__(self):
+        """
+        Return
+        ------
+        Length of the file
+        """
+        return self.reader.getEntries()
         
     def open(self):
         """
         Description
         -----------
         Open a HIPO file to read, write (from scratch), or append data.
         IMPORTANT:  Make sure you add schema before opening a file to write!
@@ -849,15 +862,15 @@
         1 is needed for scaler banks.
 
     Description
     -----------
     Chains files together so they may be read continuously.
     """
 
-    def __init__(self,names,banks=None,step=100,mode="r",tags=None):
+    def __init__(self,names,banks=None,step=100,mode="r",tags=None,experimental=False):
         self.names   = names
 
         # Parse regex NOTE: Must be full or relative path from $PWD.  ~/... does not work.
         if type(self.names)==str:
             self.names = glob.glob(names)
         else:
             newnames = []
@@ -869,17 +882,18 @@
             self.names = newnames
 
         self.banks   = banks
         self.step    = step
         self.mode    = "r"   #TODO: Does it make sense to just fix this?
         self.verbose = False #TODO: Do we really need this?
         self.tags    = tags
+        self.experimental = experimental
 
     def __iter__(self):
-        return hipochainIterator(self)
+        return hipochainIterator(self) if not self.experimental else hipochainIteratorExperimental(self)
 
 class hipochainIterator:
 
     """
     Attributes
     ----------
     chain : hipopy.hipopy.hipochain
@@ -908,14 +922,20 @@
         self.chain   = chain
         self.nnames  = len(self.chain.names) #NOTE: Assumes this will stay constant.
         self.idx     = -1
         self.counter = 0
         self.file    = None
         self.items   = {}
         self.dict    = None
+        # self.experimental = True
+        # self.tags = [0,1] #NOTE: EXPERIMENTAL
+        # if self.experimental and self.chain.banks is None: self.switchFile()
+        # if self.experimental:
+        #     self.reached_end = False
+        #     self.hbHipoFileIterator = hipopybind.HipoFileIterator(self.chain.names,self.chain.banks,self.chain.step,self.tags) #NOTE: EXPERIMENTAL
 
     def switchFile(self):
         """
         Description
         -----------
         Checks if next file in chain exists and then opens and reads requested banks if so.
         """
@@ -936,14 +956,36 @@
     def __next__(self):
         """
         Description
         -----------
         Loops files reading requested banks if they exist 
         """
 
+        # if self.experimental:
+
+        #     has_events = self.hbHipoFileIterator.__next__()
+        #     banknames = self.hbHipoFileIterator.banknames
+        #     items = self.hbHipoFileIterator.items
+        #     types = self.hbHipoFileIterator.types
+        #     datadict = {}
+        #     for idx, bankname in enumerate(banknames):
+        #         for idx2, item in enumerate(items[idx]):
+        #             item_type = types[idx][idx2]
+        #             if item_type==5: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getDoubles(bankname,item)
+        #             elif item_type==4: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getFloats(bankname,item)
+        #             elif item_type==3: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getInts(bankname,item)
+        #             elif item_type==8: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getLongs(bankname,item)
+        #             elif item_type==2: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getShorts(bankname,item)
+        #             elif item_type==1: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getBytes(bankname,item)
+
+        #     self.experimental = has_events
+        #     return datadict
+        # raise StopIteration
+        
+
         if self.idx == -1: self.switchFile() # Load first file manually
 
         if self.idx<(self.nnames): #TODO: Check this condition.
 
             # Check if output array has been initialized
             if self.dict is None:
                 self.dict = {}
@@ -982,7 +1024,82 @@
         if self.dict != None and len(self.dict.keys())>0:
             res       = self.dict
             self.dict = None
             return res #TODO: Will this return last remainder that is not necessarily stepsize?
         
         # Final stop
         raise StopIteration
+
+class hipochainIteratorExperimental:
+
+    """
+    Attributes
+    ----------
+    chain : hipopy.hipopy.hipochain
+        Hipochain object overwhich to iterate
+    idx : int
+        Index of current file in hipochain
+    counter : int
+        Event counter for batching data
+    file : hipopy.hipopy.hipoFile
+        Current file in hipochain
+    items : dict
+        Dictionary of bank names to item names to read
+    dict : dict
+        Dictionary into which Hipo bank data is read
+
+    Methods
+    -------
+    getAllBanks
+
+    Description
+    -----------
+    Experimental iterator for hipopy.hipopy.hipochain class
+    """
+
+    def __init__(self,chain):
+        self.chain   = chain
+        self.nnames  = len(self.chain.names) #NOTE: Assumes this will stay constant.
+        self.idx     = -1
+        self.file    = None
+        if self.chain.banks is None: self.getAllBankNames()
+        self.has_events = True
+        self.hbHipoFileIterator = hipopybind.HipoFileIterator(self.chain.names,self.chain.banks,self.chain.step,self.chain.tags)
+        self.banknames = self.hbHipoFileIterator.banknames
+        self.items = self.hbHipoFileIterator.items
+        self.types = self.hbHipoFileIterator.types
+
+    def getAllBankNames(self):
+        """
+        Description
+        -----------
+        Checks if next file in chain exists and then opens and reads requested banks if so.
+        """
+        # Open file
+        self.idx += 1 #NOTE: Do this before everything below since we initiate at -1.
+        if self.idx>=self.nnames: return #NOTE: Sanity check
+        self.file = hipofile(self.chain.names[self.idx],mode=self.chain.mode,tags=self.chain.tags)
+        self.file.open()
+
+        if self.chain.banks is None: self.chain.banks = self.file.getBanks() #NOTE: This assumes all the files in the chain have the same banks.
+
+    def __next__(self):
+        """
+        Description
+        -----------
+        Loops files reading requested banks if they exist 
+        """
+        
+        if self.has_events:
+            self.has_events = self.hbHipoFileIterator.__next__()
+            datadict = {}
+            for idx, bankname in enumerate(self.banknames):
+                for idx2, item in enumerate(self.items[idx]):
+                    item_type = self.types[idx][idx2]
+                    if item_type==5: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getDoubles(bankname,item)
+                    elif item_type==4: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getFloats(bankname,item)
+                    elif item_type==3: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getInts(bankname,item)
+                    elif item_type==8: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getLongs(bankname,item)
+                    elif item_type==2: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getShorts(bankname,item)
+                    elif item_type==1: datadict[bankname+"_"+item] = self.hbHipoFileIterator.getBytes(bankname,item)
+            return datadict
+        raise StopIteration
```

### Comparing `hipopy-1.3.0/pyproject.toml` & `hipopy-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "hipopy"
-version = "1.3.0"
+version = "1.3.1"
 license = "MIT"
 description = "UpROOT-Like I/O Interface for CLAS12 HIPO Files"
 authors = ["Matthew McEneaney <matthew.mceneaney@duke.edu>"]
 repository = "https://github.com/mfmceneaney/hipopy.git"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7.3"
 awkward = "^1.3.0"
 numpy = "^1.19.2"
-hipopybind = ">=1.0.1"
+hipopybind = ">=1.1.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hipopy-1.3.0/PKG-INFO` & `hipopy-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: hipopy
-Version: 1.3.0
+Version: 1.3.1
 Summary: UpROOT-Like I/O Interface for CLAS12 HIPO Files
 Home-page: https://github.com/mfmceneaney/hipopy.git
 License: MIT
 Author: Matthew McEneaney
 Author-email: matthew.mceneaney@duke.edu
 Requires-Python: >=3.7.3,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: awkward (>=1.3.0,<2.0.0)
-Requires-Dist: hipopybind (>=1.0.1)
+Requires-Dist: hipopybind (>=1.1.0)
 Requires-Dist: numpy (>=1.19.2,<2.0.0)
 Project-URL: Repository, https://github.com/mfmceneaney/hipopy.git
 Description-Content-Type: text/markdown
 
 # HIPOPy: UpROOT-like I/O Interface for CLAS12 HIPO Files
 
 ## Prerequisites
```

