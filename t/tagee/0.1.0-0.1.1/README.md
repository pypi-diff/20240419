# Comparing `tmp/tagee-0.1.0.tar.gz` & `tmp/tagee-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tagee-0.1.0.tar", last modified: Tue Mar  1 02:08:07 2022, max compression
+gzip compressed data, was "tagee-0.1.1.tar", last modified: Thu Apr 18 22:03:22 2024, max compression
```

## Comparing `tagee-0.1.0.tar` & `tagee-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 ganzk     (1000) ganzk     (1000)        0 2022-03-01 02:08:07.000000 tagee-0.1.0/
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)    35184 2022-02-13 16:03:52.000000 tagee-0.1.0/LICENSE
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)       26 2022-02-28 14:32:40.000000 tagee-0.1.0/MANIFEST.in
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)    11583 2022-03-01 02:08:07.000000 tagee-0.1.0/PKG-INFO
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)     9707 2022-03-01 02:05:55.000000 tagee-0.1.0/README.md
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)    25796 2022-02-13 16:03:52.000000 tagee-0.1.0/TAGEE-functions.js
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)       38 2022-03-01 02:08:07.000000 tagee-0.1.0/setup.cfg
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)      674 2022-02-15 14:35:42.000000 tagee-0.1.0/setup.py
-drwxrwxrwx   0 ganzk     (1000) ganzk     (1000)        0 2022-03-01 02:08:07.000000 tagee-0.1.0/tagee/
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)    25631 2022-02-15 14:33:47.000000 tagee-0.1.0/tagee/TAGEE.py
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)      425 2022-02-28 14:59:19.000000 tagee-0.1.0/tagee/__init__.py
-drwxrwxrwx   0 ganzk     (1000) ganzk     (1000)        0 2022-03-01 02:08:07.000000 tagee-0.1.0/tagee.egg-info/
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)    11583 2022-03-01 02:08:06.000000 tagee-0.1.0/tagee.egg-info/PKG-INFO
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)      234 2022-03-01 02:08:06.000000 tagee-0.1.0/tagee.egg-info/SOURCES.txt
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)        1 2022-03-01 02:08:06.000000 tagee-0.1.0/tagee.egg-info/dependency_links.txt
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)       16 2022-03-01 02:08:06.000000 tagee-0.1.0/tagee.egg-info/requires.txt
--rwxrwxrwx   0 ganzk     (1000) ganzk     (1000)        6 2022-03-01 02:08:06.000000 tagee-0.1.0/tagee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-18 22:03:22.164743 tagee-0.1.1/
+-rw-rw-rw-   0        0        0    35184 2024-04-18 22:01:20.000000 tagee-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-04-18 22:01:20.000000 tagee-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    10120 2024-04-18 22:03:22.163236 tagee-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9801 2024-04-18 22:01:20.000000 tagee-0.1.1/README.md
+-rw-rw-rw-   0        0        0    25796 2024-04-18 22:01:20.000000 tagee-0.1.1/TAGEE-functions.js
+-rw-rw-rw-   0        0        0       42 2024-04-18 22:03:22.165029 tagee-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      697 2024-04-18 22:03:15.000000 tagee-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:03:22.140731 tagee-0.1.1/tagee/
+-rw-rw-rw-   0        0        0    26248 2024-04-18 22:01:20.000000 tagee-0.1.1/tagee/TAGEE.py
+-rw-rw-rw-   0        0        0      436 2024-04-18 22:01:20.000000 tagee-0.1.1/tagee/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-18 22:03:22.163236 tagee-0.1.1/tagee.egg-info/
+-rw-rw-rw-   0        0        0    10120 2024-04-18 22:03:21.000000 tagee-0.1.1/tagee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-18 22:03:22.000000 tagee-0.1.1/tagee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-18 22:03:21.000000 tagee-0.1.1/tagee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-18 22:03:21.000000 tagee-0.1.1/tagee.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-18 22:03:21.000000 tagee-0.1.1/tagee.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tagee-0.1.0/LICENSE` & `tagee-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tagee-0.1.0/README.md` & `tagee-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+[![PyPI version](https://badge.fury.io/py/tagee.svg)](https://badge.fury.io/py/tagee)
+
 Google Earth Engine (GEE) is a high-performance cloud-based platform for processing geospatial data.
 
 There is a myriad of processing toolboxes in GEE, but this repository/package aims to contribute to the GEE community for making terrain analysis seamlessly. 
 
 # Installation
 Terrain Analysis in Google Earth Engine (TAGEE) is a repository that contains the GEE Javascript code and a Python API implementation with reproducible examples for both.
 
 You can use TAGEE in the Earth Engine code editor with a `require` statement.
 ```javascript
-var TAGEE = require('users/joselucassafanelli/TAGEE:TAGEE-functions');
+var TAGEE = require('users/zecojls/TAGEE:TAGEE-functions');
 ```
 Or install the Python package from pip:
 ```
 pip install tagee
 ```
 
 Additional examples information are below.
@@ -46,23 +48,23 @@
 ## Important note!
 
 As TAGEE uses spheroidal geometries and elevation nodes from a 3x3 moving window to calculate partial derivatives and hence terrain attributes, the visualization of the outputs is affected by the scale, which require the adjustment of the histogram for proper visualization. This happens because GEE produces different pyramids from your data (from the local up to the global scale) and consequently the pixel size changes dynamically, affecting the range of the estimated attribute values. Until you specify your final resolution, say 30m/pixel, the pyramids will dynamically affect the visualization of an output for different visualizaiton scales. You can determine your final resolution by exporting the results to assets and importing back further processing or map composition.
 
 
 # Minimal reproducible example
 
-[OPEN THE EXAMPLE DIRECTLY IN THE GEE CODE EDITOR](https://code.earthengine.google.com/2b1d977d8cb1c96dbf7c6a4d1064ea37).
+[OPEN THE EXAMPLE DIRECTLY IN THE GEE CODE EDITOR](https://code.earthengine.google.com/aa4e35435ceb259e86fe64eedd9cf53b).
 
 NOTE: Any Earth Engine user with the above link can use it to view and run the example code. However, you need to login.
 
 ## Javascript
 ```javascript
 // Importing module
 
-var TAGEE = require('users/joselucassafanelli/TAGEE:TAGEE-functions');
+var TAGEE = require('users/zecojls/TAGEE:TAGEE-functions');
 
 // World bounding box
 
 var bbox = ee.Geometry.Rectangle({coords: [-180, -60, 180, 60], geodesic: false});
 
 // Water mask
 
@@ -94,15 +96,15 @@
 Map.setCenter(0,0,2);
 ```
 ## Example description
 
 In the Javascript code editor [https://code.earthengine.google.com/](https://code.earthengine.google.com/), it is necessary to import the module **TAGEE-functions**.
 
 ```javascript
-var TAGEE = require('users/joselucassafanelli/TAGEE:TAGEE-functions');
+var TAGEE = require('users/zecojls/TAGEE:TAGEE-functions');
 ```
 
 Then, you need to define the bounding box (study region limits) and import the Digital Elevation Model for terrain analysis (e.g. SRTM 30 m).
 
 ```javascript
 // World bounding box
 
@@ -130,15 +132,17 @@
 Finally, you can run the TAGEE module for calculating the terrain attributes.
 
 ```javascript
 // Terrain analysis
 
 var DEMAttributes = TAGEE.terrainAnalysis(TAGEE, demSRTM, bbox).updateMask(waterMask);
 print(DEMAttributes.bandNames(), 'Parameters of Terrain');
-
+```
+Console output (don't copy):
+```
 List (13 elements){
 0: Elevation
 1: Slope
 2: Aspect
 3: Hillshade
 4: Northness
 5: Eastness
```

### Comparing `tagee-0.1.0/TAGEE-functions.js` & `tagee-0.1.1/TAGEE-functions.js`

 * *Files identical despite different names*

### Comparing `tagee-0.1.0/tagee/TAGEE.py` & `tagee-0.1.1/tagee/TAGEE.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,617 +1,617 @@
-import ee
-import math
-
-# Functions for calculating parameters
-
-def calculateParameters(dem, bbox):
-
-  # Defining kernels to retrieve 3x3 window elevations
-
-  # Weights for a 3x3 kernel
-  w00 = [0, 0, 0]
-  w11 = [1, 0, 0]
-  w12 = [0, 1, 0]
-  w13 = [0, 0, 1]
-
-  # Neighborhood indices
-  n1 = [w11, w00, w00]
-  n2 = [w12, w00, w00]
-  n3 = [w13, w00, w00]
-  n4 = [w00, w11, w00]
-  n5 = [w00, w12, w00]
-  n6 = [w00, w13, w00]
-  n7 = [w00, w00, w11]
-  n8 = [w00, w00, w12]
-  n9 = [w00, w00, w13]
-
-  # Kernel for each neighborhood index
-  kerneln1 = ee.Kernel.fixed(3, 3, n1, 1, 1, False)
-  kerneln2 = ee.Kernel.fixed(3, 3, n2, 1, 1, False)
-  kerneln3 = ee.Kernel.fixed(3, 3, n3, 1, 1, False)
-  kerneln4 = ee.Kernel.fixed(3, 3, n4, 1, 1, False)
-  kerneln5 = ee.Kernel.fixed(3, 3, n5, 1, 1, False)
-  kerneln6 = ee.Kernel.fixed(3, 3, n6, 1, 1, False)
-  kerneln7 = ee.Kernel.fixed(3, 3, n7, 1, 1, False)
-  kerneln8 = ee.Kernel.fixed(3, 3, n8, 1, 1, False)
-  kerneln9 = ee.Kernel.fixed(3, 3, n9, 1, 1, False)
-
-  # Function to compute single neighborhood values
-  def addNParameters(dem):
-    N1 = dem.convolve(kerneln1).rename('N1')
-    N2 = dem.convolve(kerneln2).rename('N2')
-    N3 = dem.convolve(kerneln3).rename('N3')
-    N4 = dem.convolve(kerneln4).rename('N4')
-    N5 = dem.convolve(kerneln5).rename('N5')
-    N6 = dem.convolve(kerneln6).rename('N6')
-    N7 = dem.convolve(kerneln7).rename('N7')
-    N8 = dem.convolve(kerneln8).rename('N8')
-    N9 = dem.convolve(kerneln9).rename('N9')
-    return dem.addBands([N1,N2,N3,N4,N5,N6,N7,N8,N9])
-
-  # Elevation values for each neighborhood
-  demZPar = addNParameters(dem)
-  demZParameters = demZPar.rename(['Elevation','Z1','Z2','Z3','Z4','Z5','Z6','Z7','Z8','Z9'])
-  #print(demZParameters, 'DEM with Z parameters')
-
-  # Defining positions
-  demPositions = dem.addBands(ee.Image.pixelLonLat())
-
-  # Longitude
-  long = demPositions.select('longitude')
-  longNPar = addNParameters(long)
-  longNParameters = longNPar.rename(['longitude','longN1','longN2','longN3','longN4','longN5','longN6','longN7','longN8','longN9'])
-  #print(longNParameters, 'Longitude with neighborhood parameters')
-
-  # Latitude
-  lat = demPositions.select('latitude')
-  latNPar = addNParameters(lat)
-  latNParameters = latNPar.rename(['latitude','latN1','latN2','latN3','latN4','latN5','latN6','latN7','latN8','latN9'])
-  #print(latNParameters, 'Latitude with neighborhood parameters')
-
-  # Function of haversine formula to retrieve distances between two neighborhood points on a spheroidal grid
-  def haversineFunction(demLat, demLong, latNeigh1, latNeigh2, longNeigh1, longNeigh2):
-    phi1 = demLat.select(ee.String(latNeigh1)).divide(180).multiply(math.pi) # to Radians
-    phi2 = demLat.select(ee.String(latNeigh2)).divide(180).multiply(math.pi) # to Radians
-    lambda1 = demLong.select(ee.String(longNeigh1)).divide(180).multiply(math.pi) # to Radians
-    lambda2 = demLong.select(ee.String(longNeigh2)).divide(180).multiply(math.pi) # to Radians
-    
-    deltaphi = phi2.subtract(phi1) # (phi2 - phi1)
-    deltalambda = lambda2.subtract(lambda1) # (lambda2 - lambda1)
-    p1 = deltaphi.divide(2).sin().multiply(deltaphi.divide(2).sin()) # sin(deltaphi/2) * sin(deltaphi/2)
-    p2 = phi1.cos().multiply(phi2.cos()) # cos(phi1) * cos(phi2)
-    p3 = deltalambda.divide(2).sin().multiply(deltalambda.divide(2).sin()) # sin(deltalambda/2) * sin(deltalambda/2)
-    j = p2.multiply(p3).add(p1) # j = p1 + p2 * p3
-    p4 = ee.Image(ee.Number(1)).clip(bbox) # p4 = image with constant 1
-    p5 = ee.Image(ee.Number(2)).clip(bbox) # p5 = image with constant 2
-    p6 = p4.subtract(j).sqrt() # sqrt(1-j)
-    p7 = j.sqrt() # sqrt(a)
-    p8 = p6.atan2(p7) # atan2(p6,p7)
-    k = p5.multiply(p8) # k = 2 * p8
-    R = ee.Image(ee.Number(6371000)).clip(bbox) # approximate radius of Earth
-    l = R.multiply(k) # l = R * k which is the distance between two points
-    
-    return l
-
-  # Distance values
-  lenghtOfE = haversineFunction(latNParameters, longNParameters, 'latN1', 'latN4', 'longN1', 'longN4').rename('e')
-  lenghtOfD = haversineFunction(latNParameters, longNParameters, 'latN4', 'latN7', 'longN4', 'longN7').rename('d')
-  lenghtOfC = haversineFunction(latNParameters, longNParameters, 'latN1', 'latN2', 'longN1', 'longN2').rename('c')
-  lenghtOfB = haversineFunction(latNParameters, longNParameters, 'latN4', 'latN5', 'longN4', 'longN5').rename('b')
-  lenghtOfA = haversineFunction(latNParameters, longNParameters, 'latN7', 'latN8', 'longN7', 'longN8').rename('a')
-
-  # Merging all the parameters in a single image
-  demCalculations = (demZParameters.addBands(lenghtOfA)
-                                      .addBands(lenghtOfB)
-                                      .addBands(lenghtOfC)
-                                      .addBands(lenghtOfD)
-                                      .addBands(lenghtOfE))
-  return demCalculations
-
-# Functions for calculating terrain derivatives  //
-
-def calculateDerivatives(parameters, bbox):
-
-  # Functions for Derivatives and Terrain Attributes
-
-  def addPDerivative(parameters):
-    a = parameters.select('a')
-    b = parameters.select('b')
-    c = parameters.select('c')
-    d = parameters.select('d')
-    e = parameters.select('e')
-    Z1 = parameters.select('Z1')
-    Z3 = parameters.select('Z3')
-    Z4 = parameters.select('Z4')
-    Z6 = parameters.select('Z6')
-    Z7 = parameters.select('Z7')
-    Z9 = parameters.select('Z9')
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    
-    p1 = a.pow(2).multiply(c).multiply(d).multiply(d.add(e)).multiply(Z3.subtract(Z1))
-    p2 = b.multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2)))).multiply(Z6.subtract(Z4))
-    p3 = a.multiply(c.pow(2)).multiply(e.multiply(d.add(e))).multiply(Z9.subtract(Z7))
-    p4 = p1.add(p2).add(p3)
-    
-    p5 = constant2
-    p6 = a.pow(2).multiply(c.pow(2).multiply(d.add(e).pow(2)))
-    p7 = b.pow(2).multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2))))
-    p8 = p6.add(p7).multiply(p5)
-    
-    p = p4.divide(p8).rename('PDerivative')
-    
-    return p
-  
-
-  def addQDerivative(parameters):
-    a = parameters.select('a')
-    b = parameters.select('b')
-    c = parameters.select('c')
-    d = parameters.select('d')
-    e = parameters.select('e')
-    Z1 = parameters.select('Z1')
-    Z2 = parameters.select('Z2')
-    Z3 = parameters.select('Z3')
-    Z4 = parameters.select('Z4')
-    Z5 = parameters.select('Z5')
-    Z6 = parameters.select('Z6')
-    Z7 = parameters.select('Z7')
-    Z8 = parameters.select('Z8')
-    Z9 = parameters.select('Z9')
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    constant3 = ee.Image(ee.Number(3)).clip(bbox)
-    
-    p1 = constant1.divide(constant2.multiply(d).multiply(e).multiply(d.add(e)).multiply(a.pow(4).add(b.pow(4)).add(c.pow(4))))
-    
-    p2 = d.pow(2).multiply(a.pow(4).add(b.pow(4)).add(b.pow(2).multiply(c.pow(2))))
-    p3 = c.pow(2).multiply(e.pow(2)).multiply(a.pow(2).subtract(b.pow(2)))
-    p4 = p2.add(p3).multiply(Z1.add(Z3))
-    
-    p5 = d.pow(2).multiply(a.pow(4).add(c.pow(4)).add(b.pow(2).multiply(c.pow(2))))
-    p6 = e.pow(2).multiply(a.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
-    p7 = p5.subtract(p6).multiply(Z4.add(Z6))
-    
-    p9 = e.pow(2).multiply(b.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
-    p10 = a.pow(2).multiply(d.pow(2)).multiply(b.pow(2).subtract(c.pow(2)))
-    p11 = p9.subtract(p10).multiply(Z7.add(Z9))
-    
-    p13 = d.pow(2).multiply(b.pow(4).multiply(Z2.subtract(constant3.multiply(Z5))).add(c.pow(4).multiply(constant3.multiply(Z2).subtract(Z5))).add(a.pow(4).subtract(constant2.multiply(b.pow(2)).multiply(c.pow(2))).multiply(Z2.subtract(Z5))))
-    
-    p14 = e.pow(2).multiply(a.pow(4).multiply(Z5.subtract(constant3.multiply(Z8))).add(b.pow(4).multiply(constant3.multiply(Z5).subtract(Z8))).add(c.pow(4).subtract(constant2.multiply(a.pow(2)).multiply(b.pow(2))).multiply(Z5.subtract(Z8))))
-    
-    p15 = constant2.multiply(a.pow(2).multiply(d.pow(2)).multiply(b.pow(2).subtract(c.pow(2))).multiply(Z8).add(c.pow(2).multiply(e.pow(2)).multiply(a.pow(2).subtract(b.pow(2))).multiply(Z2)))
-    
-    q = p1.multiply(p4.subtract(p7).subtract(p11).add(p13).add(p14).subtract(p15)).rename('QDerivative')
-    
-    return q
-
-  def addRDerivative(parameters):
-    a = parameters.select('a')
-    b = parameters.select('b')
-    c = parameters.select('c')
-    Z1 = parameters.select('Z1')
-    Z2 = parameters.select('Z2')
-    Z3 = parameters.select('Z3')
-    Z4 = parameters.select('Z4')
-    Z5 = parameters.select('Z5')
-    Z6 = parameters.select('Z6')
-    Z7 = parameters.select('Z7')
-    Z8 = parameters.select('Z8')
-    Z9 = parameters.select('Z9')
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    
-    p1 = c.pow(2).multiply(Z1.add(Z3).subtract(constant2.multiply(Z2)))
-    p2 = b.pow(2).multiply(Z4.add(Z6).subtract(constant2.multiply(Z5)))
-    p3 = a.pow(2).multiply(Z7.add(Z9).subtract(constant2.multiply(Z8)))
-    p4 = a.pow(4).add(b.pow(4)).add(c.pow(4))
-    
-    r = p1.add(p2).add(p3).divide(p4).rename('RDerivative')
-    
-    return r
-
-  def addSDerivative(parameters):
-    a = parameters.select('a')
-    b = parameters.select('b')
-    c = parameters.select('c')
-    d = parameters.select('d')
-    e = parameters.select('e')
-    Z1 = parameters.select('Z1')
-    Z2 = parameters.select('Z2')
-    Z3 = parameters.select('Z3')
-    Z4 = parameters.select('Z4')
-    Z5 = parameters.select('Z5')
-    Z6 = parameters.select('Z6')
-    Z7 = parameters.select('Z7')
-    Z8 = parameters.select('Z8')
-    Z9 = parameters.select('Z9')
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    
-    p1 = c.multiply(a.pow(2).multiply(d.add(e)).add(b.pow(2).multiply(e))).multiply(Z3.subtract(Z1))
-    p2 = b.multiply(a.pow(2).multiply(d).subtract(c.pow(2).multiply(e))).multiply(Z4.subtract(Z6))
-    p3 = a.multiply(c.pow(2).multiply(d.add(e)).add(b.pow(2).multiply(d))).multiply(Z7.subtract(Z9))
-    p4 = p1.subtract(p2).add(p3)
-    
-    p5 = constant2
-    p6 = a.pow(2).multiply(c.pow(2).multiply(d.add(e).pow(2)))
-    p7 = b.pow(2).multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2))))
-    p8 = p6.add(p7).multiply(p5)
-    
-    s = p4.divide(p8).rename('SDerivative')
-    
-    return s
-
-  def addTDerivative(parameters):
-    a = parameters.select('a')
-    b = parameters.select('b')
-    c = parameters.select('c')
-    d = parameters.select('d')
-    e = parameters.select('e')
-    Z1 = parameters.select('Z1')
-    Z2 = parameters.select('Z2')
-    Z3 = parameters.select('Z3')
-    Z4 = parameters.select('Z4')
-    Z5 = parameters.select('Z5')
-    Z6 = parameters.select('Z6')
-    Z7 = parameters.select('Z7')
-    Z8 = parameters.select('Z8')
-    Z9 = parameters.select('Z9')
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    constant3 = ee.Image(ee.Number(3)).clip(bbox)
-    
-    p1 = constant2.divide(constant3.multiply(d).multiply(e).multiply(d.add(e)).multiply(a.pow(4).add(b.pow(4)).add(c.pow(4))))
-    
-    p2 = d.multiply(a.pow(4).add(b.pow(4)).add(b.pow(2).multiply(c.pow(2))))
-    p3 = c.pow(2).multiply(e).multiply(a.pow(2).subtract(b.pow(2)))
-    p4 = p2.subtract(p3).multiply(Z1.add(Z3))
-    
-    p5 = d.multiply(a.pow(4).add(c.pow(4)).add(b.pow(2).multiply(c.pow(2))))
-    p6 = e.multiply(a.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
-    p7 = p5.add(p6).multiply(Z4.add(Z6))
-    
-    p9 = e.multiply(b.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
-    p10 = a.pow(2).multiply(d).multiply(b.pow(2).subtract(c.pow(2)))
-    p11 = p9.add(p10).multiply(Z7.add(Z9))
-    
-    p13 = d.multiply(b.pow(4).multiply(Z2.subtract(constant3.multiply(Z5))).add(c.pow(4).multiply(constant3.multiply(Z2).subtract(Z5))).add(a.pow(4).subtract(constant2.multiply(b.pow(2)).multiply(c.pow(2))).multiply(Z2.subtract(Z5))))
-    
-    p14 = e.multiply(a.pow(4).multiply(constant3.multiply(Z8).subtract(Z5)).add(b.pow(4).multiply(Z8.subtract(constant3.multiply(Z5)))).add(c.pow(4).subtract(constant2.multiply(a.pow(2)).multiply(b.pow(2))).multiply(Z8.subtract(Z5))))
-    
-    p15 = constant2.multiply(a.pow(2).multiply(d).multiply(b.pow(2).subtract(c.pow(2))).multiply(Z8).subtract(c.pow(2).multiply(e).multiply(a.pow(2).subtract(b.pow(2))).multiply(Z2)))
-    
-    t = p1.multiply(p4.subtract(p7).add(p11).add(p13).add(p14).subtract(p15)).rename('TDerivative')
-    
-    return t
-
-  def signPFunction(pDerivative):
-    signP = pDerivative.expression("(b('PDerivative') > 0) ? 1" + ": (b('PDerivative') == 0) ? 0" + ": -1").clip(bbox).rename("signP")
-    
-    return signP
-
-  def signQFunction(qDerivative):
-    signQ = qDerivative.expression("(b('QDerivative') > 0) ? 1" + ": (b('QDerivative') == 0) ? 0" + ": -1").clip(bbox).rename("signQ")
-    
-    return signQ
-
-  # Calculating the derivatives
-
-  pDerivative = addPDerivative(parameters)
-  qDerivative = addQDerivative(parameters)
-  rDerivative = addRDerivative(parameters)
-  sDerivative = addSDerivative(parameters)
-  tDerivative = addTDerivative(parameters)
-  signP = signPFunction(pDerivative)
-  signQ = signQFunction(qDerivative)
-
-  demWithDerivatives = (parameters.addBands(pDerivative)
-                                    .addBands(qDerivative)
-                                    .addBands(rDerivative)
-                                    .addBands(sDerivative)
-                                    .addBands(tDerivative)
-                                    .addBands(signP)
-                                    .addBands(signQ))
-
-  return demWithDerivatives
-
-# Functions for calculating terrain attributes
-
-def calculateAttributes(derivatives, bbox):
-
-  def slopeFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    
-    p2 = p.pow(2).rename('A')
-    q2 = q.pow(2).rename('A')
-    p2q2 = ee.ImageCollection([p2,q2])
-    sumP2q2 = p2q2.sum()
-    sqrtSumP2q2 = sumP2q2.sqrt()
-    slope = sqrtSumP2q2.atan().multiply(180).divide(math.pi).rename('Slope')
-    
-    return slope
-
-  def aspectFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    signP = derivatives.select('signP')
-    signQ = derivatives.select('signQ')
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
-    constant90 = ee.Image(ee.Number(90)).clip(bbox)
-    constant180 = ee.Image(ee.Number(180)).clip(bbox)
-    
-    p1 = constantNeg1.multiply(constant90).multiply(constant1.subtract(signQ)).multiply(constant1.subtract(signP.abs()))
-    p2 = constant180.multiply(constant1.add(signP))
-    p3 = constant180.divide(math.pi).multiply(signP)
-    p4 = constantNeg1.multiply(q).divide(p.pow(2).add(q.pow(2)).sqrt()).acos()
-    A = p1.add(p2).subtract(p3.multiply(p4)).rename('Aspect')
-    
-    return A
-
-  def hillshadeFunction(aspect):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    theta = ee.Image(ee.Number(45)).clip(bbox) # Azimuth
-    psi = ee.Image(ee.Number(315)).clip(bbox) # Elevation angle
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    
-    p1 = constant1.subtract(p.multiply(theta.sin()).multiply(constant1.divide(psi))).subtract(q.multiply(theta.cos()).multiply(constant1.divide(psi)))
-    p2 = constant1.add(p.pow(2)).add(q.pow(2)).sqrt().multiply(constant1.add(theta.sin().multiply(constant1.divide(psi)).pow(2)).add(theta.cos().multiply(constant1.divide(psi)).pow(2)).sqrt())
-    AH = p1.divide(p2).rename('Hillshade')
-    
-    return AH
-
-
-  def northernnessFunction(aspect):
-    A = aspect.select('Aspect')
-    
-    AN = A.multiply(math.pi).divide(180).cos().rename('Northness')
-    
-    return AN
-
-  def easternnessFunction(aspect):
-    A = aspect.select('Aspect')
-    
-    AE = A.multiply(math.pi).divide(180).sin().rename('Eastness')
-    
-    return AE
-
-  def horizontalCurvatureFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    r = derivatives.select('RDerivative')
-    s = derivatives.select('SDerivative')
-    t = derivatives.select('TDerivative')
-    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-    
-    p1 = q.pow(2).multiply(r).subtract(constant2.multiply(p).multiply(q).multiply(s)).add(p.pow(2).multiply(t))
-    p2 = p.pow(2).add(q.pow(2)).multiply(constant1.add(p.pow(2)).add(q.pow(2)).sqrt())
-    kh = constantNeg1.multiply(p1.divide(p2)).rename('HorizontalCurvature')
-    
-    return kh
-
-  def verticalCurvatureFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    r = derivatives.select('RDerivative')
-    s = derivatives.select('SDerivative')
-    t = derivatives.select('TDerivative')
-    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-
-    p2 = p.pow(2).multiply(r).add(constant2.multiply(p).multiply(q).multiply(s)).add(q.pow(2).multiply(t))
-    p3 = p.pow(2).add(q.pow(2)).multiply(constant1.add(p.pow(2)).add(q.pow(2)).pow(3).sqrt())
-    kv = constantNeg1.multiply(p2.divide(p3)).rename('VerticalCurvature')
-    
-    return kv
-
-  def meanCurvatureFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    r = derivatives.select('RDerivative')
-    s = derivatives.select('SDerivative')
-    t = derivatives.select('TDerivative')
-    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    constant2 = ee.Image(ee.Number(2)).clip(bbox)
-
-    p2 = constant1.add(q.pow(2)).multiply(r).subtract(constant2.multiply(p).multiply(q).multiply(s)).add(constant1.add(p.pow(2)).multiply(t))
-    p3 = constant2.multiply(constant1.add(p.pow(2)).add(q.pow(2)).pow(3).sqrt())
-    km = constantNeg1.multiply(p2.divide(p3)).rename('MeanCurvature')
-    
-    return km
-
-  def gaussianCurvatureFunction(derivatives):
-    p = derivatives.select('PDerivative')
-    q = derivatives.select('QDerivative')
-    r = derivatives.select('RDerivative')
-    s = derivatives.select('SDerivative')
-    t = derivatives.select('TDerivative')
-    constant1 = ee.Image(ee.Number(1)).clip(bbox)
-    
-    p1 = r.multiply(t).subtract(s.pow(2))
-    p2 = constant1.add(p.pow(2)).add(p.pow(2)).pow(2)
-    kg = p1.divide(p2).rename('GaussianCurvature')
-    
-    return kg
-
-  def minimalCurvatureFunction(gaussian, mean):
-    K = gaussian.select('GaussianCurvature')
-    H = mean.select('MeanCurvature')
-    kmin = H.subtract(H.pow(2).subtract(K).sqrt()).rename('MinimalCurvature')
-    
-    return kmin
-
-  def maximalCurvatureFunction(gaussian, mean):
-    K = gaussian.select('GaussianCurvature')
-    H = mean.select('MeanCurvature')
-    kmax = H.add(H.pow(2).subtract(K).sqrt()).rename('MaximalCurvature')
-    return kmax
-
-  def shapeIndexFunction(gaussian, mean):
-    K = gaussian.select('GaussianCurvature').rename('K')
-    H = mean.select('MeanCurvature').rename('H')
-    constant2 = ee.Image(ee.Number(2))
-    
-    index = constant2.divide(math.pi).multiply(H.divide(H.pow(2).subtract(K).sqrt())).rename('ShapeIndex')
-    
-    return index
-
-  # Calculating the Attributes
-
-  slope = slopeFunction(derivatives)
-  aspect = aspectFunction(derivatives)
-  hillshade = hillshadeFunction(derivatives)
-  northernness = northernnessFunction(aspect)
-  easternness = easternnessFunction(aspect)
-  horizontalCurvature = horizontalCurvatureFunction(derivatives)
-  verticalCurvature = verticalCurvatureFunction(derivatives)
-  meanCurvature = meanCurvatureFunction(derivatives)
-  gaussianCurvature = gaussianCurvatureFunction(derivatives)
-  minimalCurvature = minimalCurvatureFunction(gaussianCurvature, meanCurvature)
-  maximalCurvature = maximalCurvatureFunction(gaussianCurvature, meanCurvature)
-  shapeIndex = shapeIndexFunction(gaussianCurvature, meanCurvature)
-
-  demWithAttributes = (derivatives.addBands(slope)
-                                    .addBands(aspect)
-                                    .addBands(hillshade)
-                                    .addBands(northernness)
-                                    .addBands(easternness)
-                                    .addBands(horizontalCurvature)
-                                    .addBands(verticalCurvature)
-                                    .addBands(meanCurvature)
-                                    .addBands(gaussianCurvature)
-                                    .addBands(minimalCurvature)
-                                    .addBands(maximalCurvature)
-                                    .addBands(shapeIndex))
-
-  return (demWithAttributes.select('Elevation', 'Slope', 'Aspect', 'Hillshade', 'Northness', 'Eastness',
-                                  'HorizontalCurvature', 'VerticalCurvature', 'MeanCurvature',
-                                  'GaussianCurvature', 'MinimalCurvature', 'MaximalCurvature', 'ShapeIndex'))
-
-
-def terrainAnalysis(dem: ee.Image, bbox: ee.Geometry) -> ee.Image:
-  """
-  Calculate all terrain attributes for a given DEM and region.
-
-    Parameters:
-      dem (ee.Image): 
-        An image representing elevation values.
-      bbox (ee.Geometry): 
-        A geometry over which terrain attributes 
-        will be calculated.
-
-    Returns:
-      attributes (ee.Image): 
-        An image with calculated terrain attributes
-        with the following bands: Elevation, Slope, Aspect, Hillshade,
-        Northness, Eastness, HorizontalCurvature, VerticalCurvature,
-        MeanCurvature, GaussianCurvature, MinimalCurvature, MaximalCurvature
-  """
-  parameters = calculateParameters(dem, bbox)
-  derivatives = calculateDerivatives(parameters, bbox)
-  attributes = calculateAttributes(derivatives, bbox)
-  return(attributes)
-
-# Additional features
-
-def makeVisualization(result: ee.Image, bandName: str, 
-                      zoomLevel: str, bbox: ee.Geometry, palette: str) -> ee.Image:
-  """
-  Generate a visualization for a given band at a particular zoom level.
-  This function will dynamically determine the appropriate color scale
-  to display the image from a choice of palettes.
-
-  Parameters:
-    result (ee.Image): 
-      Image to be visualized.
-    bandName (str): 
-      Band within result to be visualized.
-    zoomLevel (str): 
-      Desired zoom level. Must be of form "levelX",
-      where X is from 0-15, inclusive.
-    bbox (ee.Geometry):
-      Geometry for which the color scale should be calculated. The 5th and 95th
-      percentile of result[bandName] are calculated in this region.
-    palette (str):
-      Palette to use for the visualization. Must be on of: "rainbow", "inferno",
-      "cubehelix", "red2green", "green2red", "elevation", "aspect".
-
-  Returns:
-    visualization (ee.Image):
-      An image with red, green, and blue bands set according to the
-      visualization.
-
-  """
-  
-  levelsDic = ee.Dictionary({
-        'level0': {'zoom': 0, 'scale': 157000},
-        'level1': {'zoom': 1, 'scale': 78000},
-        'level2': {'zoom': 2, 'scale': 39000},
-        'level3': {'zoom': 3, 'scale': 20000},
-        'level4': {'zoom': 4, 'scale': 10000},
-        'level5': {'zoom': 5, 'scale': 5000},
-        'level6': {'zoom': 6, 'scale': 2000},
-        'level7': {'zoom': 7, 'scale': 1000},
-        'level8': {'zoom': 8, 'scale': 611},
-        'level9': {'zoom': 9, 'scale': 306},
-        'level10': {'zoom': 10, 'scale': 153},
-        'level11': {'zoom': 11, 'scale': 76},
-        'level12': {'zoom': 12, 'scale': 38},
-        'level13': {'zoom': 13, 'scale': 19},
-        'level14': {'zoom': 14, 'scale': 10},
-        'level15': {'zoom': 15, 'scale': 5},
-  })
-
-  levelSelected = ee.Dictionary(levelsDic.get(zoomLevel))
-
-  imageSelected = result.select(bandName).rename('selection')
-
-  minMaxLegend = imageSelected.reduceRegion(
-          reducer=ee.Reducer.percentile(percentiles=[5,95], outputNames=['perc5','perc95']),
-          geometry=bbox,
-          scale=levelSelected.get('scale'),
-          bestEffort=True)
-
-  palettes = ee.Dictionary({
-    'rainbow': '6e40aa, be3caf, fe4b83, ff7747, e3b62f, b0ef5a, 53f666, 1edfa2, 23acd8, 4c6fdc',
-    'inferno': '000004, 160b39, 420a68, 6a176e, 932667, ba3655, dd513a, f3761b, fca50a, f6d746',
-    'cubehelix': '163d4e, 1f6642, 53792f, a07949, d07e93, d09cd9, c1caf3',
-    'red2green': 'a50026, d3322b, f16d43, fcab63, fedc8c, f9f7ae, d7ee8e, a4d86f, 64bc61, 23964f',
-    'green2red': '23964f, 64bc61, a4d86f, d7ee8e, f9f7ae, fedc8c, fcab63, f16d43, d3322b, a50026',
-    'elevation': 'b0f3be, e0fbb2, b8de76, 27a52a, 34883c, 9ca429, f8b004, c04a02, c04a02, 870800, 741805, 6c2a0a, 7d4a2b, 9c8170, b5b5b5, dad8da',
-    'aspect': 'red, green, blue, yellow, red',    'hillshade': 'black, white'
-  })
-  
-  visualization = imageSelected.visualize({
-    min: minMaxLegend.get('selection_perc5'),
-    max: minMaxLegend.get('selection_perc95'),
-    palette: palettes.get(palette)
-  })
-  
-  return visualization
-
-def logTransformation(result: ee.Image, bandName: str) -> ee.Image:
-  """
-  Apply a log10 transformation to an image.
-
-  Parameters:
-    result (ee.Image):
-      Image to be transformed.
-    bandName (str):
-      Band in image to be transformed.
-  
-  Returns:
-    logValue (ee.Image):
-      Log-transformed image.
-  """
-  selection = result.select(bandName).rename('selection')
-  sign = selection.expression("(b('selection') > 0) ? 1" + ": (b('selection') == 0) ? 0" + ": -1").rename("sign")
-  constant1 = ee.Image(ee.Number(1))
-  constant10 = ee.Image(ee.Number(10))
-  logValues = selection.abs().multiply(constant10.pow(4)).add(1).log10().multiply(sign).rename(bandName)
-  
-  return logValues
+import ee
+import math
+
+# Functions for calculating parameters
+
+def calculateParameters(dem, bbox):
+
+  # Defining kernels to retrieve 3x3 window elevations
+
+  # Weights for a 3x3 kernel
+  w00 = [0, 0, 0]
+  w11 = [1, 0, 0]
+  w12 = [0, 1, 0]
+  w13 = [0, 0, 1]
+
+  # Neighborhood indices
+  n1 = [w11, w00, w00]
+  n2 = [w12, w00, w00]
+  n3 = [w13, w00, w00]
+  n4 = [w00, w11, w00]
+  n5 = [w00, w12, w00]
+  n6 = [w00, w13, w00]
+  n7 = [w00, w00, w11]
+  n8 = [w00, w00, w12]
+  n9 = [w00, w00, w13]
+
+  # Kernel for each neighborhood index
+  kerneln1 = ee.Kernel.fixed(3, 3, n1, 1, 1, False)
+  kerneln2 = ee.Kernel.fixed(3, 3, n2, 1, 1, False)
+  kerneln3 = ee.Kernel.fixed(3, 3, n3, 1, 1, False)
+  kerneln4 = ee.Kernel.fixed(3, 3, n4, 1, 1, False)
+  kerneln5 = ee.Kernel.fixed(3, 3, n5, 1, 1, False)
+  kerneln6 = ee.Kernel.fixed(3, 3, n6, 1, 1, False)
+  kerneln7 = ee.Kernel.fixed(3, 3, n7, 1, 1, False)
+  kerneln8 = ee.Kernel.fixed(3, 3, n8, 1, 1, False)
+  kerneln9 = ee.Kernel.fixed(3, 3, n9, 1, 1, False)
+
+  # Function to compute single neighborhood values
+  def addNParameters(dem):
+    N1 = dem.convolve(kerneln1).rename('N1')
+    N2 = dem.convolve(kerneln2).rename('N2')
+    N3 = dem.convolve(kerneln3).rename('N3')
+    N4 = dem.convolve(kerneln4).rename('N4')
+    N5 = dem.convolve(kerneln5).rename('N5')
+    N6 = dem.convolve(kerneln6).rename('N6')
+    N7 = dem.convolve(kerneln7).rename('N7')
+    N8 = dem.convolve(kerneln8).rename('N8')
+    N9 = dem.convolve(kerneln9).rename('N9')
+    return dem.addBands([N1,N2,N3,N4,N5,N6,N7,N8,N9])
+
+  # Elevation values for each neighborhood
+  demZPar = addNParameters(dem)
+  demZParameters = demZPar.rename(['Elevation','Z1','Z2','Z3','Z4','Z5','Z6','Z7','Z8','Z9'])
+  #print(demZParameters, 'DEM with Z parameters')
+
+  # Defining positions
+  demPositions = dem.addBands(ee.Image.pixelLonLat())
+
+  # Longitude
+  long = demPositions.select('longitude')
+  longNPar = addNParameters(long)
+  longNParameters = longNPar.rename(['longitude','longN1','longN2','longN3','longN4','longN5','longN6','longN7','longN8','longN9'])
+  #print(longNParameters, 'Longitude with neighborhood parameters')
+
+  # Latitude
+  lat = demPositions.select('latitude')
+  latNPar = addNParameters(lat)
+  latNParameters = latNPar.rename(['latitude','latN1','latN2','latN3','latN4','latN5','latN6','latN7','latN8','latN9'])
+  #print(latNParameters, 'Latitude with neighborhood parameters')
+
+  # Function of haversine formula to retrieve distances between two neighborhood points on a spheroidal grid
+  def haversineFunction(demLat, demLong, latNeigh1, latNeigh2, longNeigh1, longNeigh2):
+    phi1 = demLat.select(ee.String(latNeigh1)).divide(180).multiply(math.pi) # to Radians
+    phi2 = demLat.select(ee.String(latNeigh2)).divide(180).multiply(math.pi) # to Radians
+    lambda1 = demLong.select(ee.String(longNeigh1)).divide(180).multiply(math.pi) # to Radians
+    lambda2 = demLong.select(ee.String(longNeigh2)).divide(180).multiply(math.pi) # to Radians
+    
+    deltaphi = phi2.subtract(phi1) # (phi2 - phi1)
+    deltalambda = lambda2.subtract(lambda1) # (lambda2 - lambda1)
+    p1 = deltaphi.divide(2).sin().multiply(deltaphi.divide(2).sin()) # sin(deltaphi/2) * sin(deltaphi/2)
+    p2 = phi1.cos().multiply(phi2.cos()) # cos(phi1) * cos(phi2)
+    p3 = deltalambda.divide(2).sin().multiply(deltalambda.divide(2).sin()) # sin(deltalambda/2) * sin(deltalambda/2)
+    j = p2.multiply(p3).add(p1) # j = p1 + p2 * p3
+    p4 = ee.Image(ee.Number(1)).clip(bbox) # p4 = image with constant 1
+    p5 = ee.Image(ee.Number(2)).clip(bbox) # p5 = image with constant 2
+    p6 = p4.subtract(j).sqrt() # sqrt(1-j)
+    p7 = j.sqrt() # sqrt(a)
+    p8 = p6.atan2(p7) # atan2(p6,p7)
+    k = p5.multiply(p8) # k = 2 * p8
+    R = ee.Image(ee.Number(6371000)).clip(bbox) # approximate radius of Earth
+    l = R.multiply(k) # l = R * k which is the distance between two points
+    
+    return l
+
+  # Distance values
+  lenghtOfE = haversineFunction(latNParameters, longNParameters, 'latN1', 'latN4', 'longN1', 'longN4').rename('e')
+  lenghtOfD = haversineFunction(latNParameters, longNParameters, 'latN4', 'latN7', 'longN4', 'longN7').rename('d')
+  lenghtOfC = haversineFunction(latNParameters, longNParameters, 'latN1', 'latN2', 'longN1', 'longN2').rename('c')
+  lenghtOfB = haversineFunction(latNParameters, longNParameters, 'latN4', 'latN5', 'longN4', 'longN5').rename('b')
+  lenghtOfA = haversineFunction(latNParameters, longNParameters, 'latN7', 'latN8', 'longN7', 'longN8').rename('a')
+
+  # Merging all the parameters in a single image
+  demCalculations = (demZParameters.addBands(lenghtOfA)
+                                      .addBands(lenghtOfB)
+                                      .addBands(lenghtOfC)
+                                      .addBands(lenghtOfD)
+                                      .addBands(lenghtOfE))
+  return demCalculations
+
+# Functions for calculating terrain derivatives  //
+
+def calculateDerivatives(parameters, bbox):
+
+  # Functions for Derivatives and Terrain Attributes
+
+  def addPDerivative(parameters):
+    a = parameters.select('a')
+    b = parameters.select('b')
+    c = parameters.select('c')
+    d = parameters.select('d')
+    e = parameters.select('e')
+    Z1 = parameters.select('Z1')
+    Z3 = parameters.select('Z3')
+    Z4 = parameters.select('Z4')
+    Z6 = parameters.select('Z6')
+    Z7 = parameters.select('Z7')
+    Z9 = parameters.select('Z9')
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    
+    p1 = a.pow(2).multiply(c).multiply(d).multiply(d.add(e)).multiply(Z3.subtract(Z1))
+    p2 = b.multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2)))).multiply(Z6.subtract(Z4))
+    p3 = a.multiply(c.pow(2)).multiply(e.multiply(d.add(e))).multiply(Z9.subtract(Z7))
+    p4 = p1.add(p2).add(p3)
+    
+    p5 = constant2
+    p6 = a.pow(2).multiply(c.pow(2).multiply(d.add(e).pow(2)))
+    p7 = b.pow(2).multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2))))
+    p8 = p6.add(p7).multiply(p5)
+    
+    p = p4.divide(p8).rename('PDerivative')
+    
+    return p
+  
+
+  def addQDerivative(parameters):
+    a = parameters.select('a')
+    b = parameters.select('b')
+    c = parameters.select('c')
+    d = parameters.select('d')
+    e = parameters.select('e')
+    Z1 = parameters.select('Z1')
+    Z2 = parameters.select('Z2')
+    Z3 = parameters.select('Z3')
+    Z4 = parameters.select('Z4')
+    Z5 = parameters.select('Z5')
+    Z6 = parameters.select('Z6')
+    Z7 = parameters.select('Z7')
+    Z8 = parameters.select('Z8')
+    Z9 = parameters.select('Z9')
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    constant3 = ee.Image(ee.Number(3)).clip(bbox)
+    
+    p1 = constant1.divide(constant2.multiply(d).multiply(e).multiply(d.add(e)).multiply(a.pow(4).add(b.pow(4)).add(c.pow(4))))
+    
+    p2 = d.pow(2).multiply(a.pow(4).add(b.pow(4)).add(b.pow(2).multiply(c.pow(2))))
+    p3 = c.pow(2).multiply(e.pow(2)).multiply(a.pow(2).subtract(b.pow(2)))
+    p4 = p2.add(p3).multiply(Z1.add(Z3))
+    
+    p5 = d.pow(2).multiply(a.pow(4).add(c.pow(4)).add(b.pow(2).multiply(c.pow(2))))
+    p6 = e.pow(2).multiply(a.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
+    p7 = p5.subtract(p6).multiply(Z4.add(Z6))
+    
+    p9 = e.pow(2).multiply(b.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
+    p10 = a.pow(2).multiply(d.pow(2)).multiply(b.pow(2).subtract(c.pow(2)))
+    p11 = p9.subtract(p10).multiply(Z7.add(Z9))
+    
+    p13 = d.pow(2).multiply(b.pow(4).multiply(Z2.subtract(constant3.multiply(Z5))).add(c.pow(4).multiply(constant3.multiply(Z2).subtract(Z5))).add(a.pow(4).subtract(constant2.multiply(b.pow(2)).multiply(c.pow(2))).multiply(Z2.subtract(Z5))))
+    
+    p14 = e.pow(2).multiply(a.pow(4).multiply(Z5.subtract(constant3.multiply(Z8))).add(b.pow(4).multiply(constant3.multiply(Z5).subtract(Z8))).add(c.pow(4).subtract(constant2.multiply(a.pow(2)).multiply(b.pow(2))).multiply(Z5.subtract(Z8))))
+    
+    p15 = constant2.multiply(a.pow(2).multiply(d.pow(2)).multiply(b.pow(2).subtract(c.pow(2))).multiply(Z8).add(c.pow(2).multiply(e.pow(2)).multiply(a.pow(2).subtract(b.pow(2))).multiply(Z2)))
+    
+    q = p1.multiply(p4.subtract(p7).subtract(p11).add(p13).add(p14).subtract(p15)).rename('QDerivative')
+    
+    return q
+
+  def addRDerivative(parameters):
+    a = parameters.select('a')
+    b = parameters.select('b')
+    c = parameters.select('c')
+    Z1 = parameters.select('Z1')
+    Z2 = parameters.select('Z2')
+    Z3 = parameters.select('Z3')
+    Z4 = parameters.select('Z4')
+    Z5 = parameters.select('Z5')
+    Z6 = parameters.select('Z6')
+    Z7 = parameters.select('Z7')
+    Z8 = parameters.select('Z8')
+    Z9 = parameters.select('Z9')
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    
+    p1 = c.pow(2).multiply(Z1.add(Z3).subtract(constant2.multiply(Z2)))
+    p2 = b.pow(2).multiply(Z4.add(Z6).subtract(constant2.multiply(Z5)))
+    p3 = a.pow(2).multiply(Z7.add(Z9).subtract(constant2.multiply(Z8)))
+    p4 = a.pow(4).add(b.pow(4)).add(c.pow(4))
+    
+    r = p1.add(p2).add(p3).divide(p4).rename('RDerivative')
+    
+    return r
+
+  def addSDerivative(parameters):
+    a = parameters.select('a')
+    b = parameters.select('b')
+    c = parameters.select('c')
+    d = parameters.select('d')
+    e = parameters.select('e')
+    Z1 = parameters.select('Z1')
+    Z2 = parameters.select('Z2')
+    Z3 = parameters.select('Z3')
+    Z4 = parameters.select('Z4')
+    Z5 = parameters.select('Z5')
+    Z6 = parameters.select('Z6')
+    Z7 = parameters.select('Z7')
+    Z8 = parameters.select('Z8')
+    Z9 = parameters.select('Z9')
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    
+    p1 = c.multiply(a.pow(2).multiply(d.add(e)).add(b.pow(2).multiply(e))).multiply(Z3.subtract(Z1))
+    p2 = b.multiply(a.pow(2).multiply(d).subtract(c.pow(2).multiply(e))).multiply(Z4.subtract(Z6))
+    p3 = a.multiply(c.pow(2).multiply(d.add(e)).add(b.pow(2).multiply(d))).multiply(Z7.subtract(Z9))
+    p4 = p1.subtract(p2).add(p3)
+    
+    p5 = constant2
+    p6 = a.pow(2).multiply(c.pow(2).multiply(d.add(e).pow(2)))
+    p7 = b.pow(2).multiply(a.pow(2).multiply(d.pow(2)).add(c.pow(2).multiply(e.pow(2))))
+    p8 = p6.add(p7).multiply(p5)
+    
+    s = p4.divide(p8).rename('SDerivative')
+    
+    return s
+
+  def addTDerivative(parameters):
+    a = parameters.select('a')
+    b = parameters.select('b')
+    c = parameters.select('c')
+    d = parameters.select('d')
+    e = parameters.select('e')
+    Z1 = parameters.select('Z1')
+    Z2 = parameters.select('Z2')
+    Z3 = parameters.select('Z3')
+    Z4 = parameters.select('Z4')
+    Z5 = parameters.select('Z5')
+    Z6 = parameters.select('Z6')
+    Z7 = parameters.select('Z7')
+    Z8 = parameters.select('Z8')
+    Z9 = parameters.select('Z9')
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    constant3 = ee.Image(ee.Number(3)).clip(bbox)
+    
+    p1 = constant2.divide(constant3.multiply(d).multiply(e).multiply(d.add(e)).multiply(a.pow(4).add(b.pow(4)).add(c.pow(4))))
+    
+    p2 = d.multiply(a.pow(4).add(b.pow(4)).add(b.pow(2).multiply(c.pow(2))))
+    p3 = c.pow(2).multiply(e).multiply(a.pow(2).subtract(b.pow(2)))
+    p4 = p2.subtract(p3).multiply(Z1.add(Z3))
+    
+    p5 = d.multiply(a.pow(4).add(c.pow(4)).add(b.pow(2).multiply(c.pow(2))))
+    p6 = e.multiply(a.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
+    p7 = p5.add(p6).multiply(Z4.add(Z6))
+    
+    p9 = e.multiply(b.pow(4).add(c.pow(4)).add(a.pow(2).multiply(b.pow(2))))
+    p10 = a.pow(2).multiply(d).multiply(b.pow(2).subtract(c.pow(2)))
+    p11 = p9.add(p10).multiply(Z7.add(Z9))
+    
+    p13 = d.multiply(b.pow(4).multiply(Z2.subtract(constant3.multiply(Z5))).add(c.pow(4).multiply(constant3.multiply(Z2).subtract(Z5))).add(a.pow(4).subtract(constant2.multiply(b.pow(2)).multiply(c.pow(2))).multiply(Z2.subtract(Z5))))
+    
+    p14 = e.multiply(a.pow(4).multiply(constant3.multiply(Z8).subtract(Z5)).add(b.pow(4).multiply(Z8.subtract(constant3.multiply(Z5)))).add(c.pow(4).subtract(constant2.multiply(a.pow(2)).multiply(b.pow(2))).multiply(Z8.subtract(Z5))))
+    
+    p15 = constant2.multiply(a.pow(2).multiply(d).multiply(b.pow(2).subtract(c.pow(2))).multiply(Z8).subtract(c.pow(2).multiply(e).multiply(a.pow(2).subtract(b.pow(2))).multiply(Z2)))
+    
+    t = p1.multiply(p4.subtract(p7).add(p11).add(p13).add(p14).subtract(p15)).rename('TDerivative')
+    
+    return t
+
+  def signPFunction(pDerivative):
+    signP = pDerivative.expression("(b('PDerivative') > 0) ? 1" + ": (b('PDerivative') == 0) ? 0" + ": -1").clip(bbox).rename("signP")
+    
+    return signP
+
+  def signQFunction(qDerivative):
+    signQ = qDerivative.expression("(b('QDerivative') > 0) ? 1" + ": (b('QDerivative') == 0) ? 0" + ": -1").clip(bbox).rename("signQ")
+    
+    return signQ
+
+  # Calculating the derivatives
+
+  pDerivative = addPDerivative(parameters)
+  qDerivative = addQDerivative(parameters)
+  rDerivative = addRDerivative(parameters)
+  sDerivative = addSDerivative(parameters)
+  tDerivative = addTDerivative(parameters)
+  signP = signPFunction(pDerivative)
+  signQ = signQFunction(qDerivative)
+
+  demWithDerivatives = (parameters.addBands(pDerivative)
+                                    .addBands(qDerivative)
+                                    .addBands(rDerivative)
+                                    .addBands(sDerivative)
+                                    .addBands(tDerivative)
+                                    .addBands(signP)
+                                    .addBands(signQ))
+
+  return demWithDerivatives
+
+# Functions for calculating terrain attributes
+
+def calculateAttributes(derivatives, bbox):
+
+  def slopeFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    
+    p2 = p.pow(2).rename('A')
+    q2 = q.pow(2).rename('A')
+    p2q2 = ee.ImageCollection([p2,q2])
+    sumP2q2 = p2q2.sum()
+    sqrtSumP2q2 = sumP2q2.sqrt()
+    slope = sqrtSumP2q2.atan().multiply(180).divide(math.pi).rename('Slope')
+    
+    return slope
+
+  def aspectFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    signP = derivatives.select('signP')
+    signQ = derivatives.select('signQ')
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
+    constant90 = ee.Image(ee.Number(90)).clip(bbox)
+    constant180 = ee.Image(ee.Number(180)).clip(bbox)
+    
+    p1 = constantNeg1.multiply(constant90).multiply(constant1.subtract(signQ)).multiply(constant1.subtract(signP.abs()))
+    p2 = constant180.multiply(constant1.add(signP))
+    p3 = constant180.divide(math.pi).multiply(signP)
+    p4 = constantNeg1.multiply(q).divide(p.pow(2).add(q.pow(2)).sqrt()).acos()
+    A = p1.add(p2).subtract(p3.multiply(p4)).rename('Aspect')
+    
+    return A
+
+  def hillshadeFunction(aspect):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    theta = ee.Image(ee.Number(45)).clip(bbox) # Azimuth
+    psi = ee.Image(ee.Number(315)).clip(bbox) # Elevation angle
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    
+    p1 = constant1.subtract(p.multiply(theta.sin()).multiply(constant1.divide(psi))).subtract(q.multiply(theta.cos()).multiply(constant1.divide(psi)))
+    p2 = constant1.add(p.pow(2)).add(q.pow(2)).sqrt().multiply(constant1.add(theta.sin().multiply(constant1.divide(psi)).pow(2)).add(theta.cos().multiply(constant1.divide(psi)).pow(2)).sqrt())
+    AH = p1.divide(p2).rename('Hillshade')
+    
+    return AH
+
+
+  def northernnessFunction(aspect):
+    A = aspect.select('Aspect')
+    
+    AN = A.multiply(math.pi).divide(180).cos().rename('Northness')
+    
+    return AN
+
+  def easternnessFunction(aspect):
+    A = aspect.select('Aspect')
+    
+    AE = A.multiply(math.pi).divide(180).sin().rename('Eastness')
+    
+    return AE
+
+  def horizontalCurvatureFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    r = derivatives.select('RDerivative')
+    s = derivatives.select('SDerivative')
+    t = derivatives.select('TDerivative')
+    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+    
+    p1 = q.pow(2).multiply(r).subtract(constant2.multiply(p).multiply(q).multiply(s)).add(p.pow(2).multiply(t))
+    p2 = p.pow(2).add(q.pow(2)).multiply(constant1.add(p.pow(2)).add(q.pow(2)).sqrt())
+    kh = constantNeg1.multiply(p1.divide(p2)).rename('HorizontalCurvature')
+    
+    return kh
+
+  def verticalCurvatureFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    r = derivatives.select('RDerivative')
+    s = derivatives.select('SDerivative')
+    t = derivatives.select('TDerivative')
+    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+
+    p2 = p.pow(2).multiply(r).add(constant2.multiply(p).multiply(q).multiply(s)).add(q.pow(2).multiply(t))
+    p3 = p.pow(2).add(q.pow(2)).multiply(constant1.add(p.pow(2)).add(q.pow(2)).pow(3).sqrt())
+    kv = constantNeg1.multiply(p2.divide(p3)).rename('VerticalCurvature')
+    
+    return kv
+
+  def meanCurvatureFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    r = derivatives.select('RDerivative')
+    s = derivatives.select('SDerivative')
+    t = derivatives.select('TDerivative')
+    constantNeg1 = ee.Image(ee.Number(-1)).clip(bbox)
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    constant2 = ee.Image(ee.Number(2)).clip(bbox)
+
+    p2 = constant1.add(q.pow(2)).multiply(r).subtract(constant2.multiply(p).multiply(q).multiply(s)).add(constant1.add(p.pow(2)).multiply(t))
+    p3 = constant2.multiply(constant1.add(p.pow(2)).add(q.pow(2)).pow(3).sqrt())
+    km = constantNeg1.multiply(p2.divide(p3)).rename('MeanCurvature')
+    
+    return km
+
+  def gaussianCurvatureFunction(derivatives):
+    p = derivatives.select('PDerivative')
+    q = derivatives.select('QDerivative')
+    r = derivatives.select('RDerivative')
+    s = derivatives.select('SDerivative')
+    t = derivatives.select('TDerivative')
+    constant1 = ee.Image(ee.Number(1)).clip(bbox)
+    
+    p1 = r.multiply(t).subtract(s.pow(2))
+    p2 = constant1.add(p.pow(2)).add(p.pow(2)).pow(2)
+    kg = p1.divide(p2).rename('GaussianCurvature')
+    
+    return kg
+
+  def minimalCurvatureFunction(gaussian, mean):
+    K = gaussian.select('GaussianCurvature')
+    H = mean.select('MeanCurvature')
+    kmin = H.subtract(H.pow(2).subtract(K).sqrt()).rename('MinimalCurvature')
+    
+    return kmin
+
+  def maximalCurvatureFunction(gaussian, mean):
+    K = gaussian.select('GaussianCurvature')
+    H = mean.select('MeanCurvature')
+    kmax = H.add(H.pow(2).subtract(K).sqrt()).rename('MaximalCurvature')
+    return kmax
+
+  def shapeIndexFunction(gaussian, mean):
+    K = gaussian.select('GaussianCurvature').rename('K')
+    H = mean.select('MeanCurvature').rename('H')
+    constant2 = ee.Image(ee.Number(2))
+    
+    index = constant2.divide(math.pi).multiply(H.divide(H.pow(2).subtract(K).sqrt())).rename('ShapeIndex')
+    
+    return index
+
+  # Calculating the Attributes
+
+  slope = slopeFunction(derivatives)
+  aspect = aspectFunction(derivatives)
+  hillshade = hillshadeFunction(derivatives)
+  northernness = northernnessFunction(aspect)
+  easternness = easternnessFunction(aspect)
+  horizontalCurvature = horizontalCurvatureFunction(derivatives)
+  verticalCurvature = verticalCurvatureFunction(derivatives)
+  meanCurvature = meanCurvatureFunction(derivatives)
+  gaussianCurvature = gaussianCurvatureFunction(derivatives)
+  minimalCurvature = minimalCurvatureFunction(gaussianCurvature, meanCurvature)
+  maximalCurvature = maximalCurvatureFunction(gaussianCurvature, meanCurvature)
+  shapeIndex = shapeIndexFunction(gaussianCurvature, meanCurvature)
+
+  demWithAttributes = (derivatives.addBands(slope)
+                                    .addBands(aspect)
+                                    .addBands(hillshade)
+                                    .addBands(northernness)
+                                    .addBands(easternness)
+                                    .addBands(horizontalCurvature)
+                                    .addBands(verticalCurvature)
+                                    .addBands(meanCurvature)
+                                    .addBands(gaussianCurvature)
+                                    .addBands(minimalCurvature)
+                                    .addBands(maximalCurvature)
+                                    .addBands(shapeIndex))
+
+  return (demWithAttributes.select('Elevation', 'Slope', 'Aspect', 'Hillshade', 'Northness', 'Eastness',
+                                  'HorizontalCurvature', 'VerticalCurvature', 'MeanCurvature',
+                                  'GaussianCurvature', 'MinimalCurvature', 'MaximalCurvature', 'ShapeIndex'))
+
+
+def terrainAnalysis(dem: ee.Image, bbox: ee.Geometry) -> ee.Image:
+  """
+  Calculate all terrain attributes for a given DEM and region.
+
+    Parameters:
+      dem (ee.Image): 
+        An image representing elevation values.
+      bbox (ee.Geometry): 
+        A geometry over which terrain attributes 
+        will be calculated.
+
+    Returns:
+      attributes (ee.Image): 
+        An image with calculated terrain attributes
+        with the following bands: Elevation, Slope, Aspect, Hillshade,
+        Northness, Eastness, HorizontalCurvature, VerticalCurvature,
+        MeanCurvature, GaussianCurvature, MinimalCurvature, MaximalCurvature
+  """
+  parameters = calculateParameters(dem, bbox)
+  derivatives = calculateDerivatives(parameters, bbox)
+  attributes = calculateAttributes(derivatives, bbox)
+  return(attributes)
+
+# Additional features
+
+def makeVisualization(result: ee.Image, bandName: str, 
+                      zoomLevel: str, bbox: ee.Geometry, palette: str) -> ee.Image:
+  """
+  Generate a visualization for a given band at a particular zoom level.
+  This function will dynamically determine the appropriate color scale
+  to display the image from a choice of palettes.
+
+  Parameters:
+    result (ee.Image): 
+      Image to be visualized.
+    bandName (str): 
+      Band within result to be visualized.
+    zoomLevel (str): 
+      Desired zoom level. Must be of form "levelX",
+      where X is from 0-15, inclusive.
+    bbox (ee.Geometry):
+      Geometry for which the color scale should be calculated. The 5th and 95th
+      percentile of result[bandName] are calculated in this region.
+    palette (str):
+      Palette to use for the visualization. Must be on of: "rainbow", "inferno",
+      "cubehelix", "red2green", "green2red", "elevation", "aspect".
+
+  Returns:
+    visualization (ee.Image):
+      An image with red, green, and blue bands set according to the
+      visualization.
+
+  """
+  
+  levelsDic = ee.Dictionary({
+        'level0': {'zoom': 0, 'scale': 157000},
+        'level1': {'zoom': 1, 'scale': 78000},
+        'level2': {'zoom': 2, 'scale': 39000},
+        'level3': {'zoom': 3, 'scale': 20000},
+        'level4': {'zoom': 4, 'scale': 10000},
+        'level5': {'zoom': 5, 'scale': 5000},
+        'level6': {'zoom': 6, 'scale': 2000},
+        'level7': {'zoom': 7, 'scale': 1000},
+        'level8': {'zoom': 8, 'scale': 611},
+        'level9': {'zoom': 9, 'scale': 306},
+        'level10': {'zoom': 10, 'scale': 153},
+        'level11': {'zoom': 11, 'scale': 76},
+        'level12': {'zoom': 12, 'scale': 38},
+        'level13': {'zoom': 13, 'scale': 19},
+        'level14': {'zoom': 14, 'scale': 10},
+        'level15': {'zoom': 15, 'scale': 5},
+  })
+
+  levelSelected = ee.Dictionary(levelsDic.get(zoomLevel))
+
+  imageSelected = result.select(bandName).rename('selection')
+
+  minMaxLegend = imageSelected.reduceRegion(
+          reducer=ee.Reducer.percentile(percentiles=[5,95], outputNames=['perc5','perc95']),
+          geometry=bbox,
+          scale=levelSelected.get('scale'),
+          bestEffort=True)
+
+  palettes = ee.Dictionary({
+    'rainbow': '6e40aa, be3caf, fe4b83, ff7747, e3b62f, b0ef5a, 53f666, 1edfa2, 23acd8, 4c6fdc',
+    'inferno': '000004, 160b39, 420a68, 6a176e, 932667, ba3655, dd513a, f3761b, fca50a, f6d746',
+    'cubehelix': '163d4e, 1f6642, 53792f, a07949, d07e93, d09cd9, c1caf3',
+    'red2green': 'a50026, d3322b, f16d43, fcab63, fedc8c, f9f7ae, d7ee8e, a4d86f, 64bc61, 23964f',
+    'green2red': '23964f, 64bc61, a4d86f, d7ee8e, f9f7ae, fedc8c, fcab63, f16d43, d3322b, a50026',
+    'elevation': 'b0f3be, e0fbb2, b8de76, 27a52a, 34883c, 9ca429, f8b004, c04a02, c04a02, 870800, 741805, 6c2a0a, 7d4a2b, 9c8170, b5b5b5, dad8da',
+    'aspect': 'red, green, blue, yellow, red',    'hillshade': 'black, white'
+  })
+  
+  visualization = imageSelected.visualize({
+    min: minMaxLegend.get('selection_perc5'),
+    max: minMaxLegend.get('selection_perc95'),
+    palette: palettes.get(palette)
+  })
+  
+  return visualization
+
+def logTransformation(result: ee.Image, bandName: str) -> ee.Image:
+  """
+  Apply a log10 transformation to an image.
+
+  Parameters:
+    result (ee.Image):
+      Image to be transformed.
+    bandName (str):
+      Band in image to be transformed.
+  
+  Returns:
+    logValue (ee.Image):
+      Log-transformed image.
+  """
+  selection = result.select(bandName).rename('selection')
+  sign = selection.expression("(b('selection') > 0) ? 1" + ": (b('selection') == 0) ? 0" + ": -1").rename("sign")
+  constant1 = ee.Image(ee.Number(1))
+  constant10 = ee.Image(ee.Number(10))
+  logValues = selection.abs().multiply(constant10.pow(4)).add(1).log10().multiply(sign).rename(bandName)
+  
+  return logValues
```

