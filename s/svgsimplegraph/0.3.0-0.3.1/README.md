# Comparing `tmp/svgsimplegraph-0.3.0.tar.gz` & `tmp/svgsimplegraph-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgsimplegraph-0.3.0.tar", last modified: Fri Apr 12 18:59:47 2024, max compression
+gzip compressed data, was "svgsimplegraph-0.3.1.tar", last modified: Fri Apr 19 18:34:11 2024, max compression
```

## Comparing `svgsimplegraph-0.3.0.tar` & `svgsimplegraph-0.3.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.793273 svgsimplegraph-0.3.0/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2023-05-30 04:47:02.000000 svgsimplegraph-0.3.0/LICENSE
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-12 18:59:47.792978 svgsimplegraph-0.3.0/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-02-12 21:11:46.000000 svgsimplegraph-0.3.0/README.md
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-12 18:59:47.793361 svgsimplegraph-0.3.0/setup.cfg
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      936 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/setup.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.788014 svgsimplegraph-0.3.0/svgsimplegraph/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/svgsimplegraph/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/base.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    45924 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/svgsimplegraph/categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-03-27 22:54:17.000000 svgsimplegraph-0.3.0/svgsimplegraph/ribbon.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)    10543 2024-04-08 19:58:23.000000 svgsimplegraph-0.3.0/svgsimplegraph/utils.py
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.789463 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     7149 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/PKG-INFO
--rw-r--r--   0 garrettpetersen   (501) staff       (20)      487 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/SOURCES.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/dependency_links.txt
--rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-12 18:59:47.000000 svgsimplegraph-0.3.0/svgsimplegraph.egg-info/top_level.txt
-drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-12 18:59:47.792235 svgsimplegraph-0.3.0/tests/
--rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2023-05-30 04:47:02.000000 svgsimplegraph-0.3.0/tests/__init__.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_bubble_and_arrow.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     8165 2024-04-12 18:59:30.000000 svgsimplegraph-0.3.0/tests/test_categorical.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_gist.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-02-11 22:35:12.000000 svgsimplegraph-0.3.0/tests/test_readme_examples.py
--rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2023-09-09 18:17:20.000000 svgsimplegraph-0.3.0/tests/test_ribbon.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-19 18:34:11.584167 svgsimplegraph-0.3.1/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1072 2024-01-17 17:03:33.000000 svgsimplegraph-0.3.1/LICENSE
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     8800 2024-04-19 18:34:11.583886 svgsimplegraph-0.3.1/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     6599 2024-03-11 21:11:26.000000 svgsimplegraph-0.3.1/README.md
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       38 2024-04-19 18:34:11.584216 svgsimplegraph-0.3.1/setup.cfg
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      936 2024-04-19 18:33:32.000000 svgsimplegraph-0.3.1/setup.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-19 18:34:11.581675 svgsimplegraph-0.3.1/svgsimplegraph/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      124 2024-01-17 17:03:33.000000 svgsimplegraph-0.3.1/svgsimplegraph/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10527 2024-04-19 18:25:59.000000 svgsimplegraph-0.3.1/svgsimplegraph/base.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    16487 2024-04-19 18:25:59.000000 svgsimplegraph-0.3.1/svgsimplegraph/bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    46149 2024-04-19 18:33:32.000000 svgsimplegraph-0.3.1/svgsimplegraph/categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    15007 2024-04-19 18:25:59.000000 svgsimplegraph-0.3.1/svgsimplegraph/ribbon.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)    10543 2024-04-19 18:25:59.000000 svgsimplegraph-0.3.1/svgsimplegraph/utils.py
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-19 18:34:11.582322 svgsimplegraph-0.3.1/svgsimplegraph.egg-info/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     8800 2024-04-19 18:34:11.000000 svgsimplegraph-0.3.1/svgsimplegraph.egg-info/PKG-INFO
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)      487 2024-04-19 18:34:11.000000 svgsimplegraph-0.3.1/svgsimplegraph.egg-info/SOURCES.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        1 2024-04-19 18:34:11.000000 svgsimplegraph-0.3.1/svgsimplegraph.egg-info/dependency_links.txt
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)       21 2024-04-19 18:34:11.000000 svgsimplegraph-0.3.1/svgsimplegraph.egg-info/top_level.txt
+drwxr-xr-x   0 garrettpetersen   (501) staff       (20)        0 2024-04-19 18:34:11.583516 svgsimplegraph-0.3.1/tests/
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)        0 2024-01-17 17:03:33.000000 svgsimplegraph-0.3.1/tests/__init__.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     2778 2024-01-17 17:29:02.000000 svgsimplegraph-0.3.1/tests/test_bubble_and_arrow.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     8165 2024-04-19 18:29:59.000000 svgsimplegraph-0.3.1/tests/test_categorical.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1700 2024-01-17 17:03:33.000000 svgsimplegraph-0.3.1/tests/test_gist.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     3562 2024-03-11 21:11:26.000000 svgsimplegraph-0.3.1/tests/test_readme_examples.py
+-rw-r--r--   0 garrettpetersen   (501) staff       (20)     1116 2024-01-17 17:28:43.000000 svgsimplegraph-0.3.1/tests/test_ribbon.py
```

### Comparing `svgsimplegraph-0.3.0/LICENSE` & `svgsimplegraph-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/PKG-INFO` & `svgsimplegraph-0.3.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: svgsimplegraph
-Version: 0.3.0
-Summary: Simple SVG graphing package
-Author: Garrett M. Petersen
-Author-email: garrett.m.petersen@gmail.com
-License: MIT
-Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
-Keywords: graph,svg,base64,svg simple graph
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # svgsimplegraph
 
 This is a simple little graphing package for making graphs and exporting them as raw or base64-encoded SVGs.
 
 You can also upload the SVGs to your GitHub account as Gists, so they may be embedded in any website!
 
 ## Installing svgsimplegraph
