# Comparing `tmp/ridgeplot-0.1.8.tar.gz` & `tmp/ridgeplot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ridgeplot-0.1.8.tar", last modified: Wed Feb  3 00:05:46 2021, max compression
+gzip compressed data, was "dist/ridgeplot-0.1.9.tar", last modified: Sun Jun 27 22:29:07 2021, max compression
```

## Comparing `ridgeplot-0.1.8.tar` & `ridgeplot-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,24 @@
--rw-r--r--   0        0        0     3702 2021-02-02 21:43:16.028972 ridgeplot-0.1.8/README.md
--rw-r--r--   0        0        0     1308 2021-02-03 00:05:24.486935 ridgeplot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      811 2021-02-02 23:31:41.167778 ridgeplot-0.1.8/ridgeplot/__init__.py
--rw-r--r--   0        0        0     2385 2021-02-02 22:27:53.229434 ridgeplot-0.1.8/ridgeplot/_colors.py
--rw-r--r--   0        0        0     6409 2021-02-02 23:34:08.656236 ridgeplot-0.1.8/ridgeplot/_figure_factory.py
--rw-r--r--   0        0        0     2500 2021-02-02 22:19:31.838181 ridgeplot-0.1.8/ridgeplot/_kde.py
--rw-r--r--   0        0        0     6613 2021-02-02 23:44:14.802125 ridgeplot-0.1.8/ridgeplot/_ridgeplot.py
--rw-r--r--   0        0        0      838 2021-01-21 13:04:58.236146 ridgeplot-0.1.8/ridgeplot/_utils.py
--rw-r--r--   0        0        0     2048 2021-01-17 18:29:22.930996 ridgeplot-0.1.8/ridgeplot/_violin.py
--rw-r--r--   0        0        0    70665 2021-02-02 19:13:05.390115 ridgeplot-0.1.8/ridgeplot/colors.json
--rw-r--r--   0        0        0     4524 2021-02-03 00:05:47.024348 ridgeplot-0.1.8/setup.py
--rw-r--r--   0        0        0     4313 2021-02-03 00:05:47.024837 ridgeplot-0.1.8/PKG-INFO
+drwxr-xr-x   0 t.vasconcelos   (502) staff       (20)        0 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     1100 2021-06-27 21:42:35.000000 ridgeplot-0.1.9/LICENSE
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     6996 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/PKG-INFO
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     5807 2021-06-27 22:21:42.000000 ridgeplot-0.1.9/README.md
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)      956 2021-06-27 21:51:48.000000 ridgeplot-0.1.9/pyproject.toml
+drwxr-xr-x   0 t.vasconcelos   (502) staff       (20)        0 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/ridgeplot/
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)      869 2021-06-27 22:10:09.000000 ridgeplot-0.1.9/ridgeplot/__init__.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     2385 2021-06-09 11:47:11.000000 ridgeplot-0.1.9/ridgeplot/_colors.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     6404 2021-06-27 22:11:40.000000 ridgeplot-0.1.9/ridgeplot/_figure_factory.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     2440 2021-06-27 22:10:09.000000 ridgeplot-0.1.9/ridgeplot/_kde.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     6613 2021-06-09 11:47:11.000000 ridgeplot-0.1.9/ridgeplot/_ridgeplot.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)      838 2021-06-09 11:47:11.000000 ridgeplot-0.1.9/ridgeplot/_utils.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)       22 2021-06-27 22:27:58.000000 ridgeplot-0.1.9/ridgeplot/_version.py
+drwxr-xr-x   0 t.vasconcelos   (502) staff       (20)        0 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/ridgeplot.egg-info/
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     6996 2021-06-27 22:29:06.000000 ridgeplot-0.1.9/ridgeplot.egg-info/PKG-INFO
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)      413 2021-06-27 22:29:06.000000 ridgeplot-0.1.9/ridgeplot.egg-info/SOURCES.txt
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)        1 2021-06-27 22:29:06.000000 ridgeplot-0.1.9/ridgeplot.egg-info/dependency_links.txt
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)      208 2021-06-27 22:29:06.000000 ridgeplot-0.1.9/ridgeplot.egg-info/requires.txt
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)       16 2021-06-27 22:29:06.000000 ridgeplot-0.1.9/ridgeplot.egg-info/top_level.txt
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)     1703 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/setup.cfg
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)       91 2021-06-09 11:47:33.000000 ridgeplot-0.1.9/setup.py
+drwxr-xr-x   0 t.vasconcelos   (502) staff       (20)        0 2021-06-27 22:29:07.000000 ridgeplot-0.1.9/tests/
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)        0 2021-06-09 11:47:33.000000 ridgeplot-0.1.9/tests/__init__.py
+-rw-r--r--   0 t.vasconcelos   (502) staff       (20)       98 2021-06-27 22:27:58.000000 ridgeplot-0.1.9/tests/test_ridgeplot.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ridgeplot-0.1.8/ridgeplot/__init__.py` & `ridgeplot-0.1.9/ridgeplot/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,11 +19,12 @@
   # and the returned Plotly figure is still fully customizable
   fig.update_layout(height=500, width=800)
 
   # show us the work!!
   fig.show()
 
 """
-from ridgeplot._ridgeplot import ridgeplot
 from ridgeplot._colors import named_colorscales
+from ridgeplot._ridgeplot import ridgeplot
+from ridgeplot._version import __version__
 
-__all__ = ["ridgeplot", "named_colorscales"]
+__all__ = ["ridgeplot", "named_colorscales", "__version__"]
```

### Comparing `ridgeplot-0.1.8/ridgeplot/_colors.py` & `ridgeplot-0.1.9/ridgeplot/_colors.py`

 * *Files identical despite different names*

### Comparing `ridgeplot-0.1.8/ridgeplot/_figure_factory.py` & `ridgeplot-0.1.9/ridgeplot/_figure_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                 name=label,
                 fill="tonexty",
                 mode="lines",
                 line=dict(color=line_color, width=self.linewidth),
             ),
         )
 
-    def update_layout(self, y_ticks: list) -> go.Figure:
+    def update_layout(self, y_ticks: list) -> None:
         """Update figure's layout."""
         self.fig.update_layout(
             hovermode=False,
             legend=dict(traceorder="normal"),
         )
         axes_common = dict(
             zeroline=False,
```

### Comparing `ridgeplot-0.1.8/ridgeplot/_kde.py` & `ridgeplot-0.1.9/ridgeplot/_kde.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,15 @@
     # can return a nan float if something goes
     # wrong internally. As to avoid confusion
     # further down the pipeline, I decided
     # to check whether the correct object
     # (and shape) are being returned.
     if not isinstance(densities, np.ndarray) or densities.shape != points.shape:
         raise RuntimeError(
-            f"Could now evaluate densities using the {repr(kernel)} kernel! "
-            f"Try using kernel='gau' (default)."
+            f"Could now evaluate densities using the {repr(kernel)} kernel! " f"Try using kernel='gau' (default)."
         )
 
     return points, densities
 
 
 def get_densities(samples, points, kernel, bandwidth) -> np.ndarray:
-    return np.asarray(
-        [
-            evaluate_density(samples=s, points=points, kernel=kernel, bandwidth=bandwidth)
-            for s in samples
-        ]
-    )
+    return np.asarray([evaluate_density(samples=s, points=points, kernel=kernel, bandwidth=bandwidth) for s in samples])
```

### Comparing `ridgeplot-0.1.8/ridgeplot/_ridgeplot.py` & `ridgeplot-0.1.9/ridgeplot/_ridgeplot.py`

 * *Files identical despite different names*

### Comparing `ridgeplot-0.1.8/ridgeplot/_utils.py` & `ridgeplot-0.1.9/ridgeplot/_utils.py`

 * *Files identical despite different names*

