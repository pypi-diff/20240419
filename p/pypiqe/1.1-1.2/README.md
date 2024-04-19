# Comparing `tmp/pypiqe-1.1-py3-none-any.whl.zip` & `tmp/pypiqe-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7838 bytes, number of entries: 7
+Zip file size: 7840 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat       22 b- defN 23-Jul-04 19:40 pypiqe/__init__.py
--rw-rw-rw-  2.0 fat    13703 b- defN 23-Jul-04 19:38 pypiqe/piqe.py
--rw-rw-rw-  2.0 fat     1096 b- defN 23-Jul-04 19:53 pypiqe-1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4467 b- defN 23-Jul-04 19:53 pypiqe-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-04 19:53 pypiqe-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-04 19:53 pypiqe-1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      515 b- defN 23-Jul-04 19:53 pypiqe-1.1.dist-info/RECORD
-7 files, 19902 bytes uncompressed, 6932 bytes compressed:  65.2%
+-rw-rw-rw-  2.0 fat    13703 b- defN 24-Apr-19 14:45 pypiqe/piqe.py
+-rw-rw-rw-  2.0 fat     1096 b- defN 24-Apr-19 14:54 pypiqe-1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4463 b- defN 24-Apr-19 14:54 pypiqe-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-19 14:54 pypiqe-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-19 14:54 pypiqe-1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      515 b- defN 24-Apr-19 14:54 pypiqe-1.2.dist-info/RECORD
+7 files, 19898 bytes uncompressed, 6934 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pypiqe/__init__.py
 Comment: 
 
 Filename: pypiqe/piqe.py
 Comment: 
 
-Filename: pypiqe-1.1.dist-info/LICENSE
+Filename: pypiqe-1.2.dist-info/LICENSE
 Comment: 
 
-Filename: pypiqe-1.1.dist-info/METADATA
+Filename: pypiqe-1.2.dist-info/METADATA
 Comment: 
 
-Filename: pypiqe-1.1.dist-info/WHEEL
+Filename: pypiqe-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: pypiqe-1.1.dist-info/top_level.txt
+Filename: pypiqe-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pypiqe-1.1.dist-info/RECORD
+Filename: pypiqe-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pypiqe/piqe.py

 * *Ordering differences only*

```diff
@@ -116,32 +116,32 @@
     activityThreshold = 0.1  # Threshold used to identify high spatially prominent blocks
     blockImpairedThreshold = 0.1  # Threshold used to identify blocks having noticeable artifacts
     windowSize = 6  # Considered segment size in a block edge.
     nSegments = blockSize-windowSize+1  # Number of segments for each block edge
     distBlockScores = 0  # Accumulation of distorted block scores
     NHSA = 0  # Number of high spatial active blocks.
 
+    # RGB to Gray Conversion
+    if ipImage.ndim == 3:
+        ipImage = cv2.cvtColor(ipImage, cv2.COLOR_BGR2GRAY)
+
     # Pad if size(ipImage) is not divisible by blockSize.
     originalSize = ipImage.shape  # Actual image size
     rows, columns = originalSize[:2]
     rowsPad = rows % blockSize
     columnsPad = columns % blockSize
     isPadded = False
     if rowsPad > 0 or columnsPad > 0:
         if rowsPad > 0:
             rowsPad = blockSize - rowsPad
         if columnsPad > 0:
             columnsPad = blockSize - columnsPad
         isPadded = True
         ipImage = np.pad(ipImage, ((0, rowsPad), (0, columnsPad)), mode='symmetric')
 
-    # RGB to Gray Conversion
-    if ipImage.ndim == 3:
-        ipImage = cv2.cvtColor(ipImage, cv2.COLOR_BGR2GRAY)
-
     # Convert input image to double and scaled to the range 0-255
     ipImage = np.round(255 * (ipImage / np.max(ipImage)))
 
     # Normalize image to zero mean and ~unit std
     # used circularly-symmetric Gaussian weighting function sampled out 
     # to 3 standard deviations.
     mu = cv2.GaussianBlur(ipImage, ksize=(7, 7), sigmaX=7/6, borderType=cv2.BORDER_REPLICATE)
```

## Comparing `pypiqe-1.1.dist-info/LICENSE` & `pypiqe-1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pypiqe-1.1.dist-info/METADATA` & `pypiqe-1.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pypiqe
-Version: 1.1
+Version: 1.2
 Summary: A python version of Matlab's Perception based Image Quality Evaluator (PIQE) no-reference image quality score
 Home-page: https://github.com/michael-rutherford/pypiqe
 Author: Michael W. Rutherford
 Author-email: sykiemikey@hotmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy (>=1.25.0)
-Requires-Dist: opencv-python (>=4.7.0.72)
+Requires-Dist: numpy >=1.25.0
+Requires-Dist: opencv-python >=4.7.0.72
 
 # Perception based Image Quality Evaluator (PIQE) 
 ## No-reference image quality assessment score for Python
 
 Converted from and tested against the [MATLAB function](https://www.mathworks.com/help/images/ref/piqe.html).
 
 Based on the paper:
```

## Comparing `pypiqe-1.1.dist-info/RECORD` & `pypiqe-1.2.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 pypiqe/__init__.py,sha256=ojPwA2BrJkKfxv3cQ_00NSN3ckewgAFDPxr2MRFVJXw,22
-pypiqe/piqe.py,sha256=F0zZY_BYyrCkNB7RAR5BSXDlEnzX7X4Np0SzUP8-PJ8,13703
-pypiqe-1.1.dist-info/LICENSE,sha256=S5OcQ_VkMRTZNmrF_qZ3-idbeUEnzYyIxTW_eiR5ke8,1096
-pypiqe-1.1.dist-info/METADATA,sha256=Y63L2UJg-n4DWT3KmDvmnfdWDdZMSeb31TqwULl1nw4,4467
-pypiqe-1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pypiqe-1.1.dist-info/top_level.txt,sha256=Nqv87DWtPbn3bNWwLPUbOnB0797skz_u8DD2lJKgGyE,7
-pypiqe-1.1.dist-info/RECORD,,
+pypiqe/piqe.py,sha256=d6Q_XkRAKX8Mpv1sURGjWN31pT9FjTA1fAVUfepO7GA,13703
+pypiqe-1.2.dist-info/LICENSE,sha256=S5OcQ_VkMRTZNmrF_qZ3-idbeUEnzYyIxTW_eiR5ke8,1096
+pypiqe-1.2.dist-info/METADATA,sha256=HVj8b9rKLB6AgZDBwk4DWPhRDEzqhsJ7RFCKaVwoEh4,4463
+pypiqe-1.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pypiqe-1.2.dist-info/top_level.txt,sha256=Nqv87DWtPbn3bNWwLPUbOnB0797skz_u8DD2lJKgGyE,7
+pypiqe-1.2.dist-info/RECORD,,
```

