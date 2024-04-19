# Comparing `tmp/geometool-0.1.1.tar.gz` & `tmp/geometool-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometool-0.1.1.tar", last modified: Wed Apr  3 16:49:05 2024, max compression
+gzip compressed data, was "geometool-0.1.2.tar", last modified: Fri Apr 19 00:24:24 2024, max compression
```

## Comparing `geometool-0.1.1.tar` & `geometool-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 16:49:02.000000 geometool-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 16:49:05.890499 geometool-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-03 16:49:02.000000 geometool-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/geometool/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/geometry_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-03 16:49:02.000000 geometool-0.1.1/geometool/test_geometry_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:49:05.890499 geometool-0.1.1/geometool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 16:49:05.000000 geometool-0.1.1/geometool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:49:05.890499 geometool-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 16:49:02.000000 geometool-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:24:24.881905 geometool-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-19 00:24:16.000000 geometool-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 00:24:24.881905 geometool-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-19 00:24:16.000000 geometool-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:24:24.881905 geometool-0.1.2/geometool/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 00:24:16.000000 geometool-0.1.2/geometool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 00:24:16.000000 geometool-0.1.2/geometool/geometry_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-19 00:24:16.000000 geometool-0.1.2/geometool/test_geometry_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 00:24:16.000000 geometool-0.1.2/geometool/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 00:24:24.881905 geometool-0.1.2/geometool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-19 00:24:24.000000 geometool-0.1.2/geometool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 00:24:24.000000 geometool-0.1.2/geometool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 00:24:24.000000 geometool-0.1.2/geometool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-19 00:24:24.000000 geometool-0.1.2/geometool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 00:24:24.881905 geometool-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 00:24:16.000000 geometool-0.1.2/setup.py
```

### Comparing `geometool-0.1.1/LICENSE` & `geometool-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geometool-0.1.1/PKG-INFO` & `geometool-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
-This Python package provides functions to calculate the area and perimeter of various geometric shapes.
+**New: Added the ability of defining a triangle using **kwargs** 
+
+    - Triangle(base, height) 
+
+    - Triangle(side1, side2, angle between them in degrees)
 
 
+This Python package provides functions to calculate the area and perimeter of various geometric shapes.
+
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 $ pip install geometool
 ```
 
 ## Methods
 
-The package provides the following functions (yet):
+The package provides the following functions:
 
 - `calculate_area(shape)` : Calculates the area of a given shape. Supported shapes include:
     - Circle(radius)
-    - Triangle(3 sides)
-
+    - Triangle()
+- `calculate_perimeter(shape)`: Calculates the perimeter of a given shape. Supported shapes include:
+    - Circle(radius)
+    - Triangle()
 
 ## Classes
 
 ### Shape
 Abstract base class for geometric shapes.
 
 ### Circle
 - `calc_area()` to calculate the area.
+- `calc_perimeter()` to calculate the perimeter.
 
 ### Triangle
-- `calc_area()` to calculate the area 
+- `calc_area()` to calculate the area.
+- `calc_perimeter()` to calculate the perimeter.
 - `is_rightangled()` to check if the triangle is right-angled.
 
 
 ## Usage
 
 ```bash
 import geometool as g
 
 # Declare a shape object 
 
 s1 = g.Circle(5)
 s2 = g.Triangle(6, 8, 9)
 
-# Use calculate_area() to calculate the area of the object 
-
+# Use calculate_area() and calculate_perimeter() to calculate the area and perimeter of the object
 g.calculate_area(s1)
+g.calculate_perimeter(s1)
 g.calculate_area(s2)
-
+g.calculate_perimeter(s2)
 ```
 
 
-## Authors: Idris Taha
-- Contact: dri.taha24@gmail.com
+## Authors: 
+Idris Taha
+- E-mail: dri.taha24@gmail.com
+- *@idristaha*
```

### Comparing `geometool-0.1.1/geometool.egg-info/PKG-INFO` & `geometool-0.1.2/geometool.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 Metadata-Version: 2.1
 Name: geometool
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Geometric Shape Calculator Tool
 Home-page: https://github.com/K4speeer/Geometry_Tool
 Author: Idris Taha
 Author-email: dri.taha24@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Geometool - Geometric Shape Calculation Library
 
 **```MB Task-1```**
 
-This Python package provides functions to calculate the area and perimeter of various geometric shapes.
+**New: Added the ability of defining a triangle using **kwargs** 
+
+    - Triangle(base, height) 
+
+    - Triangle(side1, side2, angle between them in degrees)
 
 
+This Python package provides functions to calculate the area and perimeter of various geometric shapes.
+
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 $ pip install geometool
 ```
 
 ## Methods
 
-The package provides the following functions (yet):
+The package provides the following functions:
 
 - `calculate_area(shape)` : Calculates the area of a given shape. Supported shapes include:
     - Circle(radius)
-    - Triangle(3 sides)
-
+    - Triangle()
+- `calculate_perimeter(shape)`: Calculates the perimeter of a given shape. Supported shapes include:
+    - Circle(radius)
+    - Triangle()
 
 ## Classes
 
 ### Shape
 Abstract base class for geometric shapes.
 
 ### Circle
 - `calc_area()` to calculate the area.
+- `calc_perimeter()` to calculate the perimeter.
 
 ### Triangle
-- `calc_area()` to calculate the area 
+- `calc_area()` to calculate the area.
+- `calc_perimeter()` to calculate the perimeter.
 - `is_rightangled()` to check if the triangle is right-angled.
 
 
 ## Usage
 
 ```bash
 import geometool as g
 
 # Declare a shape object 
 
 s1 = g.Circle(5)
 s2 = g.Triangle(6, 8, 9)
 
-# Use calculate_area() to calculate the area of the object 
-
+# Use calculate_area() and calculate_perimeter() to calculate the area and perimeter of the object
 g.calculate_area(s1)
+g.calculate_perimeter(s1)
 g.calculate_area(s2)
-
+g.calculate_perimeter(s2)
 ```
 
 
-## Authors: Idris Taha
-- Contact: dri.taha24@gmail.com
+## Authors: 
+Idris Taha
+- E-mail: dri.taha24@gmail.com
+- *@idristaha*
```

### Comparing `geometool-0.1.1/setup.py` & `geometool-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 
     
     
 setup(
     name='geometool',
-    version='0.1.1',
+    version='0.1.2',
     packages=['geometool'],
     install_requires= [],
     author='Idris Taha',
     author_email='dri.taha24@gmail.com',
     description='A Geometric Shape Calculator Tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

