# Comparing `tmp/fapyc-0.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/fapyc-0.5.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 816600 bytes, number of entries: 14
+Zip file size: 840160 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat      695 b- defN 23-Nov-24 07:45 fapyc/__init__.py
--rw-rw-rw-  2.0 fat   181248 b- defN 23-Dec-01 12:28 fapyc/_fapyc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    10276 b- defN 23-Dec-01 12:27 fapyc/include/fapec_comp.h
--rw-rw-rw-  2.0 fat    22482 b- defN 23-Dec-01 12:27 fapyc/include/fapec_decomp.h
--rw-rw-rw-  2.0 fat    38432 b- defN 23-Dec-01 12:27 fapyc/include/fapec_opts.h
--rw-rw-rw-  2.0 fat   842752 b- defN 23-Dec-01 12:27 fapyc/lib/FapecCompress.dll
--rw-rw-rw-  2.0 fat    18024 b- defN 23-Dec-01 12:27 fapyc/lib/FapecCompress.lib
--rw-rw-rw-  2.0 fat   684544 b- defN 23-Dec-01 12:27 fapyc/lib/FapecDecompress.dll
--rw-rw-rw-  2.0 fat    21836 b- defN 23-Dec-01 12:27 fapyc/lib/FapecDecompress.lib
--rw-rw-rw-  2.0 fat     1562 b- defN 23-Dec-01 12:28 fapyc-0.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     8571 b- defN 23-Dec-01 12:28 fapyc-0.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Dec-01 12:28 fapyc-0.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Dec-01 12:28 fapyc-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1139 b- defN 23-Dec-01 12:28 fapyc-0.4.0.dist-info/RECORD
-14 files, 1831667 bytes uncompressed, 814736 bytes compressed:  55.5%
+-rw-rw-rw-  2.0 fat   239616 b- defN 24-Apr-19 12:26 fapyc/_fapyc.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    10276 b- defN 24-Apr-11 10:08 fapyc/include/fapec_comp.h
+-rw-rw-rw-  2.0 fat    22482 b- defN 24-Apr-19 09:47 fapyc/include/fapec_decomp.h
+-rw-rw-rw-  2.0 fat    37841 b- defN 24-Apr-19 09:47 fapyc/include/fapec_opts.h
+-rw-rw-rw-  2.0 fat   842752 b- defN 24-Apr-11 10:08 fapyc/lib/FapecCompress.dll
+-rw-rw-rw-  2.0 fat    18024 b- defN 24-Apr-11 10:08 fapyc/lib/FapecCompress.lib
+-rw-rw-rw-  2.0 fat   684544 b- defN 24-Apr-11 10:08 fapyc/lib/FapecDecompress.dll
+-rw-rw-rw-  2.0 fat    21836 b- defN 24-Apr-11 10:08 fapyc/lib/FapecDecompress.lib
+-rw-rw-rw-  2.0 fat     1562 b- defN 24-Apr-19 12:26 fapyc-0.5.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    10048 b- defN 24-Apr-19 12:26 fapyc-0.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-Apr-19 12:26 fapyc-0.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-19 12:26 fapyc-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1140 b- defN 24-Apr-19 12:26 fapyc-0.5.0.dist-info/RECORD
+14 files, 1890922 bytes uncompressed, 838296 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: fapyc/lib/FapecDecompress.dll
 Comment: 
 
 Filename: fapyc/lib/FapecDecompress.lib
 Comment: 
 
-Filename: fapyc-0.4.0.dist-info/LICENSE
+Filename: fapyc-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: fapyc-0.4.0.dist-info/METADATA
+Filename: fapyc-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: fapyc-0.4.0.dist-info/WHEEL
+Filename: fapyc-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: fapyc-0.4.0.dist-info/top_level.txt
+Filename: fapyc-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fapyc-0.4.0.dist-info/RECORD
+Filename: fapyc-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fapyc/include/fapec_opts.h