@@ -213,8 +197,8 @@
 svg_url = graph.upload_to_github_gist(GITHUB_ACCESS_TOKEN, "my_categorical_graph")
 ```
 
 The `svg_url` variable now contains a string with the url of your new SVG, ready to be embedded in any website!
 
 ## Watermarks
 
-When you initialize a graph, you can use the watermark variable to add arbitrary svg code to the graph. It is recommended to make your watermark partially transparent, as it will be placed on top of your graph.
+When you initialize a graph, you can use the watermark variable to add arbitrary svg code to the graph. It is recommended to make your watermark partially transparent, as it will be placed on top of your graph.
```

### Comparing `svgsimplegraph-0.3.0/README.md` & `svgsimplegraph-0.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,204 +1,220 @@
-# svgsimplegraph
-
-This is a simple little graphing package for making graphs and exporting them as raw or base64-encoded SVGs.
-
-You can also upload the SVGs to your GitHub account as Gists, so they may be embedded in any website!
-
-## Installing svgsimplegraph
-Install svgsimplegraph by typing
-```
-pip install svgsimplegraph
-```
-in your terminal.
-
-## Graph Types
-### Categorical Graph
-
-The categorical graph is for data that comes in distinct categories. It can generate a bar chart, a stacked bar chart, dots, or lines.
-
-Here is an example of how to make a graph:
-
-```
-from svgsimplegraph import CategoricalGraph
-
-graph = CategoricalGraph(
-        width=600,
-        height=400,
-        bar_width=30,
-        stacked=False,
-        background_color="#404040",
-        title="Categorical Graph",
-    )
-
-graph.x_labels = ["A", "B", "C", "D", "E"]
-graph.x_axis_label = "X Axis"
-graph.primary_y_axis_label = "Primary Y Axis"
-
-# Skip adding a legend_label to exclude a series from the legend
-graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1")
-graph.add_series([15, 25, 5, 44, 56], legend_label="Series 2")
-graph.add_series([5, 35, 10, 33, 40], legend_label="Series 3", series_type="line")
-graph.add_series([35, 56, 25, 5, 44], legend_label="Series 4", series_type="dot")
-
-# You can use vertical or horizontal lines to mark specific values
-graph.add_vertical_line(
-    x=2.5,
-    label="Vertical Line",
-    label_x_position="right",
-    label_y_position="top",
-    rotate_label=True,
-)
-
-# Get the SVG string in base64 format
-svg_base64 = graph.to_base64_src()
-
-# Print the SVG string in an img tag so your browser can display it
-print(f"\n<img src='{svg_base64}' />")
-
-# Alternatively, you can get the raw SVG code with render()
-raw_svg = graph.render()
-print(raw_svg)
-```
-![Example categorical graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_categorical.svg)
-
-### Ribbon Graph
-
-The ribbon graph is for comparing two numbers on the same scale and a third number on a different scale (represented through color).
-
-The three series must be added in order, with the first representing the back of the ribbon, the second representing the point, and the (optional) third representing the color.
-
-Here's an example:
-
-```
-from svgsimplegraph import RibbonGraph
-
-graph = RibbonGraph(
-    width=600,
-    height=400,
-    bar_width=30,
-    background_color="#404040",
-    title="Ribbon Graph",
-)
-
-graph.x_labels = ["A", "B", "C", "D", "E"]
-graph.x_axis_label = "X Axis"
-graph.primary_y_axis_label = "Primary Y Axis"
-
-graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1", print_values=True)
-graph.add_series([20, 30, 40, 30, 20], legend_label="Series 2", print_values=True)
-graph.add_series(
-    [-10, -20, 30, 20, 10], legend_label="Color Series", print_values=True
-)
-
-# Get the SVG string in base64 format
-svg_base64 = graph.to_base64_src()
-
-# Print the SVG string in an img tag so your browser can display it
-print(f"\n<img src='{svg_base64}' />")
-
-# Alternatively, you can get the raw SVG code with render()
-raw_svg = graph.render()
-print(raw_svg)
-```
-![Example ribbon graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_ribbon.svg)
-
-### Bubble and Arrow Graph
-The bubble and arrow graph is for displaying relationships between nodes in a network.
-
-The user adds bubbles, which are displayed in clockwise order around a larger circle. Then the user can add arrows that exit from one bubble and enter another. Arrow width is scaled to show more important connections.
-
-Here's an example:
-```
-from svgsimplegraph import BubbleAndArrowGraph
-
-graph = BubbleAndArrowGraph(
-    width=400,
-    height=400,
-    background_color="#ffffff",
-    title="Bubble and Arrow Graph",
-)
-
-# Optional str label param can be referred to later when defining arrows
-graph.add_bubble(100, None, "Bubble 0", label="big_bubble")
-
-# Otherwise bubbles must be referred to by their index number
-graph.add_bubble(50, 25, "Bubble 1")
-graph.add_bubble(25, 12.5, "Bubble 2")
-
-graph.add_arrow(
-    origin="big_bubble",
-    destination=1,
-    size=60,
-)
-graph.add_arrow(
-    origin="big_bubble",
-    destination=2,
-    size=40,
-)
-graph.add_arrow(
-    origin=1,
-    destination=2,
-    size=30,
-)
-
-# Arrows pointing to their origin will loop around
-graph.add_arrow(
-    origin=2,
-    destination=2,
-    size=20,
-)
-
-# Get the SVG string in base64 format
-svg_base64 = graph.to_base64_src()
-
-# Print the SVG string in an img tag so your browser can display it
-print(f"\n<img src='{svg_base64}' />")
-
-# Alternatively, you can get the raw SVG code with render()
-raw_svg = graph.render()
-print(raw_svg)
-```
-![Example bubble and arrow graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_bubble_and_arrow.svg)
-
-## GitHub Gist integration
-
-The `upload_to_github_gist` function allows you to render your graph and upload it to your GitHub account as a Gist.
-
-To do this, you'll need an access token. Go to your github account and navigate to settings. Then click on Developer settings > Personal access tokens > Fine-grained tokens.
-
-Click the Generate new token button in the top right of the screen. GitHub will prompt you to login. Set a token name (something like "gist-access-token") and an expiration.
-
-Scroll down to Permissions and expand the Account permissions box. Then turn on read and write access for Gists only (you should not use this token for anything else). Finally, click the gree Generate token button at the bottom of the screen.
-
-Now you should see a screen showing your token. This is the only time Github will show you this token, so save it somewhere safe.
-
-Assuming you've done all that, you can use the token to turn your graphs into gists.
-
-```
-from svgsimplegraph import CategoricalGraph
-
-GITHUB_ACCESS_TOKEN = "your_token_goes_here"
-
-# Create an instance of a graph
-graph = CategoricalGraph(
-    width=600,
-    height=400,
-    bar_width=30,
-    stacked=False,
-    background_color="#404040",
-)
-
-graph.x_labels = ["A", "B", "C", "D", "E"]
-graph.x_axis_label = "X Axis"
-graph.primary_y_axis_label = "Primary Y Axis"
-
-graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1")
-
-svg_url = graph.upload_to_github_gist(GITHUB_ACCESS_TOKEN, "my_categorical_graph")
-```
-
-The `svg_url` variable now contains a string with the url of your new SVG, ready to be embedded in any website!
-
-## Watermarks
-
-When you initialize a graph, you can use the watermark variable to add arbitrary svg code to the graph. It is recommended to make your watermark partially transparent, as it will be placed on top of your graph.
+Metadata-Version: 2.1
+Name: svgsimplegraph
+Version: 0.3.1
+Summary: Simple SVG graphing package
+Home-page: UNKNOWN
+Author: Garrett M. Petersen
+Author-email: garrett.m.petersen@gmail.com
+License: MIT
+Project-URL: Source Code, https://github.com/GarrettPetersen/svgsimplegraph
+Description: # svgsimplegraph
+        
+        This is a simple little graphing package for making graphs and exporting them as raw or base64-encoded SVGs.
+        
+        You can also upload the SVGs to your GitHub account as Gists, so they may be embedded in any website!
+        
+        ## Installing svgsimplegraph
+        Install svgsimplegraph by typing
+        ```
+        pip install svgsimplegraph
+        ```
+        in your terminal.
+        
+        ## Graph Types
+        ### Categorical Graph
+        
+        The categorical graph is for data that comes in distinct categories. It can generate a bar chart, a stacked bar chart, dots, or lines.
+        
+        Here is an example of how to make a graph:
+        
+        ```
+        from svgsimplegraph import CategoricalGraph
+        
+        graph = CategoricalGraph(
+                width=600,
+                height=400,
+                bar_width=30,
+                stacked=False,
+                background_color="#404040",
+                title="Categorical Graph",
+            )
+        
+        graph.x_labels = ["A", "B", "C", "D", "E"]
+        graph.x_axis_label = "X Axis"
+        graph.primary_y_axis_label = "Primary Y Axis"
+        
+        # Skip adding a legend_label to exclude a series from the legend
+        graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1")
+        graph.add_series([15, 25, 5, 44, 56], legend_label="Series 2")
+        graph.add_series([5, 35, 10, 33, 40], legend_label="Series 3", series_type="line")
+        graph.add_series([35, 56, 25, 5, 44], legend_label="Series 4", series_type="dot")
+        
+        # You can use vertical or horizontal lines to mark specific values
+        graph.add_vertical_line(
+            x=2.5,
+            label="Vertical Line",
+            label_x_position="right",
+            label_y_position="top",
+            rotate_label=True,
+        )
+        
+        # Get the SVG string in base64 format
+        svg_base64 = graph.to_base64_src()
+        
+        # Print the SVG string in an img tag so your browser can display it
+        print(f"\n<img src='{svg_base64}' />")
+        
+        # Alternatively, you can get the raw SVG code with render()
+        raw_svg = graph.render()
+        print(raw_svg)
+        ```
+        ![Example categorical graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_categorical.svg)
+        
+        ### Ribbon Graph
+        
+        The ribbon graph is for comparing two numbers on the same scale and a third number on a different scale (represented through color).
+        
+        The three series must be added in order, with the first representing the back of the ribbon, the second representing the point, and the (optional) third representing the color.
+        
+        Here's an example:
+        
+        ```
+        from svgsimplegraph import RibbonGraph
+        
+        graph = RibbonGraph(
+            width=600,
+            height=400,
+            bar_width=30,
+            background_color="#404040",
+            title="Ribbon Graph",
+        )
+        
+        graph.x_labels = ["A", "B", "C", "D", "E"]
+        graph.x_axis_label = "X Axis"
+        graph.primary_y_axis_label = "Primary Y Axis"
+        
+        graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1", print_values=True)
+        graph.add_series([20, 30, 40, 30, 20], legend_label="Series 2", print_values=True)
+        graph.add_series(
+            [-10, -20, 30, 20, 10], legend_label="Color Series", print_values=True
+        )
+        
+        # Get the SVG string in base64 format
+        svg_base64 = graph.to_base64_src()
+        
+        # Print the SVG string in an img tag so your browser can display it
+        print(f"\n<img src='{svg_base64}' />")
+        
+        # Alternatively, you can get the raw SVG code with render()
+        raw_svg = graph.render()
+        print(raw_svg)
+        ```
+        ![Example ribbon graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_ribbon.svg)
+        
+        ### Bubble and Arrow Graph
+        The bubble and arrow graph is for displaying relationships between nodes in a network.
+        
+        The user adds bubbles, which are displayed in clockwise order around a larger circle. Then the user can add arrows that exit from one bubble and enter another. Arrow width is scaled to show more important connections.
+        
+        Here's an example:
+        ```
+        from svgsimplegraph import BubbleAndArrowGraph
+        
+        graph = BubbleAndArrowGraph(
+            width=400,
+            height=400,
+            background_color="#ffffff",
+            title="Bubble and Arrow Graph",
+        )
+        
+        # Optional str label param can be referred to later when defining arrows
+        graph.add_bubble(100, None, "Bubble 0", label="big_bubble")
+        
+        # Otherwise bubbles must be referred to by their index number
+        graph.add_bubble(50, 25, "Bubble 1")
+        graph.add_bubble(25, 12.5, "Bubble 2")
+        
+        graph.add_arrow(
+            origin="big_bubble",
+            destination=1,
+            size=60,
+        )
+        graph.add_arrow(
+            origin="big_bubble",
+            destination=2,
+            size=40,
+        )
+        graph.add_arrow(
+            origin=1,
+            destination=2,
+            size=30,
+        )
+        
+        # Arrows pointing to their origin will loop around
+        graph.add_arrow(
+            origin=2,
+            destination=2,
+            size=20,
+        )
+        
+        # Get the SVG string in base64 format
+        svg_base64 = graph.to_base64_src()
+        
+        # Print the SVG string in an img tag so your browser can display it
+        print(f"\n<img src='{svg_base64}' />")
+        
+        # Alternatively, you can get the raw SVG code with render()
+        raw_svg = graph.render()
+        print(raw_svg)
+        ```
+        ![Example bubble and arrow graph](https://github.com/GarrettPetersen/svgsimplegraph/blob/master/images/example_bubble_and_arrow.svg)
+        
+        ## GitHub Gist integration
+        
+        The `upload_to_github_gist` function allows you to render your graph and upload it to your GitHub account as a Gist.
+        
+        To do this, you'll need an access token. Go to your github account and navigate to settings. Then click on Developer settings > Personal access tokens > Fine-grained tokens.
+        
+        Click the Generate new token button in the top right of the screen. GitHub will prompt you to login. Set a token name (something like "gist-access-token") and an expiration.
+        
+        Scroll down to Permissions and expand the Account permissions box. Then turn on read and write access for Gists only (you should not use this token for anything else). Finally, click the gree Generate token button at the bottom of the screen.
+        
+        Now you should see a screen showing your token. This is the only time Github will show you this token, so save it somewhere safe.
+        
+        Assuming you've done all that, you can use the token to turn your graphs into gists.
+        
+        ```
+        from svgsimplegraph import CategoricalGraph
+        
+        GITHUB_ACCESS_TOKEN = "your_token_goes_here"
+        
+        # Create an instance of a graph
+        graph = CategoricalGraph(
+            width=600,
+            height=400,
+            bar_width=30,
+            stacked=False,
+            background_color="#404040",
+        )
+        
+        graph.x_labels = ["A", "B", "C", "D", "E"]
+        graph.x_axis_label = "X Axis"
+        graph.primary_y_axis_label = "Primary Y Axis"
+        
+        graph.add_series([10, 20, 30, 40, 50], legend_label="Series 1")
+        
+        svg_url = graph.upload_to_github_gist(GITHUB_ACCESS_TOKEN, "my_categorical_graph")
+        ```
+        
+        The `svg_url` variable now contains a string with the url of your new SVG, ready to be embedded in any website!
+        
+        ## Watermarks
+        
+        When you initialize a graph, you can use the watermark variable to add arbitrary svg code to the graph. It is recommended to make your watermark partially transparent, as it will be placed on top of your graph.
+Keywords: graph,svg,base64,svg simple graph
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
```

### Comparing `svgsimplegraph-0.3.0/setup.py` & `svgsimplegraph-0.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read in the README.md for the long description on PyPI
 with open("README.md", "r") as f:
     long_description = f.read()
 
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 DESCRIPTION = "Simple SVG graphing package"
 
 setup(
     name="svgsimplegraph",
     version=VERSION,
     description=DESCRIPTION,
     long_description=long_description,
```

### Comparing `svgsimplegraph-0.3.0/svgsimplegraph/base.py` & `svgsimplegraph-0.3.1/svgsimplegraph/base.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/svgsimplegraph/bubble_and_arrow.py` & `svgsimplegraph-0.3.1/svgsimplegraph/bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/svgsimplegraph/categorical.py` & `svgsimplegraph-0.3.1/svgsimplegraph/categorical.py`

 * *Files 0% similar despite different names*

```diff
@@ -931,14 +931,15 @@
                             self.svg_elements.append(
                                 self._draw_line(
                                     legend_x,
                                     legend_y + legend_rect_size / 2,
                                     legend_x + legend_rect_size,
                                     legend_y + legend_rect_size / 2,
                                     stroke=self.colors[index],
+                                    stroke_width=self.stroke_width[index],
                                 )
                             )
                         else:  # series_type == "bar"
                             self.most_extreme_dimensions["left"] = min(
                                 self.most_extreme_dimensions["left"],
                                 legend_x,
                             )
@@ -989,14 +990,15 @@
                             self.svg_elements.append(
                                 self._draw_line(
                                     legend_x,
                                     legend_y + legend_rect_size / 2,
                                     legend_x + legend_rect_size,
                                     legend_y + legend_rect_size / 2,
                                     stroke=self.colors[index],
+                                    stroke_width=self.stroke_width[index],
                                 )
                             )
                         else:  # series_type == "bar"
                             self.most_extreme_dimensions["top"] = min(
                                 self.most_extreme_dimensions["top"],
                                 legend_y,
                             )
@@ -1070,14 +1072,15 @@
                             self.svg_elements.append(
                                 self._draw_line(
                                     legend_x,
                                     legend_y + legend_rect_size / 2,
                                     legend_x + legend_rect_size,
                                     legend_y + legend_rect_size / 2,
                                     stroke=self.colors[index],
+                                    stroke_width=self.stroke_width[index],
                                 )
                             )
                         else:  # series_type == "bar"
                             self.most_extreme_dimensions["bottom"] = max(
                                 self.most_extreme_dimensions["bottom"],
                                 legend_y + legend_rect_size,
                             )
```

### Comparing `svgsimplegraph-0.3.0/svgsimplegraph/ribbon.py` & `svgsimplegraph-0.3.1/svgsimplegraph/ribbon.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/svgsimplegraph/utils.py` & `svgsimplegraph-0.3.1/svgsimplegraph/utils.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/tests/test_bubble_and_arrow.py` & `svgsimplegraph-0.3.1/tests/test_bubble_and_arrow.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/tests/test_categorical.py` & `svgsimplegraph-0.3.1/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/tests/test_gist.py` & `svgsimplegraph-0.3.1/tests/test_gist.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/tests/test_readme_examples.py` & `svgsimplegraph-0.3.1/tests/test_readme_examples.py`

 * *Files identical despite different names*

### Comparing `svgsimplegraph-0.3.0/tests/test_ribbon.py` & `svgsimplegraph-0.3.1/tests/test_ribbon.py`

 * *Files identical despite different names*