```diff
@@ -190,23 +190,14 @@
 WINDOWS_VISIBILITY void fapec_usropts_get(int fapecUsrOpts, int *verbLevel, int *askOverwrite, int *deleteInput,
 		int *enforcePriv, int *streamMode, int *noAttr, int *noCompHead,
 		int *edacOpt, int *cryptOpt, int *threadPool, int *decMode,
 		int *noNames, int *noFoot, int *abortErr,
 		int *noRecurseDir, int *keepLinks) LINUX_VISIBILITY;
 
 /**
- * Update the log level in the user configuration variable.
- * @param fapecUsrOpts The variable with all user options, which will be updated with the new log level setting.
- * @param logLevel The log level to be set: 0 means completely silent (except warnings and errors),
- *                 1 means basic logging (e.g. at part level), 2 means progress logging (e.g. percentage),
- *                 3 means more exhaustive logging (e.g. part algorithm during decompression).
- */
-WINDOWS_VISIBILITY void fapec_usropts_set_loglev(int *fapecUsrOpts, int logLev) LINUX_VISIBILITY;
-
-/**
  * Update the number of threads in the user configuration variable.
  * @param fapecUsrOpts The variable with all user options, which will be updated with the new threadPool setting.
  * @param threadPool The threads to be used: 0 (or negative) means single-thread, 1 means one thread for
  *        compression/decompression plus read/write threads, and >=2 means multi-thread for comp/decomp.
  */
 WINDOWS_VISIBILITY void fapec_usropts_set_nthreads(int *fapecUsrOpts, int threadPool) LINUX_VISIBILITY;
```

## Comparing `fapyc-0.4.0.dist-info/LICENSE` & `fapyc-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fapyc-0.4.0.dist-info/METADATA` & `fapyc-0.5.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fapyc
-Version: 0.4.0
+Version: 0.5.0
 Summary: A Python wrapper for the FAPEC data compressor.
 Home-page: https://www.dapcom.es
 Author: DAPCOM Data Services
 Author-email: fapec@dapcom.es
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -63,20 +63,42 @@
 With this example we can view a colour image compressed with FAPEC:
 
     from fapyc import Unfapyc
     import numpy as np
     from matplotlib import pyplot as plt
 
     filename = input("Path to FAPEC-compressed 8-bit RGB image file: ")
-    # For now, the API does not provide yet the image dimensions (it will be added soon), so we have to manually indicate them
-    w,h = input("Width and height (in pixels) of the image (two space-separated values): ").split()
-    w = int(w)
-    h = int(h)
+
     # Decompress the file into a byte array buffer
     uf = Unfapyc(filename = filename)
+
+    # Get the image features - assuming part index 0 (OK for a single-part archive; otherwise, we're simply taking the first part)
+    cmpOpts = uf.fapyc_get_part_cmpopts(0)
+
+    # Get the compression algorithm, which should be CILLIC, DWT or HPA for an image
+    algo = cmpOpts['algorithm'].decode('utf-8')
+    if algo != 'CILLIC' and algo != 'DWT' and algo != 'HPA':
+        raise Exception("Not an image")
+    else:
+        print("Found image compressed with the",algo,"algorithm")
+
+    # Get the image features we need
+    w = cmpOpts['imageWidth']
+    h = cmpOpts['imageHeight']
+    bpp = cmpOpts['sampleBits']
+    bands = cmpOpts['nBands']
+    coding = cmpOpts['bandsCoding']
+    coding2text = ['BIP','BIL','BSQ']
+
+    # Do some check
+    if bpp != 8 or bands != 3 or coding != 0:
+        raise Exception("This test needs 8-bit colour images (3 colour bands) in pixel-interleaved coding mode")
+    else:
+        print("Image features:",w,"x",h,"pixels,",bpp,"bits per pixel,",bands,"colour bands,",coding2text[coding],"coding")
+
     uf.decompress()
     # Check consistency (image dimensions vs. buffer size)
     if len(uf.outputBuffer) != 3*w*h:
         print("Image dimensions inconsistent with file contents!")
     else:
         # Reshape this one-dimensional array into a three-dimensional array (height, width, colours) to plot it
         ima = np.reshape(np.frombuffer(uf.outputBuffer, dtype=np.dtype('u1')), (h, w, 3))
@@ -195,9 +217,29 @@
     plt.xlabel("G magnitude")
     plt.ylabel("Parallax error")
     print("Getting 2D histogram...")
     plt.hist2d(df.phot_g_mean_mag, df.parallax_error, bins=(100, 100), norm = colors.LogNorm(), cmap=plt.cm.jet)
 
     print("Plotting...")
     plt.show()
+### Compress file with a logger
+
+In this example, the user can provide a Python `logger` to get an information message from Fapyc, like if any error occurs.
+
+    import logging
+    from fapyc import Fapyc, Unfapyc
+
+    filename = input("Path to the file to compress: ")
+    logger_file = 'fapyc.log'
+    logger = logging.getLogger(__name__)
+    logging.basicConfig(filename=logger_file, filemode='w', format='%(name)s - %(levelname)s - %(message)s')
+    logger.setLevel(logging.DEBUG)
+
+
+    file = open(filename, "rb")
+    data = file.read()
+    file.close()
+
 
+    f = Fapyc(filename = filename, logger = logger)
+    f.compress_doubles(output = "a.fapec")
```

## Comparing `fapyc-0.4.0.dist-info/RECORD` & `fapyc-0.5.0.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 fapyc/__init__.py,sha256=StBkl0B4UJyK9Cb0r3ZGMMQbLch0u5_3mxd0DjLonxQ,695
-fapyc/_fapyc.cp39-win_amd64.pyd,sha256=k9lSUyUndw3uOVa3ehdq0NEfc5_cM2g__UkXXruPk0k,181248
+fapyc/_fapyc.cp39-win_amd64.pyd,sha256=lSqplCFcUt7BKM7X8KC0th1H1HiDNGOZ4H4bRSRstaY,239616
 fapyc/include/fapec_comp.h,sha256=tNYN4no-VrdL_wgCnskCCybAy8Hzf9vnMI0a3_o-SY0,10276
 fapyc/include/fapec_decomp.h,sha256=tQv3-RB5LeD3eHEYCaFy9ZkXGx45My9Maq2zWICdvNQ,22482
-fapyc/include/fapec_opts.h,sha256=crOTMAdqmsjIkIYLmInyFOos3N1gWcRALlxjsUY6K7o,38432
+fapyc/include/fapec_opts.h,sha256=VlRgpSvZ2A5HsDqTXK3BCF9Lzape65u4y7OLZVeUZEg,37841
 fapyc/lib/FapecCompress.dll,sha256=HHPG6LVAS0-vBlol1Nw_87t_nINhscaEMAG8XHjcDsM,842752
 fapyc/lib/FapecCompress.lib,sha256=xploA0IeuucEHUVIUjnEEh7U3TVmg0lrhV7RelqgBvU,18024
 fapyc/lib/FapecDecompress.dll,sha256=3NLfImemcoz28T2wjxDaV8X0fV1t-8B_rWoVziBbMIg,684544
 fapyc/lib/FapecDecompress.lib,sha256=9omWRmkTlANQ65BEuxl2X5cz-McTWjdN8fX1-eCAISg,21836
-fapyc-0.4.0.dist-info/LICENSE,sha256=YNa31L4GxB-BGz8KRqKqZRUw6RuybSNI6c7NUCQCHWI,1562
-fapyc-0.4.0.dist-info/METADATA,sha256=x1tgSab6KzVspJvfad4-FoihGaPE8exPWhFCaofqy-c,8571
-fapyc-0.4.0.dist-info/WHEEL,sha256=QEPhY-QL5bUCGe8xLO1ow2Nlf5beRmRJkZ8YmG0I2hM,100
-fapyc-0.4.0.dist-info/top_level.txt,sha256=6mrRg_DSbXtLEwgE5fSxauj64kL7igSCWnZx2vQbpWY,6
-fapyc-0.4.0.dist-info/RECORD,,
+fapyc-0.5.0.dist-info/LICENSE,sha256=YNa31L4GxB-BGz8KRqKqZRUw6RuybSNI6c7NUCQCHWI,1562
+fapyc-0.5.0.dist-info/METADATA,sha256=Vsq9Kvo_3RO6GDR5u94zEnEdRiVPGqgFBgKRtAxGUgg,10048
+fapyc-0.5.0.dist-info/WHEEL,sha256=QEPhY-QL5bUCGe8xLO1ow2Nlf5beRmRJkZ8YmG0I2hM,100
+fapyc-0.5.0.dist-info/top_level.txt,sha256=6mrRg_DSbXtLEwgE5fSxauj64kL7igSCWnZx2vQbpWY,6
+fapyc-0.5.0.dist-info/RECORD,,
```

