# Comparing `tmp/hvplot-0.9.2rc1.tar.gz` & `tmp/hvplot-0.9.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hvplot-0.9.2rc1.tar", last modified: Sun Jan 28 22:09:36 2024, max compression
+gzip compressed data, was "hvplot-0.9.3a1.tar", last modified: Fri Apr 19 09:55:33 2024, max compression
```

## Comparing `hvplot-0.9.2rc1.tar` & `hvplot-0.9.3a1.tar`

### file list

```diff
@@ -1,220 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.967042 hvplot-0.9.2rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-01-28 22:09:36.963042 hvplot-0.9.2rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.903042 hvplot-0.9.2rc1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.907042 hvplot-0.9.2rc1/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   359182 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (127)  1080507 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151250 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.907042 hvplot-0.9.2rc1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.907042 hvplot-0.9.2rc1/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.903042 hvplot-0.9.2rc1/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.907042 hvplot-0.9.2rc1/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.911042 hvplot-0.9.2rc1/examples/reference/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/tabular/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.915042 hvplot-0.9.2rc1/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/reference/xarray/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.915042 hvplot-0.9.2rc1/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    31440 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22075 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.919042 hvplot-0.9.2rc1/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/examples/user_guide/images/simple.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.919042 hvplot-0.9.2rc1/hvplot/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot/.version
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/backend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   101785 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/cudf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.923042 hvplot-0.9.2rc1/hvplot/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.923042 hvplot-0.9.2rc1/hvplot/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   359182 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (127)  1080507 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (127)   151250 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.923042 hvplot-0.9.2rc1/hvplot/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.927042 hvplot-0.9.2rc1/hvplot/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.903042 hvplot-0.9.2rc1/hvplot/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.927042 hvplot-0.9.2rc1/hvplot/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.931042 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/tabular/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.931042 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/reference/xarray/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.935042 hvplot-0.9.2rc1/hvplot/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)    11280 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11754 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    15528 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Integrations.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13672 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    31440 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22075 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23431 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    23018 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9187 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.935042 hvplot-0.9.2rc1/hvplot/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/examples/user_guide/images/simple.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/fugue.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/ibis.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/intake.py
--rw-r--r--   0 runner    (1001) docker     (127)    36804 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/interactive.py
--rw-r--r--   0 runner    (1001) docker     (127)    21303 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/networkx.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.935042 hvplot-0.9.2rc1/hvplot/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/andrews_curves.py
--rw-r--r--   0 runner    (1001) docker     (127)    80908 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/lag_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/plotting/scatter_matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/polars.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/streamz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.939042 hvplot-0.9.2rc1/hvplot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.939042 hvplot-0.9.2rc1/hvplot/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/plotting/testcore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/plotting/testohlc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/plotting/testscattermatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testbackend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testcharts.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testfugue.py
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testgeo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testgeowithoutgv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11575 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testgridplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testhelp.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testibis.py
--rw-r--r--   0 runner    (1001) docker     (127)    41836 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testinteractive.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testnetworkx.py
--rw-r--r--   0 runner    (1001) docker     (127)    14493 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testoperations.py
--rw-r--r--   0 runner    (1001) docker     (127)    22554 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testoverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testpatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testplotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/teststreaming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testtransforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testui.py
--rw-r--r--   0 runner    (1001) docker     (127)    14116 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/testutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    32398 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)    19345 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/hvplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 22:09:36.923042 hvplot-0.9.2rc1/hvplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-28 22:09:36.000000 hvplot-0.9.2rc1/hvplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-28 22:09:36.967042 hvplot-0.9.2rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5149 2024-01-28 22:05:30.000000 hvplot-0.9.2rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/binder/postBuild
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.913921 hvplot-0.9.3a1/conda.recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/conda.recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.917921 hvplot-0.9.3a1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.917921 hvplot-0.9.3a1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.925921 hvplot-0.9.3a1/doc/_static/home/
+-rw-r--r--   0 runner    (1001) docker     (127)   198618 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/bokeh.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   244779 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/dask.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   873325 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/explorer.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    47722 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/geo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   702643 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/geopandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    23983 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/intake.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    70800 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_hvplot.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    72465 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_pandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   173838 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/interactive_xarray.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   267815 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/large_data.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   109054 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/layout.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    84928 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/matplotlib.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36604 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/networkx.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    24841 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/overlay.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95678 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/pandas.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   116788 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/plotly.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   184170 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/widgets.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   241968 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/home/xarray.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.925921 hvplot-0.9.3a1/doc/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   194737 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/images/heat_and_trees.png
+-rw-r--r--   0 runner    (1001) docker     (127)   182260 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/images/portfolio.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13196 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo_horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/_static/logo_stacked.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/about.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   359182 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1080507 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   151250 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)   463297 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16120 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1007817 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/assets/streamz_demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/developer_guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.909921 hvplot-0.9.3a1/doc/governance/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/governance/project-docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/governance/project-docs/MEMBERS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.909921 hvplot-0.9.3a1/doc/reference/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.929921 hvplot-0.9.3a1/doc/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.933921 hvplot-0.9.3a1/doc/reference/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/tabular/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.937921 hvplot-0.9.3a1/doc/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/reference/xarray/violin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    32456 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/releases.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/roadmap.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/topics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10798 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    15674 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Integrations.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21995 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Large_Timeseries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25917 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    31550 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22152 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23524 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    23107 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9281 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/doc/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/images/simple.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/doc/user_guide/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.941921 hvplot-0.9.3a1/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.10-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.11-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.11-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.12-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.8-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/envs/py3.9-tests.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10874 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/backend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109238 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7871 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/datasets.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/ibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/intake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37370 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21430 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/networkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.945921 hvplot-0.9.3a1/hvplot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/andrews_curves.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80862 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/lag_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/plotting/scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/polars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/streamz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.949921 hvplot-0.9.3a1/hvplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.949921 hvplot-0.9.3a1/hvplot/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17612 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/data/RGB-red.byte.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/hvplot/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testcore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testohlc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/plotting/testscattermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testbackend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19435 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testcharts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testfugue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgeowithoutgv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testgridplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testhelp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testibis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42090 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testnetworkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoperations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testpatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testplotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/teststreaming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testtransforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10324 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32967 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19694 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/hvplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/hvplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14677 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-19 09:55:33.000000 hvplot-0.9.3a1/hvplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:55:33.953921 hvplot-0.9.3a1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 09:55:20.000000 hvplot-0.9.3a1/scripts/update_conda_envs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:55:33.957921 hvplot-0.9.3a1/setup.cfg
```

### Comparing `hvplot-0.9.2rc1/LICENSE` & `hvplot-0.9.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/README.md` & `hvplot-0.9.3a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # hvPlot makes data analysis and visualization simple <img src="https://github.com/holoviz/hvplot/blob/main/doc/_static/logo.png?raw=true" style="width:2em;margin-bottom:-15px">
 
 |    |    |
 | --- | --- |
+| Downloads | ![https://pypistats.org/packages/hvplot](https://img.shields.io/pypi/dm/hvplot?label=pypi) ![https://anaconda.org/pyviz/hvplot](https://pyviz.org/_static/cache/hvplot_conda_downloads_badge.svg)
 | Build Status | [![Build Status](https://github.com/holoviz/hvplot/workflows/tests/badge.svg?query=branch%3Amain)](https://github.com/holoviz/hvplot/actions?query=workflow%3Atests+branch%3Amain) |
 | Coverage | [![codecov](https://codecov.io/gh/holoviz/hvplot/branch/main/graph/badge.svg)](https://codecov.io/gh/holoviz/hvplot) |
 | Latest dev release | [![Github tag](https://img.shields.io/github/tag/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/tags) [![dev-site](https://img.shields.io/website-up-down-green-red/https/holoviz-dev.github.io/hvplot.svg?label=dev%20website)](https://holoviz-dev.github.io/hvplot/) |
 | Latest release | [![Github release](https://img.shields.io/github/release/holoviz/hvplot.svg?label=tag&colorB=11ccbb)](https://github.com/holoviz/hvplot/releases) [![PyPI version](https://img.shields.io/pypi/v/hvplot.svg?colorB=cc77dd)](https://pypi.python.org/pypi/hvplot) [![hvplot version](https://img.shields.io/conda/v/pyviz/hvplot.svg?colorB=4488ff&style=flat)](https://anaconda.org/pyviz/hvplot) [![conda-forge version](https://img.shields.io/conda/v/conda-forge/hvplot.svg?label=conda%7Cconda-forge&colorB=4488ff)](https://anaconda.org/conda-forge/hvplot) [![defaults version](https://img.shields.io/conda/v/anaconda/hvplot.svg?label=conda%7Cdefaults&style=flat&colorB=4488ff)](https://anaconda.org/anaconda/hvplot) |
 | Python | [![Python support](https://img.shields.io/pypi/pyversions/hvplot.svg)](https://pypi.org/project/hvplot/) |
 | Docs | [![gh-pages](https://img.shields.io/github/last-commit/holoviz/hvplot/gh-pages.svg)](https://github.com/holoviz/hvplot/tree/gh-pages) [![site](https://img.shields.io/website-up-down-green-red/http/hvplot.holoviz.org.svg)](https://hvplot.holoviz.org) |
-| Binder | [![Binder](https://img.shields.io/badge/launch%20v0.8.1-binder-579aca.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/holoviz/hvplot/v0.8.1?urlpath=lab/tree/examples) |
+| Binder | [![Binder](https://img.shields.io/badge/launch%20v0.8.1-binder-579aca.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAB8lBMVEX///9XmsrmZYH1olJXmsr1olJXmsrmZYH1olJXmsr1olJXmsrmZYH1olL1olJXmsr1olJXmsrmZYH1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olJXmsrmZYH1olL1olL0nFf1olJXmsrmZYH1olJXmsq8dZb1olJXmsrmZYH1olJXmspXmspXmsr1olL1olJXmsrmZYH1olJXmsr1olL1olJXmsrmZYH1olL1olLeaIVXmsrmZYH1olL1olL1olJXmsrmZYH1olLna31Xmsr1olJXmsr1olJXmsrmZYH1olLqoVr1olJXmsr1olJXmsrmZYH1olL1olKkfaPobXvviGabgadXmsqThKuofKHmZ4Dobnr1olJXmsr1olJXmspXmsr1olJXmsrfZ4TuhWn1olL1olJXmsqBi7X1olJXmspZmslbmMhbmsdemsVfl8ZgmsNim8Jpk8F0m7R4m7F5nLB6jbh7jbiDirOEibOGnKaMhq+PnaCVg6qWg6qegKaff6WhnpKofKGtnomxeZy3noG6dZi+n3vCcpPDcpPGn3bLb4/Mb47UbIrVa4rYoGjdaIbeaIXhoWHmZYHobXvpcHjqdHXreHLroVrsfG/uhGnuh2bwj2Hxk17yl1vzmljzm1j0nlX1olL3AJXWAAAAbXRSTlMAEBAQHx8gICAuLjAwMDw9PUBAQEpQUFBXV1hgYGBkcHBwcXl8gICAgoiIkJCQlJicnJ2goKCmqK+wsLC4usDAwMjP0NDQ1NbW3Nzg4ODi5+3v8PDw8/T09PX29vb39/f5+fr7+/z8/Pz9/v7+zczCxgAABC5JREFUeAHN1ul3k0UUBvCb1CTVpmpaitAGSLSpSuKCLWpbTKNJFGlcSMAFF63iUmRccNG6gLbuxkXU66JAUef/9LSpmXnyLr3T5AO/rzl5zj137p136BISy44fKJXuGN/d19PUfYeO67Znqtf2KH33Id1psXoFdW30sPZ1sMvs2D060AHqws4FHeJojLZqnw53cmfvg+XR8mC0OEjuxrXEkX5ydeVJLVIlV0e10PXk5k7dYeHu7Cj1j+49uKg7uLU61tGLw1lq27ugQYlclHC4bgv7VQ+TAyj5Zc/UjsPvs1sd5cWryWObtvWT2EPa4rtnWW3JkpjggEpbOsPr7F7EyNewtpBIslA7p43HCsnwooXTEc3UmPmCNn5lrqTJxy6nRmcavGZVt/3Da2pD5NHvsOHJCrdc1G2r3DITpU7yic7w/7Rxnjc0kt5GC4djiv2Sz3Fb2iEZg41/ddsFDoyuYrIkmFehz0HR2thPgQqMyQYb2OtB0WxsZ3BeG3+wpRb1vzl2UYBog8FfGhttFKjtAclnZYrRo9ryG9uG/FZQU4AEg8ZE9LjGMzTmqKXPLnlWVnIlQQTvxJf8ip7VgjZjyVPrjw1te5otM7RmP7xm+sK2Gv9I8Gi++BRbEkR9EBw8zRUcKxwp73xkaLiqQb+kGduJTNHG72zcW9LoJgqQxpP3/Tj//c3yB0tqzaml05/+orHLksVO+95kX7/7qgJvnjlrfr2Ggsyx0eoy9uPzN5SPd86aXggOsEKW2Prz7du3VID3/tzs/sSRs2w7ovVHKtjrX2pd7ZMlTxAYfBAL9jiDwfLkq55Tm7ifhMlTGPyCAs7RFRhn47JnlcB9RM5T97ASuZXIcVNuUDIndpDbdsfrqsOppeXl5Y+XVKdjFCTh+zGaVuj0d9zy05PPK3QzBamxdwtTCrzyg/2Rvf2EstUjordGwa/kx9mSJLr8mLLtCW8HHGJc2R5hS219IiF6PnTusOqcMl57gm0Z8kanKMAQg0qSyuZfn7zItsbGyO9QlnxY0eCuD1XL2ys/MsrQhltE7Ug0uFOzufJFE2PxBo/YAx8XPPdDwWN0MrDRYIZF0mSMKCNHgaIVFoBbNoLJ7tEQDKxGF0kcLQimojCZopv0OkNOyWCCg9XMVAi7ARJzQdM2QUh0gmBozjc3Skg6dSBRqDGYSUOu66Zg+I2fNZs/M3/f/Grl/XnyF1Gw3VKCez0PN5IUfFLqvgUN4C0qNqYs5YhPL+aVZYDE4IpUk57oSFnJm4FyCqqOE0jhY2SMyLFoo56zyo6becOS5UVDdj7Vih0zp+tcMhwRpBeLyqtIjlJKAIZSbI8SGSF3k0pA3mR5tHuwPFoa7N7reoq2bqCsAk1HqCu5uvI1n6JuRXI+S1Mco54YmYTwcn6Aeic+kssXi8XpXC4V3t7/ADuTNKaQJdScAAAAAElFTkSuQmCC)](https://mybinder.org/v2/gh/holoviz/hvplot/v0.8.1?urlpath=lab/tree) |
 | Support | [![Discourse](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.holoviz.org)](https://discourse.holoviz.org/c/hvplot/8) |
 
 [Home](https://hvplot.holoviz.org/) | [Installation instructions](#installation-instructions) | [Getting Started Guide](https://hvplot.holoviz.org/getting_started/index.html) | [Reference Guides](https://hvplot.holoviz.org/reference/index.html) | [Examples](#examples) | [License](#license) | [Support](#support--feedback)
 
 ## hvPlot provides a familiar, high-level API for visualization
 
 The API is based on the familiar Pandas `.plot` API and the innovative `.interactive` API.
```

### Comparing `hvplot-0.9.2rc1/examples/assets/console.png` & `hvplot-0.9.3a1/doc/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/assets/console_server.gif` & `hvplot-0.9.3a1/doc/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/assets/diagram.png` & `hvplot-0.9.3a1/doc/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/assets/hvplot-wm.png` & `hvplot-0.9.3a1/doc/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/data/crime.csv` & `hvplot-0.9.3a1/hvplot/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/datasets.yaml` & `hvplot-0.9.3a1/hvplot/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/examples/getting_started/explorer.ipynb` & `hvplot-0.9.3a1/doc/getting_started/explorer.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'44877a38-b5b2-4ed4-8a59-7fe3571f03fa'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "explorer'])]))]}"}*

```diff
@@ -1,11 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "44877a38-b5b2-4ed4-8a59-7fe3571f03fa",
+            "metadata": {},
+            "source": [
+                "# explorer"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "a8d569ea",
             "metadata": {},
             "source": [
                 "The *Explorer* is a [Panel](https://panel.holoviz.org)-based web application with which you can easily explore your data. While using `.hvplot()` is a convenient way to create plots from data, it assumes some *a piori* knowledge about the data itself and its structure, and also knowdlege about `.hvplot()`'s API itself. The *Explorer* is a graphical interface that offers a simple way to select and visualize the kind of plot you want to see your data with, and many options to customize that plot."
             ]
         },
         {
```

### Comparing `hvplot-0.9.2rc1/examples/getting_started/hvplot.ipynb` & `hvplot-0.9.3a1/doc/getting_started/hvplot.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9969512195121951%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'158bb196-9e72-45f0-ae7d-585e66922abe'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "hvplot'])]))]}"}*

```diff
@@ -1,11 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "158bb196-9e72-45f0-ae7d-585e66922abe",
+            "metadata": {},
+            "source": [
+                "# hvplot"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "055d7cc3",
             "metadata": {},
             "source": [
                 "The core functionality provided by hvPlot is a **simple and high-level plotting interface** (API), modeled on [Pandas](https://pandas.pydata.org)'s `.plot` API and extended in various ways leveraging capabilities offered by the packages of the [HoloViz](https://holoviz.org) ecosystem, most notably [HoloViews](https://holoviews.org/). hvPlot can generate interactive plots with either [Bokeh](https://www.bokeh.org) (default) or [Plotly](https://plotly.com/python/), or static plots with [Matplotlib](https://matplotlib.org). hvPlot supports many data libraries of the Python ecosystem:\n",
                 "\n",
                 "* [Pandas](https://pandas.pydata.org): DataFrame, Series (columnar/tabular data)\n",
                 "* [XArray](https://xarray.pydata.org): Dataset, DataArray (labelled multidimensional arrays)\n",
```

### Comparing `hvplot-0.9.2rc1/examples/getting_started/interactive.ipynb` & `hvplot-0.9.3a1/doc/getting_started/interactive.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'c611b682-e4ec-4028-9aa6-b33c7745c494'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "interactive'])]))]}"}*

```diff
@@ -1,11 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "c611b682-e4ec-4028-9aa6-b33c7745c494",
+            "metadata": {},
+            "source": [
+                "# interactive"
+            ]
+        },
+        {
+            "cell_type": "markdown",
             "id": "66dddf49-c70a-4ed1-98e7-76703b82fa34",
             "metadata": {},
             "source": [
                 "hvPlot isn't only a plotting library, it is dedicated to make data exploration easier. In this guide you will see how it can help you to get better control over your data pipelines. We define a *data pipeline* as a series of commands that *transform* some data, such as aggregating, filtering, reshaping, renaming, etc. A data pipeline may include a *load* step that will provide the input data to the pipeline, e.g. reading the data from a data base. \n",
                 "\n",
                 "When you analyze some data in a notebook that is for instance held in a Pandas DataFrame, you may find yourself having to re-run many cells after changing the parameters you provide to Pandas' methods, either to get more insights on the data or fine tune an algorithm. `.interactive()` is a solution to improve this rather cumbersome workflow, by which you replace the constant parameters in the pipeline by widgets (e.g. a number slider), that will automatically get displayed next to your pipeline output and will trigger an output update on changes. With this approach all your pipeline parameters are available in one place and you get full interactive control over the pipeline.\n",
                 "\n",
```

### Comparing `hvplot-0.9.2rc1/examples/reference/geopandas/points.ipynb` & `hvplot-0.9.3a1/doc/reference/geopandas/points.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Points'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Points"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/geopandas/polygons.ipynb` & `hvplot-0.9.3a1/doc/reference/geopandas/polygons.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Polygons'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Polygons"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/andrewscurves.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/andrewscurves.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'285a3796-e7d9-45ba-8b11-418c0535a8c9'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Andrewscurves'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "285a3796-e7d9-45ba-8b11-418c0535a8c9",
+            "metadata": {},
+            "source": [
+                "# Andrewscurves"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "d8d7bf92-ae63-4122-9457-10c9ada6c6f1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/area.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/hist.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9671794871794872%*

 * *Differences: {"'cells'": "{0: {'source': ['# Hist']}, 1: {'source': {insert: [(0, 'import hvplot.pandas  # "*

 * *            'noqa\\n\'), (2, \'# hvplot.extension("matplotlib")\')], delete: [2, 0]}}, 2: '*

 * *            "{'source': ['`hist` is often a good way to start looking at continuous data to get a "*

 * *            'sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available '*

 * *            "as `density`).']}, 3: {'source': ['from bokeh.sampledata.autompg import "*

 * *            "autompg_clean\\n', '\\n […]*

```diff
@@ -1,114 +1,117 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import hvplot.pandas  # noqa"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`area` can be used to color the area under a line or to color the space between two lines. "
+                "# Hist"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from bokeh.sampledata.degrees import data\n",
+                "import hvplot.pandas  # noqa\n",
                 "\n",
-                "data.tail()"
+                "# hvplot.extension(\"matplotlib\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "First we'll look at a single curve, where we are enforcing the y axis must be between 0 and 100 and we set the background color."
+                "`hist` is often a good way to start looking at continuous data to get a sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available as `density`)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "data.hvplot.area(x='Year', y='Computer Science', label='% of Computer Science Degrees Earned by Women',\n",
-                "                 ylim=(0, 100), width=500, height=400).opts(bgcolor='goldenrod')"
+                "from bokeh.sampledata.autompg import autompg_clean\n",
+                "\n",
+                "autompg_clean.sample(n=5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pandas as pd\n",
-                "from bokeh.sampledata.stocks import MSFT\n",
-                "\n",
-                "df = pd.DataFrame(MSFT)\n",
-                "df['date'] = pd.to_datetime(df.date)\n",
-                "df.head()"
+                "autompg_clean.hvplot.hist(\"weight\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "To color the area between two curves, include both a `y` and a `y2`."
+                "When using `by` the plots are overlaid by default. To create subplots instead, use `subplots=True`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df[df.date.dt.year == 2000].hvplot.area(x='date', y='low', y2='high')"
+                "autompg_clean.hvplot.hist(\"weight\", by=\"origin\", subplots=True, width=250)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "When multiple y values are passed, they are stacked by default."
+                "You can also plot histograms of *datetime* data"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import pandas as pd\n",
+                "from bokeh.sampledata.commits import data as commits\n",
+                "\n",
+                "commits = commits.reset_index().sort_values(\"datetime\")\n",
+                "commits.head(3)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.hvplot.area(x='date', y=['open', 'close'])"
+                "commits.hvplot.hist(\n",
+                "    \"datetime\",\n",
+                "    bin_range=(pd.Timestamp('2012-11-30'), pd.Timestamp('2017-05-01')),\n",
+                "    bins=54,   \n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Area plots can also be unstacked:"
+                "If you want to plot the distribution of a categorical column you can calculate the distribution using Pandas' method `value_counts` and plot it using `.hvplot.bar`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.hvplot.area(x='date', y=['open', 'close'], stacked=False,\n",
-                "               groupby='date.year', legend='bottom_right', width=500)"
+                "autompg_clean[\"mfr\"].value_counts().hvplot.bar(invert=True, flip_yaxis=True, height=500)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/bar.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/bar.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333333%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Bar'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Bar"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import hvplot.pandas  # noqa"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/barh.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/barh.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Barh'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Barh"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/bivariate.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/step.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9658333333333333%*

 * *Differences: {"'cells'": "{2: {'source': ['`step` can be used pretty much anytime line might be used and has "*

 * *            "many of the same options available. ']}, 3: {'source': ['from "*

 * *            "bokeh.sampledata.degrees import data as deg\\n', 'deg.sample(n=5)']}, 4: {'source': "*

 * *            '["deg.hvplot.step(x=\'Year\', y=[\'Art and Performance\', \'Business\', \'Biology\', '*

 * *            '\'Education\', \'Computer Science\'], \\n", "                value_label=\'% of '*

 * *            'Degrees Earned by Women\', leg […]*

```diff
@@ -1,43 +1,50 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Step"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`bivariate()` is a statistical method for creating a 2D density plot. Bivariate plots can be a useful alternative to scatter plots if your data are too dense to plot each point individually."
+                "`step` can be used pretty much anytime line might be used and has many of the same options available. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from bokeh.sampledata.autompg import autompg_clean as df\n",
-                "\n",
-                "df.head()"
+                "from bokeh.sampledata.degrees import data as deg\n",
+                "deg.sample(n=5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.hvplot.bivariate('accel', 'mpg')"
+                "deg.hvplot.step(x='Year', y=['Art and Performance', 'Business', 'Biology', 'Education', 'Computer Science'], \n",
+                "                value_label='% of Degrees Earned by Women', legend='top', height=500, width=620)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/box.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/box.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8611111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Box'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Box"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
@@ -73,9 +80,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/errorbars.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/errorbars.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.859375%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Errorbars'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Errorbars"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
@@ -66,9 +73,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/heatmap.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/heatmap.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Heatmap'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Heatmap"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/hexbin.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/hexbin.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9708333333333333%*

 * *Differences: {"'cells'": "{2: {'source': ['`.hexbin()` offers a straightforward method for plotting dense "*

 * *            "data.']}, insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', "*

 * *            "OrderedDict()), ('source', ['# Hexbin'])]))]}"}*

```diff
@@ -1,23 +1,30 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Hexbin"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`.hebin()` offers a straightforward method for plotting dense data."
+                "`.hexbin()` offers a straightforward method for plotting dense data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/hist.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/bar.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8039772727272727%*

 * *Differences: {"'cells'": "{0: {'source': ['# Bar'], 'id': '3b507dd1-31f6-4732-bbc7-c82f2135fe1f'}, 1: "*

 * *            "{'source': ['import hvplot.xarray  # noqa\\n', 'import xarray as xr'], 'id': "*

 * *            "'5d0ed0f8-ce26-4c54-9161-d34ca73ae716'}, 2: {'source': ['## Introduction\\n', '\\n', "*

 * *            "'A `bar` plot represents **categorical data** with rectangular bars with heights "*

 * *            "proportional to the **numerical values** that they represent.\\n', 'The x-axis "*

 * *            "represents the categories  […]*

```diff
@@ -1,115 +1,84 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import hvplot.pandas  # noqa\n",
-                "\n",
-                "# hvplot.extension(\"matplotlib\")"
-            ]
-        },
-        {
             "cell_type": "markdown",
+            "id": "3b507dd1-31f6-4732-bbc7-c82f2135fe1f",
             "metadata": {},
             "source": [
-                "`hist` is often a good way to start looking at continuous data to get a sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available as `density`)."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from bokeh.sampledata.autompg import autompg_clean\n",
-                "\n",
-                "autompg_clean.sample(n=5)"
+                "# Bar"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "5d0ed0f8-ce26-4c54-9161-d34ca73ae716",
             "metadata": {},
             "outputs": [],
             "source": [
-                "autompg_clean.hvplot.hist(\"weight\")"
+                "import hvplot.xarray  # noqa\n",
+                "import xarray as xr"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e3f7e297-9576-4c36-9a9f-a4200ccf2d36",
             "metadata": {},
             "source": [
-                "When using `by` the plots are overlaid by default. To create subplots instead, use `subplots=True`."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "autompg_clean.hvplot.hist(\"weight\", by=\"origin\", subplots=True, width=250)"
+                "## Introduction\n",
+                "\n",
+                "A `bar` plot represents **categorical data** with rectangular bars with heights proportional to the **numerical values** that they represent.\n",
+                "The x-axis represents the categories and the y axis represents the numerical value scale.\n",
+                "The bars are of equal width which allows for instant comparison of data."
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "af429bbb-9a65-4b5d-b447-ce50b35dfedc",
             "metadata": {},
             "source": [
-                "You can also plot histograms of *datetime* data"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import pandas as pd\n",
-                "from bokeh.sampledata.commits import data as commits\n",
+                "## Data\n",
                 "\n",
-                "commits = commits.reset_index().sort_values(\"datetime\")\n",
-                "commits.head(3)"
+                "Let's load some data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "8db8fff7-b85f-49ea-b281-4a4d86e0f3ee",
             "metadata": {},
             "outputs": [],
             "source": [
-                "commits.hvplot.hist(\n",
-                "    \"datetime\",\n",
-                "    bin_range=(pd.Timestamp('2012-11-30'), pd.Timestamp('2017-05-01')),\n",
-                "    bins=54,   \n",
-                ")"
+                "ds = xr.tutorial.open_dataset('air_temperature').load()\n",
+                "air = ds.air\n",
+                "air1d = air.sel(lon=285.,lat=40.).groupby('time.month').mean()\n",
+                "air1d"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "629c5172-9cba-4f5f-bf3b-67e0a390385b",
             "metadata": {},
             "source": [
-                "If you want to plot the distribution of a categorical column you can calculate the distribution using Pandas' method `value_counts` and plot it using `.hvplot.bar`."
+                "## Basic Bar Plots"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "dfd1afa2-e310-4630-bd30-96e390078caf",
             "metadata": {},
             "outputs": [],
             "source": [
-                "autompg_clean[\"mfr\"].value_counts().hvplot.bar(invert=True, flip_yaxis=True, height=500)"
+                "air1d.hvplot.bar(y='air', height=500, title=\"Air Temperature by Month\")"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/kde.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/kde.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Kde'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Kde"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/labels.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/labels.ipynb`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428572%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Labels'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Labels"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
@@ -64,9 +71,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/lagplot.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/hist.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8184523809523809%*

 * *Differences: {"'cells'": "{1: {'source': ['import hvplot.xarray  # noqa\\n', 'import xarray as xr'], delete: "*

 * *            "['id']}, 2: {'source': ['`hist` is often a good way to start looking at data to get a "*

 * *            'sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available '*

 * *            'as `density`).\'], delete: [\'id\']}, 3: {\'cell_type\': \'code\', \'source\': ["ds = '*

 * *            'xr.tutorial.open_dataset(\'air_temperature\').load()\\n", \'air = ds.air\\n\', '*

 * *            "'air […]*

```diff
@@ -1,72 +1,73 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Hist"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
-            "id": "cb5dd3db-78c4-4a01-ba07-37f718f7425a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import hvplot.pandas  # noqa\n",
-                "import numpy as np\n",
-                "import pandas as pd"
+                "import hvplot.xarray  # noqa\n",
+                "import xarray as xr"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "c7af165e-4231-49ea-81d7-d07ad81a05da",
             "metadata": {},
             "source": [
-                "Lag plots are most commonly used to look for patterns in time series data."
+                "`hist` is often a good way to start looking at data to get a sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available as `density`)."
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "815a51ab-5f61-4bea-bb56-e11a0f117718",
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {},
+            "outputs": [],
             "source": [
-                "Given the following time series:"
+                "ds = xr.tutorial.open_dataset('air_temperature').load()\n",
+                "air = ds.air\n",
+                "air1d = air.sel(lon=285.,lat=40.)\n",
+                "air1d"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "283adbd9-3c42-4cb7-8c57-1d0e9fe1d25f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "np.random.seed(5)\n",
-                "x = np.cumsum(np.random.normal(loc=1, scale=5, size=50))\n",
-                "s = pd.Series(x, name='Time series')\n",
-                "\n",
-                "s.hvplot()"
+                "air1d.hvplot.hist()"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "8a877a7d-11cb-4bcb-81e4-3936f061ba65",
             "metadata": {},
             "source": [
-                "A lag plot with `lag=1` returns:"
+                "Customize the plot by changing the title and bar color."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "52be318e-fccd-461d-9813-c231b6f2997c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "hvplot.plotting.lag_plot(s, lag=1)"
+                "air1d.hvplot.hist(title=\"Air Temperature over time at lat=40,lon285\", color='gray')"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 5
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/line.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/line.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Line'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Line"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/ohlc.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/ohlc.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Ohlc'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Ohlc"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "import hvplot.pandas  # noqa"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/parallelcoordinates.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/parallelcoordinates.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666667%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'fe36abdf-7ad3-4acf-8143-b8e9eb04c9a9'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Parallelcoordinates'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "fe36abdf-7ad3-4acf-8143-b8e9eb04c9a9",
+            "metadata": {},
+            "source": [
+                "# Parallelcoordinates"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "98539b4c-af81-4ad7-9fe5-8e1b828ee3d8",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/scatter.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/scatter.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Scatter'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Scatter"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/scattermatrix.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/scattermatrix.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.993421052631579%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'78539fd7-a71f-4027-8b1b-c7fd75526a22'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Scattermatrix'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "78539fd7-a71f-4027-8b1b-c7fd75526a22",
+            "metadata": {},
+            "source": [
+                "# Scattermatrix"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "c092a604-c386-4dda-bc90-0ff11a8f880f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/step.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/table.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8256944444444445%*

 * *Differences: {"'cells'": "{2: {'source': ['`table` allows the creation of a holoviews `Table` element with all "*

 * *            'the options available on that. It can be very useful especially when paired with '*

 * *            "other visualizations. ']}, 3: {'source': ['from bokeh.sampledata.autompg import "*

 * *            "autompg_clean as df\\n', '\\n', 'df.head()']}, 4: {'source': "*

 * *            '["df.hvplot.table(columns=[\'origin\', \'name\', \'yr\'], sortable=True, '*

 * *            'selectable=True)"]}, insert: [(0, OrderedDic […]*

```diff
@@ -1,48 +1,62 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Table"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`step` can be used pretty much anytime line might be used and has many of the same options available. "
+                "`table` allows the creation of a holoviews `Table` element with all the options available on that. It can be very useful especially when paired with other visualizations. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from bokeh.sampledata.degrees import data as deg\n",
-                "deg.sample(n=5)"
+                "from bokeh.sampledata.autompg import autompg_clean as df\n",
+                "\n",
+                "df.head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "deg.hvplot.step(x='Year', y=['Art and Performance', 'Business', 'Biology', 'Education', 'Computer Science'], \n",
-                "                value_label='% of Degrees Earned by Women', legend='top', height=500, width=620)"
+                "df.hvplot.table(columns=['origin', 'name', 'yr'], sortable=True, selectable=True)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Click on the header to sort on the values in a column and on a row to select that column."
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/table.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/bivariate.ipynb`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8277777777777777%*

 * *Differences: {"'cells'": "{2: {'source': ['`bivariate()` is a statistical method for creating a 2D density "*

 * *            'plot. Bivariate plots can be a useful alternative to scatter plots if your data are '*

 * *            "too dense to plot each point individually.']}, 4: {'source': "*

 * *            '["df.hvplot.bivariate(\'accel\', \'mpg\')"]}, insert: [(0, '*

 * *            "OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Bivariate'])]))], delete: [4]}",*

 * * "'nbformat_minor'": ' […]*

```diff
@@ -1,23 +1,30 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Bivariate"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`table` allows the creation of a holoviews `Table` element with all the options available on that. It can be very useful especially when paired with other visualizations. "
+                "`bivariate()` is a statistical method for creating a 2D density plot. Bivariate plots can be a useful alternative to scatter plots if your data are too dense to plot each point individually."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -29,27 +36,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "df.hvplot.table(columns=['origin', 'name', 'yr'], sortable=True, selectable=True)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Click on the header to sort on the values in a column and on a row to select that column."
+                "df.hvplot.bivariate('accel', 'mpg')"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/tabular/violin.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/violin.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.85%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Violin'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Violin"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
@@ -42,9 +49,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/bar.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/violin.ipynb`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9351190476190476%*

 * *Differences: {"'cells'": "{1: {'id': '2ccf9fd5-9d10-4522-961d-7e8d236213b2'}, 2: {'id': "*

 * *            "'f7ed6c65-2280-4741-b89b-721110628547', 'source': ['`violin` plots are similar to box "*

 * *            'plots, but provide a better sense of the distribution of data. Note that `violin` '*

 * *            "plots depend on the `scipy` library.']}, 3: {'id': "*

 * *            "'e0f6ecc7-0f6a-4590-9c98-da10a674b9b0', 'source': {insert: [(2, 'air')], delete: [3, "*

 * *            "2]}}, 4: {'id': '2a137994-0a9d-4a75-8192-1e4bb4ead6c5', 's […]*

```diff
@@ -1,71 +1,56 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "5d0ed0f8-ce26-4c54-9161-d34ca73ae716",
+            "cell_type": "markdown",
+            "id": "cc4ff857-13b2-4f43-97dd-502a0703d276",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import hvplot.xarray  # noqa\n",
-                "import xarray as xr"
+                "# Violin"
             ]
         },
         {
-            "cell_type": "markdown",
-            "id": "e3f7e297-9576-4c36-9a9f-a4200ccf2d36",
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "2ccf9fd5-9d10-4522-961d-7e8d236213b2",
             "metadata": {},
+            "outputs": [],
             "source": [
-                "## Introduction\n",
-                "\n",
-                "A `bar` plot represents **categorical data** with rectangular bars with heights proportional to the **numerical values** that they represent.\n",
-                "The x-axis represents the categories and the y axis represents the numerical value scale.\n",
-                "The bars are of equal width which allows for instant comparison of data."
+                "import hvplot.xarray  # noqa\n",
+                "import xarray as xr"
             ]
         },
         {
             "cell_type": "markdown",
-            "id": "af429bbb-9a65-4b5d-b447-ce50b35dfedc",
+            "id": "f7ed6c65-2280-4741-b89b-721110628547",
             "metadata": {},
             "source": [
-                "## Data\n",
-                "\n",
-                "Let's load some data."
+                "`violin` plots are similar to box plots, but provide a better sense of the distribution of data. Note that `violin` plots depend on the `scipy` library."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "8db8fff7-b85f-49ea-b281-4a4d86e0f3ee",
+            "id": "e0f6ecc7-0f6a-4590-9c98-da10a674b9b0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "ds = xr.tutorial.open_dataset('air_temperature').load()\n",
                 "air = ds.air\n",
-                "air1d = air.sel(lon=285.,lat=40.).groupby('time.month').mean()\n",
-                "air1d"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "629c5172-9cba-4f5f-bf3b-67e0a390385b",
-            "metadata": {},
-            "source": [
-                "## Basic Bar Plots"
+                "air"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "dfd1afa2-e310-4630-bd30-96e390078caf",
+            "id": "2a137994-0a9d-4a75-8192-1e4bb4ead6c5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "air1d.hvplot.bar(y='air', height=500, title=\"Air Temperature by Month\")"
+                "air.hvplot.violin(y='air', by='lat', color='lat', cmap='Category20', title=\"Air Temperature vs. latitude\")"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/contour.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/contour.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Contour'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Contour"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/contourf.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/contourf.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Contourf'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Contourf"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/hist.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/line.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9726190476190476%*

 * *Differences: {"'cells'": "{2: {'source': ['`line` is useful when data is continuous and has a continuous "*

 * *            "axis.']}, 4: {'source': ['air1d.hvplot.line()']}, 5: {'source': ['Customize the plot "*

 * *            "by changing the title and line color.']}, 6: {'source': "*

 * *            '[\'air1d.hvplot.line(title="Air Temperature over time at '*

 * *            'lat=40,lon285",line_color=\\\'gray\\\')\']}, insert: [(0, '*

 * *            "OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', ['# "*

 * *    […]*

```diff
@@ -1,24 +1,31 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Line"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa\n",
                 "import xarray as xr"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "`hist` is often a good way to start looking at data to get a sense of the distribution. Similar methods include [`kde`](kde.ipynb) (also available as `density`)."
+                "`line` is useful when data is continuous and has a continuous axis."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -31,31 +38,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "air1d.hvplot.hist()"
+                "air1d.hvplot.line()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Customize the plot by changing the title and bar color."
+                "Customize the plot by changing the title and line color."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "air1d.hvplot.hist(title=\"Air Temperature over time at lat=40,lon285\", color='gray')"
+                "air1d.hvplot.line(title=\"Air Temperature over time at lat=40,lon285\",line_color='gray')"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/image.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/image.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886363636363636%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Image'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Image"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/kde.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/kde.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'a8373dcf-f097-454d-b97a-2f4e7bf20e62'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Kde'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "a8373dcf-f097-454d-b97a-2f4e7bf20e62",
+            "metadata": {},
+            "source": [
+                "# Kde"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ccf9fd5-9d10-4522-961d-7e8d236213b2",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa\n",
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/line.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/lagplot.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8184523809523809%*

 * *Differences: {"'cells'": "{1: {'source': ['import hvplot.pandas  # noqa\\n', 'import numpy as np\\n', 'import "*

 * *            "pandas as pd'], 'id': 'cb5dd3db-78c4-4a01-ba07-37f718f7425a'}, 2: {'source': ['Lag "*

 * *            "plots are most commonly used to look for patterns in time series data.'], 'id': "*

 * *            "'c7af165e-4231-49ea-81d7-d07ad81a05da'}, 3: {'cell_type': 'markdown', 'source': "*

 * *            "['Given the following time series:'], 'id': '815a51ab-5f61-4bea-bb56-e11a0f117718', "*

 * *            "delete: ['exe […]*

```diff
@@ -1,66 +1,80 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "7eb37c52-8262-4359-a6c1-3214e675fa5d",
+            "metadata": {},
+            "source": [
+                "# Lagplot"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
+            "id": "cb5dd3db-78c4-4a01-ba07-37f718f7425a",
             "metadata": {},
             "outputs": [],
             "source": [
-                "import hvplot.xarray  # noqa\n",
-                "import xarray as xr"
+                "import hvplot.pandas  # noqa\n",
+                "import numpy as np\n",
+                "import pandas as pd"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "c7af165e-4231-49ea-81d7-d07ad81a05da",
             "metadata": {},
             "source": [
-                "`line` is useful when data is continuous and has a continuous axis."
+                "Lag plots are most commonly used to look for patterns in time series data."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
+            "id": "815a51ab-5f61-4bea-bb56-e11a0f117718",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "ds = xr.tutorial.open_dataset('air_temperature').load()\n",
-                "air = ds.air\n",
-                "air1d = air.sel(lon=285.,lat=40.)\n",
-                "air1d"
+                "Given the following time series:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "283adbd9-3c42-4cb7-8c57-1d0e9fe1d25f",
             "metadata": {},
             "outputs": [],
             "source": [
-                "air1d.hvplot.line()"
+                "np.random.seed(5)\n",
+                "x = np.cumsum(np.random.normal(loc=1, scale=5, size=50))\n",
+                "s = pd.Series(x, name='Time series')\n",
+                "\n",
+                "s.hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8a877a7d-11cb-4bcb-81e4-3936f061ba65",
             "metadata": {},
             "source": [
-                "Customize the plot by changing the title and line color."
+                "A lag plot with `lag=1` returns:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "52be318e-fccd-461d-9813-c231b6f2997c",
             "metadata": {},
             "outputs": [],
             "source": [
-                "air1d.hvplot.line(title=\"Air Temperature over time at lat=40,lon285\",line_color='gray')"
+                "hvplot.plotting.lag_plot(s, lag=1)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/quadmesh.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/quadmesh.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428572%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Quadmesh'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Quadmesh"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
@@ -57,9 +64,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/rgb.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/rgb.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8541666666666667%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Rgb'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Rgb"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
@@ -48,9 +55,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/reference/xarray/vectorfield.ipynb` & `hvplot-0.9.3a1/doc/reference/xarray/vectorfield.ipynb`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8625%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Vectorfield'])]))]}",*

 * * "'nbformat_minor'": '4'}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Vectorfield"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.xarray  # noqa"
             ]
@@ -111,9 +118,9 @@
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 2
+    "nbformat_minor": 4
 }
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Customization.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Customization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9881918913398693%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, '    bgcolor: str\\n'), (5, '        Background color of "*

 * *            "the data area of the plot\\n'), (57, '    robust: bool\\n'), (58, '        If True "*

 * *            "and clim are absent, the colormap range is computed\\n'), (59, '        with 2nd and "*

 * *            "98th percentiles instead of the extreme values\\n'), (60, '        for image "*

 * *            'elements. For RGB elements, clips the "RGB", or\\n\'), (61, \'        raw reflectance '*

 * *            'values  […]*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Customization"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot\n",
                 "import hvplot.pandas  # noqa"
@@ -31,14 +38,16 @@
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generic options\n",
                 "\n",
                 "The generic set of options which may apply to all plot types include:\n",
                 "\n",
+                "    bgcolor: str\n",
+                "        Background color of the data area of the plot\n",
                 "    clim: tuple\n",
                 "        Lower and upper bound of the color scale\n",
                 "    cnorm (default='linear'): str\n",
                 "        Color scaling which must be one of 'linear', 'log' or 'eq_hist'\n",
                 "    colorbar (default=False): boolean\n",
                 "        Enables a colorbar\n",
                 "    fontscale: number\n",
@@ -82,14 +91,20 @@
                 "        upper and lower bounds.\n",
                 "    responsive: boolean\n",
                 "        Whether the plot should responsively resize depending on the\n",
                 "        size of the browser. Responsive mode will only work if at\n",
                 "        least one dimension of the plot is left undefined, e.g. when\n",
                 "        width and height or width and aspect are set the plot is set\n",
                 "        to a fixed size, ignoring any responsive option.\n",
+                "    robust: bool\n",
+                "        If True and clim are absent, the colormap range is computed\n",
+                "        with 2nd and 98th percentiles instead of the extreme values\n",
+                "        for image elements. For RGB elements, clips the \"RGB\", or\n",
+                "        raw reflectance values between 2nd and 98th percentiles.\n",
+                "        Follows the same logic as xarray's robust option.\n",
                 "    rot: number\n",
                 "        Rotates the axis ticks along the x-axis by the specified\n",
                 "        number of degrees.\n",
                 "    shared_axes (default=True): boolean\n",
                 "        Whether to link axes between plots\n",
                 "    transforms (default={}): dict\n",
                 "        A dictionary of HoloViews dim transforms to apply before plotting\n",
@@ -184,15 +199,18 @@
                 "    project (default=False):\n",
                 "        Whether to project the data before plotting (adds initial\n",
                 "        overhead but avoids projecting data when plot is dynamically\n",
                 "        updated).\n",
                 "    tiles (default=False):\n",
                 "        Whether to overlay the plot on a tile source. Tiles sources\n",
                 "        can be selected by name or a tiles object or class can be passed,\n",
-                "        the default is 'Wikipedia'."
+                "        the default is 'Wikipedia'.\n",
+                "    tiles_opts (default=None): dict\n",
+                "        Options to customize the tiles layer created when `tiles` is set,\n",
+                "        e.g. `dict(alpha=0.5)`."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Kind options\n",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Explorer.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Explorer.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285714%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'c5490881-7be7-4095-8983-0b8d9c1e7e4e'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Exploring'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "c5490881-7be7-4095-8983-0b8d9c1e7e4e",
+            "metadata": {},
+            "source": [
+                "# Exploring"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "cb9dcb54",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa\n",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Streaming.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9632165421724246%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'source': ['# Streaming'], delete: ['execution_count', "*

 * *            "'outputs']}, 1: {'source': {insert: [(0, 'hvPlot supports "*

 * *            '[streamz](https://github.com/mrocklin/streamz) DataFrame and Series objects, '*

 * *            'automatically generating streaming plots in a Jupyter notebook or deployed as a '*

 * *            '[Bokeh Server app](https://bokeh.pydata.org/en/latest/docs/user_guide/server.html). '*

 * *            "\\n'), (2, 'All hvPlot methods on stream […]*

```diff
@@ -1,275 +1,247 @@
 {
     "cells": [
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "import xarray as xr\n",
-                "import hvplot.pandas  # noqa\n",
-                "import hvplot.xarray  # noqa\n",
-                "import cartopy.crs as ccrs\n",
-                "\n",
-                "from bokeh.sampledata.airport_routes import airports"
+                "# Streaming"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Installation\n",
-                "\n",
-                "The plot API also has support for geographic data built on top of Cartopy and GeoViews. Both can be installed using conda with:\n",
+                "hvPlot supports [streamz](https://github.com/mrocklin/streamz) DataFrame and Series objects, automatically generating streaming plots in a Jupyter notebook or deployed as a [Bokeh Server app](https://bokeh.pydata.org/en/latest/docs/user_guide/server.html). \n",
                 "\n",
-                "    conda install geoviews\n",
-                "    \n",
-                "or with pip:\n",
+                "All hvPlot methods on streamz objects return HoloViews `DynamicMap` objects that update the plot whenever `streamz` triggers an event. For more information on `DynamicMap` and HoloViews dynamic plotting support, see the [HoloViews User Guide](https://holoviews.org/user_guide); here we will focus on using the simple, high-level hvPlot API rather than on the details of how events and data flow behind the scenes.\n",
                 "\n",
-                "    pip install geoviews\n",
+                "**All plots generated by the streamz plotting interface dynamically stream data from Python into the web browser.  The web version for this page includes *screen captures* of the streaming visualizations, not live streaming data.**\n",
                 "\n",
-                "## Usage\n",
-                "\n",
-                "Only certain hvPlot types support geographic coordinates, currently including: 'points', 'polygons', 'paths', 'image', 'quadmesh', 'contour', and 'contourf'. As an initial example, consider a dataframe of all US airports (including military bases overseas):"
+                "As for any of the data backends, we start by patching the streamz library with the plotting API:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "airports.head(3)"
+                "import hvplot.streamz  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Plotting points\n",
+                "## Basic plotting\n",
                 "\n",
-                "If we want to overlay our data on geographic maps or reproject it into a geographic plot, we can set ``geo=True``, which declares that the data will be plotted in a geographic coordinate system.  The default coordinate system is the ``PlateCarree`` projection, i.e., raw longitudes and latitudes. If the data is in another coordinate system, you will need to [declare an explicit ``crs``](#declaring-a-crs) as an argument, in which case `geo=True` is assumed.  Once hvPlot knows that your data is in geo coordinates, you can use the ``tiles`` option to overlay a the plot on top of map tiles."
+                "Throughout this section we will be using the ``Random`` object from streamz, which provides an easy way of generating a DataFrame of random streaming data but which could be substituted with any streamz ``DataFrame`` or ``Series`` driven by a live, external data source instead. To stop the ``Random`` stream you can call ``df.stop()`` at any point."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "airports.hvplot.points('Longitude', 'Latitude', geo=True, color='red', alpha=0.2,\n",
-                "                       xlim=(-180, -30), ylim=(0, 72), tiles='ESRI')"
+                "from streamz.dataframe import Random\n",
+                "df = Random(interval='200ms', freq='50ms')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Declaring a CRS\n",
-                "\n",
-                "To declare a geographic plot we have to supply a ``cartopy.crs.CRS`` (or coordinate reference system).  Coordinate reference systems are described in the [GeoViews documentation](https://geoviews.org/user_guide/Projections.html) and the full list of available CRSs is in the [cartopy documentation](https://scitools.org.uk/cartopy/docs/v0.15/crs/projections.html). "
+                "<img src='https://assets.holoviews.org/hvplot/gifs/df_streamz.gif' width=400px></img>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Geopandas\n",
-                "\n",
-                "Since a GeoPandas ``DataFrame`` is just a Pandas DataFrames with additional geographic information, it inherits the ``.hvplot`` method. We can thus easily load shapefiles and plot them on a map:"
+                "The plot method on Series and DataFrame is a simple wrapper around a\n",
+                "line plot, which will plot all columns:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import geopandas as gpd\n",
-                "\n",
-                "cities = gpd.read_file(gpd.datasets.get_path('naturalearth_cities'))\n",
-                "\n",
-                "cities.hvplot(global_extent=True, frame_height=450, tiles=True)"
+                "df.hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The GeoPandas support allows plotting ``GeoDataFrames`` containing ``'Point'``, ``'Polygon'``, ``'LineString'`` and ``'LineRing'`` geometries, but not ones containing a mixture of different geometry types. Calling ``.hvplot`` will automatically figure out the geometry type to plot, but it also possible to call ``.hvplot.points``, ``.hvplot.polygons``, and ``.hvplot.paths`` explicitly.\n",
-                "\n",
-                "To draw multiple GeoDataFrames onto the same plot, use the ``*`` operator:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "world = gpd.read_file(gpd.datasets.get_path('naturalearth_lowres'))\n",
-                "\n",
-                "world.hvplot(geo=True) * cities.hvplot(geo=True, color='orange')"
+                "<center><img src='https://assets.holoviews.org/hvplot/gifs/df_plot.gif' width=700px></img></center>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "It is possible to declare a specific column to use as color with the ``c`` keyword:"
+                "The plot method can also be called on a Series, plotting a specific column:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "world.hvplot(geo=True) + world.hvplot(c='continent', geo=True)"
+                "df.z.cumsum().hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Spatialpandas\n",
+                "<center><img src='https://assets.holoviews.org/hvplot/gifs/df_curve.gif' width=700px></img></center>\n",
+                "\n",
+                "Actually, *all* the functionality described in the [Plotting](Plotting.ipynb) user guide should work just the same as it does for a regular (non-streaming) dask or pandas DataFrame or Series, but will now update as new data appears.\n",
                 "\n",
-                "Spatialpandas is another powerful library for working with geometries and is optimized for rendering with datashader, making it possible to plot millions of individual geometries very quickly:"
+                "## Controlling the backlog\n",
+                "\n",
+                "The main difference when using a streaming DataFrame is that a only a certain amount of data will be buffered and displayed. The number of rows of data that will be buffered can be controlled by the ``backlog`` parameter. Here, let's buffer and display 10 rows of our streaming DataFrame as a table:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import spatialpandas as spd\n",
-                "\n",
-                "spd_world = spd.GeoDataFrame(world)\n",
-                "\n",
-                "spd_world.hvplot(datashade=True, project=True, aggregator='count_cat', c='continent', color_key='Category10')"
+                "df.hvplot.table(width=400, backlog=10)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Declaring an output projection"
+                "<center><img src='https://assets.holoviews.org/hvplot/gifs/df_table.gif' width=400px></img></center>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The ``crs=`` argument specifies the *input* projection, i.e. it declares how to interpret the incoming data values. You can independently choose any *output* projection, i.e. how you want to map the data points onto the screen for display, using the ``projection=`` argument. After loading the same temperature dataset explored in the [Gridded Data](Gridded_Data.ipynb) section, the data can be displayed on an Orthographic projection:"
+                "This of course only has an effect when we are directly streaming data point by point. When we have an aggregate DataFrame, the plot will continuously accumulate updates:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "air_ds = xr.tutorial.open_dataset('air_temperature').load()\n",
-                "\n",
-                "air_ds.hvplot.quadmesh(\n",
-                "    'lon', 'lat', 'air', projection=ccrs.Orthographic(-90, 30),\n",
-                "    global_extent=True, frame_height=540, cmap='viridis',\n",
-                "    coastline=True\n",
-                ")"
+                "df.groupby('y').sum().hvplot.bar(x='y')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If you don't need to pass any keyword arguments to a given projection and you don't have cartopy.crs (ccrs) imported, you can use the string representation: e.g. ``'LambertConformal'`` instead of ``ccrs.LambertConformal()``. Note that it is case sensitive!"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "air_ds.hvplot.quadmesh(\n",
-                "    'lon', 'lat', 'air', projection='LambertConformal',\n",
-                ")"
+                "<center><img src='https://assets.holoviews.org/hvplot/gifs/df_bars.gif' width=700px></img></center>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note that when displaying raster data in a projection other than the one in which the data is stored, it is more accurate to render it as a ``quadmesh`` rather than an ``image``. As you can see above, a QuadMesh will project each original bin or pixel into the correct non-rectangular shape determined by the projection, accurately showing the geographic extent covered by each sample. An Image, on the other hand, will always be rectangularly aligned in the 2D plane, which requires warping and resampling the data in a way that allows efficient display but loses accuracy at the pixel level. Unfortunately, rendering a large QuadMesh using Bokeh can be very slow, but there are two useful alternatives for datasets too large to be practical as native QuadMeshes.\n",
-                "\n",
-                "The first is using the ``rasterize`` or ``datashade`` options to regrid the data before rendering it, i.e., rendering the data on the backend and then sending a more efficient image-based representation to the browser. One thing to note when using these operations is that it may be necessary to project the data **before** rasterizing it, e.g. to address wrapping issues. To do this provide ``project=True``, which will project the data before it is rasterized (this also works for other types and even when not using these operations). Another reason why this is important when rasterizing the data is that if the CRS of the data does not match the displayed projection, all the data will be projected every time you zoom or pan, which can be very slow. Deciding whether to ``project`` is therefore a tradeoff between projecting the raw data ahead of time or accepting the overhead on dynamic zoom and pan actions."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "rasm = xr.tutorial.open_dataset('rasm').load()\n",
+                "## Composing Plots\n",
                 "\n",
+                "hvPlot is a convenient API for generating HoloViews objects. One of the core strengths of HoloViews objects is the ease with which they can be composed, which works with streaming plots just as with static ones. Individual plots can be composed using the ``*`` and ``+`` operators, which overlay and compose plots into layouts respectively. For more information on composing objects see the HoloViews [User Guide](https://holoviews.org/user_guide/Composing_Elements.html).\n",
                 "\n",
-                "\n",
-                "rasm.hvplot.quadmesh(\n",
-                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.PlateCarree(),\n",
-                "    ylim=(0, 90), cmap='viridis', project=True, geo=True,\n",
-                "    rasterize=True, coastline=True, frame_width=800, dynamic=False,\n",
-                ")"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Another option that's still relatively slow for larger data but avoids sending large data into your browser is to plot the data using ``contour`` and ``contourf`` visualizations, generating a line or filled contour with a discrete number of levels:"
+                "By using these operators we can combine multiple plots into composite Overlay and Layout objects, and lay them out in two columns using the ``Layout.cols`` method:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rasm.hvplot.contourf(\n",
-                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.PlateCarree(),\n",
-                "    ylim=(0, 90), frame_width=800, cmap='viridis', levels=10,\n",
-                "    coastline=True\n",
-                ")"
+                "(df.hvplot.line(width=400, backlog=100) * df.hvplot.scatter(width=400, backlog=100) +\n",
+                " df.groupby('y').sum().hvplot.bar('y', 'x', width=400) +\n",
+                " df.hvplot.box(width=400) + df.x.hvplot.kde(width=400, shared_axes=False)).cols(2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "As you can see, hvPlot makes it simple to work with geographic data visually.  For more complex plot types and additional details, see the [GeoViews](https://geoviews.org) documentation."
+                "<center><img src='https://assets.holoviews.org/hvplot/gifs/df_composite.gif' width=700px></img></center>"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Geographic options\n",
+                "## Deployment as Bokeh apps\n",
+                "\n",
+                "HoloViews objects automatically render themselves in Jupyter notebook cells, but when deploying a bokeh app the plot has to be rendered explicitly. Deploying as a Bokeh Server app allows you to share live, dynamically updated visualizations like those for streaming data, backed by a running Python process.\n",
+                "\n",
+                "The following example describes how to set up a streaming DataFrame, declare some plots, compose them, set up a callback to update the plot and finally convert the composite plot to a bokeh Document, which can be served from a script using ``bokeh serve`` on the commandline.\n",
+                "\n",
+                "```python\n",
+                "\n",
+                "import numpy as np\n",
+                "import pandas as pd\n",
+                "import hvplot.streamz\n",
+                "import holoviews as hv\n",
+                "\n",
+                "from streamz import Stream\n",
+                "from streamz.dataframe import DataFrame\n",
+                "\n",
+                "renderer = hv.renderer('bokeh')\n",
+                "\n",
+                "# Set up streaming DataFrame\n",
+                "stream = Stream()\n",
+                "index = pd.DatetimeIndex([])\n",
+                "example = pd.DataFrame({'x': [], 'y': [], 'z': []},\n",
+                "                       columns=['x', 'y', 'z'], index=[])\n",
+                "df = DataFrame(stream, example=example)\n",
+                "cumulative = df.cumsum()[['x', 'z']]\n",
+                "\n",
+                "# Declare plots\n",
+                "line = cumulative.hvplot.line(width=400)\n",
+                "scatter = cumulative.hvplot.scatter(width=400)\n",
+                "bars = df.groupby('y').sum().hvplot.bar(width=400)\n",
+                "box = df.hvplot.box(width=400)\n",
+                "kde = df.x.hvplot.kde(width=400)\n",
+                "\n",
+                "# Compose plots\n",
+                "layout = (line * scatter + bars + box + kde).cols(2)\n",
+                "\n",
+                "# Set up callback with streaming data\n",
+                "def emit():\n",
+                "    now = pd.datetime.now()\n",
+                "    delta = np.timedelta64(500, 'ms')\n",
+                "    index = pd.date_range(np.datetime64(now)-delta, now, freq='100ms')\n",
+                "    df = pd.DataFrame({'x': np.random.randn(len(index)),\n",
+                "                       'y': np.random.randint(0, 10, len(index)),\n",
+                "                       'z': np.random.randn(len(index))},\n",
+                "                      columns=['x', 'y', 'z'], index=index)\n",
+                "    stream.emit(df)\n",
+                "\n",
+                "# Render layout to bokeh server Document and attach callback\n",
+                "doc = renderer.server_doc(layout)\n",
+                "doc.title = 'Streamz HoloViews based Plotting API Bokeh App Demo'\n",
+                "doc.add_periodic_callback(emit, 500)\n",
+                "```\n",
+                "\n",
+                "For more details on deploying Bokeh apps see the HoloViews [User Guide](https://holoviews.org/user_guide/Deploying_Bokeh_Apps.html).\n",
                 "\n",
-                "The API provides various geo-specific options:\n",
+                "## Using HoloViews directly\n",
                 "\n",
-                "- ``coastline`` (default=False): Whether to display a coastline on top of the plot, setting ``coastline='10m'/'50m'/'110m'`` specifies a specific scale\n",
-                "- ``crs`` (default=None): Coordinate reference system of the data specified as Cartopy CRS object, proj.4 string or EPSG code\n",
-                "- ``features`` features (default=None): A list of features or a dictionary of features and the scale at which to render it. Available features include 'borders', 'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'. Available scales include '10m'/'50m'/'110m'.\n",
-                "- ``geo`` (default=False): Whether the plot should be treated as geographic (and assume PlateCarree, i.e. lat/lon coordinates)\n",
-                "- ``global_extent`` (default=False): Whether to expand the plot extent to span the whole globe\n",
-                "- ``project`` (default=False): Whether to project the data before plotting (adds initial overhead but avoids projecting data when plot is dynamically updated)\n",
-                "- ``tiles`` (default=False): Whether to overlay the plot on a tile source. Tiles sources can be selected by name, the default is 'Wikipedia'.\n",
-                "Other options are: 'CartoDark', 'CartoEco', 'CartoLight', 'CartoMidnight', 'EsriImagery', 'EsriNatGeo', 'EsriReference''EsriTerrain', 'EsriUSATopo', 'OSM', 'StamenLabels', 'StamenTerrain', 'StamenTerrainRetina', 'StamenToner', 'StamenTonerBackground', 'StamenWatercolor'. Stamen tile sources require a Stadia account when not running locally; see [stadiamaps.com](https://stadiamaps.com/)."
+                "HoloViews itself includes first class support for streamz DataFrame and Series; for more details see the [Streaming Data section](https://holoviews.org/user_guide/Streaming_Data.html) in the HoloViews documentation."
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Gridded_Data.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Gridded_Data.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285714%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Gridded Data'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Gridded Data"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "hvPlot provides one API to explore data of many different types. Previous sections have exclusively worked with tabular data stored in pandas (or pandas-like) DataFrames. The other most common type of data are n-dimensional arrays. hvPlot aims to eventually support different array libraries but for now focuses on [xarray](https://xarray.pydata.org/en/stable/). XArray provides a convenient and very powerful wrapper to label the axis and coordinates of multi-dimensional (n-D) arrays. This user guide will cover how to leverage ``xarray`` and ``hvplot`` to visualize and explore data of different dimensionality ranging from simple 1D data, to 2D image-like data, to multi-dimensional cubes of data.\n",
                 "\n",
                 "For these examples we\u2019ll use the North American air temperature dataset:"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Integrations.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Integrations.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978070175438596%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'a229bf0b-97ba-41ca-b68f-3011ca82198d'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Integrations'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "a229bf0b-97ba-41ca-b68f-3011ca82198d",
+            "metadata": {},
+            "source": [
+                "# Integrations"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "42ebab2c-ee59-4157-9b01-c1bb7988b407",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import numpy as np\n",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Interactive.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Interactive.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Interactive'])]))]}"}*

```diff
@@ -1,10 +1,17 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Interactive"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import ipywidgets as ipw\n",
                 "import hvplot.xarray # noqa\n",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Introduction.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Introduction.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555556%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Introduction'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Introduction"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "The PyData ecosystem has a number of core Python data containers that allow users to work with a wide array of datatypes, including:\n",
                 "\n",
                 "* [Pandas](https://pandas.pydata.org): DataFrame, Series (columnar/tabular data)\n",
                 "* [Rapids cuDF](https://docs.rapids.ai/api/cudf/stable/): GPU DataFrame, Series (columnar/tabular data)\n",
                 "* [Polars](https://www.pola.rs/): Polars is a fast DataFrame library/in-memory query engine (columnar/tabular data)\n",
                 "* [Dask](https://www.dask.org): DataFrame, Series (distributed/out of core arrays and columnar data)\n",
                 "* [XArray](https://xarray.pydata.org): Dataset, DataArray (labelled multidimensional arrays)\n",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/NetworkX.ipynb` & `hvplot-0.9.3a1/doc/user_guide/NetworkX.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971590909090909%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# NetworkX'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# NetworkX"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "The hvPlot NetworkX plotting API is meant as a drop-in replacement for the ``networkx.draw`` methods. In most cases the existing code will work as is or with minor modifications, returning a HoloViews object rendering an interactive bokeh plot, equivalent to the matplotlib plot the standard API constructs. First let us import the plotting interface and give it the canonical name ``hvnx``:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Pandas_API.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Pandas_API.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988636363636364%*

 * *Differences: {"'cells'": "{74: {'source': ['import pandas as pd\\n', 'import numpy as np']}, insert: [(0, "*

 * *            "OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Pandas API'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Pandas API"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "If hvplot and pandas are both installed, then we can use the pandas.options.plotting.backend to control the output of `pd.DataFrame.plot` and `pd.Series.plot`. This notebook is meant to recreate the [pandas visualization docs](https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -679,15 +686,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import pandas as pd, numpy as np"
+                "import pandas as pd\n",
+                "import numpy as np"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Plotting.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Plotting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981428571428572%*

 * *Differences: {"'cells'": '{25: {\'source\': {insert: [(0, "delay_min_max = flights.groupby([\'day\', '*

 * *            "'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', "*

 * *            '\'max\'])\\n")], delete: [0]}}, insert: [(0, OrderedDict([(\'cell_type\', '*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['# Plotting'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Plotting"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "As we discovered in the [Introduction](Introduction.ipynb), HoloViews allows plotting a variety of data types. Here we will use the sample data module and load the pandas and dask hvPlot API:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -231,15 +238,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg({'min': np.min, 'max': np.max})\n",
+                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', 'max'])\n",
                 "delay_mean = flights.groupby('day')['carrier_delay'].mean()\n",
                 "\n",
                 "delay_min_max.hvplot.area(x='day', y='min', y2='max', alpha=0.2) * delay_mean.hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Plotting_Extensions.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945652173913043%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('id', "*

 * *            "'94918367-ea66-4bc4-9913-c704f45686ee'), ('metadata', OrderedDict()), ('source', ['# "*

 * *            "Plotting Extensions'])]))]}"}*

```diff
@@ -1,10 +1,18 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "id": "94918367-ea66-4bc4-9913-c704f45686ee",
+            "metadata": {},
+            "source": [
+                "# Plotting Extensions"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "id": "2ce662e1",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from hvplot.sample_data import us_crime"
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982191780821918%*

 * *Differences: {"'cells'": '{25: {\'source\': {insert: [(0, "delay_min_max = flights.groupby([\'day\', '*

 * *            "'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', "*

 * *            '\'max\'])\\n")], delete: [0]}}, insert: [(0, OrderedDict([(\'cell_type\', '*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['# Plotting with "*

 * *            "Matplotlib'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Plotting with Matplotlib"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "This page demonstrates the use of the **Matplotlib** plotting backend, the equivalent page demonstrating the Plotly backend may be found [here](Plotting_with_Plotly.ipynb)\n",
                 "\n",
                 "As we discovered in the [Introduction](Introduction.ipynb), HoloViews allows plotting a variety of data types. Here we will use the sample data module and load the pandas and dask hvPlot API:"
             ]
         },
         {
             "cell_type": "code",
@@ -235,15 +242,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg({'min': np.min, 'max': np.max})\n",
+                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', 'max'])\n",
                 "delay_mean = flights.groupby('day')['carrier_delay'].mean()\n",
                 "\n",
                 "delay_min_max.hvplot.area(x='day', y='min', y2='max', alpha=0.2) * delay_mean.hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Plotting_with_Plotly.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982191780821918%*

 * *Differences: {"'cells'": '{26: {\'source\': {insert: [(0, "delay_min_max = flights.groupby([\'day\', '*

 * *            "'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', "*

 * *            '\'max\'])\\n")], delete: [0]}}, insert: [(0, OrderedDict([(\'cell_type\', '*

 * *            "'markdown'), ('metadata', OrderedDict()), ('source', ['# Plotting with Plotly'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Plotting with Plotly"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "This page demonstrates the use of the **Plotly** plotting backend, the equivalent page demonstrating the Matplotlib backend may be found [here](Plotting_with_Matplotlib.ipynb)\n",
                 "\n",
                 "As we discovered in the [Introduction](Introduction.ipynb), HoloViews allows plotting a variety of data types. Here we will use the sample data module and load the pandas and dask hvPlot API:"
             ]
         },
         {
             "cell_type": "code",
@@ -242,15 +249,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg({'min': np.min, 'max': np.max})\n",
+                "delay_min_max = flights.groupby(['day', 'carrier'])['carrier_delay'].mean().groupby('day').agg(['min', 'max'])\n",
                 "delay_mean = flights.groupby('day')['carrier_delay'].mean()\n",
                 "\n",
                 "delay_min_max.hvplot.area(x='day', y='min', y2='max', alpha=0.2) * delay_mean.hvplot()"
             ]
         },
         {
             "cell_type": "markdown",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Statistical_Plots.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Statistical_Plots.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Statistical Plots'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Statistical Plots"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "In addition to the plots available via the plot interface, hvPlot makes a number of more sophisticated, statistical plots available that are modelled on ``pandas.plotting``. To explore these, we will load the iris and stocks datasets from Bokeh:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Subplots.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Subplots.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Subplots'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Subplots"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Subplots\n",
                 "\n",
                 "When plotting multiple columns, hvPlot will overlay the plots onto one axis by default so that they can be compared easily in a compact format:"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Timeseries_Data.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Timeseries_Data.ipynb`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9888392857142857%*

 * *Differences: {"'cells'": "{22: {'source': {insert: [(0, '### Working with Large Timeseries\\n'), (2, 'Working "*

 * *            'with large timeseries presents new visualization challenges. Consult our [Large '*

 * *            "Timeseries User Guide](Large_Timeseries.ipynb) to learn about various approaches.')], "*

 * *            "delete: [4, 2, 1, 0]}}, insert: [(0, OrderedDict([('cell_type', 'markdown'), "*

 * *            "('metadata', OrderedDict()), ('source', ['# Timeseries Data'])]))], delete: [22]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Timeseries Data"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "Almost all the other sections in the user guide mention timeseries. This section demonstrates the special functionality that hvPlot provides specifically for dealing with time. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
@@ -188,28 +195,17 @@
                 "Note that xarray supports grouping and aggregation using a similar syntax. To learn more about timeseries in xarray, see the [xarray timeseries docs](https://xarray.pydata.org/en/stable/time-series.html)."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Downsample time series\n",
-                "\n",
-                "*(Available with HoloViews >= 1.16)*\n",
+                "### Working with Large Timeseries\n",
                 "\n",
-                "An option when working with large time series is to downsample the data before plotting it. This can be done with `downsample=True`, which applies the `lttb` (Largest Triangle Three Buckets) algorithm to the data."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "sst.hvplot(label=\"original\") * sst.hvplot(downsample=True, label=\"downsampled\")"
+                "Working with large timeseries presents new visualization challenges. Consult our [Large Timeseries User Guide](Large_Timeseries.ipynb) to learn about various approaches."
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Viewing.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Viewing.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99375%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Viewing'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Viewing"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "hvPlot is written to work well inside a Jupyter notebook, from the interactive Python command prompt, or inside a Python batch script. In this user guide we will discover how to use hvPlot to view plots in each of these cases and how to save the plots to a separate file."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/Widgets.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Widgets.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926470588235294%*

 * *Differences: {"'cells'": "{insert: [(0, OrderedDict([('cell_type', 'markdown'), ('metadata', OrderedDict()), "*

 * *            "('source', ['# Widgets'])]))]}"}*

```diff
@@ -1,13 +1,20 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "# Widgets"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "As we have seen in previous sections, hvPlot bakes in interactivity by automatically creating widgets when using ``groupby``. These widgets can be refined using [Panel](https://panel.holoviz.org). Panel allows you to customize the interactivity of your hvPlot output and provides more fine-grained control over the layout."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `hvplot-0.9.2rc1/examples/user_guide/images/simple.svg` & `hvplot-0.9.3a1/doc/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.9.2rc1/hvplot/__init__.py` & `hvplot-0.9.3a1/hvplot/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,55 +53,95 @@
 
 - `help` and `?` will provide you with documentation.
 - `TAB` and `SHIFT+TAB` completion will help you navigate.
 
 To ask the community go to https://discourse.holoviz.org/.
 To report issues go to https://github.com/holoviz/holoviews.
 """
+
 import inspect
+import os
 import textwrap
 
-import param
 import panel as _pn
 import holoviews as _hv
 
 from holoviews import Store, render  # noqa
 
 from .converter import HoloViewsConverter
 from .interactive import Interactive
 from .ui import explorer  # noqa
-from .utilities import hvplot_extension, output, save, show # noqa
-from .plotting import (hvPlot, hvPlotTabular,  # noqa
-                       andrews_curves, lag_plot,
-                       parallel_coordinates, scatter_matrix, plot)
-
-__version__ = str(param.version.Version(fpath=__file__, archive_commit="$Format:%h$",
-                                        reponame="hvplot"))
+from .utilities import hvplot_extension, output, save, show  # noqa
+from .plotting import (
+    hvPlot,
+    hvPlotTabular,  # noqa
+    andrews_curves,  # noqa
+    lag_plot,  # noqa
+    parallel_coordinates,  # noqa
+    scatter_matrix,  # noqa
+    plot,  # noqa
+)
+
+# Define '__version__'
+try:
+    # For performance reasons on imports, avoid importing setuptools_scm
+    # if not in a .git folder
+    if os.path.exists(os.path.join(os.path.dirname(__file__), '..', '.git')):
+        # If setuptools_scm is installed (e.g. in a development environment with
+        # an editable install), then use it to determine the version dynamically.
+        from setuptools_scm import get_version
+
+        # This will fail with LookupError if the package is not installed in
+        # editable mode or if Git is not installed.
+        __version__ = get_version(root='..', relative_to=__file__)
+    else:
+        raise FileNotFoundError
+except (ImportError, LookupError, FileNotFoundError):
+    # As a fallback, use the version that is hard-coded in the file.
+    try:
+        # __version__ was added in _version in setuptools-scm 7.0.0, we rely on
+        # the hopefully stable version variable.
+        from ._version import version as __version__
+    except (ModuleNotFoundError, ImportError):
+        # Either _version doesn't exist (ModuleNotFoundError) or version isn't
+        # in _version (ImportError). ModuleNotFoundError is a subclass of
+        # ImportError, let's be explicit anyway.
+
+        # Try something else:
+        from importlib.metadata import version as mversion, PackageNotFoundError
+
+        try:
+            __version__ = mversion('hvplot')
+        except PackageNotFoundError:
+            # The user is probably trying to run this without having installed
+            # the package.
+            __version__ = '0.0.0+unknown'
 
 _METHOD_DOCS = {}
 
+
 def _get_doc_and_signature(
     cls, kind, completions=False, docstring=True, generic=True, style=True, signature=None
 ):
     converter = HoloViewsConverter
     method = getattr(cls, kind)
     kind_opts = converter._kind_options.get(kind, [])
     eltype = converter._kind_mapping[kind]
 
     formatter = ''
     if completions:
-        formatter = "hvplot.{kind}({completions})"
+        formatter = 'hvplot.{kind}({completions})'
     if docstring:
         if formatter:
             formatter += '\n'
-        formatter += "{docstring}"
+        formatter += '{docstring}'
     if generic:
         if formatter:
             formatter += '\n'
-        formatter += "{options}"
+        formatter += '{options}'
 
     # Bokeh is the default backend
     backend = hvplot_extension.compatibility or Store.current_backend
     if eltype in Store.registry[backend]:
         valid_opts = Store.registry[backend][eltype].style_opts
         if style:
             formatter += '\n{style}'
@@ -116,31 +156,41 @@
     )
 
     sig = signature or inspect.signature(method)
     for name, p in list(sig.parameters.items())[1:]:
         if p.kind == 1:
             parameters.append((name, p.default))
 
-    filtered_signature = [p for p in sig.parameters.values()
-                            if p.kind != inspect.Parameter.VAR_KEYWORD]
-    extra_params = [inspect.Parameter(k, inspect.Parameter.KEYWORD_ONLY)
-                    for k in extra_kwargs
-                    if k not in [p.name for p in filtered_signature]]
-    all_params = (filtered_signature + extra_params
-                    + [inspect.Parameter('kwargs', inspect.Parameter.VAR_KEYWORD)])
+    filtered_signature = [
+        p for p in sig.parameters.values() if p.kind != inspect.Parameter.VAR_KEYWORD
+    ]
+    extra_params = [
+        inspect.Parameter(k, inspect.Parameter.KEYWORD_ONLY)
+        for k in extra_kwargs
+        if k not in [p.name for p in filtered_signature]
+    ]
+    all_params = (
+        filtered_signature
+        + extra_params
+        + [inspect.Parameter('kwargs', inspect.Parameter.VAR_KEYWORD)]
+    )
     signature = inspect.Signature(all_params)
 
     parameters += [(o, None) for o in extra_kwargs]
     completions = ', '.join([f'{n}={v}' for n, v in parameters])
     options = textwrap.dedent(converter.__doc__)
     method_doc = _METHOD_DOCS.get(kind, method.__doc__)
     _METHOD_DOCS[kind] = method_doc
     docstring = formatter.format(
-        kind=kind, completions=completions, docstring=textwrap.dedent(method_doc),
-        options=options, style=style_opts)
+        kind=kind,
+        completions=completions,
+        docstring=textwrap.dedent(method_doc),
+        options=options,
+        style=style_opts,
+    )
     return docstring, signature
 
 
 def help(kind=None, docstring=True, generic=True, style=True):
     """
     Provide a docstring with all valid options which apply to the plot
     type.
@@ -152,16 +202,17 @@
     docstring: boolean (default=True)
         Whether to display the docstring
     generic: boolean (default=True)
         Whether to provide list of generic options
     style: boolean (default=True)
         Whether to provide list of style options
     """
-    doc, sig = _get_doc_and_signature(cls=hvPlot, kind=kind,
-                                      docstring=docstring, generic=generic, style=style)
+    doc, sig = _get_doc_and_signature(
+        cls=hvPlot, kind=kind, docstring=docstring, generic=generic, style=style
+    )
     print(doc)
 
 
 def post_patch(extension='bokeh', logo=False):
     if extension and not getattr(_hv.extension, '_loaded', False):
         hvplot_extension(extension, logo=logo)
 
@@ -170,15 +221,14 @@
     method = getattr(cls, kind)
     docstring, signature = _get_doc_and_signature(cls, kind, False, signature=signature)
     method.__doc__ = docstring
     method.__signature__ = signature
 
 
 class _PatchHvplotDocstrings:
-
     def __init__(self):
         # Store the original signatures because the method signatures
         # are going to be patched every time an extension is changed.
         signatures = {}
         for cls in [hvPlot, hvPlotTabular]:
             for _kind in HoloViewsConverter._kind_mapping:
                 if hasattr(cls, _kind):
@@ -194,24 +244,28 @@
                     signature = self.orig_signatures[(cls, _kind)]
                     _patch_doc(cls, _kind, signature=signature)
 
 
 _patch_hvplot_docstrings = _PatchHvplotDocstrings()
 _patch_hvplot_docstrings()
 
+
 def _hook_patch_docstrings(backend):
     # Patch or re-patch the docstrings/signatures to display
     # the right styling options.
     from . import _patch_hvplot_docstrings
+
     _patch_hvplot_docstrings()
 
+
 Store._backend_switch_hooks.append(_hook_patch_docstrings)
 
 extension = hvplot_extension
 
+
 def bind(function, *args, **kwargs):
     """
     Returns a *reactive* function that can be used to start your `.interactive` pipeline by running
     a model or loading data depending on inputs from widgets, parameters or python objects.
 
     The widgets can be Panel or ipywidgets.
```

### Comparing `hvplot-0.9.2rc1/hvplot/backend_transforms.py` & `hvplot-0.9.3a1/hvplot/backend_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 """
 Set of transforms to go from a Bokeh option to another backend's option.
 """
+
 from holoviews.core.overlay import CompositeOverlay
 from holoviews.core.options import Store
 from holoviews.plotting.util import COLOR_ALIASES
 
 
 UNSET = type('UNSET', (), {})
 
 
 def _transform_size_to_mpl(width, height, aspect):
     opts = {}
     if width and height:
-        opts = {'aspect': width/height, 'fig_size': (width/300.)*100}
+        opts = {'aspect': width / height, 'fig_size': (width / 300.0) * 100}
     elif aspect and width:
-        opts = {'aspect': aspect, 'fig_size': (width/300.)*100}
+        opts = {'aspect': aspect, 'fig_size': (width / 300.0) * 100}
     elif aspect and height:
-        opts = {'aspect': aspect, 'fig_size': (height/300.)*100}
+        opts = {'aspect': aspect, 'fig_size': (height / 300.0) * 100}
     elif width:
-        opts = {'fig_size': (width/300.)*100}
+        opts = {'fig_size': (width / 300.0) * 100}
     elif height:
-        opts = {'fig_size': (height/300.)*100}
+        opts = {'fig_size': (height / 300.0) * 100}
     return opts
 
 
 def _transfer_opts(element, backend):
     """
     Transfer the bokeh options of an element to another backend
     based on an internal mapping of option transforms.
     """
     elname = type(element).__name__
     options = Store.options(backend=backend)
     transforms = BACKEND_TRANSFORMS[backend]
     if isinstance(element, CompositeOverlay):
-        element = element.apply(
-            _transfer_opts, backend=backend, per_element=True
-        )
+        element = element.apply(_transfer_opts, backend=backend, per_element=True)
     new_opts = {}
     el_options = element.opts.get(backend='bokeh', defaults=False).kwargs
     for grp, el_opts in options[elname].groups.items():
         for opt, val in el_options.items():
             transform = transforms.get(grp, {}).get(opt, None)
             # This condition could be applied to matplotlib only
             # but is applied to plotly too since there seems to be
@@ -53,16 +52,15 @@
                 if val is UNSET:
                     continue
             if opt not in el_opts.allowed_keywords:
                 continue
             new_opts[opt] = val
     if backend == 'matplotlib':
         size_opts = _transform_size_to_mpl(
-            el_options.get('width'), el_options.get('height'),
-            el_options.get('aspect')
+            el_options.get('width'), el_options.get('height'), el_options.get('aspect')
         )
         new_opts.update(size_opts)
     return element.opts(**new_opts, backend=backend)
 
 
 def _is_interactive_opt(bk_opt):
     """
@@ -196,15 +194,18 @@
         'ymarks_visible': UNSET,
         'lower_head': lambda k, v: ('lolims', v),
         'upper_head': lambda k, v: ('uplims', v),
         'whisker_color': UNSET,
         'outlier_color': UNSET,
         'text_align': lambda k, v: ('horizontalalignment', v),
         'text_alpha': lambda k, v: ('alpha', v),
-        'text_baseline': lambda k, v: ('verticalalignment', _text_baseline_bk_mpl_mapping.get(v, UNSET)),
+        'text_baseline': lambda k, v: (
+            'verticalalignment',
+            _text_baseline_bk_mpl_mapping.get(v, UNSET),
+        ),
         'text_color': lambda k, v: ('color', v),
         'text_font': UNSET,
         'text_font_size': lambda k, v: ('size', v),
         'text_font_style': UNSET,
         'box_alpha': UNSET,
         'box_cmap': UNSET,
         'box_fill_alpha': UNSET,
@@ -314,15 +315,15 @@
         'color': lambda k, v: (k, COLOR_ALIASES.get(v, v)),
         'fill_color': lambda k, v: ('fillcolor', COLOR_ALIASES.get(v, v)),
         'line_color': lambda k, v: (k, COLOR_ALIASES.get(v, v)),
         'line_dash': lambda k, v: ('dash', _line_dash_bk_plotly_mapping.get(v, UNSET)),
         'line_width': lambda k, v: ('line_width', v),
         'muted_alpha': UNSET,
         'palette': UNSET,
-    }
+    },
 }
 
 
 BACKEND_TRANSFORMS = dict(
     matplotlib=MATPLOTLIB_TRANSFORMS,
     plotly=PLOTLY_TRANSFORMS,
 )
```

### Comparing `hvplot-0.9.2rc1/hvplot/converter.py` & `hvplot-0.9.3a1/hvplot/converter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import difflib
+import sys
 from functools import partial
 
 import param
 import holoviews as hv
 import pandas as pd
 import numpy as np
 import colorcet as cc
@@ -11,34 +12,70 @@
 from holoviews.core.dimension import Dimension
 from holoviews.core.spaces import DynamicMap, HoloMap, Callable
 from holoviews.core.overlay import NdOverlay
 from holoviews.core.options import Store, Cycle, Palette
 from holoviews.core.layout import NdLayout
 from holoviews.core.util import max_range
 from holoviews.element import (
-    Curve, Scatter, Area, Bars, BoxWhisker, Dataset, Distribution,
-    Table, HeatMap, Image, HexTiles, QuadMesh, Bivariate, Histogram,
-    Violin, Contours, Polygons, Points, Path, Labels, RGB, ErrorBars,
-    VectorField, Rectangles, Segments
+    Curve,
+    Scatter,
+    Area,
+    Bars,
+    BoxWhisker,
+    Dataset,
+    Distribution,
+    Table,
+    HeatMap,
+    Image,
+    HexTiles,
+    QuadMesh,
+    Bivariate,
+    Histogram,
+    Violin,
+    Contours,
+    Polygons,
+    Points,
+    Path,
+    Labels,
+    RGB,
+    ErrorBars,
+    VectorField,
+    Rectangles,
+    Segments,
 )
 from holoviews.plotting.bokeh import OverlayPlot, colormap_generator
 from holoviews.plotting.util import process_cmap
 from holoviews.operation import histogram, apply_when
 from holoviews.streams import Buffer, Pipe
 from holoviews.util.transform import dim
 from packaging.version import Version
 from pandas import DatetimeIndex, MultiIndex
 
 from .backend_transforms import _transfer_opts_cur_backend
 from .util import (
-    filter_opts, hv_version, is_tabular, is_series, is_dask, is_intake, is_cudf,
-    is_streamz, is_ibis, is_xarray, is_xarray_dataarray, process_crs,
-    process_intake, process_xarray, check_library, is_geodataframe,
-    process_derived_datetime_xarray, process_derived_datetime_pandas,
+    filter_opts,
+    hv_version,
+    is_tabular,
+    is_series,
+    is_dask,
+    is_intake,
+    is_cudf,
+    is_streamz,
+    is_ibis,
+    is_xarray,
+    is_xarray_dataarray,
+    process_crs,
+    process_intake,
+    process_xarray,
+    check_library,
+    is_geodataframe,
+    process_derived_datetime_xarray,
+    process_derived_datetime_pandas,
     _convert_col_names_to_str,
+    import_datashader,
 )
 from .utilities import hvplot_extension
 
 renderer = hv.renderer('bokeh')
 
 
 class StreamingCallable(Callable):
@@ -50,16 +87,15 @@
     periodic = param.Parameter()
 
     def clone(self, callable=None, **overrides):
         """
         Allows making a copy of the Callable optionally overriding
         the callable and other parameters.
         """
-        old = {k: v for k, v in self.param.get_param_values()
-               if k not in ['callable', 'name']}
+        old = {k: v for k, v in self.param.get_param_values() if k not in ['callable', 'name']}
         params = dict(old, **overrides)
         callable = self.callable if callable is None else callable
         return self.__class__(callable, **params)
 
     def start(self):
         """
         Start the periodic callback
@@ -82,14 +118,16 @@
 class HoloViewsConverter:
     """
     Generic options
     ---------------
     autorange (default=None): Literal['x', 'y'] | None
         Whether to enable auto-ranging along the x- or y-axis when
         zooming. Requires HoloViews >= 1.16.
+    bgcolor (default=None): str
+        Background color of the data area of the plot
     clim: tuple
         Lower and upper bound of the color scale
     cnorm (default='linear'): str
         Color scaling which must be one of 'linear', 'log' or 'eq_hist'
     colorbar (default=False): boolean
         Enables a colorbar
     fontscale: number
@@ -140,14 +178,20 @@
         `cnorm!=`eq_hist`.
     responsive: boolean
         Whether the plot should responsively resize depending on the
         size of the browser. Responsive mode will only work if at
         least one dimension of the plot is left undefined, e.g. when
         width and height or width and aspect are set the plot is set
         to a fixed size, ignoring any responsive option.
+    robust: bool
+        If True and clim are absent, the colormap range is computed
+        with 2nd and 98th percentiles instead of the extreme values
+        for image elements. For RGB elements, clips the "RGB", or
+        raw reflectance values between 2nd and 98th percentiles.
+        Follows the same logic as xarray's robust option.
     rot: number
         Rotates the axis ticks along the x-axis by the specified
         number of degrees.
     shared_axes (default=True): boolean
         Whether to link axes between plots
     transforms (default={}): dict
         A dictionary of HoloViews dim transforms to apply before plotting
@@ -196,17 +240,36 @@
         (warning: for large groupby operations embedded data can become
         very large if dynamic=False)
     datashade (default=False):
         Whether to apply rasterization and shading (colormapping) using
         the Datashader library, returning an RGB object instead of
         individual points
     downsample (default=False):
-        Whether to apply LTTB (Largest Triangle Three Buckets)
-        downsampling to the element (note this is only well behaved for
-        timeseries data). Requires HoloViews >= 1.16.
+        Controls the application of downsampling to the plotted data,
+        which is particularly useful for large timeseries datasets to
+        reduce the amount of data sent to browser and improve
+        visualization performance. Requires HoloViews >= 1.16. Additional
+        dependencies: Installing the `tsdownsample` library is required
+        for using any downsampling methods other than the default 'lttb'.
+        Acceptable values:
+        - False: No downsampling is applied.
+        - True: Applies downsampling using HoloViews' default algorithm
+            (LTTB - Largest Triangle Three Buckets).
+        - 'lttb': Explicitly applies the Largest Triangle Three Buckets
+          algorithm.
+        - 'minmax': Applies the MinMax algorithm, selecting the minimum
+          and maximum values in each bin. Requires `tsdownsample`.
+        - 'm4': Applies the M4 algorithm, selecting the minimum, maximum,
+          first, and last values in each bin. Requires `tsdownsample`.
+        - 'minmax-lttb': Combines MinMax and LTTB algorithms for
+          downsampling, first applying MinMax to reduce to a preliminary
+          set of points, then LTTB for further reduction. Requires
+          `tsdownsample`.
+        Other string values corresponding to supported algorithms in
+        HoloViews may also be used.
     dynspread (default=False):
         For plots generated with datashade=True or rasterize=True,
         automatically increase the point size when the data is sparse
         so that individual points become more visible
     rasterize (default=False):
         Whether to apply rasterization using the Datashader library,
         returning an aggregated Image (to be colormapped by the
@@ -220,16 +283,18 @@
 
     Geographic options
     ------------------
     coastline (default=False):
         Whether to display a coastline on top of the plot, setting
         coastline='10m'/'50m'/'110m' specifies a specific scale.
     crs (default=None):
-        Coordinate reference system of the data specified as Cartopy
-        CRS object, proj.4 string or EPSG code.
+        Coordinate reference system of the data specified as a string
+        or integer EPSG code, a CRS or Proj pyproj object, a Cartopy
+        CRS object, a WKT string, or a proj.4 string. Defaults to
+        PlateCarree.
     features (default=None): dict or list
         A list of features or a dictionary of features and the scale
         at which to render it. Available features include 'borders',
         'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'.
         Available scales include '10m'/'50m'/'110m'.
     geo (default=False):
         Whether the plot should be treated as geographic (and assume
@@ -240,84 +305,145 @@
         Whether to project the data before plotting (adds initial
         overhead but avoids projecting data when plot is dynamically
         updated).
     projection (default=None): str or Cartopy CRS
         Coordinate reference system of the plot specified as Cartopy
         CRS object or class name.
     tiles (default=False):
-        Whether to overlay the plot on a tile source. Tiles sources
-        can be selected by name or a tiles object or class can be passed,
-        the default is 'Wikipedia'.
+        Whether to overlay the plot on a tile source:
+        - `True`: OpenStreetMap layer
+        - `xyzservices.TileProvider` instance (requires xyzservices to
+           be installed)
+        - a map string name based on one of the default layers made
+          available by HoloViews or GeoViews.
+        - a `holoviews.Tiles` or `geoviews.WMTS` instance or class
+    tiles_opts (default=None): dict
+        Options to customize the tiles layer created when `tiles` is set,
+        e.g. `dict(alpha=0.5)`.
     """
 
-    _gridded_types = [
-        'image', 'contour', 'contourf', 'quadmesh', 'rgb', 'points',
-        'dataset'
-    ]
+    _gridded_types = ['image', 'contour', 'contourf', 'quadmesh', 'rgb', 'points', 'dataset']
 
     _geom_types = ['paths', 'polygons']
 
-    _geo_types = sorted(_gridded_types + _geom_types + [
-        'points', 'vectorfield', 'labels', 'hexbin', 'bivariate'])
+    _geo_types = sorted(
+        _gridded_types + _geom_types + ['points', 'vectorfield', 'labels', 'hexbin', 'bivariate']
+    )
 
     _stats_types = ['hist', 'kde', 'violin', 'box', 'density']
 
     _data_options = [
-        'x', 'y', 'kind', 'by', 'use_index', 'use_dask', 'dynamic',
-        'crs', 'value_label', 'group_label', 'backlog', 'persist',
-        'sort_date'
+        'x',
+        'y',
+        'kind',
+        'by',
+        'use_index',
+        'use_dask',
+        'dynamic',
+        'crs',
+        'value_label',
+        'group_label',
+        'backlog',
+        'persist',
+        'sort_date',
     ]
 
     _geo_options = [
-        'geo', 'crs', 'features', 'project', 'coastline', 'tiles',
-        'projection', 'global_extents'
+        'geo',
+        'crs',
+        'features',
+        'project',
+        'coastline',
+        'tiles',
+        'projection',
+        'global_extents',
     ]
 
     _axis_options = [
-        'width', 'height', 'shared_axes', 'grid', 'legend',
-        'rot', 'xlim', 'ylim', 'xticks', 'yticks', 'colorbar',
-        'invert', 'title', 'logx', 'logy', 'loglog', 'xaxis',
-        'yaxis', 'xformatter', 'yformatter', 'xlabel', 'ylabel',
-        'clabel', 'padding', 'responsive', 'max_height', 'max_width',
-        'min_height', 'min_width', 'frame_height', 'frame_width',
-        'aspect', 'data_aspect', 'fontscale'
+        'width',
+        'height',
+        'shared_axes',
+        'grid',
+        'legend',
+        'rot',
+        'xlim',
+        'ylim',
+        'xticks',
+        'yticks',
+        'colorbar',
+        'invert',
+        'title',
+        'logx',
+        'logy',
+        'loglog',
+        'xaxis',
+        'yaxis',
+        'xformatter',
+        'yformatter',
+        'xlabel',
+        'ylabel',
+        'clabel',
+        'padding',
+        'responsive',
+        'max_height',
+        'max_width',
+        'min_height',
+        'min_width',
+        'frame_height',
+        'frame_width',
+        'aspect',
+        'data_aspect',
+        'fontscale',
+        'bgcolor',
     ]
 
     _style_options = [
-        'color', 'alpha', 'colormap', 'fontsize', 'c', 'cmap',
-        'color_key', 'cnorm', 'rescale_discrete_levels'
+        'color',
+        'alpha',
+        'colormap',
+        'fontsize',
+        'c',
+        'cmap',
+        'color_key',
+        'cnorm',
+        'rescale_discrete_levels',
     ]
 
     _op_options = [
-        'datashade', 'rasterize', 'x_sampling', 'y_sampling',
-        'downsample', 'aggregator', 'resample_when'
+        'datashade',
+        'rasterize',
+        'x_sampling',
+        'y_sampling',
+        'downsample',
+        'aggregator',
+        'resample_when',
     ]
 
     # Options specific to a particular plot type
     _kind_options = {
-        'area'     : ['y2'],
+        'area': ['y2'],
         'errorbars': ['yerr1', 'yerr2'],
         'bivariate': ['bandwidth', 'cut', 'filled', 'levels'],
-        'contour'  : ['z', 'levels', 'logz'],
-        'contourf' : ['z', 'levels', 'logz'],
-        'dataset'  : ['columns'],
-        'heatmap'  : ['C', 'reduce_function', 'logz'],
-        'hexbin'   : ['C', 'reduce_function', 'gridsize', 'logz', 'min_count'],
-        'hist'     : ['bins', 'bin_range', 'normed', 'cumulative'],
-        'image'    : ['z', 'logz'],
-        'kde'      : ['bw_method', 'ind', 'bandwidth', 'cut', 'filled'],
-        'labels'   : ['text', 'c', 'xoffset', 'yoffset', 'text_font', 'text_font_size'],
-        'ohlc'     : ['bar_width', 'pos_color', 'neg_color', 'line_color'],
-        'points'   : ['s', 'marker', 'c', 'scale', 'logz'],
-        'polygons' : ['logz', 'c'],
-        'rgb'      : ['z', 'bands'],
-        'scatter'  : ['s', 'c', 'scale', 'logz', 'marker'],
-        'step'     : ['where'],
-        'table'    : ['columns'],
-        'quadmesh' : ['z', 'logz'],
+        'contour': ['z', 'levels', 'logz'],
+        'contourf': ['z', 'levels', 'logz'],
+        'dataset': ['columns'],
+        'heatmap': ['C', 'reduce_function', 'logz'],
+        'hexbin': ['C', 'reduce_function', 'gridsize', 'logz', 'min_count'],
+        'hist': ['bins', 'bin_range', 'normed', 'cumulative'],
+        'image': ['z', 'logz'],
+        'kde': ['bw_method', 'ind', 'bandwidth', 'cut', 'filled'],
+        'labels': ['text', 'c', 'xoffset', 'yoffset', 'text_font', 'text_font_size'],
+        'ohlc': ['bar_width', 'pos_color', 'neg_color', 'line_color'],
+        'points': ['s', 'marker', 'c', 'scale', 'logz'],
+        'polygons': ['logz', 'c'],
+        'rgb': ['z', 'bands'],
+        'scatter': ['s', 'c', 'scale', 'logz', 'marker'],
+        'step': ['where'],
+        'table': ['columns'],
+        'quadmesh': ['z', 'logz'],
         'vectorfield': ['angle', 'mag'],
     }
 
     # Mapping from kind to HoloViews element type
     _kind_mapping = {
         'area': Area,
         'bar': Bars,
@@ -342,125 +468,212 @@
         'points': Points,
         'polygons': Polygons,
         'quadmesh': QuadMesh,
         'rgb': RGB,
         'step': Curve,
         'table': Table,
         'vectorfield': VectorField,
-        'violin': Violin
+        'violin': Violin,
     }
 
     # Types which have a colorbar by default
     _colorbar_types = [
-        'bivariate', 'contour', 'contourf', 'heatmap', 'image',
-        'hexbin', 'quadmesh', 'polygons'
+        'bivariate',
+        'contour',
+        'contourf',
+        'heatmap',
+        'image',
+        'hexbin',
+        'quadmesh',
+        'polygons',
     ]
 
     _legend_positions = (
-        "top_right", "top_left", "bottom_left", "bottom_right",
-        "right", "left", "top", "bottom"
+        'top_right',
+        'top_left',
+        'bottom_left',
+        'bottom_right',
+        'right',
+        'left',
+        'top',
+        'bottom',
     )
 
     _default_plot_opts = {
         'logx': False,
         'logy': False,
         'show_legend': True,
         'legend_position': 'right',
         'show_grid': False,
         'responsive': False,
-        'shared_axes': True
+        'shared_axes': True,
     }
 
     _default_cmaps = {
         'linear': 'kbc_r',
         'categorical': cc.palette['glasbey_category10'],
         'cyclic': 'colorwheel',
-        'diverging': 'coolwarm'
+        'diverging': 'coolwarm',
     }
 
     def __init__(
-        self, data, x, y, kind=None, by=None, use_index=True,
-        group_label=None, value_label='value', backlog=1000,
-        persist=False, use_dask=False, crs=None, fields={},
-        groupby=None, dynamic=True, grid=None, legend=None, rot=None,
-        title=None, xlim=None, ylim=None, clim=None, symmetric=None,
-        logx=None, logy=None, loglog=None, hover=None, subplots=False,
-        label=None, invert=False, stacked=False, colorbar=None,
-        datashade=False, rasterize=False, downsample=None,
-        resample_when=None, row=None, col=None,
-        debug=False, framewise=True, aggregator=None,
-        projection=None, global_extent=None, geo=False,
-        precompute=False, flip_xaxis=None, flip_yaxis=None,
-        dynspread=False, hover_cols=[], x_sampling=None,
-        y_sampling=None, project=False, tools=[], attr_labels=None,
-        coastline=False, tiles=False, sort_date=True,
-        check_symmetric_max=1000000, transforms={}, stream=None,
-        cnorm=None, features=None, rescale_discrete_levels=None,
-        autorange=None, **kwds
+        self,
+        data,
+        x,
+        y,
+        kind=None,
+        by=None,
+        use_index=True,
+        group_label=None,
+        value_label='value',
+        backlog=1000,
+        persist=False,
+        use_dask=False,
+        crs=None,
+        fields={},
+        groupby=None,
+        dynamic=True,
+        grid=None,
+        legend=None,
+        rot=None,
+        title=None,
+        xlim=None,
+        ylim=None,
+        clim=None,
+        robust=None,
+        symmetric=None,
+        logx=None,
+        logy=None,
+        loglog=None,
+        hover=None,
+        subplots=False,
+        label=None,
+        invert=False,
+        stacked=False,
+        colorbar=None,
+        datashade=False,
+        rasterize=False,
+        downsample=None,
+        resample_when=None,
+        row=None,
+        col=None,
+        debug=False,
+        framewise=True,
+        aggregator=None,
+        projection=None,
+        global_extent=None,
+        geo=False,
+        precompute=False,
+        flip_xaxis=None,
+        flip_yaxis=None,
+        dynspread=False,
+        hover_cols=[],
+        x_sampling=None,
+        y_sampling=None,
+        project=False,
+        tools=[],
+        attr_labels=None,
+        coastline=False,
+        tiles=False,
+        tiles_opts=None,
+        sort_date=True,
+        check_symmetric_max=1000000,
+        transforms={},
+        stream=None,
+        cnorm=None,
+        features=None,
+        rescale_discrete_levels=None,
+        autorange=None,
+        **kwds,
     ):
         # Process data and related options
         self._redim = fields
         self.use_index = use_index
         self.value_label = value_label
         self.label = label
         self._process_data(
-            kind, data, x, y, by, groupby, row, col, use_dask,
-            persist, backlog, label, group_label, value_label,
-            hover_cols, attr_labels, transforms, stream, kwds
+            kind,
+            data,
+            x,
+            y,
+            by,
+            groupby,
+            row,
+            col,
+            use_dask,
+            persist,
+            backlog,
+            label,
+            group_label,
+            value_label,
+            hover_cols,
+            attr_labels,
+            transforms,
+            stream,
+            robust,
+            kwds,
         )
 
         self.dynamic = dynamic
         self.geo = any([geo, crs, global_extent, projection, project, coastline, features])
         self.crs = self._process_crs(data, crs) if self.geo else None
         self.output_projection = self.crs
         self.project = project
         self.coastline = coastline
         self.features = features
         self.tiles = tiles
+        self.tiles_opts = tiles_opts or {}
         self.sort_date = sort_date
 
         # Import geoviews if geo-features requested
         if self.geo or self.datatype == 'geopandas':
             try:
-                import geoviews # noqa
+                import geoviews  # noqa
             except ImportError:
-                raise ImportError('In order to use geo-related features '
-                                  'the geoviews library must be available. '
-                                  'It can be installed with:\n  conda '
-                                  'install geoviews')
+                raise ImportError(
+                    'In order to use geo-related features '
+                    'the geoviews library must be available. '
+                    'It can be installed with:\n  conda '
+                    'install geoviews'
+                )
         if self.geo:
             if self.kind not in self._geo_types:
                 param.main.param.warning(
-                    f"geo option cannot be used with kind={self.kind!r} plot "
-                    "type. Geographic plots are only supported for "
-                    f"following plot types: {self._geo_types!r}")
+                    f'geo option cannot be used with kind={self.kind!r} plot '
+                    'type. Geographic plots are only supported for '
+                    f'following plot types: {self._geo_types!r}'
+                )
             from cartopy import crs as ccrs
             from geoviews.util import project_extents
 
             if isinstance(projection, str):
-                all_crs = [proj for proj in dir(ccrs) if
-                           callable(getattr(ccrs, proj)) and
-                           proj not in ['ABCMeta', 'CRS'] and
-                           proj[0].isupper() or
-                           proj == 'GOOGLE_MERCATOR']
+                all_crs = [
+                    proj
+                    for proj in dir(ccrs)
+                    if callable(getattr(ccrs, proj))
+                    and proj not in ['ABCMeta', 'CRS']
+                    and proj[0].isupper()
+                    or proj == 'GOOGLE_MERCATOR'
+                ]
                 if projection in all_crs and projection != 'GOOGLE_MERCATOR':
                     projection = getattr(ccrs, projection)()
                 elif projection == 'GOOGLE_MERCATOR':
                     projection = getattr(ccrs, projection)
                 else:
                     raise ValueError(
-                        "Projection must be defined as cartopy CRS or "
-                        f"one of the following CRS string:\n {all_crs}")
+                        'Projection must be defined as cartopy CRS or '
+                        f'one of the following CRS string:\n {all_crs}'
+                    )
 
             self.output_projection = projection or (ccrs.GOOGLE_MERCATOR if tiles else self.crs)
             if tiles and self.output_projection != ccrs.GOOGLE_MERCATOR:
                 raise ValueError(
-                    "Tiles can only be used with output projection of "
-                    "`cartopy.crs.GOOGLE_MERCATOR`. To get rid of this error "
-                    "remove `projection=` or `tiles=`"
+                    'Tiles can only be used with output projection of '
+                    '`cartopy.crs.GOOGLE_MERCATOR`. To get rid of this error '
+                    'remove `projection=` or `tiles=`'
                 )
             if self.crs != projection and (xlim or ylim):
                 px0, py0, px1, py1 = ccrs.GOOGLE_MERCATOR.boundary.bounds
                 x0, x1 = xlim or (px0, px1)
                 y0, y1 = ylim or (py0, py1)
                 extents = (x0, y0, x1, y1)
                 x0, y0, x1, y1 = project_extents(extents, self.crs, self.output_projection)
@@ -493,16 +706,15 @@
         if hvplot_extension.compatibility is None:
             self._backend_compat = self._backend
         else:
             self._backend_compat = hvplot_extension.compatibility
 
         self.stacked = stacked
 
-        plot_opts = dict(self._default_plot_opts,
-                         **self._process_plot())
+        plot_opts = dict(self._default_plot_opts, **self._process_plot())
         if xlim is not None:
             plot_opts['xlim'] = tuple(xlim)
         if ylim is not None:
             plot_opts['ylim'] = tuple(ylim)
 
         if autorange is not None:
             if hv_version < Version('1.16.0'):
@@ -524,35 +736,55 @@
 
         if legend is not None:
             plot_opts['show_legend'] = bool(legend)
 
         if legend in self._legend_positions:
             plot_opts['legend_position'] = legend
         elif legend not in (True, False, None):
-            raise ValueError('The legend option should be a boolean or '
-                             'a valid legend position (i.e. one of %s).'
-                             % list(self._legend_positions))
-        plotwds = ['xticks', 'yticks', 'xlabel', 'ylabel', 'clabel',
-                   'padding', 'xformatter', 'yformatter',
-                   'height', 'width', 'frame_height', 'frame_width',
-                   'min_width', 'min_height', 'max_width', 'max_height',
-                   'fontsize', 'fontscale', 'responsive', 'shared_axes',
-                   'aspect', 'data_aspect']
+            raise ValueError(
+                'The legend option should be a boolean or '
+                'a valid legend position (i.e. one of %s).' % list(self._legend_positions)
+            )
+        plotwds = [
+            'xticks',
+            'yticks',
+            'xlabel',
+            'ylabel',
+            'clabel',
+            'padding',
+            'xformatter',
+            'yformatter',
+            'height',
+            'width',
+            'frame_height',
+            'frame_width',
+            'min_width',
+            'min_height',
+            'max_width',
+            'max_height',
+            'fontsize',
+            'fontscale',
+            'responsive',
+            'shared_axes',
+            'aspect',
+            'data_aspect',
+            'bgcolor',
+        ]
         for plotwd in plotwds:
             if plotwd in kwds:
                 plot_opts[plotwd] = kwds.pop(plotwd)
 
         self._style_opts, plot_opts, kwds = self._process_style(kwds, plot_opts)
 
         for axis_name in ['xaxis', 'yaxis']:
             if axis_name in kwds:
                 axis = kwds.pop(axis_name)
                 if not axis:
                     plot_opts[axis_name] = None
-                elif axis != True:
+                elif not axis:
                     plot_opts[axis_name] = axis
                 elif axis_name in plot_opts:
                     plot_opts.pop(axis_name, None)
 
         if flip_xaxis:
             plot_opts['invert_xaxis'] = True
         if flip_yaxis:
@@ -582,72 +814,119 @@
 
         tools = list(tools) or list(plot_opts.get('tools', []))
         # Disable hover for errorbars plot as Bokeh annotations can't be hovered.
         if kind == 'errorbars':
             hover = False
         elif hover is None:
             hover = not self.datashade
-        if hover and not any(t for t in tools if isinstance(t, HoverTool)
-                             or t in ['hover', 'vline', 'hline']):
+        if hover and not any(
+            t for t in tools if isinstance(t, HoverTool) or t in ['hover', 'vline', 'hline']
+        ):
             if hover in ['vline', 'hline']:
                 tools.append(hover)
             else:
                 tools.append('hover')
         plot_opts['tools'] = tools
 
         if self.crs and global_extent:
             plot_opts['global_extent'] = global_extent
         if projection:
             plot_opts['projection'] = self.output_projection
         title = title if title is not None else getattr(self, '_title', None)
         if title is not None:
             plot_opts['title'] = title
-        if (self.kind in self._colorbar_types or self.rasterize or self.datashade or self._color_dim):
+        if (
+            self.kind in self._colorbar_types
+            or self.rasterize
+            or self.datashade
+            or self._color_dim
+        ):
             try:
                 if not use_dask:
                     symmetric = self._process_symmetric(symmetric, clim, check_symmetric_max)
                 if self._style_opts.get('cmap') is None:
-                    # Default to categorical camp if we detect categorical shading
-                    if ((self.datashade or self.rasterize) and (self.aggregator is None or 'count_cat' in str(self.aggregator)) and
-                        ((self.by and not self.subplots) or
-                         ((isinstance(self.y, list) and len(self.y) > 1) or (self.y is None and len(set(self.variables) - set(self.indexes)) > 1)))):
+                    if self._process_categorical_datashader()[0]:
                         self._style_opts['cmap'] = self._default_cmaps['categorical']
                     elif symmetric:
                         self._style_opts['cmap'] = self._default_cmaps['diverging']
                     else:
                         self._style_opts['cmap'] = self._default_cmaps['linear']
-
+                if robust:
+                    plot_opts['clim_percentile'] = True
                 if symmetric is not None:
                     plot_opts['symmetric'] = symmetric
             except TypeError:
                 pass
         if cnorm is not None:
             plot_opts['cnorm'] = cnorm
         if rescale_discrete_levels is not None and hv_version >= Version('1.15.0'):
             plot_opts['rescale_discrete_levels'] = rescale_discrete_levels
 
         self._plot_opts = plot_opts
-        self._overlay_opts = {k: v for k, v in self._plot_opts.items()
-                              if k in OverlayPlot.param.objects()}
+        self._overlay_opts = {
+            k: v for k, v in self._plot_opts.items() if k in OverlayPlot.param.objects()
+        }
 
         self._norm_opts = {'framewise': framewise, 'axiswise': not plot_opts.get('shared_axes')}
         self.kwds = kwds
 
         # Process dimensions and labels
         self.label = label
         self._relabel = {'label': label} if label else {}
         self._dim_ranges = {'c': clim or (None, None)}
 
         # High-level options
         self._validate_kwds(kwds)
         if debug:
-            kwds = dict(x=self.x, y=self.y, by=self.by, kind=self.kind,
-                        groupby=self.groupby, grid=self.grid)
-            param.main.param.warning('Plotting {kind} plot with parameters x: {x}, '
-                               'y: {y}, by: {by}, groupby: {groupby}, row/col: {grid}'.format(**kwds))
+            kwds = dict(
+                x=self.x,
+                y=self.y,
+                by=self.by,
+                kind=self.kind,
+                groupby=self.groupby,
+                grid=self.grid,
+            )
+            param.main.param.warning(
+                'Plotting {kind} plot with parameters x: {x}, '
+                'y: {y}, by: {by}, groupby: {groupby}, row/col: {grid}'.format(**kwds)
+            )
+
+    def _process_categorical_datashader(self):
+        categorical, agg = False, None
+        if not (self.datashade or self.rasterize):
+            return categorical, agg
+
+        ds = import_datashader()
+
+        categorical = False
+        if self.aggregator:
+            agg = self.aggregator
+            if isinstance(agg, str) and self._color_dim:
+                categorical = agg == 'count_cat'
+                agg = getattr(ds.reductions, agg)(self._color_dim)
+            else:
+                categorical = isinstance(agg, (ds.count_cat, ds.by))
+        elif self._color_dim:
+            agg = ds.reductions.mean(self._color_dim)
+        elif self.by and not self.subplots:
+            agg = ds.reductions.count_cat(self.by[0])
+            categorical = True
+        elif (
+            (isinstance(self.y, list) and len(self.y) > 1)
+            or (self.y is None and len(set(self.variables) - set(self.indexes)) > 1)
+        ) and self.kind in ('scatter', 'line', 'area'):
+            agg = ds.reductions.count_cat(self.group_label)
+            categorical = True
+
+        (
+            (isinstance(self.y, list) and len(self.y) > 1)
+            or (self.y is None and len(set(self.variables) - set(self.indexes)) > 1)
+        )
+
+        return categorical, agg
 
     def _process_symmetric(self, symmetric, clim, check_symmetric_max):
         if symmetric is not None or clim is not None:
             return symmetric
 
         if is_xarray(self.data):
             # chunks mean it's lazily loaded; nanquantile will eagerly load
@@ -670,36 +949,57 @@
 
         cmin = np.nanquantile(data, 0.05)
         cmax = np.nanquantile(data, 0.95)
 
         return bool(cmin < 0 and cmax > 0)
 
     def _process_crs(self, data, crs):
-        """Given crs as proj4 string, data.attr, or cartopy.crs return cartopy.crs
-        """
+        """Given crs as proj4 string, data.attr, or cartopy.crs return cartopy.crs"""
         if hasattr(data, 'rio') and data.rio.crs is not None:
             # if data is a rioxarray
             _crs = data.rio.crs.to_wkt()
-        else:
-            # get the proj string: either the value of data.attrs[crs] or crs itself
+        # get the proj string: either the value of data.attrs[crs] or crs itself
+        elif isinstance(crs, str):
             _crs = getattr(data, 'attrs', {}).get(crs or 'crs', crs)
+        else:
+            _crs = crs
 
         try:
             return process_crs(_crs)
         except ValueError as e:
             # only raise error if crs was specified in kwargs
             if crs:
                 raise ValueError(
                     f"'{crs}' must be either a valid crs or an reference to "
-                    f"a `data.attr` containing a valid crs: {e}")
+                    f'a `data.attr` containing a valid crs: {e}'
+                )
 
-    def _process_data(self, kind, data, x, y, by, groupby, row, col,
-                      use_dask, persist, backlog, label, group_label,
-                      value_label, hover_cols, attr_labels, transforms,
-                      stream, kwds):
+    def _process_data(
+        self,
+        kind,
+        data,
+        x,
+        y,
+        by,
+        groupby,
+        row,
+        col,
+        use_dask,
+        persist,
+        backlog,
+        label,
+        group_label,
+        value_label,
+        hover_cols,
+        attr_labels,
+        transforms,
+        stream,
+        robust,
+        kwds,
+    ):
         gridded = kind in self._gridded_types
         gridded_data = False
         da = None
 
         # Validate DataSource
         self.data_source = data
         self.is_series = is_series(data)
@@ -717,28 +1017,36 @@
         self.source_data = data
 
         if groupby is not None and not isinstance(groupby, list):
             groupby = [groupby]
         if by is not None and not isinstance(by, list):
             by = [by]
         grid = []
-        if row is not None: grid.append(row)
-        if col is not None: grid.append(col)
+        if row is not None:
+            grid.append(row)
+        if col is not None:
+            grid.append(col)
         streaming = False
         if is_geodataframe(data):
             datatype = 'geopandas' if hasattr(data, 'geom_type') else 'spatialpandas'
             self.data = data
             if kind is None:
                 if datatype == 'geopandas':
                     geom_types = {gt[5:] if 'Multi' in gt else gt for gt in data.geom_type}
                 else:
-                    geom_types = [type(data.geometry.dtype).__name__.replace('Multi', '').replace('Dtype', '')]
+                    geom_types = [
+                        type(data.geometry.dtype)
+                        .__name__.replace('Multi', '')
+                        .replace('Dtype', '')
+                    ]
                 if len(geom_types) > 1:
-                    raise ValueError('The GeopandasInterface can only read dataframes which '
-                                     'share a common geometry type')
+                    raise ValueError(
+                        'The GeopandasInterface can only read dataframes which '
+                        'share a common geometry type'
+                    )
                 geom_type = list(geom_types)[0]
                 if geom_type == 'Point':
                     kind = 'points'
                 elif geom_type == 'Polygon':
                     kind = 'polygons'
                 elif geom_type in ('LineString', 'LineRing', 'Line'):
                     kind = 'paths'
@@ -769,32 +1077,31 @@
             if data._stream_type == 'updating':
                 self.stream = Pipe(data=self.data)
             else:
                 self.stream = Buffer(data=self.data, length=backlog, index=False)
             data.stream.gather().sink(self.stream.send)
         elif is_xarray(data):
             import xarray as xr
+
             z = kwds.get('z')
             if isinstance(data, xr.Dataset):
                 if len(data.data_vars) == 0:
-                    raise ValueError("Cannot plot an empty xarray.Dataset object.")
+                    raise ValueError('Cannot plot an empty xarray.Dataset object.')
             if z is None:
                 if isinstance(data, xr.Dataset):
                     z = list(data.data_vars)[0]
                 else:
                     z = data.name or label or value_label
             if gridded and isinstance(data, xr.Dataset) and not isinstance(z, list):
                 data = data[z]
             self.z = z
 
             ignore = (groupby or []) + (by or []) + grid
-            coords = [c for c in data.coords if data[c].shape != ()
-                      and c not in ignore]
-            dims = [c for c in data.dims if data[c].shape != ()
-                    and c not in ignore]
+            coords = [c for c in data.coords if data[c].shape != () and c not in ignore]
+            dims = [c for c in data.dims if data[c].shape != () and c not in ignore]
 
             if kind is None and (not (x or y) or all(c in data.coords for c in (x, y))):
                 if list(data.coords) == ['band', 'y', 'x']:
                     kind = 'rgb'
                     gridded = True
                 elif len(coords) == 1:
                     kind = 'line'
@@ -813,20 +1120,44 @@
                     other_dims = [kwds['bands']]
                 else:
                     other_dims = [d for d in data.coords if d not in (groupby or [])][0]
             else:
                 other_dims = []
             da = data
             data, x, y, by_new, groupby_new = process_xarray(
-                data, x, y, by, groupby, use_dask, persist, gridded,
-                label, value_label, other_dims, kind=kind)
+                data,
+                x,
+                y,
+                by,
+                groupby,
+                use_dask,
+                persist,
+                gridded,
+                label,
+                value_label,
+                other_dims,
+                kind=kind,
+            )
+            if kind == 'rgb' and robust:
+                # adapted from xarray
+                # https://github.com/pydata/xarray/blob/6af547cdd9beac3b18420ccb204f801603e11519/xarray/plot/utils.py#L729
+                vmax = np.nanpercentile(data[z], 100 - 2)
+                vmin = np.nanpercentile(data[z], 2)
+                # Scale interval [vmin .. vmax] to [0 .. 1], with darray as 64-bit float
+                # to avoid precision loss, integer over/underflow, etc with extreme inputs.
+                # After scaling, downcast to 32-bit float.  This substantially reduces
+                # memory usage
+                data[z] = ((data[z].astype('f8') - vmin) / (vmax - vmin)).astype('f4')
+                data[z] = np.minimum(np.maximum(data[z], 0), 1)
 
             if kind not in self._stats_types:
-                if by is None: by = by_new
-                if groupby is None: groupby = groupby_new
+                if by is None:
+                    by = by_new
+                if groupby is None:
+                    groupby = groupby_new
 
             if groupby:
                 groupby = [g for g in groupby if g not in grid]
 
             # Add a title to hvplot.xarray plots that displays scalar coords values,
             # as done by xarray.plot()
             if not groupby and not grid:
@@ -837,28 +1168,30 @@
 
             self.data = data
         else:
             raise ValueError('Supplied data type %s not understood' % type(data).__name__)
 
         if stream is not None:
             if streaming:
-                raise ValueError("Cannot supply streamz.DataFrame and stream argument.")
+                raise ValueError('Cannot supply streamz.DataFrame and stream argument.')
             self.stream = stream
             self.cb = None
             if isinstance(stream, Pipe):
                 self.stream_type = 'updating'
             elif isinstance(stream, Buffer):
                 self.stream_type = 'streaming'
             else:
-                raise ValueError("Stream of type %s not recognized." % type(stream))
+                raise ValueError('Stream of type %s not recognized.' % type(stream))
             streaming = True
 
         # Validate data and arguments
-        if by is None: by = []
-        if groupby is None: groupby = []
+        if by is None:
+            by = []
+        if groupby is None:
+            groupby = []
 
         if gridded_data:
             not_found = [g for g in groupby if g not in data.coords]
             not_found, _, _ = process_derived_datetime_xarray(data, not_found)
             data_vars = list(data.data_vars) if isinstance(data, xr.Dataset) else [data.name]
             indexes = list(data.coords.indexes)
             # Handle undeclared indexes
@@ -868,49 +1201,63 @@
                 indexes.append(y)
             for data_dim in data.dims:
                 if not any(data_dim in data[c].dims for c in indexes):
                     for coord in data.coords:
                         if coord not in indexes and {data_dim} == set(data[coord].dims):
                             indexes.append(data_dim)
                             self.data = self.data.set_index({data_dim: coord})
-                            if coord not in groupby+by:
+                            if coord not in groupby + by:
                                 groupby.append(data_dim)
             self.variables = list(data.coords) + data_vars
             if groupby and not_found:
-                raise ValueError(f'The supplied groupby dimension(s) {not_found} '
-                                 'could not be found, expected one or '
-                                 f'more of: {list(data.coords)}')
+                raise ValueError(
+                    f'The supplied groupby dimension(s) {not_found} '
+                    'could not be found, expected one or '
+                    f'more of: {list(data.coords)}'
+                )
         else:
             if gridded and kind not in ('points', 'dataset'):
-                raise ValueError(f'{kind} plot type requires gridded data, '
-                                 'e.g. a NumPy array or xarray Dataset, '
-                                 f'found {type(self.data).__name__} type')
+                raise ValueError(
+                    f'{kind} plot type requires gridded data, '
+                    'e.g. a NumPy array or xarray Dataset, '
+                    f'found {type(self.data).__name__} type'
+                )
 
-            if hasattr(data, 'columns') and hasattr(data.columns, 'name') and data.columns.name and not group_label:
+            if (
+                hasattr(data, 'columns')
+                and hasattr(data.columns, 'name')
+                and data.columns.name
+                and not group_label
+            ):
                 group_label = data.columns.name
             elif not group_label:
                 group_label = 'Variable'
 
-            if isinstance(data.columns, pd.MultiIndex) and x in (None, 'index') and y is None and not by:
+            if (
+                isinstance(data.columns, pd.MultiIndex)
+                and x in (None, 'index')
+                and y is None
+                and not by
+            ):
                 self.data = data.stack().reset_index(1).rename(columns={'level_1': group_label})
                 by = group_label
                 x = 'index'
 
             # Determine valid indexes
             if isinstance(self.data, pd.DataFrame):
                 if self.data.index.names == [None]:
                     indexes = [self.data.index.name or 'index']
                 else:
                     indexes = list(self.data.index.names)
             elif hasattr(self.data, 'reset_index'):
-                indexes = [c for c in self.data.reset_index().columns
-                           if c not in self.data.columns]
+                indexes = [
+                    c for c in self.data.reset_index().columns if c not in self.data.columns
+                ]
             else:
-                indexes = [c for c in self.data.columns
-                           if c not in self.data.columns]
+                indexes = [c for c in self.data.columns if c not in self.data.columns]
 
             if len(indexes) == 2 and not (x or y or by):
                 if kind == 'heatmap':
                     x, y = indexes
                 elif kind in ('bar', 'barh'):
                     x, by = indexes
 
@@ -921,20 +1268,24 @@
             if groupby_index:
                 self.data = self.data.reset_index(groupby_index)
 
             if isinstance(by, (np.ndarray, pd.Series)):
                 by_cols = []
             else:
                 by_cols = by if isinstance(by, list) else [by]
-            not_found = [g for g in groupby+by_cols if g not in list(self.data.columns)+indexes]
+            not_found = [
+                g for g in groupby + by_cols if g not in list(self.data.columns) + indexes
+            ]
             not_found, self.data = process_derived_datetime_pandas(self.data, not_found, indexes)
             if groupby and not_found:
-                raise ValueError(f'The supplied groupby dimension(s) {not_found} '
-                                 'could not be found, expected one or '
-                                 f'more of: {list(self.data.columns)}')
+                raise ValueError(
+                    f'The supplied groupby dimension(s) {not_found} '
+                    'could not be found, expected one or '
+                    f'more of: {list(self.data.columns)}'
+                )
 
         if transforms:
             self.data = Dataset(self.data, indexes).transform(**transforms).data
 
         # Set data-level options
         self.x = x
         self.y = y
@@ -961,19 +1312,19 @@
             self.hover_cols = []
         elif isinstance(hover_cols, list):
             self.hover_cols = hover_cols
         elif hover_cols == 'all' and self.use_index:
             self.hover_cols = self.variables
         elif hover_cols == 'all' and not self.use_index:
             self.hover_cols = [v for v in self.variables if v not in self.indexes]
-        elif hover_cols !='all' and isinstance(hover_cols,str):
+        elif hover_cols != 'all' and isinstance(hover_cols, str):
             self.hover_cols = [hover_cols]
 
         if self.datatype in ('geopandas', 'spatialpandas'):
-            self.hover_cols = [c for c in self.hover_cols if c!= 'geometry']
+            self.hover_cols = [c for c in self.hover_cols if c != 'geometry']
 
         if da is not None and attr_labels is True or attr_labels is None:
             try:
                 var_tuples = [(var, da[var].attrs) for var in da.coords]
                 if isinstance(da, xr.Dataset):
                     var_tuples.extend([(var, da[var].attrs) for var in da.data_vars])
                 else:
@@ -987,64 +1338,77 @@
                         labels[var_name] = var_attrs['long_name']
                     if 'units' in var_attrs:
                         units[var_name] = var_attrs['units']
                 self._redim = self._merge_redim(labels, 'label')
                 self._redim = self._merge_redim(units, 'unit')
             except Exception as e:
                 if attr_labels is True:
-                    param.main.param.warning('Unable to auto label using xarray attrs '
-                                       f'because {e}')
+                    param.main.param.warning(
+                        'Unable to auto label using xarray attrs ' f'because {e}'
+                    )
 
     def _process_plot(self):
         kind = self.kind
         options = Store.options(backend='bokeh')
         elname = self._kind_mapping[kind].__name__
         plot_opts = options[elname].groups['plot'].options if elname in options else {}
 
         if kind.startswith('bar'):
             plot_opts['stacked'] = self.stacked
 
         if kind == 'hist':
             if self.stacked:
-                param.main.param.warning('Stacking for histograms is not yet implemented in '
-                                   'holoviews. Use bar plots if stacking is required.')
+                param.main.param.warning(
+                    'Stacking for histograms is not yet implemented in '
+                    'holoviews. Use bar plots if stacking is required.'
+                )
 
         return plot_opts
 
     def _process_style(self, kwds, plot_opts):
         kind = self.kind
         eltype = self._kind_mapping[kind]
-        registry =  Store.registry[self._backend_compat]
+        registry = Store.registry[self._backend_compat]
 
         if eltype in registry:
             valid_opts = registry[eltype].style_opts
         else:
             valid_opts = []
 
         cmap_opts = ('cmap', 'colormap', 'color_key')
-        categories = ['accent', 'category', 'dark', 'colorblind', 'pastel',
-                      'set1', 'set2', 'set3', 'paired', 'glasbey']
+        categories = [
+            'accent',
+            'category',
+            'dark',
+            'colorblind',
+            'pastel',
+            'set1',
+            'set2',
+            'set3',
+            'paired',
+            'glasbey',
+        ]
         for opt in valid_opts:
-            if (opt not in kwds or not isinstance(kwds[opt], list) or
-                opt in cmap_opts):
+            if opt not in kwds or not isinstance(kwds[opt], list) or opt in cmap_opts:
                 continue
             kwds[opt] = Cycle(kwds[opt])
 
         # Process style options
         options = Store.options(backend=self._backend_compat)
         elname = eltype.__name__
         style = options[elname].groups['style'].kwargs if elname in options else {}
-        style_opts = {k: v for k, v in style.items() if not isinstance(v, Cycle) and k not in cmap_opts}
+        style_opts = {
+            k: v for k, v in style.items() if not isinstance(v, Cycle) and k not in cmap_opts
+        }
         style_opts.update(**{k: v for k, v in kwds.items() if k in valid_opts})
 
         # Color
         cmap_kwds = set(cmap_opts).intersection(kwds)
         if len(cmap_kwds) > 1:
-            raise TypeError('Specify at most one of `cmap`, `colormap`, or '
-                            '`color_key`.')
+            raise TypeError('Specify at most one of `cmap`, `colormap`, or `color_key`.')
 
         cmap = kwds.pop(cmap_kwds.pop()) if cmap_kwds else None
         color = kwds.pop('color', kwds.pop('c', None))
 
         if color is not None:
             if (self.datashade or self.rasterize) and color in [self.x, self.y]:
                 self.data = self.data.assign(_color=self.data[color])
@@ -1053,16 +1417,19 @@
             elif isinstance(color, (np.ndarray, pd.Series)):
                 self.data = self.data.assign(_color=color)
                 style_opts['color'] = color = '_color'
                 self.variables.append('_color')
             else:
                 style_opts['color'] = color
 
-            if not isinstance(color, list) and color in self.variables and \
-                'c' in self._kind_options.get(kind, []):
+            if (
+                not isinstance(color, list)
+                and color in self.variables
+                and 'c' in self._kind_options.get(kind, [])
+            ):
                 if self.data[color].dtype.kind in 'OSU':
                     cmap = cmap or self._default_cmaps['categorical']
                 else:
                     plot_opts['colorbar'] = plot_opts.get('colorbar', True)
 
         if isinstance(cmap, str) and cmap in self._default_cmaps:
             cmap = self._default_cmaps[cmap]
@@ -1093,19 +1460,20 @@
                 else:
                     style_opts[k] = color
 
         # Size
         size = kwds.pop('size', kwds.pop('s', None))
         if size is not None:
             scale = kwds.get('scale', 1)
-            if (self.datashade or self.rasterize):
+            if self.datashade or self.rasterize:
                 param.main.param.warning(
                     'There is no reasonable way to use size (or s) with '
                     'rasterize or datashade. To aggregate along a third '
-                    'dimension, set color (or c) to the desired dimension.')
+                    'dimension, set color (or c) to the desired dimension.'
+                )
             if isinstance(size, (np.ndarray, pd.Series)):
                 size = np.sqrt(size) * scale
                 self.data = self.data.assign(_size=size)
                 style_opts['size'] = '_size'
                 self.variables.append('_size')
             elif isinstance(size, str):
                 style_opts['size'] = np.sqrt(dim(size)) * scale
@@ -1125,35 +1493,44 @@
         kind = self.kind
         eltype = self._kind_mapping[kind]
         if eltype in Store.registry[self._backend_compat]:
             valid_opts = Store.registry[self._backend_compat][eltype].style_opts
         else:
             valid_opts = []
         ds_opts = ['max_px', 'threshold']
-        mismatches = sorted(k for k in kwds if k not in kind_opts+ds_opts+valid_opts)
+        mismatches = sorted(k for k in kwds if k not in kind_opts + ds_opts + valid_opts)
         if not mismatches:
             return
 
         if 'ax' in mismatches:
             mismatches.pop(mismatches.index('ax'))
-            param.main.param.warning('hvPlot does not have the concept of axes, '
-                               'and the ax keyword will be ignored. Compose '
-                               'plots with the * operator to overlay plots or the '
-                               '+ operator to lay out plots beside each other '
-                               'instead.')
+            param.main.param.warning(
+                'hvPlot does not have the concept of axes, '
+                'and the ax keyword will be ignored. Compose '
+                'plots with the * operator to overlay plots or the '
+                '+ operator to lay out plots beside each other '
+                'instead.'
+            )
         if 'figsize' in mismatches:
             mismatches.pop(mismatches.index('figsize'))
-            param.main.param.warning('hvPlot does not have the concept of a figure, '
-                               'and the figsize keyword will be ignored. The '
-                               'size of each subplot in a layout is set '
-                               'individually using the width and height options.')
-
-        combined_opts = (self._data_options + self._axis_options +
-                         self._op_options +
-                         self._geo_options + kind_opts + valid_opts)
+            param.main.param.warning(
+                'hvPlot does not have the concept of a figure, '
+                'and the figsize keyword will be ignored. The '
+                'size of each subplot in a layout is set '
+                'individually using the width and height options.'
+            )
+
+        combined_opts = (
+            self._data_options
+            + self._axis_options
+            + self._op_options
+            + self._geo_options
+            + kind_opts
+            + valid_opts
+        )
         # Only add the global styling options in the suggestions for bokeh
         # since they may not be supported by all the backends.
         # See e.g. alpha for Area plots with plotly:
         # https://github.com/holoviz/holoviews/issues/5226
         if self._backend_compat == 'bokeh':
             combined_opts = combined_opts + self._style_options
         for mismatch in mismatches:
@@ -1165,105 +1542,128 @@
 
     def __call__(self, kind, x, y):
         kind = self.kind or kind
         method = getattr(self, kind)
 
         groups = self.groupby
         zs = self.kwds.get('z', [])
-        if not isinstance(zs, list): zs = [zs]
+        if not isinstance(zs, list):
+            zs = [zs]
         groups += self.grid
         if self.gridded and not kind == 'points':
             groups += self.by
         if groups or len(zs) > 1:
             if self.streaming:
-                raise NotImplementedError("Streaming and groupby not yet implemented")
+                raise NotImplementedError('Streaming and groupby not yet implemented')
             data = self.data
             if not self.gridded and any(g in self.indexes for g in groups):
                 data = data.reset_index()
 
             if self.datatype in ('geopandas', 'spatialpandas'):
                 columns = [c for c in data.columns if c != 'geometry']
                 shape_dims = ['Longitude', 'Latitude'] if self.geo else ['x', 'y']
-                dataset = Dataset(data, kdims=shape_dims+columns)
+                dataset = Dataset(data, kdims=shape_dims + columns)
             elif self.datatype == 'xarray':
                 import xarray as xr
+
                 if isinstance(data, xr.Dataset):
                     if kind == 'image':
                         dims_with_coords = set(data.coords.keys())
-                        missing_coords =  set(self.indexes) - dims_with_coords
-                        new_coords = {coord: np.arange(data[coord].shape[0])
-                                      for coord in missing_coords}
+                        missing_coords = set(self.indexes) - dims_with_coords
+                        new_coords = {
+                            coord: np.arange(data[coord].shape[0]) for coord in missing_coords
+                        }
                         data = data.assign_coords(**new_coords)
                     dataset = Dataset(data, self.indexes)
                 else:
                     name = data.name or self.label or self.value_label
                     dataset = Dataset(data, self.indexes, name)
             else:
                 dataset = Dataset(data)
             dataset = dataset.redim(**self._redim)
 
             if groups:
                 datasets = dataset.groupby(groups, dynamic=self.dynamic)
                 if len(zs) > 1:
-                    dimensions = [Dimension(self.group_label, values=zs)]+datasets.kdims
+                    dimensions = [Dimension(self.group_label, values=zs)] + datasets.kdims
                     if self.dynamic:
+
                         def z_wrapper(**kwargs):
                             z = kwargs.pop(self.group_label)
                             ds = datasets.select(**kwargs)
                             return ds.reindex(vdims=[ds.get_dimension(z)])
+
                         obj = DynamicMap(z_wrapper, kdims=dimensions)
+
                         def method_wrapper(ds, x, y):
                             z = ds.vdims[0].name
                             el = method(x, y, z, data=ds.data)
                             el._transforms = dataset._transforms
                             el._dataset = ds
                             return el
-                        obj = obj.apply(method_wrapper, x=x, y=y, per_element=True, link_inputs=False)
+
+                        obj = obj.apply(
+                            method_wrapper, x=x, y=y, per_element=True, link_inputs=False
+                        )
                     else:
-                        obj = HoloMap({(z,)+k: method(x, y, z, dataset[k])
-                                       for k, v in datasets.data.items() for z in zs}, kdims=dimensions)
+                        obj = HoloMap(
+                            {
+                                (z,) + k: method(x, y, z, dataset[k])
+                                for k, v in datasets.data.items()
+                                for z in zs
+                            },
+                            kdims=dimensions,
+                        )
                 else:
+
                     def method_wrapper(ds, x, y):
                         el = method(x, y, data=ds.data)
                         el._transforms = dataset._transforms
                         el._dataset = ds
                         return el
-                    obj = datasets.apply(method_wrapper, x=x, y=y, per_element=True,
-                                         link_inputs=False)
+
+                    obj = datasets.apply(
+                        method_wrapper, x=x, y=y, per_element=True, link_inputs=False
+                    )
             elif len(zs) > 1:
                 dimensions = [Dimension(self.group_label, values=zs)]
                 if self.dynamic:
-                    obj = DynamicMap(lambda z: method(x, y, z, data=dataset.data),
-                                     kdims=dimensions)
+                    obj = DynamicMap(
+                        lambda z: method(x, y, z, data=dataset.data), kdims=dimensions
+                    )
                 else:
-                    obj = HoloMap({z: method(x, y, z, data=dataset.data) for z in zs},
-                                  kdims=dimensions)
+                    obj = HoloMap(
+                        {z: method(x, y, z, data=dataset.data) for z in zs}, kdims=dimensions
+                    )
             else:
                 obj = method(x, y, data=dataset.data)
 
             if self.gridded and self.by and not kind == 'points':
                 obj = obj.layout(self.by) if self.subplots else obj.overlay(self.by)
             if self.grid:
-                obj = obj.grid(self.grid).opts(shared_xaxis=True, shared_yaxis=True, backend='bokeh')
+                obj = obj.grid(self.grid).opts(
+                    shared_xaxis=True, shared_yaxis=True, backend='bokeh'
+                )
         else:
             if self.streaming:
                 cb = partial(method, x, y)
                 if self.cb is None:
                     cbcallable = cb
                 else:
                     cbcallable = StreamingCallable(cb, periodic=self.cb)
                 obj = DynamicMap(cbcallable, streams=[self.stream])
             else:
                 data = self.source_data
                 if self.datatype in ('geopandas', 'spatialpandas'):
                     columns = [c for c in data.columns if c != 'geometry']
                     shape_dims = ['Longitude', 'Latitude'] if self.geo else ['x', 'y']
-                    dataset = Dataset(data, kdims=shape_dims+columns)
+                    dataset = Dataset(data, kdims=shape_dims + columns)
                 elif self.datatype == 'xarray':
                     import xarray as xr
+
                     if isinstance(data, xr.Dataset):
                         dataset = Dataset(data, self.indexes)
                     else:
                         name = data.name or self.label or self.value_label
                         dataset = Dataset(data, self.indexes, name)
                 else:
                     try:
@@ -1274,14 +1674,15 @@
 
                 obj = method(x, y)
                 obj._dataset = dataset
 
         if self.crs and self.project:
             # Apply projection before rasterizing
             import geoviews as gv
+
             obj = gv.project(obj, projection=self.output_projection)
 
         if not (self.datashade or self.rasterize or self.downsample):
             layers = self._apply_layers(obj)
             layers = _transfer_opts_cur_backend(layers)
             return layers
 
@@ -1293,50 +1694,34 @@
 
         if self.downsample:
             try:
                 from holoviews.operation.downsample import downsample1d
             except ImportError:
                 raise ImportError('Downsampling requires HoloViews >=1.16')
 
+            # Let HoloViews choose the default algo if 'downsample' is True.
+            # Otherwise, user-specified algorithm
+            if isinstance(self.downsample, str):
+                opts['algorithm'] = self.downsample
+
             if self.x_sampling:
                 opts['x_sampling'] = self.x_sampling
             if self._plot_opts.get('xlim') is not None:
                 opts['x_range'] = self._plot_opts['xlim']
             layers = self._resample_obj(downsample1d, obj, opts)
             layers = _transfer_opts_cur_backend(layers)
             return layers
 
-        try:
-            from holoviews.operation.datashader import datashade, rasterize, dynspread
-            from datashader import reductions
-        except ImportError:
-            raise ImportError('In order to use datashading features '
-                    'the Datashader library must be available. '
-                    'It can be installed with:\n  conda '
-                    'install datashader')
+        import_datashader()
+        from holoviews.operation.datashader import datashade, rasterize, dynspread
 
-        categorical = False
-        if self.by and not self.subplots:
-            opts['aggregator'] = reductions.count_cat(self.by[0])
-            categorical = True
-        elif ((isinstance(self.y, list) and len(self.y) > 1 or self.y is None and len(set(self.variables) - set(self.indexes)) > 1) and
-              self.kind in ('scatter', 'line', 'area')):
-            opts['aggregator'] = reductions.count_cat(self.group_label)
-            categorical = True
-        if self.aggregator:
-            import datashader as ds
-            agg = self.aggregator
-            if isinstance(agg, str) and self._color_dim:
-                categorical = agg == 'count_cat'
-                agg = getattr(reductions, agg)(self._color_dim)
-            else:
-                categorical = isinstance(agg, (ds.count_cat, ds.by))
+        categorical, agg = self._process_categorical_datashader()
+        if agg:
             opts['aggregator'] = agg
-        elif self._color_dim:
-            opts['aggregator'] = reductions.mean(self._color_dim)
+
         if self.precompute:
             opts['precompute'] = self.precompute
         if self.x_sampling:
             opts['x_sampling'] = self.x_sampling
         if self.y_sampling:
             opts['y_sampling'] = self.y_sampling
         if self._plot_opts.get('xlim') is not None:
@@ -1354,129 +1739,149 @@
 
         if 'line_width' in self._style_opts:
             opts['line_width'] = self._style_opts['line_width']
 
         style = {}
         if self.datashade:
             operation = datashade
-            if 'cmap' in opts and not 'color_key' in opts:
+            if 'cmap' in opts and 'color_key' not in opts:
                 opts['color_key'] = opts['cmap']
             eltype = 'RGB'
             if 'cnorm' in self._plot_opts:
                 opts['cnorm'] = self._plot_opts['cnorm']
             if 'rescale_discrete_levels' in self._plot_opts:
                 opts['rescale_discrete_levels'] = self._plot_opts['rescale_discrete_levels']
         elif self.rasterize:
             operation = rasterize
             if Version(hv.__version__) < Version('1.18.0a1'):
                 eltype = 'Image'
             else:
-                eltype = 'ImageStack' if self.by else 'Image'
+                eltype = 'ImageStack' if categorical else 'Image'
             if 'cmap' in self._style_opts:
                 style['cmap'] = self._style_opts['cmap']
             if self._dim_ranges.get('c', (None, None)) != (None, None):
                 style['clim'] = self._dim_ranges['c']
 
         processed = self._resample_obj(operation, obj, opts)
         if self.dynspread:
-            processed = dynspread(processed, max_px=self.kwds.get('max_px', 3),
-                                  threshold=self.kwds.get('threshold', 0.5))
+            processed = dynspread(
+                processed,
+                max_px=self.kwds.get('max_px', 3),
+                threshold=self.kwds.get('threshold', 0.5),
+            )
 
         opts = filter_opts(eltype, dict(self._plot_opts, **style), backend='bokeh')
         layers = self._apply_layers(processed).opts(eltype, **opts, backend='bokeh')
         layers = _transfer_opts_cur_backend(layers)
         return layers
 
     def _resample_obj(self, operation, obj, opts):
         def exceeds_resample_when(plot):
             return len(plot) > self.resample_when
 
         if self.resample_when is not None:
             processed = apply_when(
-                obj,
-                operation=partial(operation, **opts),
-                predicate=exceeds_resample_when
+                obj, operation=partial(operation, **opts), predicate=exceeds_resample_when
             )
         else:
             processed = operation(obj, **opts)
         return processed
 
     def _get_opts(self, eltype, backend='bokeh', **custom):
         opts = dict(self._plot_opts, **dict(self._style_opts, **self._norm_opts))
         opts.update(custom)
         return filter_opts(eltype, opts, backend=backend)
 
     def _apply_layers(self, obj):
         if self.coastline:
             import geoviews as gv
+
             coastline = gv.feature.coastline.clone()
             if self.coastline in ['10m', '50m', '110m']:
                 coastline = coastline.opts(scale=self.coastline)
             elif self.coastline is not True:
                 param.main.param.warning(
-                    "coastline scale of %s not recognized, must be one "
-                    "'10m', '50m' or '110m'." % self.coastline)
+                    'coastline scale of %s not recognized, must be one '
+                    "'10m', '50m' or '110m'." % self.coastline
+                )
             obj = obj * coastline.opts(projection=self.output_projection)
 
         if self.features:
             import geoviews as gv
+
             for feature in reversed(self.features):
                 feature_obj = getattr(gv.feature, feature)
                 if feature_obj is None:
                     raise ValueError(
-                        "Feature %r was not recognized, must be one of "
+                        'Feature %r was not recognized, must be one of '
                         "'borders', 'coastline', 'lakes', 'land', 'ocean', "
-                        "'rivers' and 'states'." % feature)
+                        "'rivers' and 'states'." % feature
+                    )
                 feature_obj = feature_obj.clone()
                 if isinstance(self.features, dict):
                     scale = self.features[feature]
                     if scale not in ['10m', '50m', '110m']:
                         param.main.param.warning(
-                            "Feature scale of %r not recognized, "
-                            "must be one of '10m', '50m' or '110m'." %
-                        scale)
+                            'Feature scale of %r not recognized, '
+                            "must be one of '10m', '50m' or '110m'." % scale
+                        )
                     else:
                         feature_obj = feature_obj.opts(scale=scale)
-                if feature_obj.group in ["Land", "Ocean"]:
+                if feature_obj.group in ['Land', 'Ocean']:
                     # Underlay land/ocean
                     obj = feature_obj.opts(projection=self.output_projection) * obj
                 else:
                     # overlay everything else
                     obj = obj * feature_obj.opts(projection=self.output_projection)
 
-        if self.tiles and not self.geo:
-            tiles = self._get_tiles(
-                self.tiles,
-                hv.element.tile_sources,
-                hv.element.tiles.Tiles
-            )
-            obj = tiles * obj
-        elif self.tiles and self.geo:
-            import geoviews as gv
-            tiles = self._get_tiles(
-                self.tiles,
-                gv.tile_sources.tile_sources,
-                (gv.element.WMTS, hv.element.tiles.Tiles),
-            )
+        if self.tiles:
+            if not self.geo:
+                tiles = self._get_tiles(self.tiles)
+            else:
+                tiles = self._get_tiles(self.tiles, lib='geoviews')
+            tiles = tiles.opts(clone=True, **self.tiles_opts)
             obj = tiles * obj
         return obj
 
-    def _get_tiles(self, source, sources, types):
-        tile_source = 'EsriImagery' if self.tiles == 'ESRI' else self.tiles
+    def _get_tiles(self, source, lib='holoviews'):
+        if lib == 'geoviews':
+            import geoviews as gv
+
+            sources = gv.tile_sources.tile_sources
+            kls = gv.element.WMTS
+            types = (kls, hv.element.tiles.Tiles)
+        else:
+            sources = hv.element.tile_sources
+            kls = hv.element.tiles.Tiles
+            types = kls
+
+        tile_source = 'EsriImagery' if source == 'ESRI' else source
+        tiles = None
         if tile_source is True:
-            tiles = sources["OSM"]()
-        elif tile_source in sources:
+            tiles = sources['OSM']()
+        elif isinstance(tile_source, str) and tile_source in sources:
             tiles = sources[tile_source]()
         elif tile_source in sources.values():
             tiles = tile_source()
         elif isinstance(tile_source, types):
             tiles = tile_source
-        else:
+        elif 'xyzservices' in sys.modules:
+            import xyzservices
+
+            if isinstance(tile_source, xyzservices.TileProvider):
+                tiles = kls(tile_source)
+        if tiles is None:
             msg = (
-                f"{tile_source} tiles not recognized, must be one of: {sorted(sources)} or a tile object"
+                f'{tile_source} tiles not recognized. tiles must be either True, a '
+                'xyzservices.TileProvider instance, a HoloViews'
+                + (' or Geoviews' if lib == 'geoviews' else '')
+                + " basemap string "
+                f"(one of {', '.join(sorted(sources))}), a HoloViews Tiles instance"
+                + (', a Geoviews WMTS instance' if lib == 'geoviews' else '')
+                + '.'
             )
             raise ValueError(msg)
         return tiles
 
     def _merge_redim(self, ranges, attr='range'):
         redim = dict(self._redim)
         for k, r in ranges.items():
@@ -1516,16 +1921,19 @@
                 dimensions.append(dimension)
         agg_col = getattr(self.aggregator, 'column', None)
         if agg_col is not None:
             if agg_col not in dimensions:
                 vdims.append(agg_col)
                 dimensions.append(agg_col)
         for dimension in self.hover_cols:
-            if (isinstance(dimension, str) and dimension in self.variables
-                and dimension not in dimensions):
+            if (
+                isinstance(dimension, str)
+                and dimension in self.variables
+                and dimension not in dimensions
+            ):
                 vdims.append(dimension)
         return kdims, vdims
 
     def _set_backends_opts(self, element, cur_opts, compat_opts):
         # Bokeh is still the main backend
         element = element.opts(**cur_opts, backend='bokeh')
         if compat_opts:
@@ -1534,17 +1942,15 @@
 
     def _get_compat_opts(self, el_name, **custom):
         # Bokeh is still the main backend
         cur_opts = self._get_opts(el_name, backend='bokeh', **custom)
         if self._backend_compat != 'bokeh':
             # Don't pass custom opts to the compatibility layer
             compat_opts = self._get_opts(el_name, backend=self._backend_compat)
-            compat_opts = {
-                k: v for k, v in compat_opts.items() if k not in cur_opts
-            }
+            compat_opts = {k: v for k, v in compat_opts.items() if k not in cur_opts}
         else:
             compat_opts = {}
         return cur_opts, compat_opts
 
     def _error_if_unavailable(self, kind, element=None):
         """
         Raise an error if the element is not available with the current backend.
@@ -1569,25 +1975,31 @@
 
         if 'xlabel' in self._plot_opts and 'x' not in labelled:
             labelled.append('x')
         if 'ylabel' in self._plot_opts and 'y' not in labelled:
             labelled.append('y')
 
         cur_el_opts = self._get_opts(element.name, labelled=labelled, backend='bokeh')
-        compat_el_opts = self._get_opts(element.name, labelled=labelled, backend=self._backend_compat)
+        compat_el_opts = self._get_opts(
+            element.name, labelled=labelled, backend=self._backend_compat
+        )
         for opts_ in [cur_el_opts, compat_el_opts]:
             if 'color' in opts_ and opts_['color'] in data.columns:
                 opts_['color'] = hv.dim(opts_['color'])
         cur_opts = {
             element.name: cur_el_opts,
-            'NdOverlay': filter_opts('NdOverlay', dict(self._overlay_opts, batched=False), backend='bokeh'),
+            'NdOverlay': filter_opts(
+                'NdOverlay', dict(self._overlay_opts, batched=False), backend='bokeh'
+            ),
         }
         compat_opts = {
             element.name: compat_el_opts,
-            'NdOverlay': filter_opts('NdOverlay', dict(self._overlay_opts), backend=self._backend_compat),
+            'NdOverlay': filter_opts(
+                'NdOverlay', dict(self._overlay_opts), backend=self._backend_compat
+            ),
         }
 
         ys = [y]
         if element is Area and self.kwds.get('y2'):
             ys += [self.kwds['y2']]
         if element is ErrorBars and self.kwds.get('yerr1') and self.kwds.get('yerr2'):
             ys += [self.kwds['yerr1'], self.kwds['yerr2']]
@@ -1595,54 +2007,62 @@
             ys += [self.kwds['yerr1']]
         kdims, vdims = self._get_dimensions([x], ys)
 
         if self.by:
             if element is Bars and not self.subplots:
                 if any(y in self.indexes for y in ys):
                     data = data.reset_index()
-                return (element(data, ([x] if x else [])+self.by, ys)
-                        .relabel(**self._relabel)
-                        .redim(**self._redim)
-                        .opts(cur_opts, backend='bokeh')
-                        .opts(compat_opts, backend=self._backend_compat))
-            chart = Dataset(data, self.by+kdims, vdims).to(
-                element, kdims, vdims, self.by).relabel(**self._relabel)
+                return (
+                    element(data, ([x] if x else []) + self.by, ys)
+                    .relabel(**self._relabel)
+                    .redim(**self._redim)
+                    .opts(cur_opts, backend='bokeh')
+                    .opts(compat_opts, backend=self._backend_compat)
+                )
+            chart = (
+                Dataset(data, self.by + kdims, vdims)
+                .to(element, kdims, vdims, self.by)
+                .relabel(**self._relabel)
+            )
             chart = chart.layout() if self.subplots else chart.overlay(sort=False)
         else:
             chart = element(data, kdims, vdims).relabel(**self._relabel)
-        return (chart.redim(**self._redim)
-                .opts(cur_opts, backend='bokeh')
-                .opts(compat_opts, backend=self._backend_compat))
+        return (
+            chart.redim(**self._redim)
+            .opts(cur_opts, backend='bokeh')
+            .opts(compat_opts, backend=self._backend_compat)
+        )
 
     def _process_chart_x(self, data, x, y, single_y, categories=None):
         """This should happen before _process_chart_y"""
         if x is False:
             return None
 
         x = x or (self.x if self.x != y else None)
         if x is None:
             if self.use_index:
                 xs = self.indexes
             else:
                 xs = list(data.columns)
-            xs = [c for c in xs if c not in self.by+self.groupby+self.grid+[y]]
+            xs = [c for c in xs if c not in self.by + self.groupby + self.grid + [y]]
             x = xs[0] if len(xs) else None
 
         if not x and not categories:
             raise ValueError('Could not determine what to plot. Set x explicitly')
         return x
 
     def _process_chart_y(self, data, x, y, single_y):
         """This should happen after _process_chart_x"""
         y = y or self.y
         if y is None:
-            ys = [c for c in data.columns if c not in [x]+self.by+self.groupby+self.grid]
+            ys = [c for c in data.columns if c not in [x] + self.by + self.groupby + self.grid]
             if len(ys) > 1:
                 # if columns have different dtypes, only include numeric columns
                 from pandas.api.types import is_numeric_dtype as isnum
+
                 num_ys = [dim for dim in ys if isnum(data[dim])]
                 if len(num_ys) >= 1:
                     ys = num_ys
             y = ys[0] if len(ys) == 1 or single_y else ys
         return y
 
     def _process_chart_args(self, data, x, y, single_y=False, categories=None):
@@ -1653,26 +2073,27 @@
 
         x = self._process_chart_x(data, x, y, single_y, categories=categories)
         y = self._process_chart_y(data, x, y, single_y)
 
         # sort by date if enabled and x is a date
         if x is not None and self.sort_date and self.datatype == 'pandas':
             from pandas.api.types import is_datetime64_any_dtype as is_datetime
+
             if x in self.indexes:
                 index = self.indexes.index(x)
                 if is_datetime(data.axes[index]):
                     data = data.sort_index(axis=self.indexes.index(x))
             elif x in data.columns:
                 if is_datetime(data[x]):
                     data = data.sort_values(x)
 
         # set index to column if needed in hover_cols
-        if self.use_index and any(c for c in self.hover_cols if
-                                  c in self.indexes and
-                                  c not in data.columns):
+        if self.use_index and any(
+            c for c in self.hover_cols if c in self.indexes and c not in data.columns
+        ):
             data = data.reset_index()
 
         # calculate any derived time
         dimensions = []
         for col in [x, y, self.by, self.hover_cols]:
             if col is not None:
                 dimensions.extend(col if isinstance(col, list) else [col])
@@ -1697,38 +2118,45 @@
         if 'xlabel' in self._plot_opts and 'x' not in labelled:
             labelled.append('x')
         if 'ylabel' in self._plot_opts and 'y' not in labelled:
             labelled.append('y')
 
         cur_opts = {
             element.name: self._get_opts(element.name, labelled=labelled, backend='bokeh'),
-            'NdOverlay': filter_opts('NdOverlay', dict(self._overlay_opts, batched=False), backend='bokeh'),
+            'NdOverlay': filter_opts(
+                'NdOverlay', dict(self._overlay_opts, batched=False), backend='bokeh'
+            ),
         }
         compat_opts = {
-            element.name: self._get_opts(element.name, labelled=labelled, backend=self._backend_compat),
-            'NdOverlay': filter_opts('NdOverlay', dict(self._overlay_opts), backend=self._backend_compat),
+            element.name: self._get_opts(
+                element.name, labelled=labelled, backend=self._backend_compat
+            ),
+            'NdOverlay': filter_opts(
+                'NdOverlay', dict(self._overlay_opts), backend=self._backend_compat
+            ),
         }
 
         charts = []
         for c in y:
             kdims, vdims = self._get_dimensions([x], [c])
             chart = element(data, kdims, vdims).redim(**{c: self.value_label})
             charts.append((c, chart.relabel(**self._relabel).redim(**self._redim)))
-        return (self._by_type(charts, self.group_label, sort=False)
-                .opts(cur_opts, backend='bokeh')
-                .opts(compat_opts, backend=self._backend_compat))
-
+        return (
+            self._by_type(charts, self.group_label, sort=False)
+            .opts(cur_opts, backend='bokeh')
+            .opts(compat_opts, backend=self._backend_compat)
+        )
 
     def line(self, x=None, y=None, data=None):
         self._error_if_unavailable('line')
         return self.chart(Curve, x, y, data)
 
     def step(self, x=None, y=None, data=None):
         where = self.kwds.get('where', 'mid')
-        return self.line(x, y, data).options('Curve', interpolation='steps-'+where)
+        return self.line(x, y, data).options('Curve', interpolation='steps-' + where)
 
     def scatter(self, x=None, y=None, data=None):
         self._error_if_unavailable('scatter')
         return self.chart(Scatter, x, y, data)
 
     def area(self, x=None, y=None, data=None):
         self._error_if_unavailable('area')
@@ -1759,30 +2187,33 @@
             labelled.append('y')
 
         cur_opts, compat_opts = self._get_compat_opts(element.name, labelled=labelled)
 
         id_vars = [x]
         if any(v in self.indexes for v in id_vars):
             data = data.reset_index()
-        data = data[y+[x]]
+        data = data[y + [x]]
 
         if check_library(data, 'dask'):
             from dask.dataframe import melt
         else:
             melt = pd.melt
 
         df = melt(data, id_vars=[x], var_name=self.group_label, value_name=self.value_label)
         kdims = [x, self.group_label]
-        vdims = [self.value_label]+self.hover_cols
+        vdims = [self.value_label] + self.hover_cols
         if self.subplots:
             obj = Dataset(df, kdims, vdims).to(element, x).layout()
         else:
             obj = element(df, kdims, vdims)
-        return (obj.redim(**self._redim).relabel(**self._relabel)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return (
+            obj.redim(**self._redim)
+            .relabel(**self._relabel)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def bar(self, x=None, y=None, data=None):
         self._error_if_unavailable('bar')
         data, x, y = self._process_chart_args(data, x, y, categories=self.by)
         if (x or self.by) and y and (self.by or not isinstance(y, (list, tuple) or len(y) == 1)):
             y = y[0] if isinstance(y, (list, tuple)) else y
             return self.single_chart(Bars, x, y, data)
@@ -1800,47 +2231,53 @@
         Helper method to generate element from indexed dataframe.
         """
         data, x, y = self._process_chart_args(data, False, y)
 
         custom = {}
         if 'color' in self._style_opts:
             prefix = 'violin' if issubclass(element, Violin) else 'box'
-            custom[prefix+'_fill_color'] = self._style_opts['color']
+            custom[prefix + '_fill_color'] = self._style_opts['color']
         cur_opts, compat_opts = self._get_compat_opts(element.name, **custom)
         ylim = self._plot_opts.get('ylim', (None, None))
         if not isinstance(y, (list, tuple)):
             ranges = {y: ylim}
-            return (element(data, self.by, y).redim.range(**ranges).relabel(**self._relabel)
-                    .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
-
+            return (
+                element(data, self.by, y)
+                .redim.range(**ranges)
+                .relabel(**self._relabel)
+                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+            )
 
         labelled = ['y' if self.invert else 'x'] if self.group_label != 'Group' else []
         if self.value_label != 'value':
             labelled.append('x' if self.invert else 'y')
 
         if 'xlabel' in self._plot_opts and 'x' not in labelled:
             labelled.append('x')
         if 'ylabel' in self._plot_opts and 'y' not in labelled:
             labelled.append('y')
 
-        cur_opts['labelled']  = labelled
+        cur_opts['labelled'] = labelled
 
         kdims = [self.group_label]
         data = data[list(y)]
         if check_library(data, 'dask'):
             from dask.dataframe import melt
         else:
             melt = pd.melt
         df = melt(data, var_name=self.group_label, value_name=self.value_label)
         if list(y) and df[self.value_label].dtype is not data[y[0]].dtype:
             df[self.value_label] = df[self.value_label].astype(data[y[0]].dtype)
         redim = self._merge_redim({self.value_label: ylim})
-        return (element(df, kdims, self.value_label).redim(**redim).relabel(**self._relabel)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
-
+        return (
+            element(df, kdims, self.value_label)
+            .redim(**redim)
+            .relabel(**self._relabel)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def box(self, x=None, y=None, data=None):
         self._error_if_unavailable('box')
         return self._stats_plot(BoxWhisker, y, data).redim(**self._redim)
 
     def violin(self, x=None, y=None, data=None):
         self._error_if_unavailable('violin')
@@ -1863,53 +2300,57 @@
 
         cur_opts = {
             'Histogram': self._get_opts('Histogram', labelled=labelled, backend='bokeh'),
             'NdOverlay': filter_opts('NdOverlay', self._overlay_opts, backend='bokeh'),
         }
         compat_opts = {
             'Histogram': self._get_opts('Histogram', backend=self._backend_compat),
-            'NdOverlay': filter_opts('NdOverlay', self._overlay_opts, backend=self._backend_compat),
+            'NdOverlay': filter_opts(
+                'NdOverlay', self._overlay_opts, backend=self._backend_compat
+            ),
+        }
+        hist_opts = {
+            'bin_range': self.kwds.get('bin_range', None),
+            'normed': self.kwds.get('normed', False),
+            'cumulative': self.kwds.get('cumulative', False),
         }
-        hist_opts = {'bin_range': self.kwds.get('bin_range', None),
-                     'normed': self.kwds.get('normed', False),
-                     'cumulative': self.kwds.get('cumulative', False)}
         if 'bins' in self.kwds:
             bins = self.kwds['bins']
             if isinstance(bins, int):
                 hist_opts['num_bins'] = bins
             else:
                 hist_opts['bins'] = bins
 
         if not isinstance(y, (list, tuple)):
-            if not 'bin_range' in self.kwds:
+            if 'bin_range' not in self.kwds:
                 ys = data[y]
                 ymin, ymax = (ys.min(), ys.max())
                 if is_dask(ys):
                     ymin, ymax = ymin.compute(), ymax.compute()
                 elif is_ibis(ys):
                     ymin, ymax = ymin.execute(), ymax.execute()
                 hist_opts['bin_range'] = ymin, ymax
 
             ds = Dataset(data, self.by)
             if self.by:
-                hist = hists = histogram(
-                    ds.groupby(self.by), dimension=y, **hist_opts
-                )
+                hist = hists = histogram(ds.groupby(self.by), dimension=y, **hist_opts)
                 hist = hists.last
                 hists = hists.layout() if self.subplots else hists.overlay(sort=False)
             else:
                 hists = histogram(ds, dimension=y, **hist_opts)
 
-            return (hists.redim(**self._redim)
-                    .opts(cur_opts, backend='bokeh')
-                    .opts(compat_opts, backend=self._backend_compat))
+            return (
+                hists.redim(**self._redim)
+                .opts(cur_opts, backend='bokeh')
+                .opts(compat_opts, backend=self._backend_compat)
+            )
 
         ranges = []
         for col in y:
-            if not 'bin_range' in self.kwds:
+            if 'bin_range' not in self.kwds:
                 ys = data[col]
                 ymin, ymax = (ys.min(), ys.max())
                 if is_dask(ys):
                     ymin, ymax = ymin.compute(), ymax.compute()
                 elif is_ibis(ys):
                     ymin, ymax = ymin.execute(), ymax.execute()
                 ranges.append((ymin, ymax))
@@ -1917,37 +2358,45 @@
             hist_opts['bin_range'] = max_range(ranges)
 
         ds = Dataset(data)
         hists = []
         for col in y:
             hist = histogram(ds, dimension=col, **hist_opts)
             hists.append((col, hist.relabel(**self._relabel)))
-        return (self._by_type(hists, sort=False)
-                .redim(**self._redim)
-                .opts(cur_opts, backend='bokeh')
-                .opts(compat_opts, backend=self._backend_compat))
+        return (
+            self._by_type(hists, self.group_label, sort=False)
+            .redim(**self._redim)
+            .opts(cur_opts, backend='bokeh')
+            .opts(compat_opts, backend=self._backend_compat)
+        )
 
     def kde(self, x=None, y=None, data=None):
         self._error_if_unavailable('kde')
         bw_method = self.kwds.pop('bw_method', None)
         ind = self.kwds.pop('ind', None)
         if bw_method is not None or ind is not None:
             raise ValueError('hvplot does not support bw_method and ind')
 
         dist_opts = dict(self.kwds)
         data, x, y = self._process_chart_args(data, x, y)
         cur_opts = {
             'Distribution': self._get_opts('Distribution', backend='bokeh', **dist_opts),
             'Area': self._get_opts('Distribution', backend='bokeh'),
-            'NdOverlay': filter_opts('NdOverlay', dict(self._overlay_opts, legend_limit=0), backend='bokeh')
+            'NdOverlay': filter_opts(
+                'NdOverlay', dict(self._overlay_opts, legend_limit=0), backend='bokeh'
+            ),
         }
         compat_opts = {
-            'Distribution': self._get_opts('Distribution', backend=self._backend_compat, **dist_opts),
+            'Distribution': self._get_opts(
+                'Distribution', backend=self._backend_compat, **dist_opts
+            ),
             'Area': self._get_opts('Distribution', backend=self._backend_compat),
-            'NdOverlay': filter_opts('NdOverlay', self._overlay_opts, backend=self._backend_compat)
+            'NdOverlay': filter_opts(
+                'NdOverlay', self._overlay_opts, backend=self._backend_compat
+            ),
         }
 
         xlim = self._plot_opts.get('xlim', (None, None))
         if not isinstance(y, (list, tuple)):
             ranges = {y: xlim}
             if self.by:
                 dists = Dataset(data).to(Distribution, y, [], self.by)
@@ -1960,22 +2409,22 @@
             df = data.melt(var_name=self.group_label, value_name=self.value_label)
             ds = Dataset(df)
             if len(df):
                 dists = ds.to(Distribution, self.value_label)
                 dists = dists.layout() if self.subplots else dists.overlay(sort=False)
             else:
                 vdim = self.value_label + ' Density'
-                dists = NdOverlay({0: Area([], self.value_label, vdim)},
-                                  [self.group_label])
+                dists = NdOverlay({0: Area([], self.value_label, vdim)}, [self.group_label])
         redim = self._merge_redim(ranges)
-        return (dists
-                .redim(**redim)
-                .relabel(**self._relabel)
-                .opts(cur_opts, backend='bokeh')
-                .opts(compat_opts, backend=self._backend_compat))
+        return (
+            dists.redim(**redim)
+            .relabel(**self._relabel)
+            .opts(cur_opts, backend='bokeh')
+            .opts(compat_opts, backend=self._backend_compat)
+        )
 
     def density(self, x=None, y=None, data=None):
         return self.kde(x, y, data)
 
     ##########################
     #      Other charts      #
     ##########################
@@ -2004,16 +2453,17 @@
             self.use_index = False
             data, x, y = self._process_chart_args(data, x, y, single_y=True)
 
         redim = self._merge_redim({z[0]: self._dim_ranges['c']})
         hmap = HeatMap(data, [x, y], z, **self._relabel)
         if 'reduce_function' in self.kwds:
             hmap = hmap.aggregate(function=self.kwds['reduce_function'])
-        return (hmap.redim(**redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return hmap.redim(**redim).apply(
+            self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts
+        )
 
     def hexbin(self, x=None, y=None, data=None):
         self._error_if_unavailable('hexbin')
         self.use_index = False
         data, x, y = self._process_chart_args(data, x, y, single_y=True)
 
         z = [self.kwds['C']] if self.kwds.get('C') else []
@@ -2025,136 +2475,152 @@
         if 'gridsize' in self.kwds:
             cur_opts['gridsize'] = self.kwds['gridsize']
         if 'min_count' in self.kwds:
             cur_opts['min_count'] = self.kwds['min_count']
         redim = self._merge_redim({(z[0] if z else 'Count'): self._dim_ranges['c']})
         element = self._get_element('hexbin')
         params = dict(self._relabel)
-        if self.geo: params['crs'] = self.crs
-        return (element(data, [x, y], z or [], **params).redim(**redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        if self.geo:
+            params['crs'] = self.crs
+        return (
+            element(data, [x, y], z or [], **params)
+            .redim(**redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def bivariate(self, x=None, y=None, data=None):
         self._error_if_unavailable('bivariate')
         self.use_index = False
         data, x, y = self._process_chart_args(data, x, y, single_y=True)
 
         cur_opts, compat_opts = self._get_compat_opts('Bivariate', **self.kwds)
         element = self._get_element('bivariate')
-        return (element(data, [x, y]).redim(**self._redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return (
+            element(data, [x, y])
+            .redim(**self._redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def ohlc(self, x=None, y=None, data=None):
         self._error_if_unavailable('ohlc', Rectangles)
         self._error_if_unavailable('ohlc', Segments)
         data = self.data if data is None else data
         if x is None:
             variables = [var for var in self.variables if var not in self.indexes]
             if data[variables[0]].dtype.kind == 'M':
                 x = variables[0]
             else:
                 x = self.indexes[0]
         width = self.kwds.get('bar_width', 0.5)
         if y is None:
-            o, h, l, c = [col for col in data.columns if col != x][:4]
+            o, h, l, c = [col for col in data.columns if col != x][:4]  # noqa: E741
         else:
-            o, h, l, c = y
+            o, h, l, c = y  # noqa: E741
         neg, pos = self.kwds.get('neg_color', 'red'), self.kwds.get('pos_color', 'green')
-        color_exp = (dim(o)>dim(c)).categorize({True: neg, False: pos})
+        color_exp = (dim(o) > dim(c)).categorize({True: neg, False: pos})
         ohlc_cols = [o, h, l, c]
         if x in self.hover_cols:
             self.hover_cols.remove(x)
         vdims = list(dict.fromkeys(ohlc_cols + self.hover_cols))
         ds = Dataset(data, [x], vdims)
-        if ds.data[x].dtype.kind in 'SUO':
+        if ds.dimension_values(x).dtype.kind in 'SUO':
             rects = Rectangles(ds, [x, o, x, c])
         else:
             if len(ds):
-                sampling = np.min(np.diff(ds[x])) * width/2.
-                ds = ds.transform(lbound=dim(x)-sampling, ubound=dim(x)+sampling)
+                sampling = np.min(np.diff(ds[x])) * width / 2.0
+                ds = ds.transform(lbound=dim(x) - sampling, ubound=dim(x) + sampling)
             else:
                 ds = ds.transform(lbound=dim(x), ubound=dim(x))
             rects = Rectangles(ds, ['lbound', o, 'ubound', c])
         segments = Segments(ds, [x, l, x, h])
         rect_cur_opts, rect_compat_opts = self._get_compat_opts('Rectangles')
         rect_cur_opts.pop('tools')
         rect_cur_opts['color'] = color_exp
         seg_cur_opts, seg_compat_opts = self._get_compat_opts('Segments')
         tools = seg_cur_opts.pop('tools', [])
         if 'hover' in tools:
-            tools[tools.index('hover')] = HoverTool(tooltips=[
-                (x, f'@{x}'), ('Open', f'@{o}'), ('High', f'@{h}'),
-                ('Low', f'@{l}'), ('Close', f'@{c}')
-            ] + [(hc, f'@{hc}') for hc in vdims[4:]])
+            tools[tools.index('hover')] = HoverTool(
+                tooltips=[
+                    (x, f'@{x}'),
+                    ('Open', f'@{o}'),
+                    ('High', f'@{h}'),
+                    ('Low', f'@{l}'),
+                    ('Close', f'@{c}'),
+                ]
+                + [(hc, f'@{hc}') for hc in vdims[4:]]
+            )
         seg_cur_opts['tools'] = tools
-        seg_cur_opts ['color'] = self.kwds.get('line_color', 'black')
+        seg_cur_opts['color'] = self.kwds.get('line_color', 'black')
         if 'xlabel' not in seg_cur_opts:
             seg_cur_opts['xlabel'] = '' if x == 'index' else x
         if 'ylabel' not in seg_cur_opts:
             seg_cur_opts['ylabel'] = ''
-        segments = (
-            segments.redim(**self._redim)
-            .apply(self._set_backends_opts,
-                   cur_opts=seg_cur_opts, compat_opts=seg_compat_opts)
-        )
-        rects = (
-            rects.redim(**self._redim)
-            .apply(self._set_backends_opts,
-                   cur_opts=rect_cur_opts, compat_opts=rect_compat_opts)
+        segments = segments.redim(**self._redim).apply(
+            self._set_backends_opts, cur_opts=seg_cur_opts, compat_opts=seg_compat_opts
+        )
+        rects = rects.redim(**self._redim).apply(
+            self._set_backends_opts, cur_opts=rect_cur_opts, compat_opts=rect_compat_opts
         )
         return segments * rects
 
     def table(self, x=None, y=None, data=None):
         self._error_if_unavailable('table')
         data = self.data if data is None else data
         if isinstance(data.index, (DatetimeIndex, MultiIndex)):
             data = data.reset_index()
 
         cur_opts, compat_opts = self._get_compat_opts('Table')
         element = self._get_element('table')
-        return (element(data, self.kwds.get('columns'), []).redim(**self._redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return (
+            element(data, self.kwds.get('columns'), [])
+            .redim(**self._redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def labels(self, x=None, y=None, data=None):
         self._error_if_unavailable('labels')
         self.use_index = False
         data, x, y = self._process_chart_args(data, x, y, single_y=True)
 
         text = self.kwds.get('text')
         if not text:
             text = [c for c in data.columns if c not in (x, y)][0]
         elif text not in data.columns:
             template_str = text  # needed for dask lazy compute
-            data["label"] = data.apply(lambda row: template_str.format(**row), axis=1)
-            text = "label"
+            data['label'] = data.apply(lambda row: template_str.format(**row), axis=1)
+            text = 'label'
 
         kdims, vdims = self._get_dimensions([x, y], [text])
         cur_opts, compat_opts = self._get_compat_opts('Labels')
         element = self._get_element('labels')
-        return (element(data, kdims, vdims).redim(**self._redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return (
+            element(data, kdims, vdims)
+            .redim(**self._redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     ##########################
     #     Gridded plots      #
     ##########################
 
     def _process_gridded_args(self, data, x, y, z):
         data = self.data if data is None else data
         x = x or self.x
         y = y or self.y
         z = z or self.kwds.get('z')
 
         if is_xarray(data):
             import xarray as xr
+
             if isinstance(data, xr.DataArray):
                 data = data.to_dataset(name=data.name or 'value')
         if is_tabular(data):
-            if self.use_index and any(c for c in self.hover_cols if
-                                      c in self.indexes and
-                                      c not in data.columns):
+            if self.use_index and any(
+                c for c in self.hover_cols if c in self.indexes and c not in data.columns
+            ):
                 data = data.reset_index()
             # calculate any derived time
             dimensions = []
             for dimension in [x, y, self.by, self.hover_cols]:
                 if dimension is not None:
                     dimensions.extend(dimension if isinstance(dimension, list) else [dimension])
 
@@ -2163,14 +2629,15 @@
 
         return data, x, y, z
 
     def _get_element(self, kind):
         element = self._kind_mapping[kind]
         if self.geo:
             import geoviews
+
             element = getattr(geoviews, element.__name__)
         return element
 
     def image(self, x=None, y=None, z=None, data=None):
         self._error_if_unavailable('image')
         data, x, y, z = self._process_gridded_args(data, x, y, z)
         if not (x and y):
@@ -2180,51 +2647,58 @@
         z = [z] + self.hover_cols
 
         params = dict(self._relabel)
         cur_opts, compat_opts = self._get_compat_opts('Image')
         redim = self._merge_redim({z[0]: self._dim_ranges['c']})
 
         element = self._get_element('image')
-        if self.geo: params['crs'] = self.crs
-        return (element(data, [x, y], z, **params).redim(**redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        if self.geo:
+            params['crs'] = self.crs
+        return (
+            element(data, [x, y], z, **params)
+            .redim(**redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def rgb(self, x=None, y=None, z=None, data=None):
         self._error_if_unavailable('rgb')
         data, x, y, z = self._process_gridded_args(data, x, y, z)
 
-        coords = [c for c in data.coords if c not in self.by+self.groupby+self.grid]
+        coords = [c for c in data.coords if c not in self.by + self.groupby + self.grid]
         if len(coords) < 3:
             raise ValueError('Data must be 3D array to be converted to RGB.')
         x = x or coords[2]
         y = y or coords[1]
         bands = self.kwds.get('bands', coords[0])
         if z is None:
             z = list(data.data_vars)[0]
         data = data[z]
         nbands = len(data.coords[bands])
         if nbands < 3:
-            raise ValueError('Selected bands coordinate (%s) has only %d channels,'
-                             'expected at least three channels to convert to RGB.' %
-                             (bands, nbands))
+            raise ValueError(
+                'Selected bands coordinate (%s) has only %d channels,'
+                'expected at least three channels to convert to RGB.' % (bands, nbands)
+            )
 
         params = dict(self._relabel)
         xres, yres = data.attrs['res'] if 'res' in data.attrs else (1, 1)
         xs = data.coords[x][::-1] if xres < 0 else data.coords[x]
         ys = data.coords[y][::-1] if yres < 0 else data.coords[y]
         eldata = (xs, ys)
         for b in range(nbands):
             eldata += (data.isel(**{bands: b}).values,)
 
         element = self._get_element('rgb')
         cur_opts, compat_opts = self._get_compat_opts('RGB')
-        if self.geo: params['crs'] = self.crs
+        if self.geo:
+            params['crs'] = self.crs
         rgb = element(eldata, [x, y], element.vdims[:nbands], **params)
-        return (rgb.redim(**self._redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return rgb.redim(**self._redim).apply(
+            self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts
+        )
 
     def quadmesh(self, x=None, y=None, z=None, data=None):
         self._error_if_unavailable('quadmesh')
         data, x, y, z = self._process_gridded_args(data, x, y, z)
 
         if not (x and y):
             x, y = list(k for k, v in data.coords.items() if v.size > 1)
@@ -2233,49 +2707,58 @@
         z = [z] + self.hover_cols
 
         params = dict(self._relabel)
         redim = self._merge_redim({z[0]: self._dim_ranges['c']})
 
         element = self._get_element('quadmesh')
         cur_opts, compat_opts = self._get_compat_opts('QuadMesh')
-        if self.geo: params['crs'] = self.crs
-        return (element(data, [x, y], z, **params).redim(**redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        if self.geo:
+            params['crs'] = self.crs
+        return (
+            element(data, [x, y], z, **params)
+            .redim(**redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     def contour(self, x=None, y=None, z=None, data=None, filled=False):
         self._error_if_unavailable('contour')
         from holoviews.operation import contours
 
         if 'projection' in self._plot_opts:
             import cartopy.crs as ccrs
+
             t = self._plot_opts['projection']
             if isinstance(t, ccrs.CRS) and not isinstance(t, ccrs.Projection):
-                raise ValueError('invalid transform:'
-                                 ' Spherical contouring is not supported - '
-                                 ' consider using PlateCarree/RotatedPole.')
+                raise ValueError(
+                    'invalid transform:'
+                    ' Spherical contouring is not supported - '
+                    ' consider using PlateCarree/RotatedPole.'
+                )
 
         cur_opts, compat_opts = self._get_compat_opts('Contours')
         qmesh = self.quadmesh(x, y, z, data)
 
         if self.geo:
             # Apply projection before contouring
             import cartopy.crs as ccrs
             from geoviews import project
+
             projection = self._plot_opts.get('projection', ccrs.GOOGLE_MERCATOR)
             qmesh = project(qmesh, projection=projection)
 
         if filled:
             cur_opts['line_alpha'] = 0
         if cur_opts['colorbar']:
             cur_opts['show_legend'] = False
         levels = self.kwds.get('levels', 5)
         if isinstance(levels, int):
             cur_opts['color_levels'] = levels
-        return (contours(qmesh, filled=filled, levels=levels)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        return contours(qmesh, filled=filled, levels=levels).apply(
+            self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts
+        )
 
     def contourf(self, x=None, y=None, z=None, data=None):
         self._error_if_unavailable('contourf')
         contourf = self.contour(x, y, z, data, filled=True)
         # The holoviews contours operation used in self.contour adapts
         # the value dim range, so we need to redimension it if the user
         # has asked for it by setting `clim`. Internally an unset `clim`
@@ -2298,17 +2781,21 @@
         mag = self.kwds.get('mag')
         z = [angle, mag] + self.hover_cols
         redim = self._merge_redim({z[1]: self._dim_ranges['c']})
         params = dict(self._relabel)
 
         element = self._get_element('vectorfield')
         cur_opts, compat_opts = self._get_compat_opts('VectorField')
-        if self.geo: params['crs'] = self.crs
-        return (element(data, [x, y], z, **params).redim(**redim)
-                .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts))
+        if self.geo:
+            params['crs'] = self.crs
+        return (
+            element(data, [x, y], z, **params)
+            .redim(**redim)
+            .apply(self._set_backends_opts, cur_opts=cur_opts, compat_opts=compat_opts)
+        )
 
     ##########################
     #    Geometry plots      #
     ##########################
 
     def _geom_plot(self, x=None, y=None, data=None, kind='polygons'):
         data, x, y, _ = self._process_gridded_args(data, x, y, z=None)
@@ -2318,39 +2805,46 @@
             if is_geodataframe(data):
                 x, y = ('Longitude', 'Latitude') if self.geo else ('x', 'y')
             elif self.gridded_data:
                 x, y = self.variables[:2:-1]
             else:
                 x, y = data.columns[:2]
 
-        redim = self._merge_redim({self._color_dim: self._dim_ranges['c']} if self._color_dim else {})
+        redim = self._merge_redim(
+            {self._color_dim: self._dim_ranges['c']} if self._color_dim else {}
+        )
         kdims, vdims = self._get_dimensions([x, y], [])
         if self.gridded_data:
             vdims = Dataset(data).vdims
         element = self._get_element(kind)
         cur_opts, compat_opts = self._get_compat_opts(element.name)
         for opts_ in [cur_opts, compat_opts]:
             if 'color' in opts_ and opts_['color'] in vdims:
                 opts_['color'] = hv.dim(opts_['color'])
             # if there is nothing to put in hover, turn it off
-            if 'tools' in opts_ and kind in ["polygons", "paths"] and not vdims:
-                opts_["tools"] = [t for t in opts_["tools"] if t != "hover"]
-        if self.geo: params['crs'] = self.crs
+            if 'tools' in opts_ and kind in ['polygons', 'paths'] and not vdims:
+                opts_['tools'] = [t for t in opts_['tools'] if t != 'hover']
+        if self.geo:
+            params['crs'] = self.crs
         if self.by:
-            obj = Dataset(data, self.by+kdims, vdims).to(element, kdims, vdims, self.by, **params)
+            obj = Dataset(data, self.by + kdims, vdims).to(
+                element, kdims, vdims, self.by, **params
+            )
             if self.subplots:
                 obj = obj.layout(sort=False)
             else:
                 obj = obj.overlay(sort=False)
         else:
             obj = element(data, kdims, vdims, **params)
 
-        return (obj.redim(**redim)
-                .opts({element.name: cur_opts}, backend='bokeh')
-                .opts({element.name: compat_opts}, backend=self._backend_compat))
+        return (
+            obj.redim(**redim)
+            .opts({element.name: cur_opts}, backend='bokeh')
+            .opts({element.name: compat_opts}, backend=self._backend_compat)
+        )
 
     def polygons(self, x=None, y=None, data=None):
         self._error_if_unavailable('polygons')
         return self._geom_plot(x, y, data, kind='polygons')
 
     def paths(self, x=None, y=None, data=None):
         self._error_if_unavailable('paths')
```

### Comparing `hvplot-0.9.2rc1/hvplot/cudf.py` & `hvplot-0.9.3a1/hvplot/cudf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from .interactive import Interactive
 
+
 def patch(name='hvplot', interactive='interactive', extension='bokeh', logo=False):
     from . import hvPlotTabular, post_patch
 
     try:
         import cudf
-    except:
-        raise ImportError('Could not patch plotting API onto cuDF. '
-                          'cuDF could not be imported.')
-    _patch_plot = lambda self: hvPlotTabular(self)
+    except ImportError:
+        raise ImportError('Could not patch plotting API onto cuDF. cuDF could not be imported.')
+    _patch_plot = lambda self: hvPlotTabular(self)  # noqa: E731
     _patch_plot.__doc__ = hvPlotTabular.__call__.__doc__
     plot_prop = property(_patch_plot)
     setattr(cudf.DataFrame, name, plot_prop)
     setattr(cudf.Series, name, plot_prop)
 
-    _patch_interactive = lambda self: Interactive(self)
+    _patch_interactive = lambda self: Interactive(self)  # noqa: E731
     _patch_interactive.__doc__ = Interactive.__call__.__doc__
     interactive_prop = property(_patch_interactive)
     setattr(cudf.DataFrame, interactive, interactive_prop)
     setattr(cudf.Series, interactive, interactive_prop)
 
     post_patch(extension, logo)
 
+
 patch()
```

### Comparing `hvplot-0.9.2rc1/hvplot/dask.py` & `hvplot-0.9.3a1/hvplot/pandas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,30 @@
-import sys
+"""Adds the `.hvplot` method to pd.DataFrame and pd.Series"""
 
 from .interactive import Interactive
 
-class DaskInteractive(Interactive):
-
-    @classmethod
-    def applies(cls, obj):
-        if 'dask.dataframe' in sys.modules:
-            import dask.dataframe as dd
-            return isinstance(obj, (dd.Series, dd.DataFrame))
-        return False
-
-    def compute(self):
-        self._method = 'compute'
-        return self.__call__()
-
 
 def patch(name='hvplot', interactive='interactive', extension='bokeh', logo=False):
     from . import hvPlotTabular, post_patch
 
     try:
-        import dask.dataframe as dd
-    except:
-        raise ImportError('Could not patch plotting API onto dask. '
-                          'Dask could not be imported.')
-    _patch_plot = lambda self: hvPlotTabular(self)
+        import pandas as pd
+    except ImportError:
+        raise ImportError(
+            'Could not patch plotting API onto pandas. Pandas could not be imported.'
+        )
+    _patch_plot = lambda self: hvPlotTabular(self)  # noqa: E731
     _patch_plot.__doc__ = hvPlotTabular.__call__.__doc__
     plot_prop = property(_patch_plot)
-    setattr(dd.DataFrame, name, plot_prop)
-    setattr(dd.Series, name, plot_prop)
+    setattr(pd.DataFrame, name, plot_prop)
+    setattr(pd.Series, name, plot_prop)
 
-    _patch_interactive = lambda self: DaskInteractive(self)
-    _patch_interactive.__doc__ = DaskInteractive.__call__.__doc__
+    _patch_interactive = lambda self: Interactive(self)  # noqa: E731
+    _patch_interactive.__doc__ = Interactive.__call__.__doc__
     interactive_prop = property(_patch_interactive)
-    setattr(dd.DataFrame, interactive, interactive_prop)
-    setattr(dd.Series, interactive, interactive_prop)
+    setattr(pd.DataFrame, interactive, interactive_prop)
+    setattr(pd.Series, interactive, interactive_prop)
 
     post_patch(extension, logo)
 
+
 patch()
```

### Comparing `hvplot-0.9.2rc1/hvplot/examples/reference/geopandas/points.ipynb` & `hvplot-0.9.3a1/doc/reference/tabular/area.ipynb`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9520833333333334%*

 * *Differences: {"'cells'": "{2: {'source': ['`area` can be used to color the area under a line or to color the "*

 * *            "space between two lines. ']}, 3: {'source': {insert: [(0, 'from "*

 * *            "bokeh.sampledata.degrees import data\\n'), (2, 'data.tail()')], delete: [3, 2, 0]}}, "*

 * *            "6: {'source': ['import pandas as pd\\n', 'from bokeh.sampledata.stocks import "*

 * *            'MSFT\\n\', \'\\n\', \'df = pd.DataFrame(MSFT)\\n\', "df[\'date\'] = '*

 * *            'pd.to_datetime(df.date)\\n", \'df.head()\']},  […]*

```diff
@@ -1,85 +1,124 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Area"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import hvplot.pandas  # noqa"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Using hvplot with geopandas is as simple as loading a geopandas dataframe and calling `hvplot` on it with `geo=True`."
+                "`area` can be used to color the area under a line or to color the space between two lines. "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import geopandas as gpd\n",
+                "from bokeh.sampledata.degrees import data\n",
                 "\n",
-                "cities = gpd.read_file(gpd.datasets.get_path('naturalearth_cities'))\n",
-                "cities.sample(5)"
+                "data.tail()"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "First we'll look at a single curve, where we are enforcing the y axis must be between 0 and 100 and we set the background color."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cities.hvplot(geo=True, tiles=True)"
+                "data.hvplot.area(\n",
+                "    x='Year', y='Computer Science',\n",
+                "    label='% of Computer Science Degrees Earned by Women',\n",
+                "    ylim=(0, 100), width=500, height=400, bgcolor='goldenrod',\n",
+                ")"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import pandas as pd\n",
+                "from bokeh.sampledata.stocks import MSFT\n",
+                "\n",
+                "df = pd.DataFrame(MSFT)\n",
+                "df['date'] = pd.to_datetime(df.date)\n",
+                "df.head()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "You can easily change the tiles, add coastlines, or which fields show up in the hover text:"
+                "To color the area between two curves, include both a `y` and a `y2`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cities.hvplot(tiles='EsriTerrain', coastline=True, hover_cols='all')"
+                "df[df.date.dt.year == 2000].hvplot.area(x='date', y='low', y2='high')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We can also alter the projection of the data using cartopy:"
+                "When multiple y values are passed, they are stacked by default."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import cartopy.crs as ccrs"
+                "df.hvplot.area(x='date', y=['open', 'close'])"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Area plots can also be unstacked:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "cities.hvplot(coastline=True, projection=ccrs.Geostationary(central_longitude=-30), global_extent=True)"
+                "df.hvplot.area(x='date', y=['open', 'close'], stacked=False,\n",
+                "               groupby='date.year', legend='bottom_right', width=500)"
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/hvplot/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Geographic_Data.ipynb`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9422102631071128%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'import xarray as xr\\n')], delete: [3, 0]}}, 2: "*

 * *            "{'source': {insert: [(0, '## Introduction\\n'), (2, 'hvPlot can display geographic "*

 * *            "data and can be used to add contextualisation layers:\\n'), (4, '- Overlay the data "*

 * *            "over a tiled web map\\n'), (5, '- Overlay the data over geographic/administrative "*

 * *            "features\\n'), (6, '- Plot the data in a specific projection\\n'), (8, 'Many, but not "*

 * *            'all, of the […]*

```diff
@@ -1,40 +1,72 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Geographic Data"
+            ]
+        },
+        {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import xarray as xr\n",
                 "import hvplot.pandas  # noqa\n",
                 "import hvplot.xarray  # noqa\n",
-                "import cartopy.crs as ccrs\n",
+                "import xarray as xr\n",
                 "\n",
                 "from bokeh.sampledata.airport_routes import airports"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Installation\n",
+                "## Introduction\n",
+                "\n",
+                "hvPlot can display geographic data and can be used to add contextualisation layers:\n",
+                "\n",
+                "- Overlay the data over a tiled web map\n",
+                "- Overlay the data over geographic/administrative features\n",
+                "- Plot the data in a specific projection\n",
                 "\n",
-                "The plot API also has support for geographic data built on top of Cartopy and GeoViews. Both can be installed using conda with:\n",
+                "Many, but not all, of these features require [GeoViews](https://geoviews.org) to be installed, which is the geographic extension of HoloViews built on [Cartopy](https://scitools.org.uk/cartopy) and [pyproj](https://pyproj4.github.io/pyproj). You can install GeoViews with `pip install geoviews` or `conda install geoviews`.\n",
                 "\n",
-                "    conda install geoviews\n",
-                "    \n",
-                "or with pip:\n",
+                "Before plotting geographical data, you should know in which [coordinate system](https://en.wikipedia.org/wiki/Spatial_reference_system) the data is represented. This is important for a few reasons:\n",
                 "\n",
-                "    pip install geoviews\n",
+                "- The data may have to be [projected](https://en.wikipedia.org/wiki/Map_projection) to another coordinate system, and to do so you may have to provide the original coordinate system.\n",
+                "- Projecting data can be a computationally expensive operation and you should be aware of when this operation happens, to perhaps optimize it.\n",
                 "\n",
-                "## Usage\n",
+                "Here are two common coordinate systems you will encounter when dealing with geographic data and using hvPlot:\n",
                 "\n",
-                "Only certain hvPlot types support geographic coordinates, currently including: 'points', 'polygons', 'paths', 'image', 'quadmesh', 'contour', and 'contourf'. As an initial example, consider a dataframe of all US airports (including military bases overseas):"
+                "- Data represented by latitude/longitude (lat/lon) coordinates are often tied to the WGS84 geographic coordinate system ([EPSG:4326](https://epsg.io/4326)), that's how GPS data are located on the Earth. For example, the coordinates of Paris in this system are `(lat=48.856697, lon=2.351462)`.\n",
+                "- Tiled web maps are displayed in the Web Mercator projection (also known as Pseudo-Mercator or Google Mercator, [EPSG:3857](https://epsg.io/3857)). Unlike WGS84 which expresses coordinates in lat/long decimal degrees, Web Mercator expresses them in easting (X) /northing (Y) metric units. For example, the coordinates of Paris in this system are `(easting=261763.552, northing=6250580.761)`."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Supported plot types\n",
+                "\n",
+                "Only certain hvPlot types support geographic coordinates, currently including: `points`, `polygons`, `paths`, `image`, `quadmesh`, `contour`, and `contourf`."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Tiled web map\n",
+                "\n",
+                "A [tiled web map](https://en.wikipedia.org/wiki/Tiled_web_map), or tile map, is an interactive map displayed on a web browser that is divided into small, pre-rendered image tiles, allowing for efficient loading and seamless navigation across various zoom levels and geographic areas. hvPlot allows to add a tile map as a basemap to a plot with the `tiles` parameter. Importantly, `tiles` is a parameter that can be used **without installing GeoViews if the data is already projected in Web Mercator**.\n",
+                "\n",
+                "We'll display this dataframe of all US airports (including military bases overseas), the points are expressed in latitude/longitude coordinates:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -42,234 +74,357 @@
                 "airports.head(3)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Plotting points\n",
+                "We'll first start by displaying the airports **without GeoViews**. To do so, we must convert the coordinates to Web Mercator, which can be easily achieved using the `lon_lat_to_easting_northing` function provided by HoloViews, that doesn't require installing any of the usual geo dependencies like `pyproj` or `cartopy`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "from holoviews.util.transform import lon_lat_to_easting_northing\n",
                 "\n",
-                "If we want to overlay our data on geographic maps or reproject it into a geographic plot, we can set ``geo=True``, which declares that the data will be plotted in a geographic coordinate system.  The default coordinate system is the ``PlateCarree`` projection, i.e., raw longitudes and latitudes. If the data is in another coordinate system, you will need to [declare an explicit ``crs``](#declaring-a-crs) as an argument, in which case `geo=True` is assumed.  Once hvPlot knows that your data is in geo coordinates, you can use the ``tiles`` option to overlay a the plot on top of map tiles."
+                "airports['x'], airports['y'] = lon_lat_to_easting_northing(airports.Longitude, airports.Latitude)\n",
+                "airports[['Latitude', 'Longitude', 'x', 'y']].head(3)"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "We can now easily display the airports on a basemap by setting `tiles` to `True`."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "airports.hvplot.points('Longitude', 'Latitude', geo=True, color='red', alpha=0.2,\n",
-                "                       xlim=(-180, -30), ylim=(0, 72), tiles='ESRI')"
+                "airports.hvplot.points('x', 'y', tiles=True, color='red', alpha=0.2)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Declaring a CRS\n",
-                "\n",
-                "To declare a geographic plot we have to supply a ``cartopy.crs.CRS`` (or coordinate reference system).  Coordinate reference systems are described in the [GeoViews documentation](https://geoviews.org/user_guide/Projections.html) and the full list of available CRSs is in the [cartopy documentation](https://scitools.org.uk/cartopy/docs/v0.15/crs/projections.html). "
+                "A common mistake is to display data referenced in WGS84 on a tile basemap without projecting the data to Web Mercator. In doing so, the data will be plotted around the [null island location](https://en.wikipedia.org/wiki/Null_Island), roughly 600km off the coast of West Africa."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "airports.hvplot.points(\n",
+                "    'Longitude', 'Latitude', tiles=True, color='red', alpha=0.2,\n",
+                "    xlim=(-1000000, 1000000), ylim=(-1000000, 1000000)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Geopandas\n",
-                "\n",
-                "Since a GeoPandas ``DataFrame`` is just a Pandas DataFrames with additional geographic information, it inherits the ``.hvplot`` method. We can thus easily load shapefiles and plot them on a map:"
+                "When **GeoViews** is installed, you can set `geo=True` to let hvPlot know that it can leverage it to display the data. You can directly plot the airports without having to project the data yourself, GeoViews will take care of projecting it to Web Mercator automatically."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import geopandas as gpd\n",
-                "\n",
-                "cities = gpd.read_file(gpd.datasets.get_path('naturalearth_cities'))\n",
-                "\n",
-                "cities.hvplot(global_extent=True, frame_height=450, tiles=True)"
+                "airports.hvplot.points(\n",
+                "    'Longitude', 'Latitude', geo=True, tiles=True, color='red', alpha=0.2\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The GeoPandas support allows plotting ``GeoDataFrames`` containing ``'Point'``, ``'Polygon'``, ``'LineString'`` and ``'LineRing'`` geometries, but not ones containing a mixture of different geometry types. Calling ``.hvplot`` will automatically figure out the geometry type to plot, but it also possible to call ``.hvplot.points``, ``.hvplot.polygons``, and ``.hvplot.paths`` explicitly.\n",
+                "The easiest ways to set `tiles` include:\n",
                 "\n",
-                "To draw multiple GeoDataFrames onto the same plot, use the ``*`` operator:"
+                "- to `True` to get the default layer which currently is from OpenStreetMap (prefer one of the explicit approaches below if you care about reproducibility)\n",
+                "- with an `xyzservices.TileProvider` instance that can be created from the optional dependency [xyzservices](https://xyzservices.readthedocs.io/) which gives you access to hundreds of tiled web maps\n",
+                "- with the name of one the layers shipped by HoloViews and GeoViews (when it's installed), like `'EsriTerrain'`.\n",
+                "\n",
+                "The tile map can be additionally configured by setting `tiles_opts` with a dictionary of options that will be applied to the basemap layer."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "world = gpd.read_file(gpd.datasets.get_path('naturalearth_lowres'))\n",
-                "\n",
-                "world.hvplot(geo=True) * cities.hvplot(geo=True, color='orange')"
+                "import xyzservices.providers as xyz"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "airports.hvplot.points(\n",
+                "    'x', 'y', tiles=xyz.Esri.WorldPhysical, tiles_opts={'alpha': 0.5}, color='red', alpha=0.2\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "It is possible to declare a specific column to use as color with the ``c`` keyword:"
+                "## Data and plot projections"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "world.hvplot(geo=True) + world.hvplot(c='continent', geo=True)"
+                "import cartopy.crs as ccrs "
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Spatialpandas\n",
+                "As we have seen in the previous section, you can set `geo=True` to let hvPlot know that your data is geographic. GeoViews **must be installed** when setting `geo=True`, or when any of the other geographic options is set, except `tiles`. In this mode hvPlot:\n",
                 "\n",
-                "Spatialpandas is another powerful library for working with geometries and is optimized for rendering with datashader, making it possible to plot millions of individual geometries very quickly:"
+                "1. Assumes the data is expressed in lat/lon coordinates. Internally, hvPlot assumes a [Plate Carr\u00e9e](https://en.wikipedia.org/wiki/Equirectangular_projection) projection, also known as the *equirectangular projection*.\n",
+                "2. Displays the data in the projection *Plate Carr\u00e9e* assumed in step (1), or, if `tiles=True`, projects and displays the data in the Web Mercator projection.\n",
+                "\n",
+                "The *input* data projection assumed in step (1), and the *output* plot projection used in step (2) can both be overridden with the `crs` (for Coordinate Reference System) and `projection` parameters, respectively. Both parameters accept cartopy `CRS` objects (see the full list of values they accept in their definition). You can now see that that setting `geo=True, tiles=True` is strictly equivalent to setting `crs=ccrs.PlateCarree(), projection=ccrs.GOOGLE_MERCATOR`! Coordinate reference systems are described in more details in the [GeoViews documentation](https://geoviews.org/user_guide/Projections.html) and the full list of available CRSs is in the [cartopy documentation](https://scitools.org.uk/cartopy/docs/latest/reference/projections.html).\n",
+                "\n",
+                "For example, we can set `projection` to display the airports on an Orthographic projection centered over North America."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import spatialpandas as spd\n",
-                "\n",
-                "spd_world = spd.GeoDataFrame(world)\n",
-                "\n",
-                "spd_world.hvplot(datashade=True, project=True, aggregator='count_cat', c='continent', color_key='Category10')"
+                "airports.hvplot.points(\n",
+                "    'Longitude', 'Latitude', color='red', alpha=0.2,\n",
+                "    coastline=True, projection=ccrs.Orthographic(-90, 30)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "### Declaring an output projection"
+                "## Raster data"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "air_ds = xr.tutorial.open_dataset('air_temperature').load()\n",
+                "air_ds"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The ``crs=`` argument specifies the *input* projection, i.e. it declares how to interpret the incoming data values. You can independently choose any *output* projection, i.e. how you want to map the data points onto the screen for display, using the ``projection=`` argument. After loading the same temperature dataset explored in the [Gridded Data](Gridded_Data.ipynb) section, the data can be displayed on an Orthographic projection:"
+                "When displaying raster data in a projection other than the one in which the data is stored, it is more accurate to render it as a `quadmesh` rather than an `image`. As you can see below, a QuadMesh will project each original bin or pixel into the correct non-rectangular shape determined by the projection, accurately showing the geographic extent covered by each sample. An Image, on the other hand, will always be rectangularly aligned in the 2D plane, which requires warping and resampling the data in a way that allows efficient display but loses accuracy at the pixel level."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "air_ds = xr.tutorial.open_dataset('air_temperature').load()\n",
+                "air_ds.isel(time=0).hvplot.quadmesh('lon', 'lat', 'air', projection=ccrs.LambertConformal())"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "Unfortunately, rendering a large QuadMesh using Bokeh can be very slow, but there are two useful alternatives for datasets too large to be practical as native QuadMeshes.\n",
                 "\n",
-                "air_ds.hvplot.quadmesh(\n",
-                "    'lon', 'lat', 'air', projection=ccrs.Orthographic(-90, 30),\n",
-                "    global_extent=True, frame_height=540, cmap='viridis',\n",
-                "    coastline=True\n",
+                "The first is using the `rasterize` or `datashade` options to regrid the data before rendering it, i.e., rendering the data on the backend and then sending a more efficient image-based representation to the browser. One thing to note when using these operations is that it may be necessary to project the data **before** rasterizing it, e.g. to address wrapping issues. To do this provide `project=True`, which will project the data before it is rasterized (this also works for other types and even when not using these operations). Another reason why this is important when rasterizing the data is that if the CRS of the data does not match the displayed projection, all the data will be projected every time you zoom or pan, which can be very slow. Deciding whether to `project` is therefore a tradeoff between projecting the raw data ahead of time or accepting the overhead on dynamic zoom and pan actions."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "rasm = xr.tutorial.open_dataset('rasm').load().isel(time=0)\n",
+                "rasm"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "rasm.hvplot.quadmesh(\n",
+                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.GOOGLE_MERCATOR,\n",
+                "    tiles=xyz.Esri.WorldGrayCanvas, project=True, rasterize=True,\n",
+                "    xlim=(-20, 40), ylim=(30, 70), cmap='viridis', frame_width=400,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "If you don't need to pass any keyword arguments to a given projection and you don't have cartopy.crs (ccrs) imported, you can use the string representation: e.g. ``'LambertConformal'`` instead of ``ccrs.LambertConformal()``. Note that it is case sensitive!"
+                "The second option that's still relatively slow for larger data but avoids sending large data into your browser is to plot the data using `contour` and `contourf` visualizations, generating a line or filled contour with a discrete number of levels:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "air_ds.hvplot.quadmesh(\n",
-                "    'lon', 'lat', 'air', projection='LambertConformal',\n",
+                "rasm.hvplot.contourf(\n",
+                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.GOOGLE_MERCATOR,\n",
+                "    tiles=xyz.Esri.WorldGrayCanvas, levels=10,\n",
+                "    xlim=(-20, 40), ylim=(30, 70), cmap='viridis', frame_width=400,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Note that when displaying raster data in a projection other than the one in which the data is stored, it is more accurate to render it as a ``quadmesh`` rather than an ``image``. As you can see above, a QuadMesh will project each original bin or pixel into the correct non-rectangular shape determined by the projection, accurately showing the geographic extent covered by each sample. An Image, on the other hand, will always be rectangularly aligned in the 2D plane, which requires warping and resampling the data in a way that allows efficient display but loses accuracy at the pixel level. Unfortunately, rendering a large QuadMesh using Bokeh can be very slow, but there are two useful alternatives for datasets too large to be practical as native QuadMeshes.\n",
+                "## Geopandas usage\n",
                 "\n",
-                "The first is using the ``rasterize`` or ``datashade`` options to regrid the data before rendering it, i.e., rendering the data on the backend and then sending a more efficient image-based representation to the browser. One thing to note when using these operations is that it may be necessary to project the data **before** rasterizing it, e.g. to address wrapping issues. To do this provide ``project=True``, which will project the data before it is rasterized (this also works for other types and even when not using these operations). Another reason why this is important when rasterizing the data is that if the CRS of the data does not match the displayed projection, all the data will be projected every time you zoom or pan, which can be very slow. Deciding whether to ``project`` is therefore a tradeoff between projecting the raw data ahead of time or accepting the overhead on dynamic zoom and pan actions."
+                "Since a GeoPandas `DataFrame` is just a Pandas DataFrames with additional geographic information, it inherits the `.hvplot` method. We can thus easily load geographic files (GeoJSON, Shapefiles, etc) and plot them on a map:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rasm = xr.tutorial.open_dataset('rasm').load()\n",
-                "\n",
-                "\n",
-                "\n",
-                "rasm.hvplot.quadmesh(\n",
-                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.PlateCarree(),\n",
-                "    ylim=(0, 90), cmap='viridis', project=True, geo=True,\n",
-                "    rasterize=True, coastline=True, frame_width=800, dynamic=False,\n",
-                ")"
+                "import geopandas as gpd\n",
+                "import geodatasets"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "path = geodatasets.get_path(\"geoda.nyc_neighborhoods\")\n",
+                "path"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "nyc = gpd.read_file(path)\n",
+                "nyc.head(3)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "nyc.hvplot(geo=True, tiles=True, c=\"poptot\", alpha=0.8, tiles_opts={'alpha': 0.5})"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Another option that's still relatively slow for larger data but avoids sending large data into your browser is to plot the data using ``contour`` and ``contourf`` visualizations, generating a line or filled contour with a discrete number of levels:"
+                "The GeoPandas support allows plotting `GeoDataFrames` containing `'Point'`, `'Polygon'`, `'LineString'` and `'LineRing'` geometries, but not ones containing a mixture of different geometry types. Calling `.hvplot` will automatically figure out the geometry type to plot, but it also possible to call `.hvplot.points`, `.hvplot.polygons`, and `.hvplot.paths` explicitly."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "## Spatialpandas usage\n",
+                "\n",
+                "Spatialpandas is another powerful library for working with geometries and is optimized for rendering with datashader, making it possible to plot millions of individual geometries very quickly:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "rasm.hvplot.contourf(\n",
-                "    'xc', 'yc', crs=ccrs.PlateCarree(), projection=ccrs.PlateCarree(),\n",
-                "    ylim=(0, 90), frame_width=800, cmap='viridis', levels=10,\n",
-                "    coastline=True\n",
+                "import spatialpandas as spd\n",
+                "\n",
+                "spd_nyc = spd.GeoDataFrame(nyc)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "spd_nyc.hvplot(\n",
+                "    datashade=True, project=True, aggregator='count_cat',\n",
+                "    c='boroname', color_key='Category10'\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "As you can see, hvPlot makes it simple to work with geographic data visually.  For more complex plot types and additional details, see the [GeoViews](https://geoviews.org) documentation."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Geographic options\n",
+                "## Options\n",
                 "\n",
                 "The API provides various geo-specific options:\n",
                 "\n",
-                "- ``coastline`` (default=False): Whether to display a coastline on top of the plot, setting ``coastline='10m'/'50m'/'110m'`` specifies a specific scale\n",
-                "- ``crs`` (default=None): Coordinate reference system of the data specified as Cartopy CRS object, proj.4 string or EPSG code\n",
-                "- ``features`` features (default=None): A list of features or a dictionary of features and the scale at which to render it. Available features include 'borders', 'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'. Available scales include '10m'/'50m'/'110m'.\n",
-                "- ``geo`` (default=False): Whether the plot should be treated as geographic (and assume PlateCarree, i.e. lat/lon coordinates)\n",
-                "- ``global_extent`` (default=False): Whether to expand the plot extent to span the whole globe\n",
-                "- ``project`` (default=False): Whether to project the data before plotting (adds initial overhead but avoids projecting data when plot is dynamically updated)\n",
-                "- ``tiles`` (default=False): Whether to overlay the plot on a tile source. Tiles sources can be selected by name, the default is 'Wikipedia'.\n",
-                "Other options are: 'CartoDark', 'CartoEco', 'CartoLight', 'CartoMidnight', 'EsriImagery', 'EsriNatGeo', 'EsriReference''EsriTerrain', 'EsriUSATopo', 'OSM', 'StamenLabels', 'StamenTerrain', 'StamenTerrainRetina', 'StamenToner', 'StamenTonerBackground', 'StamenWatercolor'. Stamen tile sources require a Stadia account when not running locally; see [stadiamaps.com](https://stadiamaps.com/)."
+                "- `coastline` (default=False): Whether to display a coastline on top of the plot, setting `coastline='10m'/'50m'/'110m'` specifies a specific scale\n",
+                "- `crs` (default=None): Coordinate reference system of the data (input projection) specified as an EPSG code (int or string), pyproj CRS or Proj object, Cartopy CRS object, proj.4 string, or WKT string. Defaults to PlateCarree.\n",
+                "- `features` features (default=None): A list of features or a dictionary of features and the scale at which to render it. Available features include 'borders', 'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'. Available scales include '10m'/'50m'/'110m'.\n",
+                "- `geo` (default=False): Whether the plot should be treated as geographic (and assume PlateCarree, i.e. lat/lon coordinates)\n",
+                "- `global_extent` (default=False): Whether to expand the plot extent to span the whole globe\n",
+                "- `project` (default=False): Whether to project the data before plotting (adds initial overhead but avoids projecting data when plot is dynamically updated)\n",
+                "- `projection` (default=None): Coordinate reference system of the plot (output projection) specified as Cartopy CRS object or name.\n",
+                "- `tiles` (default=False): Whether to overlay the plot on a tile source. Accept the following values:\n",
+                "    - `True`: OpenStreetMap layer\n",
+                "    - `xyzservices.TileProvider` instance (requires [`xyzservices`](https://xyzservices.readthedocs.io/) to be installed)\n",
+                "    - a map string name based on one of the default layers made available by [HoloViews](https://holoviews.org/reference/elements/bokeh/Tiles.html) ('CartoDark', 'CartoLight', 'EsriImagery', 'EsriNatGeo', 'EsriUSATopo', 'EsriTerrain', 'EsriStreet', 'EsriReference', 'OSM', 'OpenTopoMap') or [GeoViews](https://geoviews.org/user_guide/Working_with_Bokeh.html) ('CartoDark', 'CartoEco', 'CartoLight', 'CartoMidnight', 'EsriImagery', 'EsriNatGeo', 'EsriUSATopo', 'EsriTerrain', 'EsriReference', 'EsriOceanBase', 'EsriOceanReference', 'EsriWorldPhysical', 'EsriWorldShadedRelief', 'EsriWorldTopo', 'EsriWorldDarkGrayBase', 'EsriWorldDarkGrayReference', 'EsriWorldLightGrayBase', 'EsriWorldLightGrayReference', 'EsriWorldHillshadeDark', 'EsriWorldHillshade', 'EsriAntarcticImagery', 'EsriArcticImagery', 'EsriArcticOceanBase', 'EsriArcticOceanReference', 'EsriWorldBoundariesAndPlaces', 'EsriWorldBoundariesAndPlacesAlternate', 'EsriWorldTransportation', 'EsriDelormeWorldBaseMap', 'EsriWorldNavigationCharts', 'EsriWorldStreetMap', 'OSM', 'OpenTopoMap'). Note that Stamen tile sources require a Stadia account when not running locally; see [stadiamaps.com](https://stadiamaps.com/).\n",
+                "    - a `holoviews.Tiles` or `geoviews.WMTS` instance or class\n",
+                "- `tiles_opts` (default=None): Dictionary of plotting options to customize the tiles layer created when `tiles` is set, e.g. `dict(alpha=0.5)`."
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
```

### Comparing `hvplot-0.9.2rc1/hvplot/examples/user_guide/NetworkX.ipynb` & `hvplot-0.9.3a1/doc/user_guide/Large_Timeseries.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8214190646673767%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Large Timeseries Data\\n'), (2, 'Effectively "*

 * *            'representing temporal dynamics in large datasets requires selecting appropriate '*

 * *            'visualization techniques that ensure responsiveness while providing both a '*

 * *            'macroscopic view of overall trends and a microscopic view of fine details. This guide '*

 * *            'will explore various methods, such as **WebGL Rendering**, **LTTB Downsampling**, '*

 * *            '**Datashader Rasterizing […]*

```diff
@@ -1,759 +1,462 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "artificial-english",
             "metadata": {},
             "source": [
-                "The hvPlot NetworkX plotting API is meant as a drop-in replacement for the ``networkx.draw`` methods. In most cases the existing code will work as is or with minor modifications, returning a HoloViews object rendering an interactive bokeh plot, equivalent to the matplotlib plot the standard API constructs. First let us import the plotting interface and give it the canonical name ``hvnx``:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import hvplot.networkx as hvnx\n",
+                "# Large Timeseries Data\n",
+                "\n",
+                "Effectively representing temporal dynamics in large datasets requires selecting appropriate visualization techniques that ensure responsiveness while providing both a macroscopic view of overall trends and a microscopic view of fine details. This guide will explore various methods, such as **WebGL Rendering**, **LTTB Downsampling**, **Datashader Rasterizing**, and **Minimap Contextualizing**, each suited for different aspects of large timeseries data visualization. We predominantly demonstrate the use of hvPlot syntax, leveraging HoloViews for more complex requirements. Although hvPlot supports multiple backends, including Matplotlib and Plotly, our focus will be on Bokeh due to its advanced capabilities in handling large timeseries data.\n",
                 "\n",
-                "import networkx as nx\n",
-                "import holoviews as hv"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "In this user guide we will follow along with many of the examples in the [NetworkX tutorial](https://networkx.github.io/documentation/stable/tutorial.html#drawing-graphs) on drawing graphs.\n",
                 "\n",
-                "The ``hxnx`` namespace provides all the same plotting functions as ``nx``, this means in most cases one can simply be swapped for the other. This also includes most keywords used to customize the plots. The main difference is in the way multiple plots are composited, like all other hvPlot APIs the networkX functions returns HoloViews objects which can be composited using ``+`` and ``*`` operations:"
+                "## Getting the data \n",
+                "\n",
+                "Here we have a DataFrame with 1.2 million rows containing standardized data from 5 different sensors."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "arabic-container",
             "metadata": {},
             "outputs": [],
             "source": [
-                "G = nx.petersen_graph()\n",
-                "\n",
-                "spring = hvnx.draw(G, with_labels=True)\n",
-                "shell = hvnx.draw_shell(G, nlist=[range(5, 10), range(5)], with_labels=True, font_weight='bold')\n",
+                "import pandas as pd\n",
                 "\n",
-                "spring + shell"
+                "df = pd.read_parquet(\"https://datasets.holoviz.org/sensor/v1/data.parq\")\n",
+                "df.sample(5)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "banned-richards",
             "metadata": {},
             "outputs": [],
             "source": [
-                "H = nx.triangular_lattice_graph(1, 20)\n",
-                "hvnx.draw_planar(H, node_color='green', edge_color='brown')"
+                "df0 = df[df.sensor=='0']"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "fourth-sentence",
             "metadata": {},
             "source": [
-                "The most common ``layout`` functions have dedicated drawing methods such as the ``draw_shell`` function above, which automatically computes the node positions.\n",
+                "Let's go ahead and plot this data using various approaches.\n",
+                "\n",
+                "## WebGL Rendering\n",
+                "\n",
+                "[WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API) is a JavaScript API that allows rendering content in the browser using hardware acceleration from a Graphics Processing Unit (GPU). WebGL is standardized and available in all modern browsers.\n",
                 "\n",
-                "However layout algorithms are not necessarily deterministic, so if we want to plot and overlay subsets of either the nodes or edges using the ``nodelist`` and ``edgelist`` keywords the node positions should be computed ahead of time and passed in explicitly:"
+                "### Canvas Rendering - Prior Default\n",
+                "\n",
+                "Rendering Bokeh plots in hvPlot or HoloViews has evolved significantly. Prior to 2023, Bokeh's custom HTML **Canvas** rendering was the default. This approach works well for datasets up to a few tens of thousands of points but struggles above 100K points, particularly in terms of zooming and panning speed. These days, if you want to utilize Bokeh's Canvas rendering, use `import holoviews as hv; hv.renderer(\"bokeh\").webgl = False` prior to creating your hvPlot or HoloViews object.\n",
+                "\n",
+                "### WebGL Rendering - Current Default\n",
+                "\n",
+                "Around mid-2023, the adoption of improved **WebGL** as the default for hvPlot and HoloViews allowed for smoother interactions with larger datasets by utilizing GPU-acceleration. It's important to note that WebGL performance can vary based on your machine's specifications. For example, some Apple Mac models may not exhibit a marked improvement in WebGL performance over Canvas due to GPU hardware configuration."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "constitutional-metabolism",
             "metadata": {},
             "outputs": [],
             "source": [
-                "pos = nx.layout.spring_layout(G)\n",
+                "import holoviews as hv\n",
+                "import hvplot.pandas  # noqa\n",
                 "\n",
-                "hvnx.draw(G, pos, nodelist=[0, 1, 2, 3, 4], node_color='blue') *\\\n",
-                "hvnx.draw_networkx_nodes(G, pos, nodelist=[5, 6, 7, 8, 9], node_color='green')"
+                "# Set notebook hvPlot/HoloViews default options\n",
+                "hv.opts.defaults(hv.opts.Curve(responsive=True))\n",
+                "\n",
+                "df0.hvplot(x=\"time\", y=\"value\", autorange='y', title=\"WebGL\", min_height=300)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "428042ef",
             "metadata": {},
             "source": [
-                "The `hvnx` namespace also makes `save` and `show` utilities available to save the plot to HTML or PNG files or display it in a separate browser window when working in a standard Python interpreter."
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "G = nx.dodecahedral_graph()\n",
-                "\n",
-                "shells = [[2, 3, 4, 5, 6], [8, 1, 0, 19, 18, 17, 16, 15, 14, 7], [9, 10, 11, 12, 13]]\n",
-                "shell = hvnx.draw_shell(G, nlist=shells)\n",
+                "<div class=\"alert alert-info\">\n",
                 "\n",
-                "pos = nx.nx_agraph.graphviz_layout(G)\n",
-                "graphviz = hvnx.draw(G, pos=pos)\n",
+                "<b>Note:</b> `autorange='y'` is demonstrated here for automatic y-axis scaling, a feature from HoloViews 1.17 and hvPlot 0.9.0. You can omit that option if you prefer to set the y scaling manually using the zoom tool.\n",
                 "\n",
-                "layout = shell + graphviz\n",
-                "\n",
-                "hvnx.save(layout, 'graph_layout.png')"
+                "</div>"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "directed-proof",
             "metadata": {},
             "source": [
-                "#### Styling Graphs\n",
+                "Alone, both Canvas and WebGL rendering have a common limitation: they transfer the entire dataset from the server to the browser. This can be a significant bottleneck, especially for remote server setups or datasets larger than a million points. To address this, we'll explore other techniques like LTTB Downsampling, which focus on delivering only the necessary data for the current view. These methods offer more scalable solutions for interacting with large timeseries data, as we'll see in the following sections.\n",
+                "\n",
+                "## LTTB Downsampling\n",
                 "\n",
-                "The full set of options which are inherited from networkx's API are listed in the ``hxnx.draw()`` docstring. Using these the more common styling of nodes and edges can easily be altered through the common set of options that are inherited from networkx. In addition common HoloViews options to control the size of the plots, axes and styling are also supported. Finally, some ``layout`` functions also accept special keyword arguments such as the ``nlist`` argument for the shell layout which specifies the shells."
+                "### The Challenge with Simple Downsampling\n",
+                "\n",
+                "A straightforward approach to handling large datasets might involve plotting every _n_th datapoint using a method like `df.sample`:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "conservative-maldives",
             "metadata": {},
             "outputs": [],
             "source": [
-                "options = {\n",
-                "    'node_color': 'black',\n",
-                "    'node_size': 100,\n",
-                "    'edge_width': 3,\n",
-                "    'width': 300,\n",
-                "    'height': 300\n",
-                "}\n",
-                "\n",
-                "random = hvnx.draw_random(G, **options)\n",
-                "circular = hvnx.draw_circular(G, **options)\n",
-                "spectral = hvnx.draw_spectral(G, **options)\n",
-                "shell = hvnx.draw_shell(G, nlist=[range(5,10), range(5)], **options)\n",
-                "\n",
-                "(random + circular + spectral + shell).cols(2)"
+                "df0.hvplot(x=\"time\", y=\"value\", color= '#003366', label = \"All the data\") *\\\n",
+                "df0.sample(500).hvplot(x=\"time\", y=\"value\", alpha=0.8, color='#FF6600', min_height=300,\n",
+                "                       label=\"Decimation\", title=\"Decimation: Don't do this!\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "c38a3dea",
             "metadata": {},
             "source": [
-                "In addition to being able to set scalar style values hvPlot also supports the HoloViews concept of [style mapping](https://holoviews.org/user_guide/Style_Mapping.html#styling-mapping), which uses so called ``dim`` transforms to map attributes of the graph nodes and edges to vary the visual attributes of the plot. For example we might construct a graph with edge weights and node sizes as attributes. The plotting function will extract these attributes which means they can be used to scale visual properties of the plot such as the ``edge_width``, ``edge_color`` or ``node_size``:"
+                "However, this method, known as decimation or arbitrarily strided sampling, can lead to [aliasing](https://en.wikipedia.org/wiki/Downsampling_(signal_processing)), where the resulting plot misrepresents the actual data by missing crucial peaks, troughs, or slopes. For instance, significant variations visible in the WebGL plot of the previous section might be entirely absent in a decimated plot, making this approach generally inadvisable for accurate data representation.\n",
+                "\n",
+                "### The LTTB Solution\n",
+                "\n",
+                "To address this, a more sophisticated method like the [Largest Triangle Three Buckets (LTTB)](https://skemman.is/handle/1946/15343) algorithm can be employed. LTTB allows data points not contributing significantly to the visible shape to be dropped, reducing the amount of data to send to the browser but preserving the appearance (and particularly the envelope, i.e. highest and lowest values in a region).\n",
+                "\n",
+                "In hvPlot, adding `downsample=True` will enable the LTTB algorithm, which will automatically choose an appropriate number of samples for the current plot:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "47e52cc0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "G = nx.Graph()\n",
-                "\n",
-                "G.add_edge('a', 'b', weight=0.6)\n",
-                "G.add_edge('a', 'c', weight=0.2)\n",
-                "G.add_edge('c', 'd', weight=0.1)\n",
-                "G.add_edge('c', 'e', weight=0.7)\n",
-                "G.add_edge('c', 'f', weight=0.9)\n",
-                "G.add_edge('a', 'd', weight=0.3)\n",
-                "\n",
-                "G.add_node('a', size=20)\n",
-                "G.add_node('b', size=10)\n",
-                "G.add_node('c', size=12)\n",
-                "G.add_node('d', size=5)\n",
-                "G.add_node('e', size=8)\n",
-                "G.add_node('f', size=3)\n",
-                "\n",
-                "pos = nx.spring_layout(G)  # positions for all nodes\n",
-                "\n",
-                "hvnx.draw(G, pos, edge_color='weight', edge_cmap='viridis',\n",
-                "          edge_width=hv.dim('weight')*10, node_size=hv.dim('size')*20)"
+                "df0.hvplot(x=\"time\", y=\"value\", color='#003366', label = \"All the data\") *\\\n",
+                "df0.hvplot(x=\"time\", y=\"value\", color='#00B3B3', label=\"LTTB\", title=\"LTTB\",\n",
+                "           min_height=300, alpha=.8, downsample=True)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "a25195ea",
             "metadata": {},
             "source": [
-                "The full set of options that are supported can be accessed on the ``hvnx.draw`` function (note this does not include some bokeh specific option to control the styling of selection, nonselection and hover nodes and edges which may also be supplied and follow a pattern like ``hover_node_fill_color`` or ``selection_edge_line_alpha``).\n",
+                "The LTTB plot will closely resemble the WebGL plot in appearance, but in general, it is rendered much more quickly (especially for local browsing of remote computation).\n",
+                "\n",
+                "<div class=\"alert alert-info\">\n",
+                "\n",
+                "<b>Note:</b> As LTTB dynamically depends on Python and therefore won't update as you zoom in on our website. If you are locally running this notebook with a live Python process, the plot will automatically update with additional detail as you zoom in.\n",
+                "\n",
+                "</div>\n",
+                "\n",
                 "\n",
-                "For reference here is the docstring listing the main supported option:"
+                "With LTTB, it is now practical to include all of the different sensors in a single plot without slowdown: "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "208fada7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(hvnx.draw.__doc__)"
+                "df.hvplot(x=\"time\", y=\"value\", downsample=True, by='sensor', min_height=300, title=\"LTTB By Sensor\")"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e06b1e4d",
             "metadata": {},
             "source": [
-                "The main difference to the networkx.draw API are a few options which are not supported (such as `font_weight` and `arrowsize`) and the renaming of `width` (which controls the edge line width) to ``edge_width`` since `width` and `height` are reserved for defining the screen dimensions of the plot."
+                "This makes LTTB an ideal default method for exploring timeseries datasets, particularly when the dataset size is unknown or too large for standard WebGL rendering."
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "660510d6",
             "metadata": {},
             "source": [
-                "## Examples\n",
+                "### Enhanced Downsampling Options\n",
                 "\n",
-                "To demonstrate that the API works almost identically this section reproduces various examples from the NetworkX documentation."
+                "\n",
+                "Starting in HoloViews version 1.19.0, integration with the [tsdownsample](https://github.com/predict-idlab/tsdownsample) library introduces enhanced downsampling functionality with the following methods, which will be accepted as inputs to `downsample` in hvPlot:\n",
+                "\n",
+                "- **lttb**: Implements the Largest Triangle Three Buckets ([LTTB](https://github.com/predict-idlab/tsdownsample?tab=readme-ov-file#:~:text=performs%20the-,Largest%20Triangle%20Three%20Buckets,-algorithm)) algorithm, optimizing the selection of points to retain the visual shape of the data.\n",
+                "- **minmax**: For each segment of the data, this method retains the minimum and maximum values, ensuring that peaks and troughs are preserved.\n",
+                "- **minmax-lttb**: A hybrid approach that combines the minmax strategy with LTTB.\n",
+                "- **m4**: A [multi-step process](https://www.vldb.org/pvldb/vol7/p797-jugel.pdf) that leverages the min, max, first, and last values for each time segment."
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "conscious-collector",
             "metadata": {},
             "source": [
-                "### Plot properties\n",
                 "\n",
-                "Compute some network properties for the lollipop graph.\n",
                 "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/basic/plot_properties.html"
+                "## Datashader Rasterizing"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "39ff4ae1",
             "metadata": {},
             "outputs": [],
             "source": [
-                "#    Copyright (C) 2004-2018 by\n",
-                "#    Aric Hagberg <hagberg@lanl.gov>\n",
-                "#    Dan Schult <dschult@colgate.edu>\n",
-                "#    Pieter Swart <swart@lanl.gov>\n",
-                "#    All rights reserved.\n",
-                "#    BSD license.\n",
-                "\n",
-                "#    Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "G = nx.lollipop_graph(4, 6)\n",
-                "\n",
-                "pathlengths = []\n",
-                "\n",
-                "print(\"source vertex {target:length, }\")\n",
-                "for v in G.nodes():\n",
-                "    spl = dict(nx.single_source_shortest_path_length(G, v))\n",
-                "    print('{} {} '.format(v, spl))\n",
-                "    for p in spl:\n",
-                "        pathlengths.append(spl[p])\n",
-                "\n",
-                "print('')\n",
-                "print(\"average shortest path length %s\" % (sum(pathlengths) / len(pathlengths)))\n",
-                "\n",
-                "# histogram of path lengths\n",
-                "dist = {}\n",
-                "for p in pathlengths:\n",
-                "    if p in dist:\n",
-                "        dist[p] += 1\n",
-                "    else:\n",
-                "        dist[p] = 1\n",
-                "\n",
-                "print('')\n",
-                "print(\"length #paths\")\n",
-                "verts = dist.keys()\n",
-                "for d in sorted(verts):\n",
-                "    print('%s %d' % (d, dist[d]))\n",
-                "\n",
-                "print(\"radius: %d\" % nx.radius(G))\n",
-                "print(\"diameter: %d\" % nx.diameter(G))\n",
-                "print(\"eccentricity: %s\" % nx.eccentricity(G))\n",
-                "print(\"center: %s\" % nx.center(G))\n",
-                "print(\"periphery: %s\" % nx.periphery(G))\n",
-                "print(\"density: %s\" % nx.density(G))\n",
-                "\n",
-                "hvnx.draw(G, with_labels=True)"
+                "# Cell hidden on the website (hide-cell in tags)\n",
+                "from holoviews.operation.resample import ResampleOperation2D\n",
+                "ResampleOperation2D.width=1200\n",
+                "ResampleOperation2D.height=500"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "28acbb0b-21b7-401e-af1e-29dee1f41287",
             "metadata": {},
             "source": [
-                "### Simple Path\n",
+                "### Principles of Datashader\n",
                 "\n",
-                "Draw a graph with hvPlot.\n",
+                "While WebGL and LTTB both send individual data points to the web browser, [Datashader](https://datashader.org) rasterizing offers a fundamentally different approach to visualizing large datasets. Datashader operates by generating a fixed-size 2D binned array tailored to your screen's resolution during each zoom or pan event. In this array, each bin aggregates data points from its corresponding location, effectively creating a 2D histogram. So, instead of transmitting the entire dataset, only this optimized array is sent to the web browser, thereby displaying all relevant data at the current zoom level and facilitating the visualization of the largest datasets.\n",
                 "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_simple_path.html"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "G = nx.path_graph(8)\n",
-                "hvnx.draw(G)"
+                "\u2757 A couple important details: \u2757\n",
+                "1. As with LTTB downsampling, Datashader rasterization dynamically depends on Python and, therefore, won't update as you zoom in on our website. If you are locally running this notebook with a live Python process, the plot will automatically update with additional detail as you zoom in.\n",
+                "2. Setting `line_width` to be greater than `0` activates [anti-aliasing](https://en.wikipedia.org/wiki/Anti-aliasing), smoothing the visual representation of lines that might otherwise look too pixelated.\n",
+                "\n",
+                "### Single Line Example\n",
+                "Activating Datashader rasterization for a single large timeseries curve in hvPlot is as simple as setting `rasterize=True`!"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8bbad008-adb6-4e00-ac4e-828445c3dd57",
             "metadata": {},
             "source": [
-                "### Node colormap\n",
+                "<div class=\"alert alert-info\">\n",
                 "\n",
-                "Draw a graph with hvPlot, color by degree.\n",
+                "<b>Note:</b> When plotting a single curve, the default behavior is to flatten the count in each pixel to better match the appearance of plotting a line without Datashader rasterization (see the [relevant PR](https://github.com/holoviz/holoviews/pull/6030) for details). If you want to restore these pixel count aggregations, just import Datashader (`import datashader as ds`) and activate 'self-intersection' in a count aggregator to hvPlot (`aggregator=ds.count(self_intersect=True)`).\n",
                 "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_node_colormap.html"
+                "</div>"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "a623a983-5a91-40e1-ab98-0967d1f0afef",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Author: Aric Hagberg (hagberg@lanl.gov)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "G = nx.cycle_graph(24)\n",
-                "pos = nx.spring_layout(G, iterations=200)\n",
-                "\n",
-                "# Preferred API\n",
-                "# hvnx.draw(G, pos, node_color='index', node_size=500, cmap='Blues')\n",
-                "\n",
-                "# Original code\n",
-                "hvnx.draw(G, pos, node_color=range(24), node_size=500, cmap='Blues')"
+                "df0.hvplot(x=\"time\", y=\"value\", rasterize=True, cnorm='eq_hist', padding=(0, 0.1),\n",
+                "           min_height=300, autorange='y', title=\"Datashader Rasterize\", colorbar=False, line_width=2)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "naughty-adventure",
             "metadata": {},
             "source": [
-                "### Edge Colormap\n",
+                "### Multiple Categories Example\n",
                 "\n",
-                "Draw a graph with hvPlot, color edges.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_edge_colormap.html"
+                "For data with a line for each of several \"categories\" (sensors, in this case), Datashader can assign a different color to each of the sensor categories. The resulting image then blends these colors where data overlaps, providing visual cues for areas with high category intersection. This is particularly useful for datasets with multiple data series:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "expired-gallery",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Author: Aric Hagberg (hagberg@lanl.gov)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "G = nx.star_graph(20)\n",
-                "pos = nx.spring_layout(G)\n",
-                "colors = range(20)\n",
-                "hvnx.draw(G, pos, node_color='#A0CBE2', edge_color=colors,\n",
-                "          edge_width=4, edge_cmap='Blues', with_labels=False)"
+                "df.hvplot(x=\"time\", y=\"value\", rasterize=True, hover=True, padding=(0, 0.1), min_height=300,\n",
+                "          by='sensor', title=\"Datashader Rasterize Categories\", line_width=2, colorbar=False, cmap='glasbey')"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "5fae9346-45e2-48bb-84a3-3ba95329345d",
             "metadata": {},
             "source": [
-                "### House With Colors\n",
-                "\n",
-                "Draw a graph with hvPlot.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_house_with_colors.html"
+                "When you're zoomed out, Datashader's effectiveness is apparent. The image it creates reveals the overall data distribution and patterns, with color and intensity showing areas of higher data concentration - where lines cross through the same pixel. Datashader rendering can therefore provide a good overview of the full shape of a long timeseries, helping you understand how the signal varies even when the variations involved are smaller than the pixels on the screen."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
+            "id": "177ef209-13c8-43e4-848d-0ee40ed1b89f",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "# Author: Aric Hagberg (hagberg@lanl.gov)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "G = nx.house_graph()\n",
-                "# explicitly set positions\n",
-                "pos = {0: (0, 0),\n",
-                "       1: (1, 0),\n",
-                "       2: (0, 1),\n",
-                "       3: (1, 1),\n",
-                "       4: (0.5, 2.0)}\n",
-                "\n",
-                "hvnx.draw_networkx_nodes(G, pos, node_size=2000, nodelist=[4], padding=0.2) *\\\n",
-                "hvnx.draw_networkx_nodes(G, pos, node_size=3000, nodelist=[0, 1, 2, 3], node_color='black') *\\\n",
-                "hvnx.draw_networkx_edges(G, pos, alpha=0.5, width=6, xaxis=None, yaxis=None)"
+                "### Multiple Lines Per Category Example\n"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "467fa694-23ba-437e-8b8f-d7485bcbb514",
             "metadata": {},
             "source": [
-                "### Circular Tree\n",
-                "\n",
-                "URL: https://networkx.org/documentation/stable/auto_examples/graphviz_layout/plot_circular_tree.html"
+                "Plotting hundreds or thousands of overlapping timeseries snippets relative to a set of events is important in domains like finance, sensor monitoring, and neuroscience. In neuroscience, for example, this approach is used to reveal distinct patterns across action potential waveforms from different neurons. Let's load a dataset of neural waveforms:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "6c4d782b-5417-48ec-a773-817714929d91",
             "metadata": {},
             "outputs": [],
             "source": [
-                "try:\n",
-                "    import pygraphviz  # noqa\n",
-                "    from networkx.drawing.nx_agraph import graphviz_layout\n",
-                "except ImportError:\n",
-                "    try:\n",
-                "        import pydot  # noqa\n",
-                "        from networkx.drawing.nx_pydot import graphviz_layout\n",
-                "    except ImportError:\n",
-                "        raise ImportError(\"This example needs Graphviz and either \"\n",
-                "                          \"PyGraphviz or pydot\")\n",
-                "\n",
-                "G = nx.balanced_tree(3, 5)\n",
-                "pos = graphviz_layout(G, prog='twopi', args='')\n",
-                "hvnx.draw(G, pos, node_size=20, alpha=0.5, node_color=\"blue\", with_labels=False, width=600, height=600)"
+                "waves = pd.read_parquet(\"https://datasets.holoviz.org/waveform/v1/waveforms.parq\")\n",
+                "print(len(waves))\n",
+                "waves.head(2)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "463ae980-bd8e-4439-8fde-3804d66191ed",
             "metadata": {},
             "source": [
-                "### Spectral Embedding\n",
-                "\n",
-                "The spectral layout positions the nodes of the graph based on the eigenvectors of the graph Laplacian L=D\u2212A, where A is the adjacency matrix and D is the degree matrix of the graph. By default, the spectral layout will embed the graph in two dimensions (you can embed your graph in other dimensions using the dim argument to either draw_spectral() or spectral_layout()).\n",
-                "\n",
-                "When the edges of the graph represent similarity between the incident nodes, the spectral embedding will place highly similar nodes closer to one another than nodes which are less similar.\n",
-                "\n",
-                "This is particularly striking when you spectrally embed a grid graph. In the full grid graph, the nodes in the center of the graph are pulled apart more than nodes on the periphery. As you remove internal nodes, this effect increases.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_spectral_grid.html"
+                "This dataset contains numerous neural waveform snippets. To grasp its structure, we examine the length of each waveform and count of waveforms per neuron:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "5cabd9ea-1c75-4976-9c31-c4b745c54c00",
             "metadata": {},
             "outputs": [],
             "source": [
-                "options = {\n",
-                "    'node_size': 100,\n",
-                "    'width': 250, 'height': 250\n",
-                "}\n",
-                "\n",
-                "G = nx.grid_2d_graph(6, 6)\n",
-                "spectral1 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((2, 2), (2, 3))\n",
-                "spectral2 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((3, 2), (3, 3))\n",
-                "spectral3 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((2, 2), (3, 2))\n",
-                "spectral4 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((2, 3), (3, 3))\n",
-                "spectral5 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((1, 2), (1, 3))\n",
-                "spectral6 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "G.remove_edge((4, 2), (4, 3))\n",
-                "spectral7 = hvnx.draw_spectral(G, **options)\n",
-                "\n",
-                "(hv.Empty() + spectral1 + hv.Empty() +\n",
-                " spectral2 + spectral3 + spectral4 +\n",
-                " spectral5 + spectral6 + spectral7).cols(3)"
+                "first_waveform = waves[(waves['Neuron'] == waves['Neuron'].unique()[0]) & (waves['Waveform'] == 0)]\n",
+                "print(f'Number of samples per waveform: {len(first_waveform)}')\n",
+                "waves.groupby('Neuron')['Waveform'].nunique().reset_index().rename(columns={'Waveform': '# Waveforms'})"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "e51c2274-f963-4fa6-8b4c-fb56ba4d445a",
             "metadata": {},
             "source": [
-                "### Plot four grids\n",
-                "\n",
-                "Draw a graph with hvPlot.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_four_grids.html"
+                "With a substantial number of waveforms and multiple categories (neurons), the density of data can make it difficult to accurately visualize patterns in the data. We can utilize hvPlot and Datashader, but there is currently one caveat: each waveform must be distinctly separated in the dataframe with a row containing `NaN` to effectively separate one waveform from another and still color by neuron with Datashader. This ensures each waveform is treated as an individual entity, avoiding misleading connections between the end of one waveform and the start of the next. Below, we can see one of these `NaN` rows at the end of the first waveform."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "77cf41a3-8206-4033-b555-3e47a86c1f38",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Author: Aric Hagberg (hagberg@lanl.gov)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "#    Copyright (C) 2004-2018\n",
-                "#    Aric Hagberg <hagberg@lanl.gov>\n",
-                "#    Dan Schult <dschult@colgate.edu>\n",
-                "#    Pieter Swart <swart@lanl.gov>\n",
-                "#    All rights reserved.\n",
-                "#    BSD license.\n",
-                "\n",
-                "G = nx.grid_2d_graph(4, 4)  # 4x4 grid\n",
-                "\n",
-                "pos = nx.spring_layout(G, iterations=100)\n",
-                "\n",
-                "g1 = hvnx.draw(G, pos, font_size=8)\n",
-                "\n",
-                "g2 = hvnx.draw(G, pos, node_color='black', node_size=0, with_labels=False)\n",
-                "\n",
-                "g3 = hvnx.draw(G, pos, node_color='green', node_size=250, with_labels=False, edge_width=6)\n",
-                "\n",
-                "H = G.to_directed()\n",
-                "g4 = hvnx.draw(H, pos, node_color='blue', node_size=20, with_labels=False)\n",
-                "\n",
-                "(g1 + g2 + g3 + g4).cols(2)"
+                "first_waveform.tail(3)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "dcc55202-ee53-42e5-8beb-c68d1031095b",
             "metadata": {},
             "source": [
-                "### Ego Graph\n",
-                "\n",
-                "Example using the NetworkX ego_graph() function to return the main egonet of the largest hub in a Barab\u00e1si-Albert network.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_ego_graph.html"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Author:  Drew Conway (drew.conway@nyu.edu)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
+                "<div class=\"alert alert-info\">\n",
                 "\n",
-                "from operator import itemgetter\n",
+                "<b>Note:</b> [Work is planned](https://github.com/holoviz/holoviews/issues/5976) to avoid having to prepare your dataset with `NaN`-separators. Stay tuned!\n",
                 "\n",
-                "# Create a BA model graph\n",
-                "n = 1000\n",
-                "m = 2\n",
-                "G = nx.generators.barabasi_albert_graph(n, m)\n",
-                "# find node with largest degree\n",
-                "node_and_degree = G.degree()\n",
-                "(largest_hub, degree) = sorted(node_and_degree, key=itemgetter(1))[-1]\n",
-                "# Create ego graph of main hub\n",
-                "hub_ego = nx.ego_graph(G, largest_hub)\n",
-                "# Draw graph\n",
-                "pos = nx.spring_layout(hub_ego)\n",
-                "g = hvnx.draw(hub_ego, pos, node_color='blue', node_size=50, with_labels=False)\n",
-                "# Draw ego as large and red\n",
-                "gnodes = hvnx.draw_networkx_nodes(hub_ego, pos, nodelist=[largest_hub], node_size=300, node_color='red')\n",
-                "\n",
-                "g * gnodes"
+                "</div>"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "8be05959-aae1-4325-842a-71b7ee8b2e61",
             "metadata": {},
             "source": [
-                "### Random Geometric Graph\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_random_geometric_graph.html"
+                "With the `NaN`-separators already in place, all we need to do is specify that hvPlot should color by neuron and apply datashader rasterization:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "28cadcc8-9f09-4a1c-ae35-06ffa9e02bfa",
             "metadata": {},
             "outputs": [],
             "source": [
-                "G = nx.random_geometric_graph(200, 0.125)\n",
-                "# position is stored as node attribute data for random_geometric_graph\n",
-                "pos = nx.get_node_attributes(G, 'pos')\n",
-                "\n",
-                "# find node near center (0.5,0.5)\n",
-                "dmin = 1\n",
-                "ncenter = 0\n",
-                "for n in pos:\n",
-                "    x, y = pos[n]\n",
-                "    d = (x - 0.5)**2 + (y - 0.5)**2\n",
-                "    if d < dmin:\n",
-                "        ncenter = n\n",
-                "        dmin = d\n",
-                "\n",
-                "# color by path length from node near center\n",
-                "p = nx.single_source_shortest_path_length(G, ncenter)\n",
-                "\n",
-                "hvnx.draw_networkx_edges(G, pos, nodelist=[ncenter], alpha=0.4, width=600, height=600) *\\\n",
-                "hvnx.draw_networkx_nodes(G, pos, nodelist=list(p.keys()),\n",
-                "                         node_size=80,\n",
-                "                         node_color=list(p.values()),\n",
-                "                         cmap='Reds_r')"
+                "waves.hvplot.line('Time', 'Amplitude', by='Neuron', hover=True, datashade=True,\n",
+                "                  xlabel='Time (ms)', ylabel='Amplitude (\u00b5V)', min_height=300,\n",
+                "                  title=\"Datashade Multiple Lines Per Category\", line_width=1)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "b4fe1f6f",
             "metadata": {},
             "source": [
-                "### Weighted Graph\n",
-                "\n",
-                "An example using Graph as a weighted network.\n",
-                "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_weighted_graph.html"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Author: Aric Hagberg (hagberg@lanl.gov)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "import networkx as nx\n",
-                "\n",
-                "G = nx.Graph()\n",
-                "\n",
-                "G.add_edge('a', 'b', weight=0.6)\n",
-                "G.add_edge('a', 'c', weight=0.2)\n",
-                "G.add_edge('c', 'd', weight=0.1)\n",
-                "G.add_edge('c', 'e', weight=0.7)\n",
-                "G.add_edge('c', 'f', weight=0.9)\n",
-                "G.add_edge('a', 'd', weight=0.3)\n",
-                "\n",
-                "elarge = [(u, v) for (u, v, attr) in G.edges(data=True) if attr['weight'] > 0.5]\n",
-                "esmall = [(u, v) for (u, v, attr) in G.edges(data=True) if attr['weight'] <= 0.5]\n",
-                "\n",
-                "pos = nx.spring_layout(G)  # positions for all nodes\n",
-                "\n",
-                "# nodes\n",
-                "nodes = hvnx.draw_networkx_nodes(G, pos, node_size=700)\n",
-                "\n",
-                "# edges\n",
-                "edges1 = hvnx.draw_networkx_edges(\n",
-                "    G, pos, edgelist=elarge, edge_width=6)\n",
-                "edges2 = hvnx.draw_networkx_edges(\n",
-                "    G, pos, edgelist=esmall, edge_width=6, alpha=0.5, edge_color='blue', style='dashed')\n",
-                "labels = hvnx.draw_networkx_labels(G, pos, font_size=20, font_family='sans-serif')\n",
-                "\n",
-                "edges1 * edges2 * nodes * labels"
+                "Datashader's approach, while comprehensive for large timeseries data, focuses on the entire dataset's view at a specific resolution. To explore data across different timescales, particularly when dealing with years of data but focusing on shorter intervals like a day or an hour, the next \"minimap\" approach offers an effective solution."
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "82346bfc",
             "metadata": {},
             "source": [
-                "### Directed Graph\n",
+                "## Minimap Contextualizing\n",
                 "\n",
-                "Draw a graph with directed edges using a colormap and different node sizes.\n",
                 "\n",
-                "Edges have different colors and alphas (opacity). Drawn using matplotlib.\n",
+                "### Minimap Overview\n",
+                "Minimap introduces a way to visualize and navigate through extensive time ranges in your dataset. It allows you to maintain awareness of the larger context while focusing on a specific, smaller time range. This technique is particularly useful when dealing with timeseries data that span long durations but require detailed study of shorter intervals.\n",
                 "\n",
-                "URL: https://networkx.github.io/documentation/stable/auto_examples/drawing/plot_directed.html"
+                "### Implementing Minimap\n",
+                "To create a minimap, we use the HoloViews `RangeToolLink`, which links a main plot to a smaller overview plot. The smaller minimap plot provides a fixed, broad view of the data, and the main plot can be used for detailed examination. Note, we also make use of **Datashader rasterization** on the minimap and **LTTB downsampling** on the main plot to limit the data sent to the browser."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "smoking-findings",
             "metadata": {},
             "outputs": [],
             "source": [
-                "# Author: Rodrigo Dorantes-Gilardi (rodgdor@gmail.com)\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
+                "from holoviews.plotting.links import RangeToolLink\n",
                 "\n",
-                "G = nx.generators.directed.random_k_out_graph(10, 3, 0.5)\n",
-                "pos = nx.layout.spring_layout(G)\n",
+                "plot = df0.hvplot(x=\"time\", y=\"value\", rasterize=True, color='darkblue', line_width=2,\n",
+                "                  min_height=300, colorbar=False, ylim=(-9, 3), # optional: set initial y-range\n",
+                "                  xlim=(pd.Timestamp(\"2023-03-10\"), pd.Timestamp(\"2023-04-10\")), # optional: set initial x-range\n",
+                "                  ).opts(\n",
+                "    backend_opts={\n",
+                "        \"x_range.bounds\": (df0.time.min(), df0.time.max()), # optional: limit max viewable x-extent to data\n",
+                "        \"y_range.bounds\": (df0.value.min()-1, df0.value.max()+1), # optional: limit max viewable y-extent to data\n",
+                "    }\n",
+                ")\n",
                 "\n",
-                "node_sizes = [3 + 10 * i for i in range(len(G))]\n",
-                "M = G.number_of_edges()\n",
-                "edge_colors = range(2, M + 2)\n",
-                "edge_alphas = [(5 + i) / (M + 4) for i in range(M)]\n",
+                "minimap = df0.hvplot(x=\"time\", y=\"value\", height=150, padding=(0, 0.1), rasterize=True,\n",
+                "                     color='darkblue', colorbar=False, line_width=2).opts(toolbar='disable')\n",
                 "\n",
-                "nodes = hvnx.draw_networkx_nodes(G, pos, node_size=node_sizes, node_color='blue')\n",
-                "edges = hvnx.draw_networkx_edges(G, pos, node_size=node_sizes, arrowstyle='->',\n",
-                "                               arrowsize=10, edge_color=edge_colors,\n",
-                "                               edge_cmap='Blues', edge_width=2, colorbar=True)\n",
+                "link = RangeToolLink(minimap, plot, axes=[\"x\", \"y\"])\n",
                 "\n",
-                "nodes * edges"
+                "(plot + minimap).opts(shared_axes=False).cols(1)"
             ]
         },
         {
             "cell_type": "markdown",
+            "id": "lesser-magazine",
             "metadata": {},
             "source": [
-                "### Giant Component\n",
+                "In this setup, you can interact with the minimap by dragging the grey selection box. The main plot above will update to reflect the selected range, allowing you to explore extensive datasets while focusing on specific segments.\n",
                 "\n",
-                "This example illustrates the sudden appearance of a giant connected component in a binomial random graph.\n",
-                "\n",
-                "https://networkx.org/documentation/stable/auto_examples/graphviz_layout/plot_giant_component.html"
+                "Here, we also demonstrate the use of `backend_opts` to configure properties of the Bokeh plotting library that are not yet exposed as HoloViews/hvPlot options. By setting hard outer limits on the plot's panning/zooming, we ensure that the view remains within the data's range, enhancing the user experience."
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
+            "cell_type": "markdown",
+            "id": "fd0ffe6b",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "#    Copyright (C) 2006-2018\n",
-                "#    Aric Hagberg <hagberg@lanl.gov>\n",
-                "#    Dan Schult <dschult@colgate.edu>\n",
-                "#    Pieter Swart <swart@lanl.gov>\n",
-                "#    All rights reserved.\n",
-                "#    BSD license.\n",
-                "\n",
-                "# Adapted by Philipp Rudiger <prudiger@anaconda.com>\n",
-                "\n",
-                "import math\n",
-                "\n",
-                "try:\n",
-                "    import pygraphviz  # noqa\n",
-                "    from networkx.drawing.nx_agraph import graphviz_layout\n",
-                "    layout = graphviz_layout\n",
-                "except ImportError:\n",
-                "    try:\n",
-                "        import pydot  # noqa\n",
-                "        from networkx.drawing.nx_pydot import graphviz_layout\n",
-                "        layout = graphviz_layout\n",
-                "    except ImportError:\n",
-                "        print(\"PyGraphviz and pydot not found;\\n\"\n",
-                "              \"drawing with spring layout;\\n\"\n",
-                "              \"will be slow.\")\n",
-                "        layout = nx.spring_layout\n",
-                "\n",
-                "n = 150  # 150 nodes\n",
-                "# p value at which giant component (of size log(n) nodes) is expected\n",
-                "p_giant = 1.0 / (n - 1)\n",
-                "# p value at which graph is expected to become completely connected\n",
-                "p_conn = math.log(n) / float(n)\n",
-                "\n",
-                "# the following range of p values should be close to the threshold\n",
-                "pvals = [0.003, 0.006, 0.008, 0.015]\n",
-                "\n",
-                "region = 220  # for pylab 2x2 subplot layout\n",
-                "plots = []\n",
-                "for p in pvals:\n",
-                "    G = nx.binomial_graph(n, p)\n",
-                "    pos = layout(G)\n",
-                "    region += 1\n",
-                "    g = hvnx.draw(G, pos, with_labels=False, node_size=15)\n",
-                "    # identify largest connected component\n",
-                "    Gcc = sorted([G.subgraph(c) for c in nx.connected_components(G)], key=len, reverse=True)\n",
-                "    G0 = Gcc[0]\n",
-                "    edges = hvnx.draw_networkx_edges(\n",
-                "        G0, pos, with_labels=False, edge_color='red', edge_width=6.0)\n",
-                "    \n",
-                "    # show other connected components\n",
-                "    other_edges = []\n",
-                "    for Gi in Gcc[1:]:\n",
-                "        if len(Gi) > 1:\n",
-                "            edge = hvnx.draw_networkx_edges(Gi, pos,\n",
-                "                                   with_labels=False,\n",
-                "                                   edge_color='red',\n",
-                "                                   alpha=0.3,\n",
-                "                                   edge_width=5.0\n",
-                "                                  )\n",
-                "            other_edges.append(edge)\n",
-                "    plots.append((g*edges*hv.Overlay(other_edges)).relabel(\"p = %6.3f\" % (p)))\n",
+                "## Future Improvements\n",
+                "As we look to the future, our roadmap includes several exciting enhancements. A significant focus is to enrich Datashader inspections by incorporating rich hover tooltips for Datashader images. This addition will greatly enhance the data exploration experience, allowing users to access detailed information more intuitively.\n",
                 "\n",
-                "hv.Layout(plots).cols(2)"
+                "Additionally, we are working towards a more streamlined process for plotting multiple overlapping lines. Our goal is to evolve the current approach, eliminating the need for inserting `NaN` rows as separators in the data structure. This improvement will simplify data preparation, making the visualization of complex timeseries more accessible and user-friendly."
             ]
         }
     ],
     "metadata": {
         "language_info": {
             "name": "python",
             "pygments_lexer": "ipython3"
         }
     },
     "nbformat": 4,
-    "nbformat_minor": 4
+    "nbformat_minor": 5
 }
```

### Comparing `hvplot-0.9.2rc1/hvplot/fugue.py` & `hvplot-0.9.3a1/hvplot/fugue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Experimental support for fugue.
 """
+
 from typing import Any, Dict, Tuple
 
 import panel as _pn
 
 from . import hvPlotTabular, post_patch
 from .util import _fugue_ipython
 
-def patch(name="hvplot", extension="bokeh", logo=False):
+
+def patch(name='hvplot', extension='bokeh', logo=False):
     try:
         from fugue import DataFrames, Outputter
         from fugue.extensions import namespace_candidate, parse_outputter
-    except:
+    except ImportError:
         raise ImportError(
             'Could not add fugue support as it could not be imported. '
             'Please make sure you have installed fugue in your environment.'
         )
 
     import hvplot.pandas  # noqa: F401
 
@@ -34,27 +36,27 @@
             Parameters:
             -----------
             dfs: fugue.DataFrames
             """
             charts = []
             for df in dfs.values():
                 params = dict(self.params)
-                opts: Dict[str, Any] = params.pop("opts", {})
+                opts: Dict[str, Any] = params.pop('opts', {})
                 chart = getattr(df.as_pandas().hvplot, self._func)(**params).opts(**opts)
                 charts.append(chart)
             col = _pn.Column(*charts)
             try:
                 if not _fugue_ipython:
                     get_ipython()
             except NameError:
                 col.show()  # in script
             else:
                 from IPython.display import display
-                display(col)  # in notebook
 
+                display(col)  # in notebook
 
     @parse_outputter.candidate(namespace_candidate(name, lambda x: isinstance(x, str)))
     def _parse_hvplot(obj: Tuple[str, str]) -> Outputter:
         return _Visualize(obj[1])
 
     post_patch(extension, logo)
```

### Comparing `hvplot-0.9.2rc1/hvplot/ibis.py` & `hvplot-0.9.3a1/hvplot/ibis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Experimental support for ibis.
 """
 
+
 def patch(name='hvplot', extension='bokeh', logo=False):
     from . import hvPlotTabular, post_patch
 
     try:
         import ibis
-    except:
-        raise ImportError('Could not patch plotting API onto ibis. '
-                          'Ibis could not be imported.')
-    _patch_plot = lambda self: hvPlotTabular(self)
+    except ImportError:
+        raise ImportError('Could not patch plotting API onto ibis. Ibis could not be imported.')
+    _patch_plot = lambda self: hvPlotTabular(self)  # noqa: E731
     _patch_plot.__doc__ = hvPlotTabular.__call__.__doc__
     patch_property = property(_patch_plot)
     setattr(ibis.Expr, name, patch_property)
 
     post_patch(extension, logo)
 
+
 patch()
```

### Comparing `hvplot-0.9.2rc1/hvplot/intake.py` & `hvplot-0.9.3a1/hvplot/intake.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 from . import hvPlot, post_patch
 
 
 def patch(name='hvplot', extension='bokeh', logo=False):
     try:
         import intake
-    except:
-        raise ImportError('Could not patch plotting API onto intake. '
-                          'intake could not be imported.')
+    except ImportError:
+        raise ImportError(
+            'Could not patch plotting API onto intake. intake could not be imported.'
+        )
 
-    _patch_plot = lambda self: hvPlot(self)
+    _patch_plot = lambda self: hvPlot(self)  # noqa: E731
     _patch_plot.__doc__ = hvPlot.__call__.__doc__
     patch_property = property(_patch_plot)
     setattr(intake.source.base.DataSource, name, patch_property)
     post_patch(extension, logo)
 
+
 try:
-    import intake.plotting # noqa
+    import intake.plotting  # noqa
+
     patch()
-except:
+except Exception:
     import intake
+
     if Version(intake.__version__) <= Version('0.1.5'):
         patch()
         patch(name='plot')
     else:
         post_patch(extension='bokeh', logo=False)
```

### Comparing `hvplot-0.9.2rc1/hvplot/interactive.py` & `hvplot-0.9.3a1/hvplot/interactive.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,19 @@
 
 from panel.layout import Column, Row, VSpacer, HSpacer
 from panel.util import get_method_owner, full_groupby
 from panel.widgets.base import Widget
 
 from .converter import HoloViewsConverter
 from .util import (
-    _flatten, bokeh3, is_tabular, is_xarray, is_xarray_dataarray,
+    _flatten,
+    bokeh3,
+    is_tabular,
+    is_xarray,
+    is_xarray_dataarray,
     _convert_col_names_to_str,
 )
 
 
 def _find_widgets(op):
     widgets = []
     op_args = list(op['args']) + list(op['kwargs'].values())
@@ -130,28 +134,31 @@
             for nested_op in op_arg.ops:
                 for widget in _find_widgets(nested_op):
                     if widget not in widgets:
                         widgets.append(widget)
         # Find Ipywidgets
         if 'ipywidgets' in sys.modules:
             from ipywidgets import Widget as IPyWidget
+
             if isinstance(op_arg, IPyWidget) and op_arg not in widgets:
                 widgets.append(op_arg)
         # Find widgets introduced as `widget.param.value` in an expression
-        if (isinstance(op_arg, param.Parameter) and
-            isinstance(op_arg.owner, pn.widgets.Widget) and
-            op_arg.owner not in widgets):
+        if (
+            isinstance(op_arg, param.Parameter)
+            and isinstance(op_arg.owner, pn.widgets.Widget)
+            and op_arg.owner not in widgets
+        ):
             widgets.append(op_arg.owner)
         if isinstance(op_arg, slice):
-            if Version(hv.__version__) < Version("1.15.1"):
+            if Version(hv.__version__) < Version('1.15.1'):
                 raise ValueError(
-                    "Using interactive with slices needs to have "
-                    "Holoviews 1.15.1 or greater installed."
+                    'Using interactive with slices needs to have '
+                    'Holoviews 1.15.1 or greater installed.'
                 )
-            nested_op = {"args": [op_arg.start, op_arg.stop, op_arg.step], "kwargs": {}}
+            nested_op = {'args': [op_arg.start, op_arg.stop, op_arg.step], 'kwargs': {}}
             for widget in _find_widgets(nested_op):
                 if widget not in widgets:
                     widgets.append(widget)
     return widgets
 
 
 class Interactive:
@@ -236,33 +243,46 @@
     def applies(cls, obj):
         """
         Subclasses must implement applies and return a boolean to indicate
         whether the subclass should apply or not to the obj.
         """
         return True
 
-    def __init__(self, obj, transform=None, fn=None, plot=False, depth=0,
-                 loc='top_left', center=False, dmap=False, inherit_kwargs={},
-                 max_rows=100, method=None, _shared_obj=None, _current=None, **kwargs):
-
+    def __init__(
+        self,
+        obj,
+        transform=None,
+        fn=None,
+        plot=False,
+        depth=0,
+        loc='top_left',
+        center=False,
+        dmap=False,
+        inherit_kwargs={},
+        max_rows=100,
+        method=None,
+        _shared_obj=None,
+        _current=None,
+        **kwargs,
+    ):
         # _init is used to prevent to __getattribute__ to execute its
         # specialized code.
         self._init = False
         self._method = method
         if transform is None:
             dim = '*'
             transform = hv.util.transform.dim
             if is_xarray(obj):
                 transform = hv.util.transform.xr_dim
                 if is_xarray_dataarray(obj):
                     dim = obj.name
                 if dim is None:
                     raise ValueError(
-                        "Cannot use interactive API on DataArray without name."
-                        "Assign a name to the DataArray and try again."
+                        'Cannot use interactive API on DataArray without name.'
+                        'Assign a name to the DataArray and try again.'
                     )
             elif is_tabular(obj):
                 transform = hv.util.transform.df_dim
             self._transform = transform(dim)
         else:
             self._transform = transform
         self._plot = plot
@@ -358,40 +378,69 @@
     @property
     def _callback(self):
         def evaluate_inner():
             obj = self.eval()
             if isinstance(obj, pd.DataFrame):
                 return pn.pane.DataFrame(obj, max_rows=self._max_rows, **self._kwargs)
             return obj
+
         params = self._params
         if params:
+
             @pn.depends(*params)
             def evaluate(*args, **kwargs):
                 return evaluate_inner()
         else:
+
             def evaluate():
                 return evaluate_inner()
+
         return evaluate
 
-    def _clone(self, transform=None, plot=None, loc=None, center=None,
-               dmap=None, copy=False, max_rows=None, **kwargs):
+    def _clone(
+        self,
+        transform=None,
+        plot=None,
+        loc=None,
+        center=None,
+        dmap=None,
+        copy=False,
+        max_rows=None,
+        **kwargs,
+    ):
         plot = self._plot or plot
         transform = transform or self._transform
         loc = self._loc if loc is None else loc
         center = self._center if center is None else center
         dmap = self._dmap if dmap is None else dmap
         max_rows = self._max_rows if max_rows is None else max_rows
         depth = self._depth + 1
         if copy:
-            kwargs = dict(self._kwargs, _current=self._current, inherit_kwargs=self._inherit_kwargs, method=self._method, **kwargs)
+            kwargs = dict(
+                self._kwargs,
+                _current=self._current,
+                inherit_kwargs=self._inherit_kwargs,
+                method=self._method,
+                **kwargs,
+            )
         else:
             kwargs = dict(self._inherit_kwargs, **dict(self._kwargs, **kwargs))
-        return type(self)(self._obj, fn=self._fn, transform=transform, plot=plot, depth=depth,
-                         loc=loc, center=center, dmap=dmap, _shared_obj=self._shared_obj,
-                         max_rows=max_rows, **kwargs)
+        return type(self)(
+            self._obj,
+            fn=self._fn,
+            transform=transform,
+            plot=plot,
+            depth=depth,
+            loc=loc,
+            center=center,
+            dmap=dmap,
+            _shared_obj=self._shared_obj,
+            max_rows=max_rows,
+            **kwargs,
+        )
 
     def _repr_mimebundle_(self, include=[], exclude=[]):
         return self.layout()._repr_mimebundle_()
 
     def __dir__(self):
         current = self._current
         if self._method:
@@ -450,17 +499,19 @@
 
     @staticmethod
     def _get_ax_fn():
         @pn.depends()
         def get_ax():
             from matplotlib.backends.backend_agg import FigureCanvas
             from matplotlib.pyplot import Figure
+
             Interactive._fig = fig = Figure()
             FigureCanvas(fig)
             return fig.subplots()
+
         return get_ax
 
     def __call__(self, *args, **kwargs):
         """
         The `.interactive` API enhances the API of data analysis libraries
         like Pandas, Dask, and Xarray, by allowing to replace in a pipeline
         static values by dynamic widgets. When displayed, an interactive
@@ -517,17 +568,17 @@
             clone = new._clone(method(*args, **kwargs), plot=new._method == 'plot')
         finally:
             # If an error occurs reset _method anyway so that, e.g. the next
             # attempt in a Notebook, is set appropriately.
             new._method = None
         return clone
 
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
     # Interactive pipeline APIs
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
 
     def __array_ufunc__(self, *args, **kwargs):
         # TODO: How to trigger this method?
         new = self._resolve_accessor()
         transform = new._transform
         transform = args[0](transform, *args[3:], **kwargs)
         return new._clone(transform)
@@ -546,134 +597,166 @@
     def __round__(self, ndigits=None):
         args = () if ndigits is None else (ndigits,)
         return self._apply_operator(round, *args)
 
     # Unary operators
     def __neg__(self):
         return self._apply_operator(operator.neg)
+
     def __not__(self):
         return self._apply_operator(operator.not_)
+
     def __invert__(self):
         return self._apply_operator(operator.inv)
+
     def __pos__(self):
         return self._apply_operator(operator.pos)
 
     # Binary operators
     def __add__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.add, other)
+
     def __and__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.and_, other)
+
     def __eq__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.eq, other)
+
     def __floordiv__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.floordiv, other)
+
     def __ge__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.ge, other)
+
     def __gt__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.gt, other)
+
     def __le__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.le, other)
+
     def __lt__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.lt, other)
+
     def __lshift__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.lshift, other)
+
     def __mod__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.mod, other)
+
     def __mul__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.mul, other)
+
     def __ne__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.ne, other)
+
     def __or__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.or_, other)
+
     def __rshift__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.rshift, other)
+
     def __pow__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.pow, other)
+
     def __sub__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.sub, other)
+
     def __truediv__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.truediv, other)
 
     # Reverse binary operators
     def __radd__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.add, other, reverse=True)
+
     def __rand__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.and_, other, reverse=True)
+
     def __rdiv__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.div, other, reverse=True)
+
     def __rfloordiv__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.floordiv, other, reverse=True)
+
     def __rlshift__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.rlshift, other)
+
     def __rmod__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.mod, other, reverse=True)
+
     def __rmul__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.mul, other, reverse=True)
+
     def __ror__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.or_, other, reverse=True)
+
     def __rpow__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.pow, other, reverse=True)
+
     def __rrshift__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.rrshift, other)
+
     def __rsub__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.sub, other, reverse=True)
+
     def __rtruediv__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.truediv, other, reverse=True)
 
     def __getitem__(self, other):
         other = other._transform if isinstance(other, Interactive) else other
         return self._apply_operator(operator.getitem, other)
 
     def _plot(self, *args, **kwargs):
         # TODO: Seems totally unused to me, as self._plot is set to a boolean in __init__
         @pn.depends()
         def get_ax():
             from matplotlib.backends.backend_agg import FigureCanvas
             from matplotlib.pyplot import Figure
+
             Interactive._fig = fig = Figure()
             FigureCanvas(fig)
             return fig.subplots()
+
         kwargs['ax'] = get_ax
         new = self._resolve_accessor()
         transform = new._transform
         transform = type(transform)(transform, 'plot', accessor=True)
         return new._clone(transform(*args, **kwargs), plot=True)
 
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
     # Public API
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
 
     def dmap(self):
         """
         Wraps the output in a DynamicMap. Only valid if the output
         is a HoloViews object.
         """
         return hv.DynamicMap(self._callback)
@@ -738,17 +821,25 @@
                 components = [panel]
         elif center:
             if loc.startswith('left'):
                 components = [widgets, HSpacer(), panel, HSpacer()]
             elif loc.startswith('right'):
                 components = [HSpacer(), panel, HSpacer(), widgets]
             elif loc.startswith('top'):
-                components = [HSpacer(), Column(widgets, Row(HSpacer(), panel, HSpacer())), HSpacer()]
+                components = [
+                    HSpacer(),
+                    Column(widgets, Row(HSpacer(), panel, HSpacer())),
+                    HSpacer(),
+                ]
             elif loc.startswith('bottom'):
-                components = [HSpacer(), Column(Row(HSpacer(), panel, HSpacer()), widgets), HSpacer()]
+                components = [
+                    HSpacer(),
+                    Column(Row(HSpacer(), panel, HSpacer()), widgets),
+                    HSpacer(),
+                ]
         else:
             if loc.startswith('left'):
                 components = [widgets, panel]
             elif loc.startswith('right'):
                 components = [panel, widgets]
             elif loc.startswith('top'):
                 components = [Column(widgets, panel)]
@@ -769,15 +860,15 @@
             'top_left': (Column, 'start', True),
             'top_right': (Column, ('end', 'start'), True),
             'bottom_left': (Column, ('start', 'end'), False),
             'bottom_right': (Column, 'end', False),
             'left_top': (Row, 'start', True),
             'left_bottom': (Row, ('start', 'end'), True),
             'right_top': (Row, ('end', 'start'), False),
-            'right_bottom': (Row, 'end', False)
+            'right_bottom': (Row, 'end', False),
         }
         layout, align, widget_first = alignments[loc]
         widget_box.align = align
         if not len(widget_box):
             if center:
                 components = [HSpacer(), panel, HSpacer()]
             else:
@@ -830,40 +921,39 @@
 
         Returns
         -------
         A Column of widgets
         """
         widgets = []
         for p in self._fn_params:
-            if (isinstance(p.owner, pn.widgets.Widget) and
-                p.owner not in widgets):
+            if isinstance(p.owner, pn.widgets.Widget) and p.owner not in widgets:
                 widgets.append(p.owner)
         for op in self._transform.ops:
             for w in _find_widgets(op):
                 if w not in widgets:
                     widgets.append(w)
         return pn.Column(*widgets)
 
 
 class _hvplot:
     _kinds = tuple(HoloViewsConverter._kind_mapping)
 
-    __slots__ = ["_interactive"]
+    __slots__ = ['_interactive']
 
     def __init__(self, _interactive):
         self._interactive = _interactive
 
     def __call__(self, *args, _kind=None, **kwargs):
         # The underscore in _kind is to not overwrite it
         # if 'kind' is in kwargs and the function
         # is used with partial.
-        if _kind and "kind" in kwargs:
+        if _kind and 'kind' in kwargs:
             raise TypeError(f"{_kind}() got an unexpected keyword argument 'kind'")
         if _kind:
-            kwargs["kind"] = _kind
+            kwargs['kind'] = _kind
 
         new = self._interactive._resolve_accessor()
         transform = new._transform
         transform = type(transform)(transform, 'hvplot', accessor=True)
         dmap = 'kind' not in kwargs or isinstance(kwargs['kind'], str)
         return new._clone(transform(*args, **kwargs), dmap=dmap)
```

### Comparing `hvplot-0.9.2rc1/hvplot/networkx.py` & `hvplot-0.9.3a1/hvplot/networkx.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from holoviews.core.options import Store
 from holoviews.core.util import dimension_sanitizer
 from holoviews.plotting.bokeh import GraphPlot, LabelsPlot
 from holoviews.plotting.bokeh.styles import markers
 
 from .backend_transforms import _transfer_opts_cur_backend
 from .util import process_crs
-from .utilities import save, show # noqa
+from .utilities import save, show  # noqa
 
 if _hv.extension and not getattr(_hv.extension, '_loaded', False):
     _hv.extension('bokeh', logo=False)
 
 
 def _from_networkx(G, positions, nodes=None, cls=Graph, **kwargs):
     """
@@ -46,28 +46,29 @@
     """
 
     # Unpack edges
     edges = defaultdict(list)
     for start, end in G.edges():
         for attr, value in sorted(G.adj[start][end].items()):
             if isinstance(value, (list, dict)):
-                continue # Cannot handle list or dict attrs
+                continue  # Cannot handle list or dict attrs
             edges[attr].append(value)
 
         # Handle tuple node indexes (used in 2D grid Graphs)
         if isinstance(start, tuple):
             start = str(start)
         if isinstance(end, tuple):
             end = str(end)
         edges['start'].append(start)
         edges['end'].append(end)
-    edge_cols = sorted(k for k in edges if k not in ('start', 'end')
-                        and len(edges[k]) == len(edges['start']))
+    edge_cols = sorted(
+        k for k in edges if k not in ('start', 'end') and len(edges[k]) == len(edges['start'])
+    )
     edge_vdims = [str(col) if isinstance(col, int) else col for col in edge_cols]
-    edge_data = tuple(edges[col] for col in ['start', 'end']+edge_cols)
+    edge_data = tuple(edges[col] for col in ['start', 'end'] + edge_cols)
 
     # Unpack user node info
     xdim, ydim, idim = cls.node_type.kdims[:3]
     if nodes:
         node_columns = nodes.columns()
         idx_dim = nodes.kdims[0].name
         info_cols, values = zip(*((k, v) for k, v in node_columns.items() if k != idx_dim))
@@ -88,19 +89,22 @@
         for attr, value in node.items():
             if isinstance(value, (list, dict, tuple)):
                 continue
             node_columns[attr].append(value)
         for i, col in enumerate(info_cols):
             node_columns[col].append(node_info[idx][i])
         if isinstance(idx, tuple):
-            idx = str(idx) # Tuple node indexes handled as strings
+            idx = str(idx)  # Tuple node indexes handled as strings
         node_columns[idim.name].append(idx)
-    node_cols = sorted(k for k in node_columns if k not in cls.node_type.kdims
-                        and len(node_columns[k]) == len(node_columns[xdim.name]))
-    columns = [xdim.name, ydim.name, idim.name]+node_cols+list(info_cols)
+    node_cols = sorted(
+        k
+        for k in node_columns
+        if k not in cls.node_type.kdims and len(node_columns[k]) == len(node_columns[xdim.name])
+    )
+    columns = [xdim.name, ydim.name, idim.name] + node_cols + list(info_cols)
     node_data = tuple(node_columns[col] for col in columns)
 
     # Construct nodes
     vdims = []
     for col in node_cols:
         if isinstance(col, int):
             dim = str(col)
@@ -210,17 +214,19 @@
 
     params, label_params = {}, {}
     label_element = Labels
     if kwargs.get('geo', False) or 'crs' in kwargs:
         try:
             import geoviews
         except ImportError:
-            raise ImportError('In order to use geo-related features '
-                              'the geoviews library must be available. '
-                              'It can be installed with pip or conda.')
+            raise ImportError(
+                'In order to use geo-related features '
+                'the geoviews library must be available. '
+                'It can be installed with pip or conda.'
+            )
         crs = process_crs(kwargs.get('crs'))
         label_element = geoviews.Labels
         params['cls'] = geoviews.Graph
         params['crs'] = crs
         label_params['crs'] = crs
 
     # Construct Graph object
@@ -248,15 +254,16 @@
         directed=kwargs.pop('arrows', isinstance(G, nx.DiGraph)),
         colorbar=kwargs.pop('colorbar', False),
         padding=kwargs.get('padding', 0.1),
         width=kwargs.pop('width', 400),
         height=kwargs.pop('height', 400),
         selection_policy=kwargs.pop('selection_policy', 'nodes'),
         inspection_policy=inspection_policy,
-        node_fill_color='red')
+        node_fill_color='red',
+    )
 
     if '_axis_defaults':
         opts.update(xaxis=None, yaxis=None, show_frame=False)
 
     opts.update({k: kwargs.pop(k) for k in list(kwargs) if k in GraphPlot.style_opts})
     if 'node_size' in opts:
         if isinstance(opts['node_size'], str):
@@ -285,15 +292,20 @@
         opts['edge_line_width'] = kwargs.pop('edge_width')
     if 'style' in kwargs:
         opts['edge_line_dash'] = kwargs.pop('style')
 
     node_styles = ('node_fill_color', 'node_size', 'node_alpha', 'node_line_width')
     for node_style in node_styles:
         if isinstance(opts.get(node_style), (np.ndarray, list, range)):
-            g = g.clone((g.data, g.nodes.add_dimension(node_style, len(g.nodes.vdims), opts[node_style], True)))
+            g = g.clone(
+                (
+                    g.data,
+                    g.nodes.add_dimension(node_style, len(g.nodes.vdims), opts[node_style], True),
+                )
+            )
             opts[node_style] = node_style
 
     edge_styles = ('edge_line_color', 'edge_line_alpha', 'edge_alpha', 'edge_line_width')
     for edge_style in edge_styles:
         if isinstance(opts.get(edge_style), (np.ndarray, list, range)):
             g = g.add_dimension(edge_style, len(g.vdims), opts[edge_style], True)
             opts[edge_style] = edge_style
@@ -307,21 +319,27 @@
     if opts.get('edge_line_color') in g.dimensions():
         lims = (kwargs.get('edge_vmin', None), kwargs.get('edge_vmax', None))
         if lims != (None, None):
             dimension = g.get_dimension(opts.get('edge_line_color'))
             dimension.range = lims
 
     if inspection_policy == 'nodes':
-        tooltip_dims = [(d.label, 'index_hover' if d in g.nodes.kdims else d.name)
-                        for d in g.nodes.kdims[2:] + g.nodes.vdims]
+        tooltip_dims = [
+            (d.label, 'index_hover' if d in g.nodes.kdims else d.name)
+            for d in g.nodes.kdims[2:] + g.nodes.vdims
+        ]
     else:
-        tooltip_dims = [(d.label, d.name+'_values' if d in g.kdims else d.name)
-                        for d in g.kdims + g.vdims]
-    tooltips = [(label, '@{%s}' % dimension_sanitizer(name))
-                for label, name in tooltip_dims if name not in node_styles + edge_styles]
+        tooltip_dims = [
+            (d.label, d.name + '_values' if d in g.kdims else d.name) for d in g.kdims + g.vdims
+        ]
+    tooltips = [
+        (label, '@{%s}' % dimension_sanitizer(name))
+        for label, name in tooltip_dims
+        if name not in node_styles + edge_styles
+    ]
     opts['tools'] = [HoverTool(tooltips=tooltips), 'tap']
 
     g.opts(**opts, backend='bokeh')
 
     # Construct Labels
     if kwargs.get('with_labels', kwargs.get('labels', False)):
         label_opts = {k: kwargs.pop(k) for k in list(kwargs) if k in LabelsPlot.style_opts}
@@ -582,14 +600,15 @@
     Returns
     -------
     graph : holoviews.Graph or holoviews.Overlay
        Graph element or Graph and Labels
     """
     return draw(G, nx.spring_layout, **kwargs)
 
+
 def draw_planar(G, **kwargs):
     """Draw networkx graph with planar layout.
 
     Parameters
     ----------
     G : graph
        A networkx graph
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/__init__.py` & `hvplot-0.9.3a1/hvplot/plotting/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import holoviews as hv
 from ..util import with_hv_extension, is_polars
 
-from .core import hvPlot, hvPlotTabular   # noqa
+from .core import hvPlot, hvPlotTabular  # noqa
 
-from .andrews_curves import andrews_curves   # noqa
-from .parallel_coordinates import parallel_coordinates   # noqa
-from .lag_plot import lag_plot   # noqa
-from .scatter_matrix import scatter_matrix   # noqa
+from .andrews_curves import andrews_curves  # noqa
+from .parallel_coordinates import parallel_coordinates  # noqa
+from .lag_plot import lag_plot  # noqa
+from .scatter_matrix import scatter_matrix  # noqa
 
 
 @with_hv_extension
 def plot(data, kind, **kwargs):
     # drop reuse_plot
     kwargs.pop('reuse_plot', None)
 
@@ -28,14 +28,15 @@
     no_none_kwargs = {}
     for k, v in kwargs.items():
         if v is not None:
             no_none_kwargs[k] = v
 
     if is_polars(data):
         from .core import hvPlotTabularPolars
+
         return hvPlotTabularPolars(data)(kind=kind, **no_none_kwargs)
     return hvPlotTabular(data)(kind=kind, **no_none_kwargs)
 
 
 def boxplot_series(*args, **kwargs):
     return plot(*args, kind='box', **kwargs)
 
@@ -44,16 +45,17 @@
     return plot(*args, kind='box', **kwargs)
 
 
 def boxplot_frame_groupby(grouped, **kwargs):
     width = kwargs.pop('width', 300)
     subplots = kwargs.pop('subplots', True)
     layout = hv.Layout if subplots else hv.Overlay
-    plots = [plot(data=data, kind='box', title=name, width=width, **kwargs)
-             for name, data in grouped]
+    plots = [
+        plot(data=data, kind='box', title=name, width=width, **kwargs) for name, data in grouped
+    ]
     return layout(plots)
 
 
 def hist_series(*args, **kwargs):
     return plot(*args, kind='hist', **kwargs)
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/andrews_curves.py` & `hvplot-0.9.3a1/hvplot/plotting/andrews_curves.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,25 @@
 import colorcet as cc
 
 from ..backend_transforms import _transfer_opts_cur_backend
 from ..util import with_hv_extension
 
 
 @with_hv_extension
-def andrews_curves(data, class_column, samples=200, alpha=0.5,
-                   width=600, height=300, cmap=None, colormap=None,
-                   **kwds):
+def andrews_curves(
+    data,
+    class_column,
+    samples=200,
+    alpha=0.5,
+    width=600,
+    height=300,
+    cmap=None,
+    colormap=None,
+    **kwds,
+):
     """
     Generate a plot of Andrews curves, for visualising clusters of
     multivariate data.
 
     Andrews curves have the functional form:
 
     f(t) = x_1/sqrt(2) + x_2 sin(t) + x_3 cos(t) +
@@ -54,28 +62,38 @@
     for i in range(1, len(vals)):
         ft = ((i + 1) // 2) * t
         if i % 2 == 1:
             curves += np.outer(vals[i], np.sin(ft))
         else:
             curves += np.outer(vals[i], np.cos(ft))
 
-    df = pd.DataFrame({'t': np.tile(np.arange(samples), curves.shape[0]),
-                       'sample': np.repeat(np.arange(curves.shape[0]), curves.shape[1]),
-                       'value': curves.ravel(),
-                       class_column: np.repeat(data[class_column], samples)})
+    df = pd.DataFrame(
+        {
+            't': np.tile(np.arange(samples), curves.shape[0]),
+            'sample': np.repeat(np.arange(curves.shape[0]), curves.shape[1]),
+            'value': curves.ravel(),
+            class_column: np.repeat(data[class_column], samples),
+        }
+    )
 
     labelled = ['x']
-    options = {'Overlay': dict(legend_limit=5000),
-               'Curve': dict(kwds, labelled=labelled, alpha=alpha,
-                             width=width, height=height, **kwds)}
+    options = {
+        'Overlay': dict(legend_limit=5000),
+        'Curve': dict(kwds, labelled=labelled, alpha=alpha, width=width, height=height, **kwds),
+    }
     dataset = hv.Dataset(df)
     groups = dataset.to(hv.Curve, 't', 'value').overlay('sample').items()
 
     if cmap and colormap:
-        raise TypeError("Only specify one of `cmap` and `colormap`.")
+        raise TypeError('Only specify one of `cmap` and `colormap`.')
     cmap = cmap or colormap or cc.palette['glasbey_category10']
     colors = hv.plotting.util.process_cmap(cmap, categorical=True, ncolors=len(groups))
 
-    el = hv.Overlay([curve.relabel(k).options('Curve', color=c, backend='bokeh')
-                       for c, (k, v) in zip(colors, groups) for curve in v]).options(options, backend='bokeh')
+    el = hv.Overlay(
+        [
+            curve.relabel(k).options('Curve', color=c, backend='bokeh')
+            for c, (k, v) in zip(colors, groups)
+            for curve in v
+        ]
+    ).options(options, backend='bokeh')
     el = _transfer_opts_cur_backend(el)
     return el
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/core.py` & `hvplot-0.9.3a1/hvplot/plotting/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 import param
 
 try:
     import panel as pn
 
     panel_available = True
-except:
+except ImportError:
     panel_available = False
 
 from ..converter import HoloViewsConverter
 from ..util import is_list_like, process_dynamic_args
 
 # Color palette for examples: https://www.color-hex.com/color-palette/1018056
 # light green: #55a194
 # Dark green: #3b7067
 # Blue: #1e85f7
 # Orange: #f8b014
 # Red: #f16a6f
 
+
 class hvPlotBase:
     """
     Internal base class.
 
     Concrete subclasses must implement plotting methods (e.g. `line`, `scatter`, `image`).
     A plotting method must call `self` which will effectively create a HoloViewsConverter
     and call it to return a HoloViews object.
@@ -37,51 +38,49 @@
     setattr(pd.DataFrame, 'hvplot', plot_prop)
     ```
     """
 
     __all__ = []
 
     def __init__(self, data, custom_plots={}, **metadata):
-        if "query" in metadata:
-            data = data.query(metadata.pop("query"))
-        if "sel" in metadata:
-            data = data.sel(**metadata.pop("sel"))
-        if "isel" in metadata:
-            data = data.isel(**metadata.pop("isel"))
+        if 'query' in metadata:
+            data = data.query(metadata.pop('query'))
+        if 'sel' in metadata:
+            data = data.sel(**metadata.pop('sel'))
+        if 'isel' in metadata:
+            data = data.isel(**metadata.pop('isel'))
         self._data = data
         self._plots = custom_plots
         self._metadata = metadata
 
     def __call__(self, x=None, y=None, kind=None, **kwds):
         # Convert an array-like to a list
         x = list(x) if is_list_like(x) else x
         y = list(y) if is_list_like(y) else y
 
         if isinstance(kind, str) and kind not in self.__all__:
-            raise NotImplementedError(
-                f"kind='{kind}' for data of type {type(self._data)}"
-            )
+            raise NotImplementedError(f"kind='{kind}' for data of type {type(self._data)}")
 
-        if isinstance(kind, str) and kind == "explorer":
+        if isinstance(kind, str) and kind == 'explorer':
             return self.explorer(x=x, y=y, **kwds)
 
         if panel_available:
-            panel_args = ["widgets", "widget_location", "widget_layout", "widget_type"]
+            panel_args = ['widgets', 'widget_location', 'widget_layout', 'widget_type']
             panel_dict = {}
             for k in panel_args:
                 if k in kwds:
                     panel_dict[k] = kwds.pop(k)
             dynamic, arg_deps, arg_names = process_dynamic_args(x, y, kind, **kwds)
             if dynamic or arg_deps:
 
                 @pn.depends(*arg_deps, **dynamic)
                 def callback(*args, **dyn_kwds):
-                    xd = dyn_kwds.pop("x", x)
-                    yd = dyn_kwds.pop("y", y)
-                    kindd = dyn_kwds.pop("kind", kind)
+                    xd = dyn_kwds.pop('x', x)
+                    yd = dyn_kwds.pop('y', y)
+                    kindd = dyn_kwds.pop('kind', kind)
 
                     combined_kwds = dict(kwds, **dyn_kwds)
                     fn_args = defaultdict(list)
                     for name, arg in zip(arg_names, args):
                         fn_args[(name, kwds[name])].append(arg)
                     for (name, fn), args in fn_args.items():
                         combined_kwds[name] = fn(*args)
@@ -93,40 +92,40 @@
                 plot = self._get_converter(x, y, kind, **kwds)(kind, x, y)
                 return pn.panel(plot, **panel_dict)
 
         return self._get_converter(x, y, kind, **kwds)(kind, x, y)
 
     def _get_converter(self, x=None, y=None, kind=None, **kwds):
         params = dict(self._metadata, **kwds)
-        x = x or params.pop("x", None)
-        y = y or params.pop("y", None)
-        kind = kind or params.pop("kind", None)
+        x = x or params.pop('x', None)
+        y = y or params.pop('y', None)
+        kind = kind or params.pop('kind', None)
         return HoloViewsConverter(self._data, x, y, kind=kind, **params)
 
     def __dir__(self):
         """
         List default attributes and custom defined plots.
         """
         dirs = super().__dir__()
         return sorted(list(dirs) + list(self._plots))
 
     def __getattribute__(self, name):
         """
         Custom getattribute to expose user defined subplots.
         """
-        plots = object.__getattribute__(self, "_plots")
+        plots = object.__getattribute__(self, '_plots')
         if name in plots:
             plot_opts = plots[name]
-            if "kind" in plot_opts and name in HoloViewsConverter._kind_mapping:
+            if 'kind' in plot_opts and name in HoloViewsConverter._kind_mapping:
                 param.main.param.warning(
-                    "Custom options for existing plot types should not "
+                    'Custom options for existing plot types should not '
                     "declare the 'kind' argument. The .{} plot method "
-                    "was unexpectedly customized with kind={!r}.".format(plot_opts["kind"], name)
+                    'was unexpectedly customized with kind={!r}.'.format(plot_opts['kind'], name)
                 )
-                plot_opts["kind"] = name
+                plot_opts['kind'] = name
             return hvPlotBase(self._data, **dict(self._metadata, **plot_opts))
         return super().__getattribute__(name)
 
     def explorer(self, x=None, y=None, **kwds):
         """
         The `explorer` plot allows you to interactively explore your data.
 
@@ -161,14 +160,15 @@
                     "date": pd.date_range("2022-01-03", "2022-01-09"),
                     "string": ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"],
                 },
             )
             df.hvplot.explorer()
         """
         from ..ui import explorer as ui_explorer
+
         return ui_explorer(self._data, x=x, y=y, **kwds)
 
 
 class hvPlotTabular(hvPlotBase):
     """
     The plotting method: `df.hvplot(...)` creates a plot similarly to the familiar Pandas
     `df.plot` method.
@@ -242,38 +242,38 @@
         line * markers
 
     Please note that you can pass widgets or reactive functions as arguments instead of
     literal values, c.f. https://hvplot.holoviz.org/user_guide/Widgets.html.
     """
 
     __all__ = [
-        "line",
-        "step",
-        "scatter",
-        "area",
-        "errorbars",
-        "ohlc",
-        "heatmap",
-        "hexbin",
-        "bivariate",
-        "bar",
-        "barh",
-        "box",
-        "violin",
-        "hist",
-        "kde",
-        "density",
-        "table",
-        "dataset",
-        "points",
-        "vectorfield",
-        "polygons",
-        "paths",
-        "labels",
-        "explorer",
+        'line',
+        'step',
+        'scatter',
+        'area',
+        'errorbars',
+        'ohlc',
+        'heatmap',
+        'hexbin',
+        'bivariate',
+        'bar',
+        'barh',
+        'box',
+        'violin',
+        'hist',
+        'kde',
+        'density',
+        'table',
+        'dataset',
+        'points',
+        'vectorfield',
+        'polygons',
+        'paths',
+        'labels',
+        'explorer',
     ]
 
     def line(self, x=None, y=None, **kwds):
         """
         The `line` plot connects the points with a continuous curve.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/line.html
@@ -363,17 +363,17 @@
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Curve.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.line.html
         - Plotly: https://plotly.com/python/line-charts/
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.plot.html
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.lineplot.html
         - Wiki: https://en.wikipedia.org/wiki/Line_chart
         """
-        return self(x, y, kind="line", **kwds)
+        return self(x, y, kind='line', **kwds)
 
-    def step(self, x=None, y=None, where="mid", **kwds):
+    def step(self, x=None, y=None, where='mid', **kwds):
         """
         The `step` plot connects the points with piece-wise constant curves.
 
         The `step` plot can be used pretty much anytime the `line` plot might be used, and has many
         of the same options available.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/step.html
@@ -462,15 +462,15 @@
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/reference/models/glyphs/step.html
         - HoloViews: https://holoviews.org/gallery/demos/bokeh/step_chart.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.line.html (use `draw_style='step')
         - Plotly: https://plotly.com/python/line-charts/ (See the Interpolation Section)
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.step.html
         """
-        return self(x, y, kind="step", where=where, **kwds)
+        return self(x, y, kind='step', where=where, **kwds)
 
     def scatter(self, x=None, y=None, **kwds):
         """
         The `scatter` plot visualizes your points as markers in 2D space. You can visualize
         one more dimension by using colors.
 
         The `scatter` plot is a good first way to plot data with non continuous axes.
@@ -569,15 +569,15 @@
         - HoloViews: https://holoviews.org/reference/elements/matplotlib/Scatter.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.scatter.html
         - Plotly: https://plotly.com/python/line-and-scatter/
         - Matplotlib:  https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.scatter.html
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.scatterplot.html
         - Wiki: https://en.wikipedia.org/wiki/Scatter_plot
         """
-        return self(x, y, kind="scatter", **kwds)
+        return self(x, y, kind='scatter', **kwds)
 
     def area(self, x=None, y=None, y2=None, stacked=True, **kwds):
         """
         The `area` plot can be used to color the area under a line or to color the space between two
         lines.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/area.html
@@ -647,17 +647,17 @@
         - Bokeh: https://docs.bokeh.org/en/latest/docs/user_guide/plotting.html#directed-areas
         - HoloViews: https://holoviews.org/reference/elements/matplotlib/Area.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.area.html
         - Plotly: https://plotly.com/python/filled-area-plots/
         - Matplotlib:  https://matplotlib.org/stable/gallery/lines_bars_and_markers/fill_between_demo.html
         - Wiki: https://en.wikipedia.org/wiki/Area_chart
         """
-        if "alpha" not in kwds and not stacked:
-            kwds["alpha"] = 0.5
-        return self(x, y, y2=y2, kind="area", stacked=stacked, **kwds)
+        if 'alpha' not in kwds and not stacked:
+            kwds['alpha'] = 0.5
+        return self(x, y, y2=y2, kind='area', stacked=stacked, **kwds)
 
     def errorbars(self, x=None, y=None, yerr1=None, yerr2=None, **kwds):
         """
         `errorbars` provide a visual indicator for the variability of the plotted data on a graph.
         They are usually overlaid with other plots such as `scatter` , `line` or `bar` plots to
         indicate the variability.
 
@@ -736,15 +736,15 @@
         - Bokeh: https://docs.bokeh.org/en/latest/docs/user_guide/annotations.html#whiskers
         - HoloViews: https://holoviews.org/reference/elements/bokeh/ErrorBars.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.errorbar.html
         - Pandas: https://pandas.pydata.org/docs/user_guide/visualization.html#visualization-errorbars
         - Plotly: https://plotly.com/python/error-bars/
         - Wikipedia: https://en.wikipedia.org/wiki/Error_bar
         """
-        return self(x, y, kind="errorbars", yerr1=yerr1, yerr2=yerr2, **kwds)
+        return self(x, y, kind='errorbars', yerr1=yerr1, yerr2=yerr2, **kwds)
 
     def ohlc(self, x=None, y=None, **kwds):
         """
         The `ohlc` plot visualizes the open, high, low and close prices of stocks and other assets.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/ohlc.html
 
@@ -793,15 +793,15 @@
         ----------
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/candlestick.html
         - Matplotlib: https://www.statology.org/matplotlib-python-candlestick-chart/
         - Plotly: https://plotly.com/python/ohlc-charts/
         - Wikipedia: https://en.wikipedia.org/wiki/Candlestick_chart
         """
-        return self(kind="ohlc", x=x, y=y, **kwds)
+        return self(kind='ohlc', x=x, y=y, **kwds)
 
     def heatmap(self, x=None, y=None, C=None, colorbar=True, **kwds):
         """
         `heatmap` visualises tabular data indexed by two key dimensions as a grid of colored values.
         This allows spotting correlations in multivariate data and provides a high-level overview
         of how the two variables are plotted.
 
@@ -856,15 +856,15 @@
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/categorical_heatmap.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/HeatMap.html
         - Matplotlib: https://matplotlib.org/stable/gallery/images_contours_and_fields/image_annotated_heatmap.html
         - Plotly: https://plotly.com/python/heatmaps/
         - Wiki: https://en.wikipedia.org/wiki/Heat_map
         """
-        return self(x, y, kind="heatmap", C=C, colorbar=colorbar, **kwds)
+        return self(x, y, kind='heatmap', C=C, colorbar=colorbar, **kwds)
 
     def hexbin(self, x=None, y=None, C=None, colorbar=True, **kwds):
         """
         The `hexbin` plot uses hexagons to split the area into several parts and attribute a color
         to it.
 
         `hexbin` offers a straightforward method for plotting dense data.
@@ -924,15 +924,15 @@
         ----------
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/hexbin.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/HexTiles.html
         - Plotly: https://plotly.com/python/hexbin-mapbox/
         - Wiki: https://think.design/services/data-visualization-data-design/hexbin/
         """
-        return self(x, y, kind="hexbin", C=C, colorbar=colorbar, **kwds)
+        return self(x, y, kind='hexbin', C=C, colorbar=colorbar, **kwds)
 
     def bivariate(self, x=None, y=None, colorbar=True, **kwds):
         """
         A bivariate, density plot uses nested contours (or contours plus colors) to indicate
         regions of higher local density.
 
         `bivariate` plots can be a useful alternative to scatter plots, if your data are too dense
@@ -996,15 +996,15 @@
         - ggplot: https://bio304-class.github.io/bio304-fall2017/ggplot-bivariate.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Bivariate.html
         - Plotly: https://plotly.com/python/2d-histogram-contour/
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.kdeplot.html
         - Wiki: https://en.wikipedia.org/wiki/Bivariate_analysis
         """
-        return self(x, y, kind="bivariate", colorbar=colorbar, **kwds)
+        return self(x, y, kind='bivariate', colorbar=colorbar, **kwds)
 
     def bar(self, x=None, y=None, **kwds):
         """
         A vertical bar plot
 
         A `bar` plot represents categorical data with rectangular bars
         with heights proportional to the values that they represent. The x-axis
@@ -1085,15 +1085,15 @@
         - Bokeh: https://docs.bokeh.org/en/latest/docs/reference/models/glyphs/vbar.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Bars.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.bar.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.bar.html
         - Plotly: https://plotly.com/python/bar-charts/
         - Wiki: https://en.wikipedia.org/wiki/Bar_chart
         """
-        return self(x, y, kind="bar", **kwds)
+        return self(x, y, kind='bar', **kwds)
 
     def barh(self, x=None, y=None, **kwds):
         """
         A horizontal bar plot
 
         A `barh` plot represents categorical data with rectangular bars
         with heights proportional to the values that they represent. The y-axis of the chart
@@ -1149,15 +1149,15 @@
         - Bokeh: https://docs.bokeh.org/en/latest/docs/reference/models/glyphs/hbar.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Bars.html
         - Matplotlib: https://matplotlib.org/stable/gallery/lines_bars_and_markers/barh.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.barh.html
         - Plotly: https://plotly.com/python/horizontal-bar-charts/
         - Wiki: https://en.wikipedia.org/wiki/Bar_chart
         """
-        return self(x, y, kind="barh", **kwds)
+        return self(x, y, kind='barh', **kwds)
 
     def box(self, y=None, by=None, **kwds):
         """
         The `box` plot gives you a visual idea about the *locality*, *spread* and *skewness* of
         numerical data through their quartiles. It is also known as *box and whiskers plot*.
 
         `box` plots are most useful when grouped by additional dimensions.
@@ -1215,15 +1215,15 @@
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/boxplot.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/BoxWhisker.html
         - Matplotlib: https://matplotlib.org/stable/plot_types/stats/boxplot_plot.html#sphx-glr-plot-types-stats-boxplot-plot-py
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.boxplot.html
         - Plotly: https://plotly.com/python/box-plots/
         - Wiki: https://en.wikipedia.org/wiki/Box_plot
         """
-        return self(kind="box", x=None, y=y, by=by, **dict(kwds, hover=False))
+        return self(kind='box', x=None, y=y, by=by, **dict(kwds, hover=False))
 
     def violin(self, y=None, by=None, **kwds):
         """
         `violin`  plots are similar to `box` plots, but they provide a better sense of the
         distribution of data.
 
         Note that `violin` plots depend on the `scipy` library.
@@ -1281,15 +1281,15 @@
 
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.violinplot.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Violin.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.violinplot.html
         - Plotly: https://plotly.com/python/violin/
         - Wiki: https://en.wikipedia.org/wiki/Violin_plot
         """
-        return self(kind="violin", x=None, y=y, by=by, **dict(kwds, hover=False))
+        return self(kind='violin', x=None, y=y, by=by, **dict(kwds, hover=False))
 
     def hist(self, y=None, by=None, **kwds):
         """
         A `histogram` displays an approximate representation of the distribution of continuous data.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/hist.html
 
@@ -1362,15 +1362,15 @@
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Histogram.html
         - Pandas: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.plot.hist.html
         - Plotly: https://plotly.com/python/histograms/
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.hist.html
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.histplot.html
         - Wiki: https://en.wikipedia.org/wiki/Histogram
         """
-        return self(kind="hist", x=None, y=y, by=by, **kwds)
+        return self(kind='hist', x=None, y=y, by=by, **kwds)
 
     def kde(self, y=None, by=None, **kwds):
         """
         The Kernel density estimate (`kde`) plot shows the distribution and spread of the data.
 
         The `kde` and `density` plots are the same.
 
@@ -1440,15 +1440,15 @@
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Distribution.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.kde.html
         - Plotly: https://plotly.com/python/distplot/
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.kdeplot.html
         - Wiki: https://en.wikipedia.org/wiki/Kernel_density_estimation
         """
-        return self(kind="kde", x=None, y=y, by=by, **kwds)
+        return self(kind='kde', x=None, y=y, by=by, **kwds)
 
     def density(self, y=None, by=None, **kwds):
         """
         The Kernel density estimate (`density`) plot shows the distribution and spread of the data.
 
         The `kde` and `density` plots are the same.
 
@@ -1518,15 +1518,15 @@
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Distribution.html
         - Pandas: https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.plot.kde.html
         - Plotly: https://plotly.com/python/distplot/
         - Seaborn: https://seaborn.pydata.org/generated/seaborn.kdeplot.html
         - Wiki: https://en.wikipedia.org/wiki/Kernel_density_estimation
         """
-        return self(kind="kde", x=None, y=y, by=by, **kwds)
+        return self(kind='kde', x=None, y=y, by=by, **kwds)
 
     def table(self, columns=None, **kwds):
         """
         Displays a 'table'.
 
         Reference: https://hvplot.holoviz.org/reference/tabular/table.html
 
@@ -1565,15 +1565,15 @@
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Table.html
         - Plotly: https://plotly.com/python/table/
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.table.html
         """
-        return self(kind="table", **dict(kwds, columns=columns))
+        return self(kind='table', **dict(kwds, columns=columns))
 
     def dataset(self, columns=None, **kwds):
         """
         The 'dataset' wraps a tabular or gridded dataset and can be further transformed and
         annotated via methods from HoloViews.
 
         Parameters
@@ -1605,15 +1605,15 @@
 
         References
         ----------
 
         - HoloViews Tabular: https://holoviews.org/getting_started/Tabular_Datasets.html
         - HoloViews Gridded: https://holoviews.org/getting_started/Gridded_Datasets.html
         """
-        return self(kind="dataset", **dict(kwds, columns=columns))
+        return self(kind='dataset', **dict(kwds, columns=columns))
 
     def points(self, x=None, y=None, **kwds):
         """
         A `points` plot visualizes positions in a 2D space. This is useful for example for
         geographic plots.
 
         There is no assumption that 'y' depends on 'x'. This is different from a `scatter` plot
@@ -1665,15 +1665,15 @@
             plot
 
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Points.html
         """
-        return self(x, y, kind="points", **kwds)
+        return self(x, y, kind='points', **kwds)
 
     def vectorfield(self, x=None, y=None, angle=None, mag=None, **kwds):
         """
         `vectorfield visualizes vectors given by the (`x , `y`) starting point, a magnitude (`mag`)
         and an `angle` . A `vectorfield` plot is also known as a `quiver` plot.
 
         Reference: https://hvplot.holoviz.org/reference/xarray/vectorfield.html
@@ -1726,15 +1726,15 @@
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/quiver.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/VectorField.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.quiver.html
         - Plotly: https://plotly.com/python/quiver-plots/
         - Wiki: https://simple.wikipedia.org/wiki/Vector_field
         """
-        return self(x, y, angle=angle, mag=mag, kind="vectorfield", **kwds)
+        return self(x, y, angle=angle, mag=mag, kind='vectorfield', **kwds)
 
     def polygons(self, x=None, y=None, c=None, **kwds):
         """
         Polygon plot for geopandas dataframes.
 
         Reference: https://hvplot.holoviz.org/reference/geopandas/polygons.html
 
@@ -1768,15 +1768,15 @@
 
             import geopandas as gpd
             import hvplot.pandas
 
             countries = gpd.read_file(gpd.datasets.get_path('naturalearth_lowres'))
             countries.hvplot.polygons(geo=True, c='pop_est', hover_cols='all')
         """
-        return self(x, y, c=c, kind="polygons", **kwds)
+        return self(x, y, c=c, kind='polygons', **kwds)
 
     def paths(self, x=None, y=None, c=None, **kwds):
         """
         LineString and LineRing plot for geopandas dataframes.
 
         Parameters
         ----------
@@ -1795,15 +1795,15 @@
         to learn more about its parameters and options.
 
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Path.html
         """
-        return self(x, y, c=c, kind="paths", **kwds)
+        return self(x, y, c=c, kind='paths', **kwds)
 
     def labels(self, x=None, y=None, text=None, **kwds):
         """
         Labels plot.
 
         `labels` are mostly useful when overlaid on top of other plots using the `*`
         operator.
@@ -1856,40 +1856,40 @@
         ----------
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/reference/models/glyphs/text.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Labels.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.text.html#matplotlib.pyplot.text
         - Plotly: https://plotly.com/python/text-and-annotations/
         """
-        return self(x, y, text=text, kind="labels", **kwds)
+        return self(x, y, text=text, kind='labels', **kwds)
 
 
 class hvPlotTabularPolars(hvPlotTabular):
     def _get_converter(self, x=None, y=None, kind=None, **kwds):
         import polars as pl
 
         params = dict(self._metadata, **kwds)
-        x = x or params.pop("x", None)
-        y = y or params.pop("y", None)
-        kind = kind or params.pop("kind", None)
+        x = x or params.pop('x', None)
+        y = y or params.pop('y', None)
+        kind = kind or params.pop('kind', None)
 
         # Find columns which should be converted for LazyDataFrame and DataFrame
         if isinstance(self._data, (pl.LazyFrame, pl.DataFrame)):
-            if params.get("hover_cols") == "all":
+            if params.get('hover_cols') == 'all':
                 columns = list(self._data.columns)
             else:
                 possible_columns = [
                     [v] if isinstance(v, str) else v
                     for v in params.values()
                     if isinstance(v, (str, list))
                 ]
 
-                columns = (
-                    set(self._data.columns) & set(itertools.chain(*possible_columns))
-                ) or {self._data.columns[0]}
+                columns = (set(self._data.columns) & set(itertools.chain(*possible_columns))) or {
+                    self._data.columns[0]
+                }
                 if y is None:
                     # When y is not specified HoloViewsConverter finds all the numeric
                     # columns and use them as y values (see _process_chart_y). We meed
                     # to include these columns too.
                     columns |= set(self._data.select(pl.col(pl.NUMERIC_DTYPES)).columns)
                 xs = x if is_list_like(x) else (x,)
                 ys = y if is_list_like(y) else (y,)
@@ -1901,17 +1901,15 @@
         if isinstance(self._data, pl.DataFrame):
             data = self._data.select(columns).to_pandas()
         elif isinstance(self._data, pl.Series):
             data = self._data.to_pandas()
         elif isinstance(self._data, pl.LazyFrame):
             data = self._data.select(columns).collect().to_pandas()
         else:
-            raise ValueError(
-                "Only Polars DataFrame, Series, and LazyFrame are supported"
-            )
+            raise ValueError('Only Polars DataFrame, Series, and LazyFrame are supported')
 
         return HoloViewsConverter(data, x, y, kind=kind, **params)
 
 
 class hvPlot(hvPlotTabular):
     """
     The plotting method: `df.hvplot(...)` creates a plot similarly to the familiar Pandas
@@ -1980,42 +1978,42 @@
         line * markers
 
     Please note that you can pass widgets or reactive functions as arguments instead of
     literal values, c.f. https://hvplot.holoviz.org/user_guide/Widgets.html.
     """
 
     __all__ = [
-        "line",
-        "step",
-        "scatter",
-        "area",
-        "errorbars",
-        "heatmap",
-        "hexbin",
-        "bivariate",
-        "bar",
-        "barh",
-        "box",
-        "violin",
-        "hist",
-        "kde",
-        "density",
-        "table",
-        "dataset",
-        "points",
-        "vectorfield",
-        "polygons",
-        "paths",
-        "labels",
-        "image",
-        "rgb",
-        "quadmesh",
-        "contour",
-        "contourf",
-        "explorer",
+        'line',
+        'step',
+        'scatter',
+        'area',
+        'errorbars',
+        'heatmap',
+        'hexbin',
+        'bivariate',
+        'bar',
+        'barh',
+        'box',
+        'violin',
+        'hist',
+        'kde',
+        'density',
+        'table',
+        'dataset',
+        'points',
+        'vectorfield',
+        'polygons',
+        'paths',
+        'labels',
+        'image',
+        'rgb',
+        'quadmesh',
+        'contour',
+        'contourf',
+        'explorer',
     ]
 
     def image(self, x=None, y=None, z=None, colorbar=True, **kwds):
         """
         Image plot
 
         You can use `image` to display for example geographic data with independent `latitude` and
@@ -2062,15 +2060,15 @@
         ----------
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/gallery/image.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Image.html
         - Matplotlib: https://matplotlib.org/stable/tutorials/introductory/images.html
         - Plotly: https://plotly.com/python/imshow/
         """
-        return self(x, y, z=z, kind="image", colorbar=colorbar, **kwds)
+        return self(x, y, z=z, kind='image', colorbar=colorbar, **kwds)
 
     def rgb(self, x=None, y=None, z=None, bands=None, **kwds):
         """
         RGB plot
 
         `rgb`  can be used to display images that are distributed as three separate "channels" or
         "bands".
@@ -2106,16 +2104,16 @@
 
         - Bokeh: https://docs.bokeh.org/en/latest/docs/reference/models/glyphs/image_rgba.html
         - HoloViews: https://holoviews.org/reference/elements/bokeh/RGB.html
         - Matplotlib: https://matplotlib.org/stable/tutorials/introductory/images.html
         - Plotly: https://plotly.com/python/imshow/
         """
         if bands is not None:
-            kwds["bands"] = bands
-        return self(x, y, z=z, kind="rgb", **kwds)
+            kwds['bands'] = bands
+        return self(x, y, z=z, kind='rgb', **kwds)
 
     def quadmesh(self, x=None, y=None, z=None, colorbar=True, **kwds):
         """
         QuadMesh plot
 
         `quadmesh` allows you to plot values on an irregular grid by representing each value as a
         polygon.
@@ -2158,15 +2156,15 @@
             ds.Tair.hvplot.quadmesh(x='xc', y='yc', geo=True, widget_location='bottom')
 
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/QuadMesh.html
         """
-        return self(x, y, z=z, kind="quadmesh", colorbar=colorbar, **kwds)
+        return self(x, y, z=z, kind='quadmesh', colorbar=colorbar, **kwds)
 
     def contour(self, x=None, y=None, z=None, colorbar=True, **kwds):
         """
         Line contour plot
 
         Reference: https://hvplot.holoviz.org/reference/xarray/contour.html
 
@@ -2221,15 +2219,15 @@
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Contours.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
         - Plotly: https://plotly.com/python/contour-plots/
         """
-        return self(x, y, z=z, kind="contour", colorbar=colorbar, **kwds)
+        return self(x, y, z=z, kind='contour', colorbar=colorbar, **kwds)
 
     def contourf(self, x=None, y=None, z=None, colorbar=True, **kwds):
         """
         Filled contour plot
 
         Reference. https://hvplot.holoviz.org/reference/xarray/contourf.html
 
@@ -2283,8 +2281,8 @@
         References
         ----------
 
         - HoloViews: https://holoviews.org/reference/elements/bokeh/Contours.html
         - Matplotlib: https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
         - Plotly: https://plotly.com/python/contour-plots/
         """
-        return self(x, y, z=z, kind="contourf", colorbar=colorbar, **kwds)
+        return self(x, y, z=z, kind='contourf', colorbar=colorbar, **kwds)
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/lag_plot.py` & `hvplot-0.9.3a1/hvplot/plotting/lag_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,18 @@
 
     Returns:
     --------
     obj : HoloViews object
         The HoloViews representation of the plot.
     """
     if lag != int(lag) or int(lag) <= 0:
-        raise ValueError("lag must be a positive integer")
+        raise ValueError('lag must be a positive integer')
     lag = int(lag)
 
     values = data.values
     y1 = 'y(t)'
     y2 = f'y(t + {lag})'
-    lags = pd.DataFrame({y1: values[:-lag].T.ravel(),
-                         y2: values[lag:].T.ravel()})
+    lags = pd.DataFrame({y1: values[:-lag].T.ravel(), y2: values[lag:].T.ravel()})
     if isinstance(data, pd.DataFrame):
         lags['variable'] = np.repeat(data.columns, lags.shape[0] / data.shape[1])
         kwds['c'] = 'variable'
     return hvPlotTabular(lags)(y1, y2, kind='scatter', **kwds)
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/parallel_coordinates.py` & `hvplot-0.9.3a1/hvplot/plotting/parallel_coordinates.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 import colorcet as cc
 
 from ..backend_transforms import _transfer_opts_cur_backend
 from ..util import with_hv_extension
 
 
 @with_hv_extension
-def parallel_coordinates(data, class_column, cols=None, alpha=0.5,
-                         width=600, height=300, var_name='variable',
-                         value_name='value', cmap=None, colormap=None,
-                         **kwds):
+def parallel_coordinates(
+    data,
+    class_column,
+    cols=None,
+    alpha=0.5,
+    width=600,
+    height=300,
+    var_name='variable',
+    value_name='value',
+    cmap=None,
+    colormap=None,
+    **kwds,
+):
     """
     Parallel coordinates plotting.
 
     To show a set of points in an n-dimensional space, a backdrop is drawn
     consisting of n parallel lines. A point in n-dimensional space is
     represented as a polyline with vertices on the parallel axes; the
     position of the vertex on the i-th axis corresponds to the i-th coordinate
@@ -43,28 +52,34 @@
     # Transform the dataframe to be used in Vega-Lite
     if cols is not None:
         data = data[list(cols) + [class_column]]
     cols = data.columns
     df = data.reset_index()
     index = (set(df.columns) - set(cols)).pop()
     assert index in df.columns
-    df = df.melt([index, class_column],
-                 var_name=var_name, value_name=value_name)
+    df = df.melt([index, class_column], var_name=var_name, value_name=value_name)
 
     labelled = [] if var_name == 'variable' else ['x']
     if value_name != 'value':
         labelled.append('y')
-    options = {'Curve': dict(kwds, labelled=labelled, alpha=alpha, width=width, height=height),
-               'Overlay': dict(legend_limit=5000)}
+    options = {
+        'Curve': dict(kwds, labelled=labelled, alpha=alpha, width=width, height=height),
+        'Overlay': dict(legend_limit=5000),
+    }
 
     dataset = hv.Dataset(df)
     groups = dataset.to(hv.Curve, var_name, value_name).overlay(index).items()
 
     if cmap and colormap:
-        raise TypeError("Only specify one of `cmap` and `colormap`.")
+        raise TypeError('Only specify one of `cmap` and `colormap`.')
     cmap = cmap or colormap or cc.palette['glasbey_category10']
     colors = hv.plotting.util.process_cmap(cmap, categorical=True, ncolors=len(groups))
 
-    el = hv.Overlay([curve.relabel(k).options('Curve', color=c, backend='bokeh')
-                       for c, (k, v) in zip(colors, groups) for curve in v]).options(options, backend='bokeh')
+    el = hv.Overlay(
+        [
+            curve.relabel(k).options('Curve', color=c, backend='bokeh')
+            for c, (k, v) in zip(colors, groups)
+            for curve in v
+        ]
+    ).options(options, backend='bokeh')
     el = _transfer_opts_cur_backend(el)
     return el
```

### Comparing `hvplot-0.9.2rc1/hvplot/plotting/scatter_matrix.py` & `hvplot-0.9.3a1/hvplot/plotting/scatter_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,33 @@
 
 from ..backend_transforms import _transfer_opts_cur_backend
 from ..converter import HoloViewsConverter
 from ..util import with_hv_extension, _convert_col_names_to_str
 
 
 @with_hv_extension
-def scatter_matrix(data, c=None, chart='scatter', diagonal='hist',
-                   alpha=0.5, nonselection_alpha=0.1,
-                   tools=None, cmap=None, colormap=None,
-                   diagonal_kwds=None, hist_kwds=None, density_kwds=None,
-                   datashade=False, rasterize=False, dynspread=False, spread=False,
-                   **kwds):
+def scatter_matrix(
+    data,
+    c=None,
+    chart='scatter',
+    diagonal='hist',
+    alpha=0.5,
+    nonselection_alpha=0.1,
+    tools=None,
+    cmap=None,
+    colormap=None,
+    diagonal_kwds=None,
+    hist_kwds=None,
+    density_kwds=None,
+    datashade=False,
+    rasterize=False,
+    dynspread=False,
+    spread=False,
+    **kwds,
+):
     """
     Scatter matrix of numeric columns.
 
     A scatter_matrix shows all the pairwise relationships between the columns.
     Each non-diagonal plots the corresponding columns against each other,
     while the diagonal plot shows the distribution of each individual column.
 
@@ -88,49 +101,49 @@
     diagonal = HoloViewsConverter._kind_mapping[diagonal]
     chart = HoloViewsConverter._kind_mapping[chart]
 
     if rasterize or datashade:
         try:
             import datashader  # noqa
         except ImportError:
-            raise ImportError("rasterize and datashade require "
-                              "datashader to be installed.")
+            raise ImportError('rasterize and datashade require datashader to be installed.')
         from ..util import hv_version
+
         if hv_version <= Version('1.14.6'):
             warnings.warn(
-                "Versions of holoviews before 1.14.7 did not support "
-                "dynamic update of rasterized/datashaded scatter matrix. "
-                "Update holoviews to a newer version."
+                'Versions of holoviews before 1.14.7 did not support '
+                'dynamic update of rasterized/datashaded scatter matrix. '
+                'Update holoviews to a newer version.'
             )
 
     if rasterize and datashade:
-        raise ValueError("Choose to either rasterize or "
-                         "datashade the scatter matrix, not both.")
+        raise ValueError('Choose to either rasterize or datashade the scatter matrix, not both.')
 
     if not rasterize and not datashade and (spread or dynspread):
-        raise ValueError("dynspread or spread need rasterize "
-                         "or datashade to be set to True.")
+        raise ValueError('dynspread or spread need rasterize or datashade to be set to True.')
 
     if rasterize:
         import holoviews.operation.datashader as hd
+
         if dynspread or spread:
             if hd.ds_version < Version('0.12.0'):
                 raise RuntimeError(
                     'Any version of datashader less than 0.12.0 does '
-                    'not support rasterize with dynspread or spread.')
+                    'not support rasterize with dynspread or spread.'
+                )
 
-    #remove datashade kwds
+    # remove datashade kwds
     if datashade or rasterize:
         import holoviews.operation.datashader as hd
 
         ds_kwds = {}
         if 'aggregator' in kwds:
             ds_kwds['aggregator'] = kwds.pop('aggregator')
 
-    #remove dynspread kwds
+    # remove dynspread kwds
     sp_kwds = {}
     if dynspread:
         if 'max_px' in kwds:
             sp_kwds['max_px'] = kwds.pop('max_px')
         if 'threshold' in kwds:
             sp_kwds['threshold'] = kwds.pop('threshold')
         if 'shape' in kwds:
@@ -146,46 +159,47 @@
             sp_kwds['shape'] = kwds.pop('shape')
         if 'how' in kwds:
             sp_kwds['how'] = kwds.pop('how')
         if 'mask' in kwds:
             sp_kwds['mask'] = kwds.pop('mask')
 
     tools = tools or ['box_select', 'lasso_select']
-    chart_opts = dict(alpha=alpha, tools=tools,
-                      nonselection_alpha=nonselection_alpha, **kwds)
+    chart_opts = dict(alpha=alpha, tools=tools, nonselection_alpha=nonselection_alpha, **kwds)
     if c:
         if cmap and colormap:
-            raise TypeError("Only specify `cmap` or `colormap`.")
+            raise TypeError('Only specify `cmap` or `colormap`.')
         ncolors = len(_np.unique(data.dimension_values(c)))
         cmap = cmap or colormap or 'Category10'
         cmap = _hv.plotting.util.process_cmap(cmap, ncolors=ncolors, categorical=True)
         chart_opts['cmap'] = cmap
 
-    #get initial scatter matrix.  No color.
+    # get initial scatter matrix.  No color.
     grid = _hv.operation.gridmatrix(data, diagonal_type=diagonal, chart_type=chart)
 
     if c:
-        #change colors for scatter matrix
+        # change colors for scatter matrix
         chart_opts['color'] = c
         # Add color vdim to each plot.
-        grid = grid.map(lambda x: x.clone(vdims=x.vdims+[c]), 'Scatter')
+        grid = grid.map(lambda x: x.clone(vdims=x.vdims + [c]), 'Scatter')
         # create a new scatter matrix with groups for each catetory, so now the histogram will
         # show separate colors for each group.
-        groups = _hv.operation.gridmatrix(data.groupby(c).overlay(),
-                                          chart_type=chart,
-                                          diagonal_type=diagonal)
+        groups = _hv.operation.gridmatrix(
+            data.groupby(c).overlay(), chart_type=chart, diagonal_type=diagonal
+        )
         # take the correct layer from each Overlay object within the scatter matrix.
-        grid = (grid * groups).map(lambda x: x.get(0) if isinstance(x.get(0), chart) else x.get(1),
-                                   _hv.Overlay)
-
-    if (diagonal_kwds and hist_kwds) or \
-       (diagonal_kwds and density_kwds) or \
-       (hist_kwds and density_kwds):
-        raise TypeError('Specify at most one of `diagonal_kwds`, `hist_kwds`, or '
-                        '`density_kwds`.')
+        grid = (grid * groups).map(
+            lambda x: x.get(0) if isinstance(x.get(0), chart) else x.get(1), _hv.Overlay
+        )
+
+    if (
+        (diagonal_kwds and hist_kwds)
+        or (diagonal_kwds and density_kwds)
+        or (hist_kwds and density_kwds)
+    ):
+        raise TypeError('Specify at most one of `diagonal_kwds`, `hist_kwds`, or `density_kwds`.')
 
     diagonal_opts = diagonal_kwds or hist_kwds or density_kwds or {}
     # set the histogram colors
     if c:
         diagonal_opts['fill_color'] = _hv.Cycle(cmap)
     # actually changing to the same color scheme for both scatter and histogram plots.
     grid = grid.options(
```

### Comparing `hvplot-0.9.2rc1/hvplot/streamz.py` & `hvplot-0.9.3a1/hvplot/streamz.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 def patch(name='hvplot', extension='bokeh', logo=False):
     from . import hvPlotTabular, post_patch
 
     try:
         import streamz.dataframe as sdf
     except ImportError:
-        raise ImportError('Could not patch plotting API onto streamz. '
-                          'Streamz could not be imported.')
-    _patch_plot = lambda self: hvPlotTabular(self)
+        raise ImportError(
+            'Could not patch plotting API onto streamz. Streamz could not be imported.'
+        )
+    _patch_plot = lambda self: hvPlotTabular(self)  # noqa: E731
     _patch_plot.__doc__ = hvPlotTabular.__call__.__doc__
     patch_property = property(_patch_plot)
     setattr(sdf.DataFrame, name, patch_property)
     setattr(sdf.DataFrames, name, patch_property)
     setattr(sdf.Series, name, patch_property)
     setattr(sdf.Seriess, name, patch_property)
 
     post_patch(extension, logo)
 
+
 patch()
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/conftest.py` & `hvplot-0.9.3a1/hvplot/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,44 @@
+import dask
+
 optional_markers = {
-    "geo": {
-        "help": "Run the tests that require GeoViews",
-        "marker-descr": "Geo test marker",
-        "skip-reason": "Test only runs with the --geo option."
+    'geo': {
+        'help': 'Run the tests that require GeoViews',
+        'marker-descr': 'Geo test marker',
+        'skip-reason': 'Test only runs with the --geo option.',
     },
 }
 
 
 def pytest_addoption(parser):
     for marker, info in optional_markers.items():
-        parser.addoption("--{}".format(marker), action="store_true",
-                         default=False, help=info['help'])
+        parser.addoption(
+            '--{}'.format(marker), action='store_true', default=False, help=info['help']
+        )
 
 
 def pytest_configure(config):
     for marker, info in optional_markers.items():
-        config.addinivalue_line("markers",
-                                "{}: {}".format(marker, info['marker-descr']))
+        config.addinivalue_line('markers', '{}: {}'.format(marker, info['marker-descr']))
 
 
 def pytest_collection_modifyitems(config, items):
     skipped, selected = [], []
-    markers = [m for m in optional_markers if config.getoption(f"--{m}")]
+    markers = [m for m in optional_markers if config.getoption(f'--{m}')]
     empty = not markers
     for item in items:
         if empty and any(m in item.keywords for m in optional_markers):
             skipped.append(item)
         elif empty:
             selected.append(item)
         elif not empty and any(m in item.keywords for m in markers):
             selected.append(item)
         else:
             skipped.append(item)
 
     config.hook.pytest_deselected(items=skipped)
     items[:] = selected
+
+
+# From Dask 2024.3.0 they now use `dask_expr` by default
+# https://github.com/dask/dask/issues/10995
+dask.config.set({'dataframe.query-planning': False})
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/plotting/testohlc.py` & `hvplot-0.9.3a1/hvplot/tests/plotting/testohlc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import pandas as pd
 import hvplot.pandas  # noqa
 
 
-df = pd.DataFrame({
+df = pd.DataFrame(
+    {
         'Open': [100.00, 101.25, 102.75],
         'High': [104.10, 105.50, 110.00],
         'Low': [94.00, 97.10, 99.20],
         'Close': [101.15, 99.70, 109.50],
         'Volume': [10012, 5000, 18000],
-    }, index=[pd.Timestamp('2022-08-01'), pd.Timestamp('2022-08-03'), pd.Timestamp('2022-08-04')])
+    },
+    index=[pd.Timestamp('2022-08-01'), pd.Timestamp('2022-08-03'), pd.Timestamp('2022-08-04')],
+)
 
 ohlc_cols = ['Open', 'High', 'Low', 'Close']
 
 
 def test_ohlc_hover_cols():
     plot = df.hvplot.ohlc(y=ohlc_cols, hover_cols=['Volume'])
     segments = plot.Segments.I
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/plotting/testscattermatrix.py` & `hvplot-0.9.3a1/hvplot/tests/plotting/testscattermatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     Distribution,
     HexTiles,
     Histogram,
     Scatter,
 )
 from hvplot import scatter_matrix
 
-class TestScatterMatrix(TestCase):
 
+class TestScatterMatrix(TestCase):
     def setUp(self):
         self.df = pd.DataFrame(np.random.randn(1000, 4), columns=['a', 'b', 'c', 'd'])
 
     def test_returns_gridmatrix(self):
         sm = scatter_matrix(self.df)
         self.assertIsInstance(sm, GridMatrix)
 
@@ -76,19 +76,18 @@
 
         self.assertIsInstance(sm['a', 'b'], Scatter)
         offdiag_vdims = sm['a', 'b'].vdims
         self.assertTrue('e' in (d.name for d in offdiag_vdims))
 
 
 class TestDatashader(TestCase):
-
     def setUp(self):
         try:
-            import datashader # noqa
-        except:
+            import datashader  # noqa
+        except ImportError:
             raise SkipTest('Datashader not available')
         if sys.maxsize < 2**32:
             raise SkipTest('Datashader does not support 32-bit systems')
         self.df = pd.DataFrame(np.random.randn(1000, 3), columns=['a', 'b', 'c'])
 
     def test_rasterize_datashade_mutually_exclusive(self):
         with self.assertRaises(ValueError):
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/test_links.py` & `hvplot-0.9.3a1/hvplot/tests/test_links.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,57 +11,59 @@
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from urllib.request import urlopen
 import glob
 
 import pytest
 
 # Note: The regex will find urls from code cells in notebooks ending with '\\' because the are really inside \"some_url\"
-URL_REGEX = r"(?i)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+|(\([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\s()<>]+\)))*\)|[^\s`!()\[\]{};:'\".,<>?«»“”‘’]))" # pylint: disable=line-too-long
+URL_REGEX = r"(?i)\b((?:https?://|www\d{0,3}[.]|[a-z0-9.\-]+[.][a-z]{2,4}/)(?:[^\s()<>]+|\(([^\s()<>]+|(\([^\s()<>]+\)))*\))+(?:\(([^\s()<>]+|(\([^\s()<>]+\)))*\)|[^\s`!()\[\]{};:'\".,<>?«»“”‘’]))"  # pylint: disable=line-too-long
 ROOT = pathlib.Path(__file__).parent
 PACKAGE_ROOT = ROOT.parent
 MAX_WORKERS = 10
-POST_FIXES = [".py", ".ipynb", ".md", ".yaml"]
+POST_FIXES = ['.py', '.ipynb', '.md', '.yaml']
 SKIP_URLS = [
-    "https://anaconda.org/anaconda/hvplot",
-    "https://anaconda.org/conda-forge/hvplot",
-    "https://anaconda.org/pyviz/hvplot",
-    "https://creativecommons.org/publicdomain/zero/1.0/",
-    "https://github.com/rasterio/rasterio",
-    "https://www.dask.org",
-    "pyproject.toml/equivalent",
+    'https://anaconda.org/anaconda/hvplot',
+    'https://anaconda.org/conda-forge/hvplot',
+    'https://anaconda.org/pyviz/hvplot',
+    'https://creativecommons.org/publicdomain/zero/1.0/',
+    'https://github.com/rasterio/rasterio',
+    'https://www.dask.org',
+    'pyproject.toml/equivalent',
 ]
 
 
 def _get_files_to_check():
     for post_fix in POST_FIXES:
-        for file in glob.glob("**/*" + post_fix, recursive=True):
+        for file in glob.glob('**/*' + post_fix, recursive=True):
             yield pathlib.Path(file)
 
 
 FIXTURES = [pytest.param(file, id=str(file)) for file in _get_files_to_check()]
 
 
 def _skip_url(url: str):
     if url in SKIP_URLS:
         return True
-    if url.startswith("https://github.com/holoviz/hvplot/pull/"):
+    if url.startswith('https://github.com/holoviz/hvplot/pull/'):
         return True
-    if url.startswith("https://img.shields.io"):
+    if url.startswith('https://img.shields.io'):
         return True
-    if url.startswith("assets.holoviews.org/data/"):
+    if url.startswith('assets.holoviews.org/data/'):
         return True
-    if url.startswith("Math.PI"):
+    if url.startswith('Math.PI'):
         return True
     return False
 
+
 def _clean_url(url: str):
-    if url.endswith("\\"):
+    if url.endswith('\\'):
         return url[0:-1]
     return url
 
+
 def _find_urls(text):
     url = re.findall(URL_REGEX, text)
     return {_clean_url(x[0]) for x in url if not _skip_url(x[0])}
 
 
 def _request_a_response(url):
     return urlopen(url)
@@ -76,19 +78,17 @@
             futures[executor.submit(_request_a_response, url)] = url
 
         for future in as_completed(futures):
             url = futures[future]
             try:
                 result = future.result()
             except Exception as ex:
-                raise ValueError(f"The url {url} raised an exception") from ex
+                raise ValueError(f'The url {url} raised an exception') from ex
             if not result.status == 200:
-                raise ValueError(
-                    f"The url {url} responded with status {result.status}, not 200."
-                )
+                raise ValueError(f'The url {url} responded with status {result.status}, not 200.')
 
         return True
 
 
 # @pytest.mark.parametrize(["file"], FIXTURES)
 # def test_urls(file: pathlib.Path):
 #     """The urls is docstring should be valid"""
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testbackend_transforms.py` & `hvplot-0.9.3a1/hvplot/tests/testbackend_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,28 @@
     ('width', 'height', 'aspect', 'opts'),
     (
         (300, 100, None, {'aspect': 3.0, 'fig_size': 100.0}),
         (300, None, 3, {'aspect': 3, 'fig_size': 100.0}),
         (None, 300, 3, {'aspect': 3, 'fig_size': 100.0}),
         (300, None, None, {'fig_size': 100.0}),
         (None, 300, None, {'fig_size': 100.0}),
-    )
+    ),
 )
 def test_transform_size_to_mpl(width, height, aspect, opts):
     assert _transform_size_to_mpl(width, height, aspect) == opts
 
 
 @pytest.mark.parametrize(
     ('element', 'opt', 'val', 'backend', 'opt_kind', 'transf_opt', 'transf_val'),
     (
         (Curve([]), 'line_dash', 'dashed', 'matplotlib', 'style', 'linestyle', 'dashed'),
         (Curve([]), 'line_alpha', 0.123, 'matplotlib', 'style', None, None),
         (Area([]), 'line_cap', 'square', 'matplotlib', 'style', 'capstyle', 'projecting'),
         (Curve([]), 'line_dash', 'dashed', 'plotly', 'style', 'dash', 'dash'),
-    )
+    ),
 )
 def test_transfer_opts(element, opt, val, backend, opt_kind, transf_opt, transf_val):
     current_backend = Store.current_backend
     if backend not in Store.registry:
         holoviews.extension(backend)
     Store.set_current_backend(backend)
     try:
@@ -46,20 +46,21 @@
             assert val not in new_opts.values()
         else:
             assert transf_opt in new_opts
             assert new_opts[transf_opt] == transf_val
     finally:
         Store.set_current_backend(current_backend)
 
+
 @pytest.mark.parametrize(
     ('opt', 'val', 'backend', 'opt_kind', 'transf_opt', 'transf_val'),
     (
         ('line_dash', 'dashed', 'matplotlib', 'style', 'linestyle', 'dashed'),
         ('line_dash', 'dashed', 'plotly', 'style', 'dash', 'dash'),
-    )
+    ),
 )
 def test_transfer_opts_compositeoverlay(opt, val, backend, opt_kind, transf_opt, transf_val):
     current_backend = Store.current_backend
     if backend not in Store.registry:
         holoviews.extension(backend)
     Store.set_current_backend(backend)
     try:
@@ -68,20 +69,21 @@
         transformed_element = new_element.Curve.I
         new_opts = transformed_element.opts.get(opt_kind).kwargs
         assert transf_opt in new_opts
         assert new_opts[transf_opt] == transf_val
     finally:
         Store.set_current_backend(current_backend)
 
+
 @pytest.mark.parametrize(
     ('bk_option', 'expected'),
     (
         ('height', False),
         ('hover_line_alpha', True),
         ('nonselection_line_alpha', True),
         ('muted_line_alpha', True),
         ('selection_line_alpha', True),
-        ('annular_muted_alpha', True)
-    )
+        ('annular_muted_alpha', True),
+    ),
 )
 def test_is_interactive_opt(bk_option, expected):
     assert _is_interactive_opt(bk_option) == expected
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testcharts.py` & `hvplot-0.9.3a1/hvplot/tests/testcharts.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 from holoviews.element import Curve, Area, Scatter, Points, Path, HeatMap
 from holoviews.element.comparison import ComparisonTestCase
 
 from ..util import is_dask
 
 
 class TestChart2D(ComparisonTestCase):
-
     def setUp(self):
         try:
             import pandas as pd
-        except:
+        except ImportError:
             raise SkipTest('Pandas not available')
-        import hvplot.pandas   # noqa
+        import hvplot.pandas  # noqa
+
         self.df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
-        self.cat_df = pd.DataFrame([[1, 2, 'A'], [3, 4, 'B'], [5, 6, 'C']],
-                                   columns=['x', 'y', 'category'])
-        self.time_df = pd.DataFrame({
-            'time': pd.date_range('1/1/2000', periods=5*24, freq='1h', tz='UTC'),
-            'temp': np.sin(np.linspace(0, 5*2*np.pi, 5*24)).cumsum()})
+        self.cat_df = pd.DataFrame(
+            [[1, 2, 'A'], [3, 4, 'B'], [5, 6, 'C']], columns=['x', 'y', 'category']
+        )
+        self.time_df = pd.DataFrame(
+            {
+                'time': pd.date_range('1/1/2000', periods=5 * 24, freq='1h', tz='UTC'),
+                'temp': np.sin(np.linspace(0, 5 * 2 * np.pi, 5 * 24)).cumsum(),
+            }
+        )
 
     @parameterized.expand([('points', Points), ('paths', Path)])
     def test_2d_defaults(self, kind, element):
         plot = self.df.hvplot(kind=kind)
         self.assertEqual(plot, element(self.df, ['x', 'y']))
 
     @parameterized.expand([('points', Points), ('paths', Path)])
@@ -54,109 +58,134 @@
         self.assertEqual(plot, element(self.cat_df.reset_index(), ['x', 'y'], ['index']))
 
     @parameterized.expand([('points', Points), ('paths', Path)])
     def test_2d_set_hover_cols_to_all(self, kind, element):
         plot = self.cat_df.hvplot(x='x', y='y', hover_cols='all', kind=kind)
         data = plot.data[0] if kind == 'paths' else plot.data
         assert 'index' in data.columns
-        self.assertEqual(plot, element(self.cat_df.reset_index(), ['x', 'y'], ['index', 'category']))
+        self.assertEqual(
+            plot, element(self.cat_df.reset_index(), ['x', 'y'], ['index', 'category'])
+        )
 
     @parameterized.expand([('points', Points), ('paths', Path)])
     def test_2d_set_hover_cols_to_all_with_use_index_as_false(self, kind, element):
         plot = self.cat_df.hvplot(x='x', y='y', hover_cols='all', use_index=False, kind=kind)
         self.assertEqual(plot, element(self.cat_df, ['x', 'y'], ['category']))
 
     def test_heatmap_2d_index_columns(self):
         plot = self.df.hvplot.heatmap()
-        self.assertEqual(plot, HeatMap((['x', 'y'], [0, 1, 2], self.df.values),
-                                       ['columns', 'index'], 'value'))
+        self.assertEqual(
+            plot, HeatMap((['x', 'y'], [0, 1, 2], self.df.values), ['columns', 'index'], 'value')
+        )
 
     def test_heatmap_2d_derived_x_and_y(self):
         plot = self.time_df.hvplot.heatmap(x='time.hour', y='time.day', C='temp')
         assert plot.kdims == ['time.hour', 'time.day']
         assert plot.vdims == ['temp']
 
-
     def test_xarray_dataset_with_attrs(self):
         try:
             import xarray as xr
             import hvplot.xarray  # noqa
         except ImportError:
             raise SkipTest('xarray not available')
 
-
         dset = xr.Dataset(
-            {"u": ("t", [1, 3]), "v": ("t", [4, 2])},
-            coords={"t": ("t", [0, 1], {"long_name": "time", "units": "s"})},
+            {'u': ('t', [1, 3]), 'v': ('t', [4, 2])},
+            coords={'t': ('t', [0, 1], {'long_name': 'time', 'units': 's'})},
         )
         ndoverlay = dset.hvplot.line()
 
-        assert render(ndoverlay, "bokeh").xaxis.axis_label == "time (s)"
+        assert render(ndoverlay, 'bokeh').xaxis.axis_label == 'time (s)'
 
 
 class TestChart2DDask(TestChart2D):
-
     def setUp(self):
         super().setUp()
         try:
             import dask.dataframe as dd
-        except:
+        except ImportError:
             raise SkipTest('Dask not available')
-        import hvplot.dask   # noqa
+        import hvplot.dask  # noqa
+
         self.df = dd.from_pandas(self.df, npartitions=2)
         self.cat_df = dd.from_pandas(self.cat_df, npartitions=3)
 
     @expectedFailure
     def test_heatmap_2d_index_columns(self):
         self.df.hvplot.heatmap()
 
 
 class TestChart1D(ComparisonTestCase):
-
     def setUp(self):
         try:
             import pandas as pd
-        except:
+        except ImportError:
             raise SkipTest('Pandas not available')
-        import hvplot.pandas   # noqa
+        import hvplot.pandas  # noqa
+
         self.df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
         self.df_desc = self.df.describe().transpose().sort_values('mean')
-        self.dt_df = pd.DataFrame(np.random.rand(90), index=pd.date_range('2019-01-01', '2019-03-31'))
-        self.cat_df = pd.DataFrame([[1, 2, 'A'], [3, 4, 'B'], [5, 6, 'C']],
-                                   columns=['x', 'y', 'category'])
-        self.cat_only_df = pd.DataFrame([['A', 'a'], ['B', 'b'], ['C', 'c']],
-                                        columns=['upper', 'lower'])
-        self.time_df = pd.DataFrame({
-            'time': pd.date_range('1/1/2000', periods=10, tz='UTC'),
-            'A': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-            'B': list('abcdefghij')})
-        self.edge_df = pd.DataFrame({
-            "Latitude": [-34.58, -15.78, -33.45],
-            "Longitude": [-58.66, -47.91, -70.66],
-            "Volume {m3}": ["1", "2", "3"],
-        })
+        self.dt_df = pd.DataFrame(
+            np.random.rand(90), index=pd.date_range('2019-01-01', '2019-03-31')
+        )
+        self.cat_df = pd.DataFrame(
+            [[1, 2, 'A'], [3, 4, 'B'], [5, 6, 'C']], columns=['x', 'y', 'category']
+        )
+        self.cat_only_df = pd.DataFrame(
+            [['A', 'a'], ['B', 'b'], ['C', 'c']], columns=['upper', 'lower']
+        )
+        self.time_df = pd.DataFrame(
+            {
+                'time': pd.date_range('1/1/2000', periods=10, tz='UTC'),
+                'A': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+                'B': list('abcdefghij'),
+            }
+        )
+        self.edge_df = pd.DataFrame(
+            {
+                'Latitude': [-34.58, -15.78, -33.45],
+                'Longitude': [-58.66, -47.91, -70.66],
+                'Volume {m3}': ['1', '2', '3'],
+            }
+        )
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_wide_chart(self, kind, element):
         plot = self.df.hvplot(kind=kind)
-        obj = NdOverlay({'x': element(self.df, 'index', 'x').redim(x='value'),
-                         'y': element(self.df, 'index', 'y').redim(y='value')}, 'Variable')
+        obj = NdOverlay(
+            {
+                'x': element(self.df, 'index', 'x').redim(x='value'),
+                'y': element(self.df, 'index', 'y').redim(y='value'),
+            },
+            'Variable',
+        )
         self.assertEqual(plot, obj)
 
     def test_by_datetime_accessor(self):
         plot = self.dt_df.hvplot.line('index.dt.day', '0', by='index.dt.month')
-        obj = NdOverlay({m: Curve((g.index.day, g[0]), 'index.dt.day', '0')
-                         for m, g in self.dt_df.groupby(self.dt_df.index.month)}, 'index.dt.month')
+        obj = NdOverlay(
+            {
+                m: Curve((g.index.day, g[0]), 'index.dt.day', '0')
+                for m, g in self.dt_df.groupby(self.dt_df.index.month)
+            },
+            'index.dt.month',
+        )
         self.assertEqual(plot, obj)
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_wide_chart_labels(self, kind, element):
         plot = self.df.hvplot(kind=kind, value_label='Test', group_label='Category')
-        obj = NdOverlay({'x': element(self.df, 'index', 'x').redim(x='Test'),
-                         'y': element(self.df, 'index', 'y').redim(y='Test')}, 'Category')
+        obj = NdOverlay(
+            {
+                'x': element(self.df, 'index', 'x').redim(x='Test'),
+                'y': element(self.df, 'index', 'y').redim(y='Test'),
+            },
+            'Category',
+        )
         self.assertEqual(plot, obj)
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_wide_chart_legend_position(self, kind, element):
         plot = self.df.hvplot(kind=kind, value_label='Test', group_label='Category', legend='left')
         opts = Store.lookup_options('bokeh', plot, 'plot')
         self.assertEqual(opts.kwargs['legend_position'], 'left')
@@ -175,17 +204,22 @@
     def test_tidy_chart_index(self, kind, element):
         plot = self.df.hvplot(x='index', y='y', kind=kind)
         self.assertEqual(plot, element(self.df, 'index', 'y'))
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_tidy_chart_index_by(self, kind, element):
         plot = self.df.hvplot(x='index', y='y', by='x', kind=kind)
-        obj = NdOverlay({1: element(self.df[self.df.x==1], 'index', 'y'),
-                         3: element(self.df[self.df.x==3], 'index', 'y'),
-                         5: element(self.df[self.df.x==5], 'index', 'y')}, 'x')
+        obj = NdOverlay(
+            {
+                1: element(self.df[self.df.x == 1], 'index', 'y'),
+                3: element(self.df[self.df.x == 3], 'index', 'y'),
+                5: element(self.df[self.df.x == 5], 'index', 'y'),
+            },
+            'x',
+        )
         self.assertEqual(plot, obj)
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_tidy_chart_index_by_legend_position(self, kind, element):
         plot = self.df.hvplot(x='index', y='y', by='x', kind=kind, legend='left')
         opts = Store.lookup_options('bokeh', plot, 'plot')
         self.assertEqual(opts.kwargs['legend_position'], 'left')
@@ -230,16 +264,21 @@
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_tidy_chart_with_hover_cols_as_all_with_use_index_as_false(self, kind, element):
         plot = self.cat_df.hvplot(x='x', y='y', kind=kind, hover_cols='all', use_index=False)
         self.assertEqual(plot, element(self.cat_df, 'x', ['y', 'category']))
 
     def test_area_stacked(self):
         plot = self.df.hvplot.area(stacked=True)
-        obj = NdOverlay({'x': Area(self.df, 'index', 'x').redim(x='value'),
-                         'y': Area(self.df, 'index', 'y').redim(y='value')}, 'Variable')
+        obj = NdOverlay(
+            {
+                'x': Area(self.df, 'index', 'x').redim(x='value'),
+                'y': Area(self.df, 'index', 'y').redim(y='value'),
+            },
+            'Variable',
+        )
         self.assertEqual(plot, Area.stack(obj))
 
     def test_scatter_color_set_to_series(self):
         if is_dask(self.df['y']):
             y = self.df['y'].compute()
         else:
             y = self.df['y']
@@ -264,35 +303,47 @@
         self.assertEqual(opts.kwargs['legend_position'], 'left')
 
     def test_histogram_by_category_legend_position(self):
         plot = self.cat_df.hvplot.hist('y', by='category', legend='left')
         opts = Store.lookup_options('bokeh', plot, 'plot')
         self.assertEqual(opts.kwargs['legend_position'], 'left')
 
+    def test_histogram_wide_set_group_label(self):
+        plot = self.df.hvplot.hist(group_label='Test')
+        assert plot.kdims[0].name == 'Test'
+
     def test_scatter_color_internally_set_to_dim(self):
         altered_df = self.cat_df.copy().rename(columns={'category': 'red'})
         plot = altered_df.hvplot.scatter('x', 'y', c='red')
         opts = Store.lookup_options('bokeh', plot, 'style')
         self.assertIsInstance(opts.kwargs['color'], dim)
         self.assertEqual(opts.kwargs['color'].dimension.name, 'red')
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_only_includes_num_chart(self, kind, element):
         plot = self.cat_df.hvplot(kind=kind)
-        obj = NdOverlay({'x': element(self.cat_df, 'index', 'x').redim(x='value'),
-                         'y': element(self.cat_df, 'index', 'y').redim(y='value'),
-                        }, 'Variable')
+        obj = NdOverlay(
+            {
+                'x': element(self.cat_df, 'index', 'x').redim(x='value'),
+                'y': element(self.cat_df, 'index', 'y').redim(y='value'),
+            },
+            'Variable',
+        )
         self.assertEqual(plot, obj)
 
     @parameterized.expand([('line', Curve), ('area', Area), ('scatter', Scatter)])
     def test_includes_str_if_no_num_chart(self, kind, element):
         plot = self.cat_only_df.hvplot(kind=kind)
-        obj = NdOverlay({'upper': element(self.cat_only_df, 'index', 'upper').redim(upper='value'),
-                         'lower': element(self.cat_only_df, 'index', 'lower').redim(lower='value'),
-                        }, 'Variable')
+        obj = NdOverlay(
+            {
+                'upper': element(self.cat_only_df, 'index', 'upper').redim(upper='value'),
+                'lower': element(self.cat_only_df, 'index', 'lower').redim(lower='value'),
+            },
+            'Variable',
+        )
         self.assertEqual(plot, obj)
 
     def test_time_df_sorts_on_plot(self):
         scrambled = self.time_df.sample(frac=1)
         plot = scrambled.hvplot(x='time')
         assert (plot.data == self.time_df).all().all()
         assert len(plot.data.time.unique()) == len(plot.data.time)
@@ -303,23 +354,27 @@
         assert (plot.data == scrambled).all().all()
         assert len(plot.data.time.unique()) == len(plot.data.time)
 
     def test_time_df_sorts_on_plot_using_index_as_x(self):
         df = self.time_df.set_index('time')
         scrambled = df.sample(frac=1)
         plot = scrambled.hvplot()
-        assert (plot.data['time'] == df.index).all()
-        assert len(plot.data.time.unique()) == len(plot.data.time)
+        # HoloViews 1.18 uses reset_index and 1.19 does not.
+        time = plot.data.time if 'time' in plot.data.columns else plot.data.index
+        assert (time == df.index).all()
+        assert len(time.unique()) == len(time)
 
     def test_time_df_does_not_sort_on_plot_if_sort_date_off_using_index_as_x(self):
         df = self.time_df.set_index('time')
         scrambled = df.sample(frac=1)
         plot = scrambled.hvplot(sort_date=False)
-        assert (plot.data.time == scrambled.index).all().all()
-        assert len(plot.data.time.unique()) == len(plot.data.time)
+        # HoloViews 1.18 uses reset_index and 1.19 does not.
+        time = plot.data.time if 'time' in plot.data.columns else plot.data.index
+        assert (time == scrambled.index).all().all()
+        assert len(time.unique()) == len(time)
 
     def test_time_df_with_groupby_as_derived_datetime(self):
         plot = self.time_df.hvplot(groupby='time.dayofweek', dynamic=False)
         assert list(plot.keys()) == [0, 1, 2, 3, 4, 5, 6]
         assert list(plot.dimensions()) == ['time.dayofweek', 'index', 'A']
 
     def test_time_df_with_by_as_derived_datetime(self):
@@ -350,37 +405,48 @@
     def test_errorbars_no_hover(self):
         plot = self.df_desc.hvplot.errorbars(y='mean', yerr1='std')
         assert list(plot.dimensions()) == ['index', 'mean', 'std']
         bkplot = Store.renderers['bokeh'].get_plot(plot)
         assert not bkplot.tools
 
     def test_labels_format(self):
-        plot = self.df.hvplot("x", "y", text="({x}, {y})", kind="labels")
+        plot = self.df.hvplot('x', 'y', text='({x}, {y})', kind='labels')
         assert list(plot.dimensions()) == [Dimension('x'), Dimension('y'), Dimension('label')]
-        assert list(plot.data["label"]) == ['(1, 2)', '(3, 4)', '(5, 6)']
+        assert list(plot.data['label']) == ['(1, 2)', '(3, 4)', '(5, 6)']
 
     def test_labels_no_format_edge_case(self):
-        plot = self.edge_df.hvplot.labels("Longitude", "Latitude")
-        assert list(plot.dimensions()) == [Dimension('Longitude'), Dimension('Latitude'), Dimension('Volume {m3}')]
-        assert list(plot.data["Volume {m3}"]) == ['1', '2', '3']
+        plot = self.edge_df.hvplot.labels('Longitude', 'Latitude')
+        assert list(plot.dimensions()) == [
+            Dimension('Longitude'),
+            Dimension('Latitude'),
+            Dimension('Volume {m3}'),
+        ]
+        assert list(plot.data['Volume {m3}']) == ['1', '2', '3']
 
     def test_labels_format_float(self):
-        plot = self.edge_df.hvplot.labels("Longitude", "Latitude", text="{Longitude:.1f}E {Latitude:.2f}N")
-        assert list(plot.dimensions()) == [Dimension('Longitude'), Dimension('Latitude'), Dimension('label')]
-        assert list(plot.data["label"]) == ['-58.7E -34.58N', '-47.9E -15.78N', '-70.7E -33.45N']
+        plot = self.edge_df.hvplot.labels(
+            'Longitude', 'Latitude', text='{Longitude:.1f}E {Latitude:.2f}N'
+        )
+        assert list(plot.dimensions()) == [
+            Dimension('Longitude'),
+            Dimension('Latitude'),
+            Dimension('label'),
+        ]
+        assert list(plot.data['label']) == ['-58.7E -34.58N', '-47.9E -15.78N', '-70.7E -33.45N']
 
-class TestChart1DDask(TestChart1D):
 
+class TestChart1DDask(TestChart1D):
     def setUp(self):
         super().setUp()
         try:
             import dask.dataframe as dd
-        except:
+        except ImportError:
             raise SkipTest('Dask not available')
-        import hvplot.dask   # noqa
+        import hvplot.dask  # noqa
+
         self.df = dd.from_pandas(self.df, npartitions=2)
         self.dt_df = dd.from_pandas(self.dt_df, npartitions=3)
         self.cat_df = dd.from_pandas(self.cat_df, npartitions=3)
         self.cat_only_df = dd.from_pandas(self.cat_only_df, npartitions=1)
 
     def test_by_datetime_accessor(self):
         raise SkipTest("Can't expand dt accessor columns when using dask")
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testgeo.py` & `hvplot-0.9.3a1/hvplot/tests/testgeo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 These tests depends on GeoViews.
 """
+
 import pathlib
 import sys
 
 from unittest import TestCase, SkipTest
 
 import holoviews as hv
 import numpy as np
@@ -14,83 +15,94 @@
 from hvplot.util import proj_to_cartopy
 from packaging.version import Version
 
 pytestmark = pytest.mark.geo
 
 bk_renderer = hv.Store.renderers['bokeh']
 
+
 @pytest.fixture
 def simple_df():
     return pd.DataFrame(np.random.rand(10, 2), columns=['x', 'y'])
 
 
 class TestGeo(TestCase):
-
     def setUp(self):
-        if sys.platform == "win32":
-            raise SkipTest("Skip geo tests on windows for now")
+        if sys.platform == 'win32':
+            raise SkipTest('Skip geo tests on windows for now')
         try:
             import xarray as xr  # noqa
             import rasterio  # noqa
             import geoviews  # noqa
             import cartopy.crs as ccrs  # noqa
+            import pyproj  # noqa
             import rioxarray as rxr
-        except:
-            raise SkipTest('xarray, rasterio, geoviews, cartopy, or rioxarray not available')
+        except ImportError:
+            raise SkipTest(
+                'xarray, rasterio, geoviews, cartopy, pyproj or rioxarray not available'
+            )
         import hvplot.xarray  # noqa
         import hvplot.pandas  # noqa
+
         self.da = rxr.open_rasterio(
-           pathlib.Path(__file__).parent / 'data' / 'RGB-red.byte.tif'
+            pathlib.Path(__file__).parent / 'data' / 'RGB-red.byte.tif'
         ).isel(band=0)
         self.crs = proj_to_cartopy(self.da.spatial_ref.attrs['crs_wkt'])
 
     def assertCRS(self, plot, proj='utm'):
         import cartopy
+
         if Version(cartopy.__version__) < Version('0.20'):
             assert plot.crs.proj4_params['proj'] == proj
         else:
             assert plot.crs.to_dict()['proj'] == proj
 
     def assert_projection(self, plot, proj):
         opts = hv.Store.lookup_options('bokeh', plot, 'plot')
         assert opts.kwargs['projection'].proj4_params['proj'] == proj
 
 
 class TestCRSInference(TestGeo):
-
     def setUp(self):
-        if sys.platform == "win32":
-            raise SkipTest("Skip CRS inference on Windows")
+        if sys.platform == 'win32':
+            raise SkipTest('Skip CRS inference on Windows')
         super().setUp()
 
     def test_plot_with_crs_as_proj_string(self):
         da = self.da.copy()
         da.rio._crs = False  # To not treat it as a rioxarray
 
-        plot = self.da.hvplot.image('x', 'y', crs="epsg:32618")
+        plot = self.da.hvplot.image('x', 'y', crs='epsg:32618')
         self.assertCRS(plot)
 
     def test_plot_with_geo_as_true_crs_undefined(self):
         plot = self.da.hvplot.image('x', 'y', geo=True)
         self.assertCRS(plot)
 
 
 class TestProjections(TestGeo):
-
     def test_plot_with_crs_as_object(self):
         plot = self.da.hvplot.image('x', 'y', crs=self.crs)
         self.assertCRS(plot)
 
     def test_plot_with_crs_as_attr_str(self):
         da = self.da.copy()
         da.rio._crs = False  # To not treat it as a rioxarray
         da.attrs = {'bar': self.crs}
         plot = da.hvplot.image('x', 'y', crs='bar')
         self.assertCRS(plot)
 
+    def test_plot_with_crs_as_pyproj_Proj(self):
+        import pyproj
+
+        da = self.da.copy()
+        da.rio._crs = False  # To not treat it as a rioxarray
+        plot = da.hvplot.image('x', 'y', crs=pyproj.Proj(self.crs))
+        self.assertCRS(plot)
+
     def test_plot_with_crs_as_nonexistent_attr_str(self):
         da = self.da.copy()
         da.rio._crs = False  # To not treat it as a rioxarray
 
         # Used to test crs='foo' but this is parsed under-the-hood
         # by PROJ (projinfo) which matches a geographic projection named
         # 'Amersfoort'
@@ -111,127 +123,150 @@
 
     def test_plot_with_projection_as_string_google_mercator(self):
         da = self.da.copy()
         plot = da.hvplot.image('x', 'y', crs=self.crs, projection='GOOGLE_MERCATOR')
         self.assert_projection(plot, 'merc')
 
     def test_plot_with_projection_as_invalid_string(self):
-        with self.assertRaisesRegex(ValueError, "Projection must be defined"):
+        with self.assertRaisesRegex(ValueError, 'Projection must be defined'):
             self.da.hvplot.image('x', 'y', projection='foo')
 
     def test_plot_with_projection_raises_an_error_when_tiles_set(self):
         da = self.da.copy()
-        with self.assertRaisesRegex(ValueError, "Tiles can only be used with output projection"):
+        with self.assertRaisesRegex(ValueError, 'Tiles can only be used with output projection'):
             da.hvplot.image('x', 'y', crs=self.crs, projection='Robinson', tiles=True)
 
     def test_overlay_with_projection(self):
         # Regression test for https://github.com/holoviz/hvplot/issues/1090
-        df = pd.DataFrame({"lon": [0, 10], "lat": [40, 50], "v": [0, 1]})
+        df = pd.DataFrame({'lon': [0, 10], 'lat': [40, 50], 'v': [0, 1]})
 
-        plot1 = df.hvplot.points(x="lon", y="lat", s=200, c="y", geo=True, tiles="CartoLight")
-        plot2 = df.hvplot.points(x="lon", y="lat", c="v", geo=True)
+        plot1 = df.hvplot.points(x='lon', y='lat', s=200, c='y', geo=True, tiles='CartoLight')
+        plot2 = df.hvplot.points(x='lon', y='lat', c='v', geo=True)
 
         # This should work without erroring
         plot = plot1 * plot2
-        hv.renderer("bokeh").get_plot(plot)
+        hv.renderer('bokeh').get_plot(plot)
 
     def test_geo_with_rasterize(self):
         import xarray as xr
         import cartopy.crs as ccrs
         import geoviews as gv
+
         try:
             from holoviews.operation.datashader import rasterize
-        except:
+        except ImportError:
             raise SkipTest('datashader not available')
 
-        ds = xr.tutorial.open_dataset("air_temperature")
+        ds = xr.tutorial.open_dataset('air_temperature')
         hvplot_output = ds.isel(time=0).hvplot.points(
-            "lon",
-            "lat",
+            'lon',
+            'lat',
             crs=ccrs.PlateCarree(),
             projection=ccrs.LambertConformal(),
             rasterize=True,
             dynamic=False,
-            aggregator="max",
+            aggregator='max',
             project=True,
         )
 
-        p1 = gv.Points(ds.isel(time=0), kdims=["lon", "lat"], crs=ccrs.PlateCarree())
+        p1 = gv.Points(ds.isel(time=0), kdims=['lon', 'lat'], crs=ccrs.PlateCarree())
         p2 = gv.project(p1, projection=ccrs.LambertConformal())
-        expected = rasterize(p2, dynamic=False, aggregator="max")
+        expected = rasterize(p2, dynamic=False, aggregator='max')
 
         xr.testing.assert_allclose(hvplot_output.data, expected.data)
 
 
 class TestGeoAnnotation(TestCase):
-
     def setUp(self):
         try:
             import geoviews  # noqa
-            import cartopy.crs as ccrs # noqa
-        except:
+            import cartopy.crs as ccrs  # noqa
+        except ImportError:
             raise SkipTest('geoviews or cartopy not available')
         import hvplot.pandas  # noqa
+
         self.crs = ccrs.PlateCarree()
         self.df = pd.DataFrame(np.random.rand(10, 2), columns=['x', 'y'])
 
     def test_plot_with_coastline(self):
         import geoviews as gv
+
         plot = self.df.hvplot.points('x', 'y', geo=True, coastline=True)
         self.assertEqual(len(plot), 2)
         coastline = plot.get(1)
         self.assertIsInstance(coastline, gv.Feature)
 
     def test_plot_with_coastline_sets_geo_by_default(self):
         import geoviews as gv
+
         plot = self.df.hvplot.points('x', 'y', coastline=True)
         self.assertEqual(len(plot), 2)
         coastline = plot.get(1)
         self.assertIsInstance(coastline, gv.Feature)
 
     def test_plot_with_coastline_scale(self):
         plot = self.df.hvplot.points('x', 'y', geo=True, coastline='10m')
         opts = plot.get(1).opts.get('plot')
-        assert opts.kwargs["scale"] == '10m'
+        assert opts.kwargs['scale'] == '10m'
 
     def test_plot_with_tiles(self):
         plot = self.df.hvplot.points('x', 'y', geo=False, tiles=True)
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), hv.Tiles)
         self.assertIn('openstreetmap', plot.get(0).data)
 
+    def test_plot_with_tiles_with_tiles_opts(self):
+        plot = self.df.hvplot.points('x', 'y', geo=False, tiles=True, tiles_opts=dict(alpha=0.5))
+        assert len(plot) == 2
+        tiles = plot.get(0)
+        assert isinstance(tiles, hv.Tiles)
+        assert 'openstreetmap' in tiles.data
+        assert tiles.opts['alpha'] == 0.5
+
     def test_plot_with_tiles_with_geo(self):
         import geoviews as gv
 
         plot = self.df.hvplot.points('x', 'y', geo=True, tiles=True)
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), gv.element.WMTS)
         self.assertIn('openstreetmap', plot.get(0).data)
 
+    def test_plot_with_tiles_with_tiles_opts_with_geo(self):
+        import geoviews as gv
+
+        plot = self.df.hvplot.points('x', 'y', geo=True, tiles=True, tiles_opts=dict(alpha=0.5))
+        assert len(plot) == 2
+        tiles = plot.get(0)
+        assert isinstance(tiles, gv.element.WMTS)
+        assert 'openstreetmap' in tiles.data
+        assert tiles.opts['alpha'] == 0.5
+
     def test_plot_with_specific_tiles(self):
         plot = self.df.hvplot.points('x', 'y', geo=False, tiles='ESRI')
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), hv.Tiles)
         self.assertIn('ArcGIS', plot.get(0).data)
 
     def test_plot_with_specific_tiles_geo(self):
         import geoviews as gv
+
         plot = self.df.hvplot.points('x', 'y', geo=True, tiles='ESRI')
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), gv.element.WMTS)
         self.assertIn('ArcGIS', plot.get(0).data)
 
     def test_plot_with_specific_tile_class(self):
         plot = self.df.hvplot.points('x', 'y', geo=False, tiles=hv.element.tiles.EsriImagery)
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), hv.Tiles)
         self.assertIn('ArcGIS', plot.get(0).data)
 
     def test_plot_with_specific_tile_class_with_geo(self):
         import geoviews as gv
+
         plot = self.df.hvplot.points('x', 'y', geo=True, tiles=gv.tile_sources.EsriImagery)
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), gv.element.WMTS)
         self.assertIn('ArcGIS', plot.get(0).data)
 
     def test_plot_with_specific_tile_obj(self):
         plot = self.df.hvplot.points('x', 'y', geo=False, tiles=hv.element.tiles.EsriImagery())
@@ -243,34 +278,46 @@
         plot = self.df.hvplot.points('x', 'y', geo=True, tiles=hv.element.tiles.EsriImagery())
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), hv.Tiles)
         self.assertIn('ArcGIS', plot.get(0).data)
 
     def test_plot_with_specific_gv_tile_obj(self):
         import geoviews as gv
+
         plot = self.df.hvplot.points('x', 'y', geo=True, tiles=gv.tile_sources.CartoDark)
         self.assertEqual(len(plot), 2)
         self.assertIsInstance(plot.get(0), gv.element.WMTS)
 
+    def test_plot_with_xyzservices_tiles(self):
+        xyzservices = pytest.importorskip('xyzservices')
+        import geoviews as gv
+
+        plot = self.df.hvplot.points(
+            'x', 'y', geo=True, tiles=xyzservices.providers.Esri.WorldImagery
+        )
+        assert len(plot) == 2
+        assert isinstance(plot.get(0), gv.element.WMTS)
+        assert isinstance(plot.get(0).data, xyzservices.TileProvider)
+
     def test_plot_with_features_properly_overlaid_underlaid(self):
         # land should be under, borders should be over
-        plot = self.df.hvplot.points('x', 'y', features=["land", "borders"])
-        assert plot.get(0).group == "Land"
-        assert plot.get(2).group == "Borders"
+        plot = self.df.hvplot.points('x', 'y', features=['land', 'borders'])
+        assert plot.get(0).group == 'Land'
+        assert plot.get(2).group == 'Borders'
 
 
 class TestGeoElements(TestCase):
-
     def setUp(self):
         try:
             import geoviews  # noqa
-            import cartopy.crs as ccrs # noqa
-        except:
+            import cartopy.crs as ccrs  # noqa
+        except ImportError:
             raise SkipTest('geoviews or cartopy not available')
         import hvplot.pandas  # noqa
+
         self.crs = ccrs.PlateCarree()
         self.df = pd.DataFrame(np.random.rand(10, 2), columns=['x', 'y'])
 
     def test_geo_hexbin(self):
         hextiles = self.df.hvplot.hexbin('x', 'y', geo=True)
         self.assertEqual(hextiles.crs, self.crs)
 
@@ -296,32 +343,30 @@
         opts = hv.Store.lookup_options('bokeh', points, 'plot').kwargs
         self.assertEqual(opts.get('data_aspect'), 1)
         self.assertEqual(opts.get('width'), 200)
         self.assertEqual(opts.get('height'), None)
 
 
 class TestGeoPandas(TestCase):
-
     def setUp(self):
         try:
             import geopandas as gpd  # noqa
             import geoviews  # noqa
-            import cartopy.crs as ccrs # noqa
+            import cartopy.crs as ccrs  # noqa
             import shapely  # noqa
-        except:
+        except ImportError:
             raise SkipTest('geopandas, geoviews, shapely or cartopy not available')
         import hvplot.pandas  # noqa
 
-
         from shapely.geometry import Polygon
 
         p_geometry = gpd.points_from_xy(
             x=[12.45339, 12.44177, 9.51667, 6.13000, 158.14997],
             y=[41.90328, 43.93610, 47.13372, 49.61166, 6.91664],
-            crs='EPSG:4326'
+            crs='EPSG:4326',
         )
         p_names = ['Vatican City', 'San Marino', 'Vaduz', 'Luxembourg', 'Palikir']
         self.cities = gpd.GeoDataFrame(dict(name=p_names), geometry=p_geometry)
 
         pg_geometry = [
             Polygon(((0, 0), (0, 1), (1, 1), (1, 0), (0, 0))),
             Polygon(((2, 2), (2, 3), (3, 3), (3, 2), (2, 2))),
@@ -381,40 +426,43 @@
     def test_points_project_xlim_and_ylim_with_geo(self):
         points = self.cities.hvplot(geo=True, xlim=(-10, 10), ylim=(-20, -10))
         opts = hv.Store.lookup_options('bokeh', points, 'plot').options
         np.testing.assert_allclose(opts['xlim'], (-10, 10))
         np.testing.assert_allclose(opts['ylim'], (-20, -10))
 
     def test_polygons_by_subplots(self):
-        polygons = self.polygons.hvplot(geo=True, by="name", subplots=True)
+        polygons = self.polygons.hvplot(geo=True, by='name', subplots=True)
         assert isinstance(polygons, hv.core.layout.NdLayout)
 
     def test_polygons_turns_off_hover_when_there_are_no_fields_to_include(self):
         polygons = self.polygons.hvplot(geo=True)
         opts = hv.Store.lookup_options('bokeh', polygons, 'plot').kwargs
         assert 'hover' not in opts.get('tools')
 
 
 class TestGeoUtil(TestCase):
-
     def setUp(self):
-        if sys.platform == "win32":
-            raise SkipTest("Skip geo tests on windows for now")
+        if sys.platform == 'win32':
+            raise SkipTest('Skip geo tests on windows for now')
         try:
             import cartopy.crs as ccrs
-        except:
+        except ImportError:
             raise SkipTest('cartopy not available')
         self.ccrs = ccrs
 
     def test_proj_to_cartopy(self):
         from ..util import proj_to_cartopy
+
         crs = proj_to_cartopy('+init=epsg:26911')
 
         assert isinstance(crs, self.ccrs.CRS)
 
     def test_proj_to_cartopy_wkt_string(self):
         from ..util import proj_to_cartopy
-        crs = proj_to_cartopy('GEOGCRS["unnamed",BASEGEOGCRS["unknown",DATUM["unknown",ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1,ID["EPSG",9001]]]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8901]]],DERIVINGCONVERSION["unknown",METHOD["PROJ ob_tran o_proj=latlon"],PARAMETER["o_lon_p",0,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],PARAMETER["o_lat_p",37.5,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],PARAMETER["lon_0",357.5,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]]],CS[ellipsoidal,2],AXIS["longitude",east,ORDER[1],ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],AXIS["latitude",north,ORDER[2],ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]]]')  # noqa: E501
+
+        crs = proj_to_cartopy(
+            'GEOGCRS["unnamed",BASEGEOGCRS["unknown",DATUM["unknown",ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1,ID["EPSG",9001]]]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8901]]],DERIVINGCONVERSION["unknown",METHOD["PROJ ob_tran o_proj=latlon"],PARAMETER["o_lon_p",0,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],PARAMETER["o_lat_p",37.5,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],PARAMETER["lon_0",357.5,ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]]],CS[ellipsoidal,2],AXIS["longitude",east,ORDER[1],ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]],AXIS["latitude",north,ORDER[2],ANGLEUNIT["degree",0.0174532925199433,ID["EPSG",9122]]]]'
+        )  # noqa: E501
 
         assert isinstance(crs, self.ccrs.RotatedPole)
-        assert crs.proj4_params["lon_0"] == 357.5
-        assert crs.proj4_params["o_lat_p"] == 37.5
+        assert crs.proj4_params['lon_0'] == 357.5
+        assert crs.proj4_params['o_lat_p'] == 37.5
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testgeowithoutgv.py` & `hvplot-0.9.3a1/hvplot/tests/testgeowithoutgv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Geo tests **without** importing GeoViews.
 """
+
 import holoviews as hv
 import hvplot.pandas  # noqa
 import numpy as np
 import pandas as pd
 import pytest
 
 
 bk_renderer = hv.Store.renderers['bokeh']
 
+
 @pytest.fixture
 def simple_df():
     return pd.DataFrame(np.random.rand(10, 2), columns=['x', 'y'])
 
 
 class TestAnnotationNotGeo:
-
     def test_plot_tiles_doesnt_set_geo(self, simple_df):
         plot = simple_df.hvplot.points('x', 'y', tiles=True)
         assert len(plot) == 2
         assert isinstance(plot.get(0), hv.Tiles)
         assert 'openstreetmap' in plot.get(0).data
         bk_plot = bk_renderer.get_plot(plot)
         assert bk_plot.projection == 'mercator'
@@ -44,7 +45,16 @@
     def test_plot_with_specific_tile_obj(self, simple_df):
         plot = simple_df.hvplot.points('x', 'y', tiles=hv.element.tiles.EsriImagery())
         assert len(plot) == 2
         assert isinstance(plot.get(0), hv.Tiles)
         assert 'ArcGIS' in plot.get(0).data
         bk_plot = bk_renderer.get_plot(plot)
         assert bk_plot.projection == 'mercator'
+
+    def test_plot_with_xyzservices_tileprovider(self, simple_df):
+        xyzservices = pytest.importorskip('xyzservices')
+        plot = simple_df.hvplot.points('x', 'y', tiles=xyzservices.providers.Esri.WorldImagery)
+        assert len(plot) == 2
+        assert isinstance(plot.get(0), hv.Tiles)
+        assert isinstance(plot.get(0).data, xyzservices.TileProvider)
+        bk_plot = bk_renderer.get_plot(plot)
+        assert bk_plot.projection == 'mercator'
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testgridplots.py` & `hvplot-0.9.3a1/hvplot/tests/testgridplots.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,96 +7,110 @@
 import numpy as np
 from holoviews import Store
 from holoviews.element import RGB, Image
 from holoviews.element.comparison import ComparisonTestCase
 
 try:
     import xarray as xr
-except:
+except ImportError:
     raise SkipTest('XArray not available')
 else:
-    import hvplot.xarray   # noqa
+    import hvplot.xarray  # noqa
 
-class TestGridPlots(ComparisonTestCase):
 
+class TestGridPlots(ComparisonTestCase):
     def setUp(self):
         coords = OrderedDict([('band', [1, 2, 3]), ('y', [0, 1]), ('x', [0, 1])])
-        self.da_rgb = xr.DataArray(np.arange(12).reshape((3, 2, 2)),
-                                   coords, ['band', 'y', 'x'])
+        self.da_rgb = xr.DataArray(np.arange(12).reshape((3, 2, 2)), coords, ['band', 'y', 'x'])
         coords = OrderedDict([('time', [0, 1]), ('band', [1, 2, 3]), ('y', [0, 1]), ('x', [0, 1])])
-        self.da_rgb_by_time = xr.DataArray(np.arange(24).reshape((2, 3, 2, 2)),
-                                           coords, ['time', 'band', 'y', 'x'])
+        self.da_rgb_by_time = xr.DataArray(
+            np.arange(24).reshape((2, 3, 2, 2)), coords, ['time', 'band', 'y', 'x']
+        )
 
         coords = OrderedDict([('time', [0, 1]), ('lat', [0, 1]), ('lon', [0, 1])])
-        self.da_img_by_time = xr.DataArray(np.arange(8).reshape((2, 2, 2)),
-                                           coords, ['time', 'lat', 'lon']).assign_coords(
-                                               lat1=xr.DataArray([2,3], dims=['lat']))
+        self.da_img_by_time = xr.DataArray(
+            np.arange(8).reshape((2, 2, 2)), coords, ['time', 'lat', 'lon']
+        ).assign_coords(lat1=xr.DataArray([2, 3], dims=['lat']))
 
         self.xarr_with_attrs = xr.DataArray(
-            np.random.rand(10, 10), coords=[('x', range(10)), ('y', range(10))],
-            dims=['y', 'x'], attrs={'long_name': 'luminosity', 'units': 'lm'})
+            np.random.rand(10, 10),
+            coords=[('x', range(10)), ('y', range(10))],
+            dims=['y', 'x'],
+            attrs={'long_name': 'luminosity', 'units': 'lm'},
+        )
         self.xarr_with_attrs.x.attrs['long_name'] = 'Declination'
         self.xarr_with_attrs.y.attrs['long_name'] = 'Right Ascension'
 
-        self.xds_with_attrs = xr.Dataset({'light': self.xarr_with_attrs })
+        self.xds_with_attrs = xr.Dataset({'light': self.xarr_with_attrs})
         self.da_img = xr.DataArray(np.arange(-2, 2).reshape((2, 2)), name='foo')
         self.big_img = xr.DataArray(np.arange(-1e6, 1e6).reshape(1000, 2000))
 
-        self.ds = xr.Dataset({
-            'temp': (('lon', 'lat'), 15 + 8 * np.random.randn(2, 2)),
-            'precip': (('lon', 'lat'), 10 * np.random.rand(2, 2))},
-            coords={'lon': [-99.83, -99.32],'lat': [42.25, 42.21]})
+        self.ds = xr.Dataset(
+            {
+                'temp': (('lon', 'lat'), 15 + 8 * np.random.randn(2, 2)),
+                'precip': (('lon', 'lat'), 10 * np.random.rand(2, 2)),
+            },
+            coords={'lon': [-99.83, -99.32], 'lat': [42.25, 42.21]},
+        )
 
         xs = np.linspace(0, 10, 5)
-        lon = xs*xs[np.newaxis, :].T
-        lat = xs+xs[:, np.newaxis]
+        lon = xs * xs[np.newaxis, :].T
+        lat = xs + xs[:, np.newaxis]
         coords = {
             'lon': (('ny', 'nx'), lon),
             'lat': (('ny', 'nx'), lat),
             'time': [1, 2, 3],
-            'samples': ('nsamples', [0, 1, 2, 3])
+            'samples': ('nsamples', [0, 1, 2, 3]),
         }
         self.ds_unindexed = xr.DataArray(
             np.random.rand(5, 5, 3, 4), coords=coords, dims=('nx', 'ny', 'time', 'nsamples')
         )
 
     def test_rgb_dataarray_no_args(self):
         rgb = self.da_rgb.hvplot()
-        self.assertEqual(rgb, RGB(([0, 1], [0, 1])+tuple(self.da_rgb.values)))
+        self.assertEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
 
     def test_rgb_dataarray_explicit_args(self):
         rgb = self.da_rgb.hvplot('x', 'y')
-        self.assertEqual(rgb, RGB(([0, 1], [0, 1])+tuple(self.da_rgb.values)))
+        self.assertEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
 
     def test_rgb_dataarray_explicit_args_and_kind(self):
         rgb = self.da_rgb.hvplot.rgb('x', 'y')
-        self.assertEqual(rgb, RGB(([0, 1], [0, 1])+tuple(self.da_rgb.values)))
+        self.assertEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
 
     def test_rgb_dataset(self):
         rgb = self.da_rgb.to_dataset(name='z').hvplot.rgb()
-        self.assertEqual(rgb, RGB(([0, 1], [0, 1])+tuple(self.da_rgb.values)))
+        self.assertEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
 
     def test_rgb_dataset_explicit_z(self):
         rgb = self.da_rgb.to_dataset(name='z').hvplot.rgb(z='z')
-        self.assertEqual(rgb, RGB(([0, 1], [0, 1])+tuple(self.da_rgb.values)))
+        self.assertEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
+
+    def test_rgb_dataset_robust(self):
+        rgb = self.da_rgb.to_dataset(name='z').hvplot.rgb(robust=True)
+        self.assertNotEqual(rgb, RGB(([0, 1], [0, 1]) + tuple(self.da_rgb.values)))
 
     def test_rgb_dataarray_groupby_explicit(self):
         rgb = self.da_rgb_by_time.hvplot.rgb('x', 'y', groupby='time')
-        self.assertEqual(rgb[0], RGB(([0, 1], [0, 1])+tuple(self.da_rgb_by_time.values[0])))
-        self.assertEqual(rgb[1], RGB(([0, 1], [0, 1])+tuple(self.da_rgb_by_time.values[1])))
+        self.assertEqual(rgb[0], RGB(([0, 1], [0, 1]) + tuple(self.da_rgb_by_time.values[0])))
+        self.assertEqual(rgb[1], RGB(([0, 1], [0, 1]) + tuple(self.da_rgb_by_time.values[1])))
 
     def test_rgb_dataarray_groupby_infer(self):
         rgb = self.da_rgb_by_time.hvplot.rgb('x', 'y', bands='band')
-        self.assertEqual(rgb[0], RGB(([0, 1], [0, 1])+tuple(self.da_rgb_by_time.values[0])))
-        self.assertEqual(rgb[1], RGB(([0, 1], [0, 1])+tuple(self.da_rgb_by_time.values[1])))
+        self.assertEqual(rgb[0], RGB(([0, 1], [0, 1]) + tuple(self.da_rgb_by_time.values[0])))
+        self.assertEqual(rgb[1], RGB(([0, 1], [0, 1]) + tuple(self.da_rgb_by_time.values[1])))
 
     def test_img_dataarray_infers_correct_other_dims(self):
         img = self.da_img_by_time[0].hvplot()
         self.assertEqual(img, Image(self.da_img_by_time[0], ['lon', 'lat'], ['value']))
 
+    def test_img_dataarray_robust_to_clim_percentile(self):
+        img = self.da_img_by_time[0].hvplot(robust=True)
+        assert img.opts['clim_percentile'] is True
+
     def test_img_dataarray_groupby_infers_correct_other_dims(self):
         img = self.da_img_by_time.hvplot(groupby='time')
         self.assertEqual(img[0], Image(self.da_img_by_time[0], ['lon', 'lat'], ['value']))
         self.assertEqual(img[1], Image(self.da_img_by_time[1], ['lon', 'lat'], ['value']))
 
     def test_line_infer_dimension_params_from_xarray_attrs(self):
         hmap = self.xarr_with_attrs.hvplot.line(groupby='x', dynamic=False)
@@ -196,37 +210,37 @@
 
     def test_symmetric_dataset_not_in_memory(self):
         # Creating a netcdf file and loading it as to get an non in memory
         # DataArray.
         da = xr.DataArray(
             data=np.arange(-100, 100).reshape(10, 10, 2),
             dims=['x', 'y', 'z'],
-            coords={'x': np.arange(10), 'y': np.arange(10), 'z': np.arange(2)}
+            coords={'x': np.arange(10), 'y': np.arange(10), 'z': np.arange(2)},
         )
         ds = xr.Dataset(data_vars={'value': da})
         with tempfile.TemporaryDirectory() as tempdir:
             fpath = os.path.join(tempdir, 'data.nc')
             ds.to_netcdf(fpath)
             ds = xr.open_dataset(fpath)
-            plot = ds.value.hvplot(x='x', y='y', check_symmetric_max=ds.value.size+1)
+            plot = ds.value.hvplot(x='x', y='y', check_symmetric_max=ds.value.size + 1)
             plot[(0)]
             plot_opts = Store.lookup_options('bokeh', plot.last, 'plot')
             # If a DataArray is not in memory, computing whether it's symmetric should
             # not be done and return False.
             assert not plot_opts.kwargs['symmetric']
             ds.close()
 
     def test_symmetric_dataset_in_memory(self):
         da = xr.DataArray(
             data=np.arange(-100, 100).reshape(10, 10, 2),
             dims=['x', 'y', 'z'],
-            coords={'x': np.arange(10), 'y': np.arange(10), 'z': np.arange(2)}
+            coords={'x': np.arange(10), 'y': np.arange(10), 'z': np.arange(2)},
         )
         ds = xr.Dataset(data_vars={'value': da})
-        plot = ds.value.hvplot(x='x', y='y', check_symmetric_max=ds.value.size+1)
+        plot = ds.value.hvplot(x='x', y='y', check_symmetric_max=ds.value.size + 1)
         plot[(0)]
         plot_opts = Store.lookup_options('bokeh', plot.last, 'plot')
         # This DataArray happens to be symmetric.
         assert plot_opts.kwargs['symmetric']
 
     def test_dataarray_unnamed_label(self):
         plot = self.da_rgb.sel(band=1).hvplot.image(label='test')
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testhelp.py` & `hvplot-0.9.3a1/hvplot/tests/testhelp.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,48 +19,57 @@
         kind='line',
         completions=False,
         docstring=False,
         generic=False,
         style=True,
         signature=None,
     )
-    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(sorted(Store.registry['bokeh'][Curve].style_opts))
+    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(
+        sorted(Store.registry['bokeh'][Curve].style_opts)
+    )
 
     # The current backend becomes matplotlib
     hvplot.extension('matplotlib', 'plotly')
     docstring, signature = hvplot._get_doc_and_signature(
         cls=hvplot.hvPlot,
         kind='line',
         completions=False,
         docstring=False,
         generic=False,
         style=True,
         signature=None,
     )
-    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(sorted(Store.registry['matplotlib'][Curve].style_opts))
+    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(
+        sorted(Store.registry['matplotlib'][Curve].style_opts)
+    )
 
     # The current backend becomes plotly
     hvplot.output(backend='plotly')
     docstring, signature = hvplot._get_doc_and_signature(
         cls=hvplot.hvPlot,
         kind='line',
         completions=False,
         docstring=False,
         generic=False,
         style=True,
         signature=None,
     )
-    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(sorted(Store.registry['plotly'][Curve].style_opts))
+    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(
+        sorted(Store.registry['plotly'][Curve].style_opts)
+    )
+
 
 def test_help_style_compatibility(reset_default_backend):
     # The current backend is plotly but the style options are those of matplotlib
     hvplot.extension('plotly', 'matplotlib', compatibility='matplotlib')
     docstring, signature = hvplot._get_doc_and_signature(
         cls=hvplot.hvPlot,
         kind='line',
         completions=False,
         docstring=False,
         generic=False,
         style=True,
         signature=None,
     )
-    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(sorted(Store.registry['matplotlib'][Curve].style_opts))
+    assert docstring == '\nStyle options\n-------------\n\n' + '\n'.join(
+        sorted(Store.registry['matplotlib'][Curve].style_opts)
+    )
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testinteractive.py` & `hvplot-0.9.3a1/hvplot/tests/testinteractive.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 from holoviews.util.transform import dim
 from hvplot import bind
 from hvplot.interactive import Interactive
 from hvplot.tests.util import makeDataFrame, makeMixedDataFrame
 from hvplot.xarray import XArrayInteractive
 from hvplot.util import bokeh3, param2
 
-is_bokeh2 = pytest.mark.skipif(bokeh3, reason="requires bokeh 2.x")
-is_bokeh3 = pytest.mark.skipif(not bokeh3, reason="requires bokeh 3.x")
+is_bokeh2 = pytest.mark.skipif(bokeh3, reason='requires bokeh 2.x')
+is_bokeh3 = pytest.mark.skipif(not bokeh3, reason='requires bokeh 3.x')
 
 
 @pytest.fixture(scope='module')
 def series():
     return pd.Series(np.arange(5.0), name='A')
 
 
@@ -41,17 +41,15 @@
     return dataset.air
 
 
 class CallCtxt:
     def __init__(self, call_args, call_kwargs, **kwargs):
         for k, v in kwargs.items():
             if k in ['args', 'kwargs']:
-                raise ValueError(
-                    "**kwargs passed to CallCtxt can't be named args or kwargs"
-                )
+                raise ValueError("**kwargs passed to CallCtxt can't be named args or kwargs")
             setattr(self, k, v)
         self.args = call_args
         self.kwargs = call_kwargs
 
     def __repr__(self):
         inner = ''
         for attr in vars(self):
@@ -171,15 +169,15 @@
 
     select.value = 'B'
     assert dfi._obj is df.B
 
 
 def test_interactive_xarray_function(dataset):
     ds = dataset.copy()
-    ds['air2'] = ds.air*2
+    ds['air2'] = ds.air * 2
 
     select = pn.widgets.Select(options=list(ds))
 
     def sel_col(sel):
         return ds[sel]
 
     dsi = Interactive(bind(sel_col, select))
@@ -192,31 +190,31 @@
     select.value = 'air2'
     assert (dsi._obj == ds.air2).all()
     assert dsi._transform == dim('air2')
 
 
 def test_interactive_nested_widgets():
     df = makeDataFrame()
-    w = pn.widgets.RadioButtonGroup(value="A", options=list("ABC"))
+    w = pn.widgets.RadioButtonGroup(value='A', options=list('ABC'))
 
     idf = Interactive(df)
-    pipeline = idf.groupby(["D", w]).mean()
+    pipeline = idf.groupby(['D', w]).mean()
     ioutput = pipeline.panel().object().object
     iw = pipeline.widgets()
 
-    output = df.groupby(["D", "A"]).mean()
+    output = df.groupby(['D', 'A']).mean()
 
     pd.testing.assert_frame_equal(ioutput, output)
     assert len(iw) == 1
     assert iw[0] == w
 
 
 @pytest.mark.skipif(
-    Version(hv.__version__) < Version("1.15.1"),
-    reason="Needs holoviews 1.15.1",
+    Version(hv.__version__) < Version('1.15.1'),
+    reason='Needs holoviews 1.15.1',
 )
 def test_interactive_slice():
     df = makeDataFrame()
     w = pn.widgets.IntSlider(start=10, end=40)
 
     idf = Interactive(df)
     pipeline = idf.iloc[:w]
@@ -234,27 +232,27 @@
     output = df.iloc[:15]
     pd.testing.assert_frame_equal(ioutput, output)
 
 
 def test_interactive_pandas_dataframe_hvplot_accessor(df):
     dfi = df.interactive()
 
-    assert dfi.hvplot(kind="scatter")._transform == dfi.hvplot.scatter()._transform
+    assert dfi.hvplot(kind='scatter')._transform == dfi.hvplot.scatter()._transform
 
     with pytest.raises(TypeError):
-        dfi.hvplot.scatter(kind="area")
+        dfi.hvplot.scatter(kind='area')
 
 
 def test_interactive_xarray_dataset_hvplot_accessor(dataarray):
     dai = dataarray.interactive
 
-    assert dai.hvplot(kind="line")._transform == dai.hvplot.line()._transform
+    assert dai.hvplot(kind='line')._transform == dai.hvplot.line()._transform
 
     with pytest.raises(TypeError):
-        dai.hvplot.line(kind="area")
+        dai.hvplot.line(kind='area')
 
 
 def test_interactive_pandas_dataframe_hvplot_accessor_dmap(df):
     dfi = df.interactive()
     dfi = dfi.hvplot.line(y='A')
 
     # TODO: Not sure about the logic
@@ -266,15 +264,15 @@
     dfi = df.interactive()
     dfi = dfi.hvplot(kind=w, y='A')
 
     assert dfi._dmap is False
 
 
 def test_interactive_with_bound_function_calls():
-    df = pd.DataFrame({"species": [1, 1, 1, 2, 2, 2], "sex": 3 * ["MALE", "FEMALE"]})
+    df = pd.DataFrame({'species': [1, 1, 1, 2, 2, 2], 'sex': 3 * ['MALE', 'FEMALE']})
 
     w_species = pn.widgets.Select(name='Species', options=[1, 2])
     w_sex = pn.widgets.MultiSelect(name='Sex', value=['MALE'], options=['MALE', 'FEMALE'])
 
     def load_data(species, watch=True):
         if watch:
             load_data.COUNT += 1
@@ -287,46 +285,44 @@
     dfi = dfi.loc[dfi['sex'].isin(w_sex)]
 
     out = dfi.output()
 
     assert isinstance(out, pn.param.ParamFunction)
     assert isinstance(out._pane, pn.pane.DataFrame)
     pd.testing.assert_frame_equal(
-        out._pane.object,
-        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)]
+        out._pane.object, load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)]
     )
 
     (dfi.loc[dfi['sex'].isin(w_sex)])
-    assert load_data.COUNT ==  1
+    assert load_data.COUNT == 1
 
     w_species.value = 2
 
     pd.testing.assert_frame_equal(
-        out._pane.object,
-        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)]
+        out._pane.object, load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)]
     )
 
     assert load_data.COUNT == 2
 
     dfi = dfi.head(1)
 
     assert load_data.COUNT == 2
 
     out = dfi.output()
 
     pd.testing.assert_frame_equal(
         out._pane.object,
-        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)].head(1)
+        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)].head(1),
     )
 
     w_species.value = 1
 
     pd.testing.assert_frame_equal(
         out._pane.object,
-        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)].head(1)
+        load_data(w_species.value, watch=False).loc[df['sex'].isin(w_sex.value)].head(1),
     )
 
     assert load_data.COUNT == 3
 
 
 def test_interactive_pandas_series_init(series, clone_spy):
     si = Interactive(series)
@@ -440,15 +436,14 @@
     # 2nd _clone in __call__
     assert clone_spy.calls[2].depth == 3
     assert len(clone_spy.calls[2].args) == 1
     assert repr(clone_spy.calls[2].args[0]) == "dim('*').pd.head(n=2)"
     assert clone_spy.calls[2].kwargs == {'plot': False}
 
 
-
 def test_interactive_pandas_series_method_not_called(series, clone_spy):
     si = Interactive(series)
     si = si.head
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
     pd.testing.assert_series_equal(si._current.A, si._obj)
@@ -525,15 +520,15 @@
     assert clone_spy.calls[4].depth == 5
     assert len(clone_spy.calls[4].args) == 1
     assert repr(clone_spy.calls[4].args[0]) == "(dim('*').pd+2).head(2)"
     assert clone_spy.calls[4].kwargs == {'plot': False}
 
 
 def test_interactive_pandas_series_operator_widget(series):
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
 
     si = Interactive(series)
 
     si = si + w
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
@@ -563,38 +558,41 @@
     assert si._method is None
 
     assert len(si._params) == 1
     assert si._params[0] is w.param.value
 
 
 def test_interactive_pandas_series_operator_and_method_widget(series):
-    w1 = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w1 = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     w2 = pn.widgets.IntSlider(value=2, start=1, end=5)
 
     si = Interactive(series)
 
     si = (si + w1).head(w2)
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
     pd.testing.assert_series_equal(si._current.A, (series + w1.value).head(w2.value))
     assert si._obj is series
-    assert repr(si._transform) == "(dim('*').pd+FloatSlider(end=5.0, start=1.0, value=2.0)).head(IntSlider(end=5, start=1, value=2))"
+    assert (
+        repr(si._transform)
+        == "(dim('*').pd+FloatSlider(end=5.0, start=1.0, value=2.0)).head(IntSlider(end=5, start=1, value=2))"
+    )
     assert si._depth == 5
     assert si._method is None
 
     assert len(si._params) == 2
     assert si._params[0] is w1.param.value
     assert si._params[1] is w2.param.value
 
 
 def test_interactive_pandas_series_operator_ipywidgets(series):
-    ipywidgets = pytest.importorskip("ipywidgets")
+    ipywidgets = pytest.importorskip('ipywidgets')
 
-    w = ipywidgets.FloatSlider(value=2., min=1., max=5.)
+    w = ipywidgets.FloatSlider(value=2.0, min=1.0, max=5.0)
 
     si = Interactive(series)
 
     si = si + w
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
@@ -612,15 +610,15 @@
     assert isinstance(widgets, pn.Column)
     assert len(widgets) == 1
     assert isinstance(widgets[0], pn.pane.IPyWidget)
     assert widgets[0].object is w
 
 
 def test_interactive_pandas_series_operator_out_widgets(series):
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     si = Interactive(series)
     si = si + w
 
     widgets = si.widgets()
 
     assert isinstance(widgets, pn.Column)
     assert len(widgets) == 1
@@ -636,15 +634,15 @@
 
     assert isinstance(widgets, pn.Column)
     assert len(widgets) == 1
     assert widgets[0] is w
 
 
 def test_interactive_pandas_series_operator_and_method_out_widgets(series):
-    w1 = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w1 = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     w2 = pn.widgets.IntSlider(value=2, start=1, end=5)
     si = Interactive(series)
 
     si = (si + w1).head(w2)
 
     widgets = si.widgets()
 
@@ -673,79 +671,82 @@
     select = pn.widgets.Select(value='A', options=list(df.columns))
 
     def sel_col(col):
         return df[col]
 
     dfi = Interactive(bind(sel_col, select))
 
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     dfi = dfi + w
 
     widgets = dfi.widgets()
 
     assert isinstance(widgets, pn.Column)
     assert len(widgets) == 2
     assert widgets[0] is select
     assert widgets[1] is w
 
 
 def test_interactive_reevaluate_uses_cached_value(series):
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     si = Interactive(series)
     si = si + w
 
-    w.value = 3.
+    w.value = 3.0
     assert repr(si._transform) == "dim('*').pd+FloatSlider(end=5.0, start=1.0, value=3.0)"
 
     assert si._callback().object is si._callback().object
 
 
 def test_interactive_pandas_series_operator_widget_update(series):
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     si = Interactive(series)
     si = si + w
 
-    w.value = 3.
+    w.value = 3.0
     assert repr(si._transform) == "dim('*').pd+FloatSlider(end=5.0, start=1.0, value=3.0)"
 
     out = si._callback()
     assert out.object is si.eval()
     assert isinstance(out, pn.pane.DataFrame)
-    pd.testing.assert_series_equal(out.object.A, series + 3.)
+    pd.testing.assert_series_equal(out.object.A, series + 3.0)
 
 
 def test_interactive_pandas_series_method_widget_update(series):
     w = pn.widgets.IntSlider(value=2, start=1, end=5)
     si = Interactive(series)
     si = si.head(w)
 
     w.value = 3
-    assert repr(si._transform) =="dim('*').pd.head(IntSlider(end=5, start=1, value=3))"
+    assert repr(si._transform) == "dim('*').pd.head(IntSlider(end=5, start=1, value=3))"
 
     out = si._callback()
     assert out.object is si.eval()
     assert isinstance(out, pn.pane.DataFrame)
     pd.testing.assert_series_equal(out.object.A, series.head(3))
 
 
 def test_interactive_pandas_series_operator_and_method_widget_update(series):
-    w1 = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w1 = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
     w2 = pn.widgets.IntSlider(value=2, start=1, end=5)
     si = Interactive(series)
     si = (si + w1).head(w2)
 
-    w1.value = 3.
+    w1.value = 3.0
     w2.value = 3
 
-    assert repr(si._transform) == "(dim('*').pd+FloatSlider(end=5.0, start=1.0, value=3.0)).head(IntSlider(end=5, start=1, value=3))"
+    assert (
+        repr(si._transform)
+        == "(dim('*').pd+FloatSlider(end=5.0, start=1.0, value=3.0)).head(IntSlider(end=5, start=1, value=3))"
+    )
 
     out = si._callback()
     assert out.object is si.eval()
     assert isinstance(out, pn.pane.DataFrame)
-    pd.testing.assert_series_equal(out.object.A, (series + 3.).head(3))
+    pd.testing.assert_series_equal(out.object.A, (series + 3.0).head(3))
 
 
 def test_interactive_pandas_frame_loc(df):
     dfi = Interactive(df)
 
     dfi = dfi.loc[:, 'A']
 
@@ -956,23 +957,24 @@
 
     # In that case the default behavior is to return the object transformed
     # and to which _method is applied
     assert isinstance(out, pd.Series)
     pd.testing.assert_series_equal(df.A, out)
 
 
-@pytest.mark.parametrize('op', [
-    '-',   # __neg__
-
-    # Doesn't any of the supported data implement __not__?
-    # e.g. `not series` raises an error.
-    # 'not', # __not__
-
-    '+',   # _pos__
-])
+@pytest.mark.parametrize(
+    'op',
+    [
+        '-',  # __neg__
+        # Doesn't any of the supported data implement __not__?
+        # e.g. `not series` raises an error.
+        # 'not', # __not__
+        '+',  # _pos__
+    ],
+)
 def test_interactive_pandas_series_operator_unary(series, op):
     if op == '~':
         series = pd.Series([True, False, True], name='A')
     si = Interactive(series)
     si = eval(f'{op} si')
 
     assert isinstance(si, Interactive)
@@ -994,75 +996,81 @@
     pd.testing.assert_series_equal(si._current.A, ~series)
     assert si._obj is series
     assert repr(si._transform) == "dim('*', inv)"
     assert si._depth == 2
     assert si._method is None
 
 
-@pytest.mark.parametrize('op', [
-    '+',  # __add__
-    '&',  # __and__
-    '/',  # __div__
-    '==', # __eq__
-    '//', # __floordiv__
-    '>=', # __ge__
-    '>',  # __gt__
-    '<=', # __le__
-    '<',  # __lt__
-    '<',  # __lt__
-    # '<<',  # __lshift__
-    '%',  # __mod__
-    '*',  # __mul__
-    '!=',  # __ne__
-    '|',  # __or__
-    # '>>',  # __rshift__
-    '**',  # __pow__
-    '-',  # __sub__
-    '/',  # __truediv__
-])
+@pytest.mark.parametrize(
+    'op',
+    [
+        '+',  # __add__
+        '&',  # __and__
+        '/',  # __div__
+        '==',  # __eq__
+        '//',  # __floordiv__
+        '>=',  # __ge__
+        '>',  # __gt__
+        '<=',  # __le__
+        '<',  # __lt__
+        '<',  # __lt__
+        # '<<',  # __lshift__
+        '%',  # __mod__
+        '*',  # __mul__
+        '!=',  # __ne__
+        '|',  # __or__
+        # '>>',  # __rshift__
+        '**',  # __pow__
+        '-',  # __sub__
+        '/',  # __truediv__
+    ],
+)
 def test_interactive_pandas_series_operator_binary(series, op):
     if op in ['&', '|']:
         series = pd.Series([True, False, True], name='A')
         val = True
     else:
-        val = 2.
+        val = 2.0
     si = Interactive(series)
     si = eval(f'si {op} {val}')
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
     pd.testing.assert_series_equal(si._current.A, eval(f'series {op} {val}'))
     assert si._obj is series
     val_repr = '2.0' if isinstance(val, float) else 'True'
     assert repr(si._transform) == f"dim('*').pd{op}{val_repr}"
     assert si._depth == 2
     assert si._method is None
 
 
-@pytest.mark.parametrize('op', [
-    '+',  # __radd__
-    '&',  # __rand__
-    '/',  # __rdiv__
-    '//', # __rfloordiv__
-    # '<<',  # __rlshift__
-    '%',  # __rmod__
-    '*',  # __rmul__
-    '|',  # __ror__
-    '**',  # __rpow__
-    # '>>',  # __rshift__
-    '-',  # __rsub__
-    '/',  # __rtruediv__
-])
+@pytest.mark.parametrize(
+    'op',
+    [
+        '+',  # __radd__
+        '&',  # __rand__
+        '/',  # __rdiv__
+        '//',  # __rfloordiv__
+        # '<<',  # __rlshift__
+        '%',  # __rmod__
+        '*',  # __rmul__
+        '|',  # __ror__
+        '**',  # __rpow__
+        # '>>',  # __rshift__
+        '-',  # __rsub__
+        '/',  # __rtruediv__
+    ],
+)
 def test_interactive_pandas_series_operator_reverse_binary(op):
     if op in ['&', '|']:
         series = pd.Series([True, False, True], name='A')
         val = True
     else:
         series = pd.Series([1.0, 2.0, 3.0], name='A')
-        val = 2.
+        val = 2.0
     si = Interactive(series)
     si = eval(f'{val} {op} si')
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
     pd.testing.assert_series_equal(si._current.A, eval(f'{val} {op} series'))
     assert si._obj is series
@@ -1102,15 +1110,17 @@
     si = Interactive(series)
 
     si = si.plot()
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, matplotlib.axes.Axes)
     assert si._obj is series
-    assert "dim('*').pd.plot(ax=<function Interactive._get_ax_fn.<locals>.get_ax" in repr(si._transform)
+    assert "dim('*').pd.plot(ax=<function Interactive._get_ax_fn.<locals>.get_ax" in repr(
+        si._transform
+    )
     assert si._depth == 3
     assert si._method is None
 
     assert clone_spy.count == 3
 
     # _clone(True) in _resolve_accessor in __getattribute__(name='plot')
     assert clone_spy.calls[0].depth == 1
@@ -1123,15 +1133,17 @@
     assert clone_spy.calls[1].kwargs == {'copy': True}
 
     # 2nd _clone in __call__
     assert clone_spy.calls[2].depth == 3
     assert len(clone_spy.calls[2].args) == 1
     # Not the complete repr as the function doesn't have a nice repr,
     # its repr displays  the memory address.
-    assert "dim('*').pd.plot(ax=<function Interactive._get_ax_fn.<locals>.get_ax" in repr(clone_spy.calls[2].args[0])
+    assert "dim('*').pd.plot(ax=<function Interactive._get_ax_fn.<locals>.get_ax" in repr(
+        clone_spy.calls[2].args[0]
+    )
     assert clone_spy.calls[2].kwargs == {'plot': True}
 
     assert not si._dmap
     assert isinstance(si._fig, matplotlib.figure.Figure)
 
     # Just test that it doesn't raise any error.
     si.output()
@@ -1140,15 +1152,14 @@
 def test_interactive_pandas_series_plot_kind_attr(series, clone_spy):
     # TODO: Not checking the dim reprs in this test as that was
     # affecting the pipeline.
     si = Interactive(series)
 
     si = si.plot.line()
 
-
     assert isinstance(si, Interactive)
     assert isinstance(si._current, matplotlib.axes.Axes)
     assert si._obj is series
     # assert "dim('*').pd.plot).line(ax=<function Interactive._get_ax_fn.<locals>.get_ax" in repr(si._transform)
     assert si._depth == 4
     assert si._method is None
 
@@ -1182,15 +1193,14 @@
     assert not si._dmap
     assert isinstance(si._fig, matplotlib.figure.Figure)
 
     # Just test that it doesn't raise any error.
     si.output()
 
 
-
 def test_interactive_pandas_dir_no_type_change(df):
     dfi = Interactive(df)
     dfi = dfi.head()
 
     attrs = dir(dfi)
 
     assert all(col in attrs for col in list(df.columns))
@@ -1199,37 +1209,39 @@
 
 def test_interactive_pandas_dir_with_type_change(df):
     dfi = Interactive(df)
     dfi = dfi.head().A.head()
 
     attrs = dir(dfi)
 
-    assert not any(col in attrs for col in  list(df.columns))
+    assert not any(col in attrs for col in list(df.columns))
     assert 'T' in attrs
 
 
-@pytest.mark.xfail(reason='hvplot.util.check_library expects the obj to have __module__, which is not true for a float')
+@pytest.mark.xfail(
+    reason='hvplot.util.check_library expects the obj to have __module__, which is not true for a float'
+)
 def test_interactive_pandas_dir_with_type_change_to_float(df):
     dfi = Interactive(df)
     dfi = dfi.head().A.max()
 
     attrs = dir(dfi)
 
-    assert not any(col in attrs for col in  list(df.columns))
+    assert not any(col in attrs for col in list(df.columns))
     assert 'describe' not in attrs
     assert 'real' not in attrs
 
 
 def test_interactive_pandas_dir_attrib(df):
     dfi = Interactive(df)
     dfi = dfi.head().A
 
     attrs = dir(dfi)
 
-    assert not any(col in attrs for col in  list(df.columns))
+    assert not any(col in attrs for col in list(df.columns))
     assert 'T' in attrs
 
 
 def test_interactive_pandas_layout_default_no_widgets(df):
     dfi = Interactive(df)
     dfi = dfi.head()
 
@@ -1292,14 +1304,15 @@
     assert isinstance(layout[0], pn.Column)
     assert len(layout[0]) == 2
     assert isinstance(layout[0][0], pn.Column)
     assert isinstance(layout[0][1], pn.pane.PaneBase)
     assert len(layout[0][0]) == 1
     assert isinstance(layout[0][0][0], pn.widgets.IntSlider)
 
+
 @is_bokeh2
 def test_interactive_pandas_layout_center_with_widgets(df):
     w = pn.widgets.IntSlider(value=2, start=1, end=5)
     dfi = df.interactive(center=True)
     dfi = dfi.head(w)
 
     assert dfi._center is True
@@ -1369,15 +1382,15 @@
 
     evaled = dfi.eval()
 
     assert isinstance(evaled, hv.Curve)
 
 
 def test_interactive_pandas_series_widget_value(series):
-    w = pn.widgets.FloatSlider(value=2., start=1., end=5.)
+    w = pn.widgets.FloatSlider(value=2.0, start=1.0, end=5.0)
 
     si = Interactive(series)
 
     si = si + w.param.value
 
     assert isinstance(si, Interactive)
     assert isinstance(si._current, pd.DataFrame)
@@ -1405,15 +1418,15 @@
     df = pd.DataFrame()
     msgs = []
 
     def piped(df, msg):
         msgs.append(msg)
         return df
 
-    df.interactive.pipe(piped, msg="1").pipe(piped, msg="2")
+    df.interactive.pipe(piped, msg='1').pipe(piped, msg='2')
 
     assert len(msgs) == 3
 
 
 def test_interactive_accept_non_str_columnar_data():
     df = pd.DataFrame(np.random.random((10, 2)))
     assert all(not isinstance(col, str) for col in df.columns)
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testnetworkx.py` & `hvplot-0.9.3a1/hvplot/tests/testnetworkx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest import TestCase, SkipTest
 
 try:
     import numpy as np
     import networkx as nx
     import hvplot.networkx as hvnx
-except:
+except ImportError:
     raise SkipTest('NetworkX not available')
 
-class TestOptions(TestCase):
 
+class TestOptions(TestCase):
     def setUp(self):
         # Create nodes (1-10) in unsorted order
         nodes = np.array([1, 4, 5, 10, 8, 9, 3, 7, 2, 6])
         edges = list(zip(nodes[:-1], nodes[1:]))
 
         g = nx.Graph()
         g.add_nodes_from(nodes)
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testoperations.py` & `hvplot-0.9.3a1/hvplot/tests/testoperations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import sys
 
 from unittest import SkipTest
 from parameterized import parameterized
 
-import colorcet as cc
 import holoviews as hv
 import hvplot.pandas  # noqa
 import numpy as np
 import pandas as pd
 import pytest
 
 from holoviews import Store, render
@@ -18,52 +17,66 @@
 from holoviews.element.comparison import ComparisonTestCase
 from hvplot.converter import HoloViewsConverter
 from hvplot.tests.util import makeTimeDataFrame
 from packaging.version import Version
 
 
 class TestDatashader(ComparisonTestCase):
-
     def setUp(self):
         try:
-            import datashader # noqa
-        except:
+            import datashader  # noqa
+        except ImportError:
             raise SkipTest('Datashader not available')
         if sys.maxsize < 2**32:
             raise SkipTest('Datashader does not support 32-bit systems')
-        import hvplot.pandas # noqa
-        self.df = pd.DataFrame([[1, 2, 'A', 0.1], [3, 4, 'B', 0.2], [5, 6, 'C', 0.3]],
-                               columns=['x', 'y', 'category', 'number'])
+        import hvplot.pandas  # noqa
+
+        self.df = pd.DataFrame(
+            [[1, 2, 'A', 0.1], [3, 4, 'B', 0.2], [5, 6, 'C', 0.3]],
+            columns=['x', 'y', 'category', 'number'],
+        )
 
     def test_rasterize_by_cat(self):
         from datashader.reductions import count_cat
+
         dmap = self.df.hvplot.scatter('x', 'y', by='category', rasterize=True)
         agg = dmap.callback.inputs[0].callback.operation.p.aggregator
         self.assertIsInstance(agg, count_cat)
         self.assertEqual(agg.column, 'category')
 
+    def test_rasterize_by_cat_agg(self):
+        from datashader.reductions import count_cat
+
+        dmap = self.df.hvplot.scatter('x', 'y', aggregator=count_cat('category'), rasterize=True)
+        agg = dmap.callback.inputs[0].callback.operation.p.aggregator
+        self.assertIsInstance(agg, count_cat)
+        self.assertEqual(agg.column, 'category')
+
     @parameterized.expand([('rasterize',), ('datashade',)])
     def test_color_dim_with_default_agg(self, operation):
         from datashader.reductions import mean
+
         dmap = self.df.hvplot.scatter('x', 'y', c='number', **{operation: True})
         agg = dmap.callback.inputs[0].callback.operation.p.aggregator
         self.assertIsInstance(agg, mean)
         self.assertEqual(agg.column, 'number')
 
     @parameterized.expand([('rasterize',), ('datashade',)])
     def test_color_dim_with_string_agg(self, operation):
         from datashader.reductions import sum
+
         dmap = self.df.hvplot.scatter('x', 'y', c='number', aggregator='sum', **{operation: True})
         agg = dmap.callback.inputs[0].callback.operation.p.aggregator
         self.assertIsInstance(agg, sum)
         self.assertEqual(agg.column, 'number')
 
     @parameterized.expand([('rasterize',), ('datashade',)])
     def test_color_dim_also_an_axis(self, operation):
         from datashader.reductions import mean
+
         original_data = self.df.copy(deep=True)
         dmap = self.df.hvplot.scatter('x', 'y', c='y', **{operation: True})
         agg = dmap.callback.inputs[0].callback.operation.p.aggregator
         self.assertIsInstance(agg, mean)
         self.assertEqual(agg.column, '_color')
         assert original_data.equals(self.df)
 
@@ -118,27 +131,30 @@
         self.assertEqual(opts[opt], 2)
         self.assertEqual(opts.get('frame_height'), 150)
         self.assertEqual(opts.get('height'), None)
         self.assertEqual(opts.get('frame_width'), None)
 
     @parameterized.expand([('aspect',), ('data_aspect',)])
     def test_aspect_and_frame_height_with_datashade_and_dynamic_is_false(self, opt):
-        plot = self.df.hvplot(x='x', y='y', frame_height=150, datashade=True, dynamic=False, **{opt: 2})
+        plot = self.df.hvplot(
+            x='x', y='y', frame_height=150, datashade=True, dynamic=False, **{opt: 2}
+        )
         opts = Store.lookup_options('bokeh', plot[()], 'plot').kwargs
         self.assertEqual(opts[opt], 2)
         self.assertEqual(opts.get('frame_height'), 150)
         self.assertEqual(opts.get('height'), None)
         self.assertEqual(opts.get('frame_width'), None)
 
     def test_cmap_can_be_color_key(self):
         color_key = {'A': '#ff0000', 'B': '#00ff00', 'C': '#0000ff'}
         self.df.hvplot.points(x='x', y='y', by='category', cmap=color_key, datashade=True)
         with self.assertRaises(TypeError):
-            self.df.hvplot.points(x='x', y='y', by='category', datashade=True,
-                                  cmap='kbc_r', color_key=color_key)
+            self.df.hvplot.points(
+                x='x', y='y', by='category', datashade=True, cmap='kbc_r', color_key=color_key
+            )
 
     def test_when_datashade_is_true_set_hover_to_false_by_default(self):
         plot = self.df.hvplot(x='x', y='y', datashade=True)
         opts = Store.lookup_options('bokeh', plot[()], 'plot').kwargs
         assert 'hover' not in opts.get('tools')
 
     def test_when_datashade_is_true_hover_can_still_be_true(self):
@@ -153,50 +169,78 @@
 
     @parameterized.expand([('scatter',), ('line',), ('area',)])
     def test_wide_charts_categorically_shaded_explicit_ys(self, kind):
         df = makeTimeDataFrame()
         plot = makeTimeDataFrame().hvplot(y=list(df.columns), datashade=True, kind=kind)
         expected_cmap = HoloViewsConverter._default_cmaps['categorical']
         assert plot.callback.inputs[0].callback.operation.p.cmap == expected_cmap
-        assert  plot.callback.inputs[0].callback.operation.p.aggregator.column == 'Variable'
+        assert plot.callback.inputs[0].callback.operation.p.aggregator.column == 'Variable'
 
     @parameterized.expand([('scatter',), ('line',), ('area',)])
     def test_wide_charts_categorically_shaded_implicit_ys(self, kind):
         plot = makeTimeDataFrame().hvplot(datashade=True, kind=kind)
         expected_cmap = HoloViewsConverter._default_cmaps['categorical']
         assert plot.callback.inputs[0].callback.operation.p.cmap == expected_cmap
-        assert  plot.callback.inputs[0].callback.operation.p.aggregator.column == 'Variable'
+        assert plot.callback.inputs[0].callback.operation.p.aggregator.column == 'Variable'
 
-    def test_wide_charts_categorically_shaded_by(self):
+    def test_tidy_charts_categorically_datashade_by(self):
         cat_col = 'category'
         plot = self.df.hvplot.scatter('x', 'y', by=cat_col, datashade=True)
         expected_cmap = HoloViewsConverter._default_cmaps['categorical']
-        assert  plot.callback.inputs[0].callback.operation.p.cmap == expected_cmap
-        assert  plot.callback.inputs[0].callback.operation.p.aggregator.column == cat_col
+        assert plot.callback.inputs[0].callback.operation.p.cmap == expected_cmap
+        assert plot.callback.inputs[0].callback.operation.p.aggregator.column == cat_col
+
+    @pytest.mark.xfail(
+        reason='Assume this is fixed: https://github.com/holoviz/holoviews/issues/6187'
+    )
+    def test_tidy_charts_categorically_rasterized_by(self):
+        cat_col = 'category'
+        plot = self.df.hvplot.scatter('x', 'y', by=cat_col, rasterize=True)
+        expected_cmap = HoloViewsConverter._default_cmaps['categorical']
+        opts = Store.lookup_options('bokeh', plot[()], 'style').kwargs
+        # Failing line
+        assert opts.get('cmap') == expected_cmap
+
+        assert plot.callback.inputs[0].callback.operation.p.aggregator.column == cat_col
+
+    def test_tidy_charts_categorically_rasterized_aggregator_count_cat(self):
+        cat_col = 'category'
+        from datashader.reductions import count_cat
+
+        plot = self.df.hvplot.scatter('x', 'y', aggregator=count_cat(cat_col), rasterize=True)
+        expected_cmap = HoloViewsConverter._default_cmaps['categorical']
+        opts = Store.lookup_options('bokeh', plot[()], 'style').kwargs
+        assert opts.get('cmap') == expected_cmap
+        assert plot.callback.inputs[0].callback.operation.p.aggregator.column == cat_col
+
     def test_rasterize_cnorm(self):
         expected = 'eq_hist'
         plot = self.df.hvplot(x='x', y='y', rasterize=True, cnorm=expected)
         opts = Store.lookup_options('bokeh', plot[()], 'plot').kwargs
         assert opts.get('cnorm') == expected
 
     def test_datashade_cnorm(self):
         expected = 'eq_hist'
         plot = self.df.hvplot(x='x', y='y', datashade=True, cnorm=expected)
         actual = plot.callback.inputs[0].callback.operation.p['cnorm']
         assert actual == expected
 
     def test_rasterize_rescale_discrete_levels(self):
         expected = False
-        plot = self.df.hvplot(x='x', y='y', rasterize=True, cnorm='eq_hist', rescale_discrete_levels=expected)
+        plot = self.df.hvplot(
+            x='x', y='y', rasterize=True, cnorm='eq_hist', rescale_discrete_levels=expected
+        )
         opts = Store.lookup_options('bokeh', plot[()], 'plot').kwargs
         assert opts.get('rescale_discrete_levels') is expected
 
     def test_datashade_rescale_discrete_levels(self):
         expected = False
-        plot = self.df.hvplot(x='x', y='y', datashade=True, cnorm='eq_hist', rescale_discrete_levels=expected)
+        plot = self.df.hvplot(
+            x='x', y='y', datashade=True, cnorm='eq_hist', rescale_discrete_levels=expected
+        )
         actual = plot.callback.inputs[0].callback.operation.p['rescale_discrete_levels']
         assert actual is expected
 
     def test_datashade_rescale_discrete_levels_default_True(self):
         expected = True
         plot = self.df.hvplot(x='x', y='y', datashade=True, cnorm='eq_hist')
         actual = plot.callback.inputs[0].callback.operation.p['rescale_discrete_levels']
@@ -207,35 +251,47 @@
             raise SkipTest('hv.ImageStack introduced after 1.18.0a1')
 
         from holoviews.element import ImageStack
 
         expected = 'category'
         plot = self.df.hvplot(x='x', y='y', by=expected, rasterize=True, dynamic=False)
         assert isinstance(plot, ImageStack)
-        assert plot.opts["cmap"] == cc.palette['glasbey_category10']
+        assert plot.opts['cmap'] == HoloViewsConverter._default_cmaps['categorical']
+
+    def test_rasterize_aggregator_count_cat(self):
+        if Version(hv.__version__) < Version('1.18.0a1'):
+            raise SkipTest('hv.ImageStack introduced after 1.18.0a1')
+
+        from holoviews.element import ImageStack
+        from datashader.reductions import count_cat
+
+        expected = 'category'
+        plot = self.df.hvplot(
+            x='x', y='y', aggregator=count_cat(expected), rasterize=True, width=999, dynamic=False
+        )
+        assert isinstance(plot, ImageStack)
+        assert plot.opts['width'] == 999
+        assert plot.opts['cmap'] == HoloViewsConverter._default_cmaps['categorical']
 
     def test_rasterize_single_y_in_list_linear_cmap(self):
         # Regression, see https://github.com/holoviz/hvplot/issues/1210
         plot = self.df.hvplot.line(y=['y'], rasterize=True)
         opts = Store.lookup_options('bokeh', plot[()], 'style').kwargs
         assert opts.get('cmap') == 'kbc_r'
 
     def test_resample_when_error_unset_operation(self):
-        with pytest.raises(
-            ValueError,
-            match='At least one resampling operation'
-        ):
+        with pytest.raises(ValueError, match='At least one resampling operation'):
             self.df.hvplot(x='x', y='y', resample_when=10)
 
     @parameterized.expand([('rasterize',), ('datashade',)])
     def test_operation_resample_when(self, operation):
         df = pd.DataFrame(
             np.random.multivariate_normal((0, 0), [[0.1, 0.1], [0.1, 1.0]], (5000,))
-        ).rename({0: "x", 1: "y"}, axis=1)
-        dmap = df.hvplot.scatter("x", "y", resample_when=1000, **{operation: True})
+        ).rename({0: 'x', 1: 'y'}, axis=1)
+        dmap = df.hvplot.scatter('x', 'y', resample_when=1000, **{operation: True})
         assert isinstance(dmap, DynamicMap)
 
         render(dmap)  # trigger dynamicmap
         overlay = dmap.items()[0][1]
         assert isinstance(overlay, Overlay)
 
         image = overlay.get(0)
@@ -246,16 +302,16 @@
         assert isinstance(scatter, Scatter)
         assert len(scatter.data) == 0
 
     @parameterized.expand([('points', Points), ('scatter', Scatter)])
     def test_downsample_resample_when(self, kind, eltype):
         df = pd.DataFrame(
             np.random.multivariate_normal((0, 0), [[0.1, 0.1], [0.1, 1.0]], (5000,))
-        ).rename({0: "x", 1: "y"}, axis=1)
-        dmap = df.hvplot(kind=kind, x="x", y="y", resample_when=1000, downsample=True)
+        ).rename({0: 'x', 1: 'y'}, axis=1)
+        dmap = df.hvplot(kind=kind, x='x', y='y', resample_when=1000, downsample=True)
         assert isinstance(dmap, DynamicMap)
 
         render(dmap)  # trigger dynamicmap
         overlay = dmap.items()[0][1]
         assert isinstance(overlay, Overlay)
 
         downsampled = overlay.get(0)
@@ -264,58 +320,66 @@
 
         element = overlay.get(1)
         assert isinstance(element, eltype)
         assert len(element) == 0
 
 
 class TestChart2D(ComparisonTestCase):
-
     def setUp(self):
         try:
             import xarray as xr
-            import datashader as ds # noqa
-        except:
+            import datashader as ds  # noqa
+        except ImportError:
             raise SkipTest('xarray or datashader not available')
         if sys.maxsize < 2**32:
             raise SkipTest('Datashader does not support 32-bit systems')
         import hvplot.xarray  # noqa
+
         data = np.arange(0, 60).reshape(6, 10)
         x = np.arange(10)
         y = np.arange(6)
-        self.da = xr.DataArray(data,
-                               coords={'y': y, 'x': x},
-                               dims=('y', 'x'))
+        self.da = xr.DataArray(data, coords={'y': y, 'x': x}, dims=('y', 'x'))
 
     @parameterized.expand([('image', Image), ('quadmesh', QuadMesh)])
     def test_plot_resolution(self, kind, element):
         plot = self.da.hvplot(kind=kind)
         assert all(plot.data.x.diff('x').round(0) == 1)
         assert all(plot.data.y.diff('y').round(0) == 1)
 
     @parameterized.expand([('image', Image), ('quadmesh', QuadMesh)])
     def test_plot_resolution_with_rasterize(self, kind, element):
-        plot = self.da.hvplot(kind=kind, dynamic=False, rasterize=True,
-                              x_sampling=5, y_sampling=2)
+        plot = self.da.hvplot(kind=kind, dynamic=False, rasterize=True, x_sampling=5, y_sampling=2)
         assert all(plot.data.x.diff('x').round(0) == 5)
         assert all(plot.data.y.diff('y').round(0) == 2)
 
 
 class TestDownsample(ComparisonTestCase):
     def setUp(self):
-        import hvplot.pandas # noqa
+        import hvplot.pandas  # noqa
+
         self.df = pd.DataFrame(np.random.random(100))
 
     def test_downsample_default(self):
         from holoviews.operation.downsample import downsample1d
 
         plot = self.df.hvplot.line(downsample=True)
 
         assert isinstance(plot.callback.operation, downsample1d)
-        assert plot.callback.operation.algorithm == "lttb"
+        assert plot.callback.operation.algorithm == 'lttb'
 
     def test_downsample_opts(self):
-        plot = self.df.hvplot.line(downsample=True, width=100, height=50, x_sampling=5, xlim=(0, 5))
+        plot = self.df.hvplot.line(
+            downsample=True, width=100, height=50, x_sampling=5, xlim=(0, 5)
+        )
 
         assert plot.callback.operation.p.width == 100
         assert plot.callback.operation.p.height == 50
         assert plot.callback.operation.p.x_sampling == 5
         assert plot.callback.operation.p.x_range == (0, 5)
+
+    def test_downsample_algorithm_minmax(self):
+        from holoviews.operation.downsample import downsample1d
+
+        plot = self.df.hvplot.line(downsample='minmax')
+
+        assert isinstance(plot.callback.operation, downsample1d)
+        assert plot.callback.operation_kwargs['algorithm'] == 'minmax'
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testoptions.py` & `hvplot-0.9.3a1/hvplot/tests/testoptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,72 +22,83 @@
 @pytest.fixture(params=['bokeh', 'matplotlib', 'plotly'], scope='class')
 def backend(request):
     backend = request.param
     backend_copy = Store.current_backend
     if backend not in Store.registry:
         hvplot.extension(backend, compatibility='bokeh')
     Store.set_current_backend(backend)
-    store_copy = OptionTree(sorted(Store.options().items()),
-                                    groups=Options._option_groups)
+    store_copy = OptionTree(sorted(Store.options().items()), groups=Options._option_groups)
     yield backend
     Store.options(val=store_copy)
-    Store._custom_options = {k:{} for k in Store._custom_options.keys()}
+    Store._custom_options = {k: {} for k in Store._custom_options.keys()}
     Store.set_current_backend(backend_copy)
 
 
 @pytest.fixture(scope='module')
 def df():
-    return pd.DataFrame([[1, 2, 'A', 0.1], [3, 4, 'B', 0.2], [5, 6, 'C', 0.3]],
-                            columns=['x', 'y', 'category', 'number'])
+    return pd.DataFrame(
+        [[1, 2, 'A', 0.1], [3, 4, 'B', 0.2], [5, 6, 'C', 0.3]],
+        columns=['x', 'y', 'category', 'number'],
+    )
 
 
 @pytest.fixture(scope='module')
 def symmetric_df():
-    return pd.DataFrame([[1, 2, -1], [3, 4, 0], [5, 6, 1]],
-                                        columns=['x', 'y', 'number'])
+    return pd.DataFrame([[1, 2, -1], [3, 4, 0], [5, 6, 1]], columns=['x', 'y', 'number'])
 
 
 @pytest.mark.usefixtures('load_pandas_accessor')
 class TestOptions:
-
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='legend_position not supported w/ matplotlib for scatter')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='legend_position not supported w/ plotly for scatter')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(
+                    reason='legend_position not supported w/ matplotlib for scatter'
+                ),
+            ),
+            pytest.param(
+                'plotly',
+                marks=pytest.mark.xfail(
+                    reason='legend_position not supported w/ plotly for scatter'
+                ),
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_scatter_legend_position(self, df, backend):
         plot = df.hvplot.scatter('x', 'y', c='category', legend='left')
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['legend_position'] == 'left'
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
             'matplotlib',
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='legend_position not supported w/ plotly for hist')),
+            pytest.param(
+                'plotly',
+                marks=pytest.mark.xfail(reason='legend_position not supported w/ plotly for hist'),
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_histogram_by_category_legend_position(self, df, backend):
         plot = df.hvplot.hist('y', by='category', legend='left')
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['legend_position'] == 'left'
 
     @pytest.mark.parametrize('kind', ['scatter', 'points'])
     def test_logz(self, df, kind, backend):
         plot = df.hvplot('x', 'y', c='x', logz=True, kind=kind)
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['logz'] is True
 
-
     @pytest.mark.parametrize('kind', ['scatter', 'points'])
     def test_color_dim(self, df, kind, backend):
         plot = df.hvplot('x', 'y', c='number', kind=kind)
         opts = Store.lookup_options(backend, plot, 'style')
         assert opts.kwargs['color'] == 'number'
         assert 'number' in plot.vdims
 
@@ -102,18 +113,23 @@
         assert opts.kwargs[param] == 'number'
         assert 'number' in plot.vdims
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ matplotlib')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ plotly')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ matplotlib'),
+            ),
+            pytest.param(
+                'plotly', marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ plotly')
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     @pytest.mark.parametrize('kind', ['scatter', 'points'])
     def test_alpha_dim(self, df, kind, backend):
         plot = df.hvplot('x', 'y', alpha='number', kind=kind)
         opts = Store.lookup_options(backend, plot, 'style')
         assert opts.kwargs['alpha'] == 'number'
         assert 'number' in plot.vdims
@@ -148,17 +164,19 @@
         assert 'number' in plot.last.vdims
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
             'matplotlib',
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ plotly')),
+            pytest.param(
+                'plotly', marks=pytest.mark.xfail(reason='cannot map a dim to alpha w/ plotly')
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     @pytest.mark.parametrize('kind', ['scatter', 'points'])
     def test_alpha_dim_overlay(self, df, kind, backend):
         plot = df.hvplot('x', 'y', alpha='number', by='category', kind=kind)
         opts = Store.lookup_options(backend, plot.last, 'style')
         assert opts.kwargs['alpha'] == 'number'
         assert 'number' in plot.last.vdims
@@ -183,18 +201,23 @@
         assert opts.kwargs['logy'] is False
         assert opts.kwargs.get('logz') is None
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='default opts not supported w/ plotly')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib'),
+            ),
+            pytest.param(
+                'plotly', marks=pytest.mark.xfail(reason='default opts not supported w/ plotly')
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_holoviews_defined_default_opts(self, df, backend):
         hv.opts.defaults(hv.opts.Scatter(height=400, width=900, show_grid=True))
         plot = df.hvplot.scatter('x', 'y', c='category')
         opts = Store.lookup_options(backend, plot, 'plot')
         # legend_position shouldn't apply only to bokeh
         if backend == 'bokeh':
@@ -203,18 +226,23 @@
         assert opts.kwargs['height'] == 400
         assert opts.kwargs['width'] == 900
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='default opts not supported w/ plotly')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib'),
+            ),
+            pytest.param(
+                'plotly', marks=pytest.mark.xfail(reason='default opts not supported w/ plotly')
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_holoviews_defined_default_opts_overwritten_in_call(self, df, backend):
         hv.opts.defaults(hv.opts.Scatter(height=400, width=900, show_grid=True))
         plot = df.hvplot.scatter('x', 'y', c='category', width=300, legend='left')
         opts = Store.lookup_options(backend, plot, 'plot')
         # legend_position shouldn't apply only to bokeh
         if backend == 'bokeh':
@@ -223,18 +251,28 @@
         assert opts.kwargs['height'] == 400
         assert opts.kwargs['width'] == 300
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='default opts not supported not supported w/ matplotlib')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='default opts not supported not supported w/ plotly')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(
+                    reason='default opts not supported not supported w/ matplotlib'
+                ),
+            ),
+            pytest.param(
+                'plotly',
+                marks=pytest.mark.xfail(
+                    reason='default opts not supported not supported w/ plotly'
+                ),
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_holoviews_defined_default_opts_are_not_mutable(self, df, backend):
         hv.opts.defaults(hv.opts.Scatter(tools=['tap']))
         plot = df.hvplot.scatter('x', 'y', c='category')
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['tools'] == ['tap', 'hover']
         default_opts = Store.options(backend=backend)['Scatter'].groups['plot'].options
@@ -287,18 +325,23 @@
         assert opts.kwargs['logy'] is True
         assert opts.kwargs.get('logz') is None
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
-            pytest.param('matplotlib', marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib')),
-            pytest.param('plotly', marks=pytest.mark.xfail(reason='defaykt opts not supported w/ plotly')),
+            pytest.param(
+                'matplotlib',
+                marks=pytest.mark.xfail(reason='default opts not supported w/ matplotlib'),
+            ),
+            pytest.param(
+                'plotly', marks=pytest.mark.xfail(reason='defaykt opts not supported w/ plotly')
+            ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_holoviews_defined_default_opts_logx(self, df, backend):
         hv.opts.defaults(hv.opts.Scatter(logx=True))
         plot = df.hvplot.scatter('x', 'y', c='category')
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['logx'] is True
         assert opts.kwargs['logy'] is False
@@ -310,14 +353,15 @@
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['logx'] is False
         assert opts.kwargs['logy'] is False
         assert opts.kwargs.get('logz') is None
 
     def test_hvplot_default_cat_cmap_opts(self, df, backend):
         import colorcet as cc
+
         plot = df.hvplot.scatter('x', 'y', c='category')
         opts = Store.lookup_options(backend, plot, 'style')
         assert opts.kwargs['cmap'] == cc.palette['glasbey_category10']
 
     def test_hvplot_default_num_cmap_opts(self, df, backend):
         plot = df.hvplot.scatter('x', 'y', c='number')
         opts = Store.lookup_options(backend, plot, 'style')
@@ -348,19 +392,20 @@
         [
             ('aspect', 'bokeh'),
             ('aspect', 'matplotlib'),
             ('aspect', 'plotly'),
             ('data_aspect', 'bokeh'),
             ('data_aspect', 'matplotlib'),
             pytest.param(
-                'data_aspect', 'plotly',
-                marks=pytest.mark.xfail(reason='data_aspect not supported w/ plotly')
+                'data_aspect',
+                'plotly',
+                marks=pytest.mark.xfail(reason='data_aspect not supported w/ plotly'),
             ),
         ],
-        indirect=['backend']
+        indirect=['backend'],
     )
     def test_aspect(self, df, opt, backend):
         plot = df.hvplot(x='x', y='y', **{opt: 2})
         opts = Store.lookup_options(backend, plot, 'plot').kwargs
         assert opts[opt] == 2
         if backend in ['bokeh', 'matplotlib']:
             assert opts.get('width') is None
@@ -373,34 +418,35 @@
         [
             ('aspect', 'bokeh'),
             ('aspect', 'matplotlib'),
             ('aspect', 'plotly'),
             ('data_aspect', 'bokeh'),
             ('data_aspect', 'matplotlib'),
             pytest.param(
-                'data_aspect', 'plotly',
-                marks=pytest.mark.xfail(reason='data_aspect not supported w/ plotly')
+                'data_aspect',
+                'plotly',
+                marks=pytest.mark.xfail(reason='data_aspect not supported w/ plotly'),
             ),
         ],
-        indirect=['backend']
+        indirect=['backend'],
     )
     def test_aspect_and_width(self, df, opt, backend):
         plot = df.hvplot(x='x', y='y', width=150, **{opt: 2})
         opts = hv.Store.lookup_options(backend, plot, 'plot').kwargs
         assert opts[opt] == 2
         if backend in ['bokeh', 'plotly']:
             assert opts.get('width') == 150
             assert opts.get('height') is None
         elif backend == 'matplotlib':
             assert opts.get('fig_size') == pytest.approx(50.0)
 
     def test_symmetric_dataframe(self, backend):
         import pandas as pd
-        df = pd.DataFrame([[1, 2, -1], [3, 4, 0], [5, 6, 1]],
-                          columns=['x', 'y', 'number'])
+
+        df = pd.DataFrame([[1, 2, -1], [3, 4, 0], [5, 6, 1]], columns=['x', 'y', 'number'])
         plot = df.hvplot.scatter('x', 'y', c='number')
         plot_opts = Store.lookup_options(backend, plot, 'plot')
         assert plot_opts.kwargs['symmetric'] is True
         style_opts = Store.lookup_options(backend, plot, 'style')
         assert style_opts.kwargs['cmap'] == 'coolwarm'
 
     def test_symmetric_is_deduced_dataframe(self, symmetric_df, backend):
@@ -421,33 +467,33 @@
         plot = symmetric_df.hvplot.scatter('x', 'y', c='number', symmetric=False)
         plot_opts = Store.lookup_options(backend, plot, 'plot')
         assert plot_opts.kwargs['symmetric'] is False
         style_opts = Store.lookup_options(backend, plot, 'style')
         assert style_opts.kwargs['cmap'] == 'kbc_r'
 
     def test_if_clim_is_set_symmetric_is_not_deduced(self, symmetric_df, backend):
-        plot = symmetric_df.hvplot.scatter('x', 'y', c='number', clim=(-1,1))
+        plot = symmetric_df.hvplot.scatter('x', 'y', c='number', clim=(-1, 1))
         plot_opts = Store.lookup_options(backend, plot, 'plot')
         assert plot_opts.kwargs.get('symmetric') is None
         style_opts = Store.lookup_options(backend, plot, 'style')
         assert style_opts.kwargs['cmap'] == 'kbc_r'
 
     @pytest.mark.parametrize(
         'backend',
         [
             'bokeh',
             'matplotlib',
             pytest.param(
                 'plotly',
                 marks=pytest.mark.xfail(
                     reason='bandwidth, cut, levels not supported w/ plotly for bivariate'
-                )
+                ),
             ),
         ],
-        indirect=True
+        indirect=True,
     )
     def test_bivariate_opts(self, df, backend):
         plot = df.hvplot.bivariate('x', 'y', bandwidth=0.2, cut=1, levels=5, filled=True)
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['bandwidth'] == 0.2
         assert opts.kwargs['cut'] == 1
         assert opts.kwargs['levels'] == 5
@@ -456,14 +502,19 @@
     def test_kde_opts(self, df, backend):
         plot = df.hvplot.kde('x', bandwidth=0.2, cut=1, filled=True)
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['bandwidth'] == 0.2
         assert opts.kwargs['cut'] == 1
         assert opts.kwargs['filled'] is True
 
+    def test_bgcolor(self, df, backend):
+        plot = df.hvplot.scatter('x', 'y', bgcolor='black')
+        opts = Store.lookup_options(backend, plot, 'plot')
+        assert opts.kwargs['bgcolor'] == 'black'
+
 
 @pytest.fixture(scope='module')
 def da():
     return xr.DataArray(
         data=np.arange(16).reshape((2, 2, 2, 2)),
         coords={'time': [0, 1], 'y': [0, 1], 'x': [0, 1], 'band': [0, 1]},
         dims=['time', 'y', 'x', 'band'],
@@ -473,15 +524,15 @@
 
 @pytest.fixture(scope='module')
 def da2():
     return xr.DataArray(
         data=np.arange(27).reshape((3, 3, 3)),
         coords={'y': [0, 1, 2], 'x': [0, 1, 2]},
         dims=['y', 'x', 'other'],
-        name='test2'
+        name='test2',
     )
 
 
 @pytest.fixture(scope='module')
 def ds1(da):
     return xr.Dataset(dict(foo=da))
 
@@ -489,15 +540,14 @@
 @pytest.fixture(scope='module')
 def ds2(da, da2):
     return xr.Dataset(dict(foo=da, bar=da2))
 
 
 @pytest.mark.usefixtures('load_xarray_accessor')
 class TestXarrayTitle:
-
     def test_dataarray_2d_with_title(self, da, backend):
         da_sel = da.sel(time=0, band=0)
         plot = da_sel.hvplot()  # Image plot
         opts = Store.lookup_options(backend, plot, 'plot')
         assert opts.kwargs['title'] == 'time = 0, band = 0'
 
     def test_dataarray_1d_with_title(self, da, backend):
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testoverrides.py` & `hvplot-0.9.3a1/hvplot/tests/testoverrides.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from hvplot.plotting import hvPlot, hvPlotTabular
 from holoviews import Store, Scatter
 from holoviews.element.comparison import ComparisonTestCase
 
 
 class TestOverrides(ComparisonTestCase):
-
     def setUp(self):
         import hvplot.pandas  # noqa
+
         self.df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
 
     def test_define_default_options(self):
         hvplot = hvPlotTabular(self.df, width=42, height=42)
         curve = hvplot(y='y')
         opts = Store.lookup_options('bokeh', curve, 'plot')
         self.assertEqual(opts.options.get('width'), 42)
@@ -50,20 +50,19 @@
 
     def test_pandas_query_metadata(self):
         hvplot = hvPlotTabular(self.df, query='x>2')
         assert len(hvplot._data) == 2
 
 
 class TestXArrayOverrides(ComparisonTestCase):
-
     def setUp(self):
         coords = OrderedDict([('time', [0, 1]), ('lat', [0, 1]), ('lon', [0, 1])])
-        self.da_img_by_time = xr.DataArray(np.arange(8).reshape((2, 2, 2)),
-                                           coords, ['time', 'lat', 'lon']).assign_coords(
-                                               lat1=xr.DataArray([2,3], dims=['lat']))
+        self.da_img_by_time = xr.DataArray(
+            np.arange(8).reshape((2, 2, 2)), coords, ['time', 'lat', 'lon']
+        ).assign_coords(lat1=xr.DataArray([2, 3], dims=['lat']))
 
     def test_xarray_isel_scalar_metadata(self):
         hvplot = hvPlot(self.da_img_by_time, isel={'time': 1})
         assert hvplot._data.ndim == 2
 
     def test_xarray_isel_nonscalar_metadata(self):
         hvplot = hvPlot(self.da_img_by_time, isel={'time': [1]})
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testpanel.py` & `hvplot-0.9.3a1/hvplot/tests/testpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """
 Tests for panel widgets and param objects as arguments
 """
+
 from unittest import TestCase, SkipTest
 
 from hvplot.util import process_xarray  # noqa
 
+
 def look_for_class(panel, classname, items=None):
     """
     Descend a panel object and find any instances of the given class
     """
     import panel as pn
 
     if items is None:
@@ -18,27 +20,26 @@
             items = look_for_class(p, classname, items)
     elif isinstance(panel, classname):
         items.append(panel)
     return items
 
 
 class TestPanelObjects(TestCase):
-
     def setUp(self):
         try:
             import panel as pn  # noqa
             import hvplot.pandas  # noqa
-        except:
+        except ImportError:
             raise SkipTest('panel not available')
 
         from bokeh.sampledata.iris import flowers
+
         self.flowers = flowers
         self.cols = list(self.flowers.columns[:-1])
 
-
     def test_using_explicit_widgets_works(self):
         import panel as pn
 
         x = pn.widgets.Select(name='x', value='sepal_length', options=self.cols)
         y = pn.widgets.Select(name='y', value='sepal_width', options=self.cols)
         kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
         by_species = pn.widgets.Checkbox(name='By species')
@@ -50,16 +51,16 @@
 
         self.flowers.hvplot(x, y=y, kind=kind.param.value, c=color)
 
     def test_casting_widgets_to_different_classes(self):
         import panel as pn
 
         pane = self.flowers.hvplot.scatter(
-            groupby='species', legend='top_right',
-            widgets={'species': pn.widgets.DiscreteSlider})
+            groupby='species', legend='top_right', widgets={'species': pn.widgets.DiscreteSlider}
+        )
 
         assert len(look_for_class(pane, pn.widgets.DiscreteSlider)) == 1
 
     def test_using_explicit_widgets_with_groupby_does_not_raise_error(self):
         import panel as pn
 
         x = pn.widgets.Select(name='x', value='sepal_length', options=self.cols)
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testpatch.py` & `hvplot-0.9.3a1/hvplot/tests/testpatch.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,122 +6,130 @@
 
 import numpy as np
 
 from hvplot.plotting import hvPlotTabular, hvPlot
 
 
 class TestPatchPandas(TestCase):
-
     def setUp(self):
-        import hvplot.pandas   # noqa
+        import hvplot.pandas  # noqa
 
     def test_pandas_series_patched(self):
         import pandas as pd
+
         series = pd.Series([0, 1, 2])
         self.assertIsInstance(series.hvplot, hvPlotTabular)
 
     def test_pandas_dataframe_patched(self):
         import pandas as pd
+
         df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
         self.assertIsInstance(df.hvplot, hvPlotTabular)
 
 
 class TestPatchDask(TestCase):
-
     def setUp(self):
         try:
-            import dask.dataframe as dd # noqa
-        except:
+            import dask.dataframe as dd  # noqa
+        except ImportError:
             raise SkipTest('Dask not available')
-        import hvplot.dask   # noqa
+        import hvplot.dask  # noqa
 
     def test_dask_series_patched(self):
         import pandas as pd
         import dask.dataframe as dd
+
         series = pd.Series([0, 1, 2])
         dseries = dd.from_pandas(series, 2)
         self.assertIsInstance(dseries.hvplot, hvPlotTabular)
 
     def test_dask_dataframe_patched(self):
         import pandas as pd
         import dask.dataframe as dd
+
         df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
         ddf = dd.from_pandas(df, 2)
         self.assertIsInstance(ddf.hvplot, hvPlotTabular)
 
 
 class TestPatchXArray(TestCase):
-
     def setUp(self):
         try:
-            import xarray as xr # noqa
-        except:
+            import xarray as xr  # noqa
+        except ImportError:
             raise SkipTest('XArray not available')
-        import hvplot.xarray # noqa
+        import hvplot.xarray  # noqa
 
     def test_xarray_dataarray_patched(self):
         import xarray as xr
+
         array = np.random.rand(100, 100)
         xr_array = xr.DataArray(array, coords={'x': range(100), 'y': range(100)}, dims=('y', 'x'))
         self.assertIsInstance(xr_array.hvplot, hvPlot)
 
     def test_xarray_dataset_patched(self):
         import xarray as xr
+
         array = np.random.rand(100, 100)
         xr_array = xr.DataArray(array, coords={'x': range(100), 'y': range(100)}, dims=('y', 'x'))
         xr_ds = xr.Dataset({'z': xr_array})
         self.assertIsInstance(xr_ds.hvplot, hvPlot)
 
 
 class TestPatchStreamz(TestCase):
-
     def setUp(self):
         try:
-            import streamz # noqa
-        except:
+            import streamz  # noqa
+        except ImportError:
             raise SkipTest('streamz not available')
-        import hvplot.streamz   # noqa
+        import hvplot.streamz  # noqa
 
     def test_streamz_dataframe_patched(self):
         from streamz.dataframe import Random
+
         random_df = Random()
         self.assertIsInstance(random_df.hvplot, hvPlotTabular)
 
     def test_streamz_series_patched(self):
         from streamz.dataframe import Random
+
         random_df = Random()
         self.assertIsInstance(random_df.x.hvplot, hvPlotTabular)
 
     def test_streamz_dataframes_patched(self):
         from streamz.dataframe import Random
+
         random_df = Random()
         self.assertIsInstance(random_df.groupby('x').sum().hvplot, hvPlotTabular)
 
     def test_streamz_seriess_patched(self):
         from streamz.dataframe import Random
+
         random_df = Random()
         self.assertIsInstance(random_df.groupby('x').sum().y.hvplot, hvPlotTabular)
 
 
 class TestPatchPolars(TestCase):
-
     def setUp(self):
         try:
-            import polars as pl # noqa
-        except:
+            import polars as pl  # noqa
+        except ImportError:
             raise SkipTest('Polars not available')
-        import hvplot.polars   # noqa
+        import hvplot.polars  # noqa
 
     def test_polars_series_patched(self):
         import polars as pl
+
         pseries = pl.Series([0, 1, 2])
         self.assertIsInstance(pseries.hvplot, hvPlotTabular)
 
     def test_polars_dataframe_patched(self):
         import polars as pl
+
         pdf = pl.DataFrame({'x': [1, 3, 5], 'y': [2, 4, 6]})
         self.assertIsInstance(pdf.hvplot, hvPlotTabular)
 
     def test_polars_lazyframe_patched(self):
         import polars as pl
+
         pldf = pl.LazyFrame({'x': [1, 3, 5], 'y': [2, 4, 6]})
         self.assertIsInstance(pldf.hvplot, hvPlotTabular)
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testplotting.py` & `hvplot-0.9.3a1/hvplot/tests/testplotting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Tests pandas.options.backend setting
 """
+
 from unittest import TestCase, SkipTest
 
 import holoviews as hv
 import pandas as pd
 import pytest
 
 from packaging.version import Version
@@ -13,26 +14,24 @@
 from hvplot.converter import HoloViewsConverter
 from hvplot.plotting import plot
 from hvplot.tests.util import makeDataFrame
 
 no_args = ['line', 'area', 'hist', 'box', 'kde', 'density', 'bar', 'barh']
 x_y = ['scatter', 'hexbin']
 
-no_args_mapping = [(kind, el) for kind, el in HoloViewsConverter._kind_mapping.items()
-                   if kind in no_args]
-x_y_mapping = [(kind, el) for kind, el in HoloViewsConverter._kind_mapping.items()
-               if kind in x_y]
+no_args_mapping = [
+    (kind, el) for kind, el in HoloViewsConverter._kind_mapping.items() if kind in no_args
+]
+x_y_mapping = [(kind, el) for kind, el in HoloViewsConverter._kind_mapping.items() if kind in x_y]
 
 
 class TestPandasHoloviewsPlotting(TestCase):
-
     def setUp(self):
         if Version(pd.__version__) < Version('0.25.1'):
-            raise SkipTest('entrypoints for plotting.backends was added '
-                           'in pandas 0.25.1')
+            raise SkipTest('entrypoints for plotting.backends was added in pandas 0.25.1')
         pd.options.plotting.backend = 'holoviews'
 
     @parameterized.expand(no_args_mapping)
     def test_pandas_series_plot_returns_holoviews_object(self, kind, el):
         series = pd.Series([0, 1, 2])
         plot = getattr(series.plot, kind)()
         self.assertIsInstance(plot, el)
@@ -47,26 +46,24 @@
     def test_pandas_dataframe_plot_returns_holoviews_object_when_x_and_y_set(self, kind, el):
         df = pd.DataFrame({'a': [0, 1, 2], 'b': [5, 7, 2]})
         plot = getattr(df.plot, kind)(x='a', y='b')
         self.assertIsInstance(plot, el)
 
     def test_pandas_dataframe_plot_does_not_implement_pie(self):
         df = pd.DataFrame({'a': [0, 1, 2], 'b': [5, 7, 2]})
-        with self.assertRaisesRegex(NotImplementedError, "pie"):
+        with self.assertRaisesRegex(NotImplementedError, 'pie'):
             df.plot.pie(y='a')
 
 
 class TestPandasHvplotPlotting(TestPandasHoloviewsPlotting):
-
     def setUp(self):
         if Version(pd.__version__) < Version('0.25.1'):
-            raise SkipTest('entrypoints for plotting.backends was added '
-                           'in pandas 0.25.1')
+            raise SkipTest('entrypoints for plotting.backends was added in pandas 0.25.1')
         pd.options.plotting.backend = 'hvplot'
 
 
 def test_plot_supports_polars():
-    pl = pytest.importorskip("polars")
+    pl = pytest.importorskip('polars')
     dfp = pl.DataFrame(makeDataFrame())
     out = plot(dfp, 'line')
     assert isinstance(out, hv.NdOverlay)
     assert out.keys() == dfp.columns
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/teststreaming.py` & `hvplot-0.9.3a1/hvplot/tests/teststreaming.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import pandas as pd
 
 from holoviews.streams import Buffer, Pipe
 
 
 class TestExplicitStreamPlotting(TestCase):
-
     def setUp(self):
-        import hvplot.pandas   # noqa
+        import hvplot.pandas  # noqa
+
         self.df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], columns=['x', 'y'])
 
     def test_pipe_stream(self):
         stream = Pipe(data=self.df)
         plot = self.df.hvplot('x', 'y', stream=stream)
         pd.testing.assert_frame_equal(plot[()].data, self.df)
         new_df = pd.DataFrame([[7, 8], [9, 10]], columns=['x', 'y'])
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testtransforms.py` & `hvplot-0.9.3a1/hvplot/tests/testtransforms.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,41 +4,36 @@
 import numpy as np
 import pandas as pd
 
 from holoviews.element.comparison import ComparisonTestCase
 
 
 class TestPandasTransforms(ComparisonTestCase):
-
     def setUp(self):
-        import hvplot.pandas # noqa
+        import hvplot.pandas  # noqa
 
     def test_pandas_transform(self):
-        demo_df = pd.DataFrame({'value':np.random.randn(50), 'probability':np.random.rand(50)})
-        percent = hv.dim('probability')*100
+        demo_df = pd.DataFrame({'value': np.random.randn(50), 'probability': np.random.rand(50)})
+        percent = hv.dim('probability') * 100
         scatter = demo_df.hvplot.scatter(
             x='value', y='probability', transforms=dict(probability=percent)
         )
-        self.assertEqual((scatter.data['probability']).values,
-                         demo_df['probability'].values*100)
+        self.assertEqual((scatter.data['probability']).values, demo_df['probability'].values * 100)
 
 
 class TestXArrayTransforms(ComparisonTestCase):
-
     def setUp(self):
-
         try:
-            import xarray as xr # noqa
-        except:
+            import xarray as xr  # noqa
+        except ImportError:
             raise SkipTest('xarray not available')
-        import hvplot.xarray # noqa
+        import hvplot.xarray  # noqa
 
     def test_xarray_transform(self):
         import xarray as xr
+
         data = np.arange(0, 60).reshape(6, 10)
         x = np.arange(10)
         y = np.arange(6)
         da = xr.DataArray(data, coords={'y': y, 'x': x}, dims=('y', 'x'), name='value')
-        img = da.hvplot.image(
-            transforms=dict(value=hv.dim('value')*10)
-        )
-        self.assertEqual(img.data.value.data, da.data*10)
+        img = da.hvplot.image(transforms=dict(value=hv.dim('value') * 10))
+        self.assertEqual(img.data.value.data, da.data * 10)
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testui.py` & `hvplot-0.9.3a1/hvplot/tests/testui.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 ds_air_temperature = xr.tutorial.open_dataset('air_temperature')
 
 
 def test_explorer_basic():
     explorer = hvplot.explorer(df)
 
     assert isinstance(explorer, hvDataFrameExplorer)
-    assert explorer.kind == "scatter"
-    assert explorer.x == "index"
-    assert explorer.y == "species"
+    assert explorer.kind == 'scatter'
+    assert explorer.x == 'index'
+    assert explorer.y == 'species'
 
 
 def test_explorer_settings():
     explorer = hvplot.explorer(df)
 
     explorer.param.update(
         kind='scatter',
@@ -34,18 +34,18 @@
         y_multi=['bill_depth_mm'],
         by=['species'],
     )
 
     settings = explorer.settings()
 
     assert settings == dict(
-        by=["species"],
-        kind="scatter",
-        x="bill_length_mm",
-        y=["bill_depth_mm"],
+        by=['species'],
+        kind='scatter',
+        x='bill_length_mm',
+        y=['bill_depth_mm'],
     )
 
 
 def test_explorer_plot_code():
     explorer = hvplot.explorer(df)
 
     explorer.param.update(
@@ -53,40 +53,36 @@
         x='bill_length_mm',
         y_multi=['bill_depth_mm'],
         by=['species'],
     )
 
     hvplot_code = explorer.plot_code()
 
-    assert (
-        hvplot_code == (
-            "df.hvplot(\n"
-            "    by=['species'],\n"
-            "    kind='scatter',\n"
-            "    x='bill_length_mm',\n"
-            "    y=['bill_depth_mm'],\n"
-            "    legend='bottom_right',\n"
-            "    widget_location='bottom',\n"
-            ")"
-        )
-    )
-
-    hvplot_code = explorer.plot_code(var_name="othername")
-
-    assert (
-        hvplot_code == (
-            "othername.hvplot(\n"
-            "    by=['species'],\n"
-            "    kind='scatter',\n"
-            "    x='bill_length_mm',\n"
-            "    y=['bill_depth_mm'],\n"
-            "    legend='bottom_right',\n"
-            "    widget_location='bottom',\n"
-            ")"
-        )
+    assert hvplot_code == (
+        'df.hvplot(\n'
+        "    by=['species'],\n"
+        "    kind='scatter',\n"
+        "    x='bill_length_mm',\n"
+        "    y=['bill_depth_mm'],\n"
+        "    legend='bottom_right',\n"
+        "    widget_location='bottom',\n"
+        ')'
+    )
+
+    hvplot_code = explorer.plot_code(var_name='othername')
+
+    assert hvplot_code == (
+        'othername.hvplot(\n'
+        "    by=['species'],\n"
+        "    kind='scatter',\n"
+        "    x='bill_length_mm',\n"
+        "    y=['bill_depth_mm'],\n"
+        "    legend='bottom_right',\n"
+        "    widget_location='bottom',\n"
+        ')'
     )
 
 
 def test_explorer_hvplot():
     explorer = hvplot.explorer(df)
 
     explorer.param.update(
@@ -94,38 +90,38 @@
         x='bill_length_mm',
         y_multi=['bill_depth_mm'],
     )
 
     plot = explorer.hvplot()
 
     assert isinstance(plot, hv.Scatter)
-    assert plot.kdims[0].name == "bill_length_mm"
-    assert plot.vdims[0].name == "bill_depth_mm"
+    assert plot.kdims[0].name == 'bill_length_mm'
+    assert plot.vdims[0].name == 'bill_depth_mm'
 
 
 def test_explorer_save(tmp_path):
     explorer = hvplot.explorer(df)
 
     explorer.param.update(
         kind='scatter',
         x='bill_length_mm',
         y_multi=['bill_depth_mm'],
     )
 
-    outfile = tmp_path / "plot.html"
+    outfile = tmp_path / 'plot.html'
 
     explorer.save(outfile)
 
     assert outfile.exists()
 
 
 def test_explorer_kwargs_controls():
-    explorer = hvplot.explorer(df, title="Dummy title", width=200)
+    explorer = hvplot.explorer(df, title='Dummy title', width=200)
 
-    assert explorer.labels.title == "Dummy title"
+    assert explorer.labels.title == 'Dummy title'
     assert explorer.axes.width == 200
 
 
 def test_explorer_kwargs_controls_error_not_supported():
     with pytest.raises(
         TypeError,
         match=re.escape(
@@ -244,33 +240,33 @@
     assert isinstance(explorer, hvGridExplorer)
     assert explorer.kind == 'image'
     assert explorer.x == 'lat'
     assert explorer.y == 'lon'
 
 
 def test_explorer_method_kind():
-    explorer = df.hvplot.explorer(kind="scatter")
+    explorer = df.hvplot.explorer(kind='scatter')
 
     assert isinstance(explorer, hvDataFrameExplorer)
     assert explorer.kind == 'scatter'
     assert explorer.x == 'index'
     assert explorer.y == 'species'
 
 
 def test_explorer_method_as_kind():
-    explorer = df.hvplot(kind="explorer")
+    explorer = df.hvplot(kind='explorer')
 
     assert isinstance(explorer, hvDataFrameExplorer)
     assert explorer.kind == 'scatter'
     assert explorer.x == 'index'
     assert explorer.y == 'species'
 
 
 def test_explorer_method_propagates_kwargs():
-    explorer = df.hvplot.explorer(title="Dummy title", x="bill_length_mm")
+    explorer = df.hvplot.explorer(title='Dummy title', x='bill_length_mm')
 
     assert isinstance(explorer, hvDataFrameExplorer)
     assert explorer.kind == 'scatter'
     assert explorer.x == 'bill_length_mm'
     assert explorer.y == 'species'
     assert explorer.labels.title == 'Dummy title'
 
@@ -280,27 +276,25 @@
     assert explorer.code == dedent("""\
         df.hvplot(
             kind='points',
             x='bill_length_mm',
             y='species',
             legend='bottom_right',
             widget_location='bottom',
-        )"""
-    )
+        )""")
     assert explorer._code_pane.object == dedent("""\
         ```python
         df.hvplot(
             kind='points',
             x='bill_length_mm',
             y='species',
             legend='bottom_right',
             widget_location='bottom',
         )
-        ```"""
-    )
+        ```""")
 
 
 def test_explorer_code_gridded():
     explorer = hvplot.explorer(ds_air_temperature, x='lon', y='lat', kind='image')
     code = explorer.code
     assert code == dedent("""\
         ds['air'].hvplot(
@@ -320,16 +314,15 @@
             groupby=['time'],
             kind='image',
             x='lon',
             y='lat',
             legend='bottom_right',
             widget_location='bottom',
         )
-        ```"""
-    )
+        ```""")
 
 
 def test_explorer_code_gridded_dataarray():
     da = ds_air_temperature['air']
     explorer = hvplot.explorer(da, x='lon', y='lat', kind='image')
     code = explorer.code
     assert code == dedent("""\
@@ -350,16 +343,15 @@
             groupby=['time'],
             kind='image',
             x='lon',
             y='lat',
             legend='bottom_right',
             widget_location='bottom',
         )
-        ```"""
-    )
+        ```""")
 
 
 def test_explorer_code_opts():
     da = ds_air_temperature['air']
     explorer = hvplot.explorer(da, x='lon', y='lat', kind='image', opts={'color_levels': 3})
     code = explorer.code
     assert code == dedent("""\
@@ -384,9 +376,8 @@
             x='lon',
             y='lat',
             legend='bottom_right',
             widget_location='bottom',
         ).opts(
             color_levels=3,
         )
-        ```"""
-    )
+        ```""")
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/testutil.py` & `hvplot-0.9.3a1/hvplot/tests/testutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Tests  utilities to convert data and projections
 """
+
 import numpy as np
 import pandas as pd
 import pytest
 
 from unittest import TestCase, SkipTest
 
 from hvplot.util import (
-    check_crs, is_list_like, process_crs, process_xarray,
-    _convert_col_names_to_str, instantiate_crs_str
+    check_crs,
+    is_list_like,
+    process_crs,
+    process_xarray,
+    _convert_col_names_to_str,
+    instantiate_crs_str,
 )
 
 
 class TestProcessXarray(TestCase):
-
     def setUp(self):
         try:
             import xarray as xr
             import pandas as pd  # noqa
-        except:
+        except ImportError:
             raise SkipTest('xarray or pandas not available')
         self.default_kwargs = {
             'value_label': 'value',
             'label': None,
             'gridded': False,
             'persist': False,
             'use_dask': False,
@@ -35,74 +39,66 @@
         }
         self.ds = xr.tutorial.open_dataset('air_temperature')
 
     def test_process_1d_xarray_dataarray_with_no_coords(self):
         import xarray as xr
         import pandas as pd
 
-        da = xr.DataArray(
-            data=[1, 2, 3])
+        da = xr.DataArray(data=[1, 2, 3])
 
         data, x, y, by, groupby = process_xarray(data=da, **self.default_kwargs)
         assert isinstance(data, pd.DataFrame)
         assert x == 'index'
         assert y == ['value']
         assert not by
         assert not groupby
 
     def test_process_1d_xarray_dataarray_with_coords(self):
         import xarray as xr
         import pandas as pd
 
-        da = xr.DataArray(
-            data=[1, 2, 3],
-            coords={'day': [5, 6, 7]},
-            dims=['day'])
+        da = xr.DataArray(data=[1, 2, 3], coords={'day': [5, 6, 7]}, dims=['day'])
 
         data, x, y, by, groupby = process_xarray(data=da, **self.default_kwargs)
         assert isinstance(data, pd.DataFrame)
         assert x == 'day'
         assert y == ['value']
         assert not by
         assert not groupby
 
     def test_process_1d_xarray_dataarray_with_coords_and_name(self):
         import xarray as xr
         import pandas as pd
 
-        da = xr.DataArray(
-            data=[1, 2, 3],
-            coords={'day': [5, 6, 7]},
-            dims=['day'],
-            name='temp')
+        da = xr.DataArray(data=[1, 2, 3], coords={'day': [5, 6, 7]}, dims=['day'], name='temp')
 
         data, x, y, by, groupby = process_xarray(data=da, **self.default_kwargs)
         assert isinstance(data, pd.DataFrame)
         assert x == 'day'
         assert y == ['temp']
         assert not by
         assert not groupby
 
     def test_process_2d_xarray_dataarray_with_no_coords(self):
         import xarray as xr
         import pandas as pd
 
-        da = xr.DataArray(np.random.randn(4,5))
+        da = xr.DataArray(np.random.randn(4, 5))
 
         data, x, y, by, groupby = process_xarray(data=da, **self.default_kwargs)
         assert isinstance(data, pd.DataFrame)
         assert x == 'index'
         assert y == ['value']
         assert not by
         assert not groupby
 
     def test_process_2d_xarray_dataarray_with_no_coords_as_gridded(self):
         import xarray as xr
 
-        da = xr.DataArray(np.random.randn(4,5))
+        da = xr.DataArray(np.random.randn(4, 5))
 
         kwargs = self.default_kwargs
         kwargs.update(gridded=True)
 
         data, x, y, by, groupby = process_xarray(data=da, **kwargs)
         assert isinstance(data, xr.Dataset)
         assert list(data.data_vars.keys()) == ['value']
@@ -111,17 +107,16 @@
         assert not by
         assert not groupby
 
     def test_process_2d_xarray_dataarray_with_coords_as_gridded(self):
         import xarray as xr
 
         da = xr.DataArray(
-            data=np.random.randn(4,5),
-            coords={'y': [3, 4, 5, 6, 7]},
-            dims=['x', 'y'])
+            data=np.random.randn(4, 5), coords={'y': [3, 4, 5, 6, 7]}, dims=['x', 'y']
+        )
 
         kwargs = self.default_kwargs
         kwargs.update(gridded=True)
 
         data, x, y, by, groupby = process_xarray(data=da, **kwargs)
         assert isinstance(data, xr.Dataset)
         assert list(data.data_vars.keys()) == ['value']
@@ -194,27 +189,28 @@
         assert x == 'time.dayofyear'
         assert y == 'air'
         assert not by
         assert not groupby
 
 
 class TestDynamicArgs(TestCase):
-
     def setUp(self):
         try:
             import panel as pn  # noqa
-        except:
+        except ImportError:
             raise SkipTest('panel not available')
 
     def test_dynamic_and_static(self):
         import panel as pn
         from ..util import process_dynamic_args
 
         x = 'sepal_width'
-        y = pn.widgets.Select(name='y', value='sepal_length', options=['sepal_length', 'petal_length'])
+        y = pn.widgets.Select(
+            name='y', value='sepal_length', options=['sepal_length', 'petal_length']
+        )
         kind = pn.widgets.Select(name='kind', value='scatter', options=['bivariate', 'scatter'])
 
         dynamic, arg_deps, arg_names = process_dynamic_args(x, y, kind)
         assert 'x' not in dynamic
         assert 'y' in dynamic
         assert arg_deps == []
 
@@ -249,90 +245,102 @@
         dynamic, arg_deps, arg_names = process_dynamic_args(x, y, kind, c=by_species_fn)
         assert dynamic == {}
         assert arg_names == ['c', 'c']
         assert len(arg_deps) == 2
 
 
 def test_check_crs():
-    pytest.importorskip("pyproj")
+    pytest.importorskip('pyproj')
     p = check_crs('epsg:26915 +units=m')
     assert p.srs == '+proj=utm +zone=15 +datum=NAD83 +units=m +no_defs'
     p = check_crs('wrong')
     assert p is None
 
 
-@pytest.mark.parametrize("input", [
-    "+init=epsg:26911",
-])
+@pytest.mark.parametrize(
+    'input',
+    [
+        '+init=epsg:26911',
+    ],
+)
 def test_process_crs(input):
-    pytest.importorskip("pyproj")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pytest.importorskip('pyproj')
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = process_crs(input)
     assert isinstance(crs, ccrs.CRS)
 
 
 def test_process_crs_pyproj_crs():
-    pyproj = pytest.importorskip("pyproj")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pyproj = pytest.importorskip('pyproj')
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = process_crs(pyproj.CRS.from_epsg(4326))
     assert isinstance(crs, ccrs.PlateCarree)
 
 
 def test_process_crs_pyproj_proj():
-    pyproj = pytest.importorskip("pyproj")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pyproj = pytest.importorskip('pyproj')
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = process_crs(pyproj.Proj(init='epsg:4326'))
     assert isinstance(crs, ccrs.PlateCarree)
 
 
-@pytest.mark.parametrize("input", [
-    "4326",
-    4326,
-    "epsg:4326",
-    "EPSG: 4326",
-    "+init=epsg:4326",
-    # Created with pyproj.CRS("EPSG:4326").to_wkt()
-    'GEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],MEMBER["World Geodetic System 1984 (G2139)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],CS[ellipsoidal,2],AXIS["geodetic latitude (Lat)",north,ORDER[1],ANGLEUNIT["degree",0.0174532925199433]],AXIS["geodetic longitude (Lon)",east,ORDER[2],ANGLEUNIT["degree",0.0174532925199433]],USAGE[SCOPE["Horizontal component of 3D system."],AREA["World."],BBOX[-90,-180,90,180]],ID["EPSG",4326]]',
-], ids=lambda x: str(x)[:20])
+@pytest.mark.parametrize(
+    'input',
+    [
+        '4326',
+        4326,
+        'epsg:4326',
+        'EPSG: 4326',
+        '+init=epsg:4326',
+        # Created with pyproj.CRS("EPSG:4326").to_wkt()
+        'GEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],MEMBER["World Geodetic System 1984 (G2139)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],CS[ellipsoidal,2],AXIS["geodetic latitude (Lat)",north,ORDER[1],ANGLEUNIT["degree",0.0174532925199433]],AXIS["geodetic longitude (Lon)",east,ORDER[2],ANGLEUNIT["degree",0.0174532925199433]],USAGE[SCOPE["Horizontal component of 3D system."],AREA["World."],BBOX[-90,-180,90,180]],ID["EPSG",4326]]',
+    ],
+    ids=lambda x: str(x)[:20],
+)
 def test_process_crs_platecarree(input):
-    pytest.importorskip("pyproj")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pytest.importorskip('pyproj')
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = process_crs(input)
     assert isinstance(crs, ccrs.PlateCarree)
 
 
-@pytest.mark.parametrize("input", [
-    "3857",
-    3857,
-    "epsg:3857",
-    "EPSG: 3857",
-    "+init=epsg:3857",
-    'PROJCS["WGS 84 / Pseudo-Mercator",GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0,AUTHORITY["EPSG","8901"]],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]],PROJECTION["Mercator_1SP"],PARAMETER["central_meridian",0],PARAMETER["scale_factor",1],PARAMETER["false_easting",0],PARAMETER["false_northing",0],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["Easting",EAST],AXIS["Northing",NORTH],EXTENSION["PROJ4","+proj=merc +a=6378137 +b=6378137 +lat_ts=0 +lon_0=0 +x_0=0 +y_0=0 +k=1 +units=m +nadgrids=@null +wktext +no_defs"],AUTHORITY["EPSG","3857"]]',
-    # Created with pyproj.CRS("EPSG:3857").to_wkt()
-    'PROJCRS["WGS 84 / Pseudo-Mercator",BASEGEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],MEMBER["World Geodetic System 1984 (G2139)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],ID["EPSG",4326]],CONVERSION["Popular Visualisation Pseudo-Mercator",METHOD["Popular Visualisation Pseudo Mercator",ID["EPSG",1024]],PARAMETER["Latitude of natural origin",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8801]],PARAMETER["Longitude of natural origin",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8802]],PARAMETER["False easting",0,LENGTHUNIT["metre",1],ID["EPSG",8806]],PARAMETER["False northing",0,LENGTHUNIT["metre",1],ID["EPSG",8807]]],CS[Cartesian,2],AXIS["easting (X)",east,ORDER[1],LENGTHUNIT["metre",1]],AXIS["northing (Y)",north,ORDER[2],LENGTHUNIT["metre",1]],USAGE[SCOPE["Web mapping and visualisation."],AREA["World between 85.06°S and 85.06°N."],BBOX[-85.06,-180,85.06,180]],ID["EPSG",3857]]',
-], ids=lambda x: str(x)[:20])
+@pytest.mark.parametrize(
+    'input',
+    [
+        '3857',
+        3857,
+        'epsg:3857',
+        'EPSG: 3857',
+        '+init=epsg:3857',
+        'PROJCS["WGS 84 / Pseudo-Mercator",GEOGCS["WGS 84",DATUM["WGS_1984",SPHEROID["WGS 84",6378137,298.257223563,AUTHORITY["EPSG","7030"]],AUTHORITY["EPSG","6326"]],PRIMEM["Greenwich",0,AUTHORITY["EPSG","8901"]],UNIT["degree",0.0174532925199433,AUTHORITY["EPSG","9122"]],AUTHORITY["EPSG","4326"]],PROJECTION["Mercator_1SP"],PARAMETER["central_meridian",0],PARAMETER["scale_factor",1],PARAMETER["false_easting",0],PARAMETER["false_northing",0],UNIT["metre",1,AUTHORITY["EPSG","9001"]],AXIS["Easting",EAST],AXIS["Northing",NORTH],EXTENSION["PROJ4","+proj=merc +a=6378137 +b=6378137 +lat_ts=0 +lon_0=0 +x_0=0 +y_0=0 +k=1 +units=m +nadgrids=@null +wktext +no_defs"],AUTHORITY["EPSG","3857"]]',
+        # Created with pyproj.CRS("EPSG:3857").to_wkt()
+        'PROJCRS["WGS 84 / Pseudo-Mercator",BASEGEOGCRS["WGS 84",ENSEMBLE["World Geodetic System 1984 ensemble",MEMBER["World Geodetic System 1984 (Transit)"],MEMBER["World Geodetic System 1984 (G730)"],MEMBER["World Geodetic System 1984 (G873)"],MEMBER["World Geodetic System 1984 (G1150)"],MEMBER["World Geodetic System 1984 (G1674)"],MEMBER["World Geodetic System 1984 (G1762)"],MEMBER["World Geodetic System 1984 (G2139)"],ELLIPSOID["WGS 84",6378137,298.257223563,LENGTHUNIT["metre",1]],ENSEMBLEACCURACY[2.0]],PRIMEM["Greenwich",0,ANGLEUNIT["degree",0.0174532925199433]],ID["EPSG",4326]],CONVERSION["Popular Visualisation Pseudo-Mercator",METHOD["Popular Visualisation Pseudo Mercator",ID["EPSG",1024]],PARAMETER["Latitude of natural origin",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8801]],PARAMETER["Longitude of natural origin",0,ANGLEUNIT["degree",0.0174532925199433],ID["EPSG",8802]],PARAMETER["False easting",0,LENGTHUNIT["metre",1],ID["EPSG",8806]],PARAMETER["False northing",0,LENGTHUNIT["metre",1],ID["EPSG",8807]]],CS[Cartesian,2],AXIS["easting (X)",east,ORDER[1],LENGTHUNIT["metre",1]],AXIS["northing (Y)",north,ORDER[2],LENGTHUNIT["metre",1]],USAGE[SCOPE["Web mapping and visualisation."],AREA["World between 85.06°S and 85.06°N."],BBOX[-85.06,-180,85.06,180]],ID["EPSG",3857]]',
+    ],
+    ids=lambda x: str(x)[:20],
+)
 def test_process_crs_mercator(input):
-    pytest.importorskip("pyproj")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pytest.importorskip('pyproj')
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = process_crs(input)
     assert isinstance(crs, ccrs.Mercator)
 
 
 def test_process_crs_rasterio():
-    pytest.importorskip("pyproj")
-    rcrs = pytest.importorskip("rasterio.crs")
-    ccrs = pytest.importorskip("cartopy.crs")
+    pytest.importorskip('pyproj')
+    rcrs = pytest.importorskip('rasterio.crs')
+    ccrs = pytest.importorskip('cartopy.crs')
     input = rcrs.CRS.from_epsg(4326).to_wkt()
     crs = process_crs(input)
     assert isinstance(crs, ccrs.CRS)
 
+
 def test_process_crs_raises_error():
-    pytest.importorskip("pyproj")
-    pytest.importorskip("cartopy.crs")
-    with pytest.raises(ValueError, match="must be defined as a EPSG code, proj4 string"):
+    pytest.importorskip('pyproj')
+    pytest.importorskip('cartopy.crs')
+    with pytest.raises(ValueError, match='must be defined as a EPSG code, proj4 string'):
         process_crs(43823)
 
 
 def test_is_list_like():
     assert not is_list_like(0)
     assert not is_list_like('string')
     assert not is_list_like(np.array('a'))
@@ -348,23 +356,23 @@
     df = pd.DataFrame(np.random.random((10, 2)))
     assert all(not isinstance(col, str) for col in df.columns)
     df = _convert_col_names_to_str(df)
     assert all(isinstance(col, str) for col in df.columns)
 
 
 def test_instantiate_crs_str():
-    ccrs = pytest.importorskip("cartopy.crs")
+    ccrs = pytest.importorskip('cartopy.crs')
     assert isinstance(instantiate_crs_str('PlateCarree'), ccrs.PlateCarree)
 
 
 def test_instantiate_crs_google_mercator():
-    ccrs = pytest.importorskip("cartopy.crs")
+    ccrs = pytest.importorskip('cartopy.crs')
     assert instantiate_crs_str('GOOGLE_MERCATOR') == ccrs.GOOGLE_MERCATOR
     assert instantiate_crs_str('google_mercator') == ccrs.GOOGLE_MERCATOR
 
 
 def test_instantiate_crs_str_kwargs():
-    ccrs = pytest.importorskip("cartopy.crs")
+    ccrs = pytest.importorskip('cartopy.crs')
     crs = instantiate_crs_str('PlateCarree', globe=ccrs.Globe(datum='WGS84'))
     assert isinstance(crs, ccrs.PlateCarree)
     assert isinstance(crs.globe, ccrs.Globe)
     assert crs.globe.datum == 'WGS84'
```

### Comparing `hvplot-0.9.2rc1/hvplot/tests/util.py` & `hvplot-0.9.3a1/hvplot/tests/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 
 
 # Pandas removed its make<> test utilities in version 2.2.0.
 
 _N = 30
 _K = 4
 
+
 def getCols(k):
     return string.ascii_uppercase[:k]
 
 
-def rands_array(
-    nchars, size, dtype="O", replace=True
-):
+def rands_array(nchars, size, dtype='O', replace=True):
     """
     Generate an array of byte strings.
     """
     chars = np.array(list(string.ascii_letters + string.digits), dtype=(np.str_, 1))
     retval = (
         np.random.default_rng(2)
         .choice(chars, size=nchars * np.prod(size), replace=replace)
@@ -33,18 +32,18 @@
 
 def makeStringIndex(k=10, name=None):
     return pd.Index(rands_array(nchars=10, size=k), name=name)
 
 
 def makeMixedDataFrame():
     data = {
-        "A": [0.0, 1.0, 2.0, 3.0, 4.0],
-        "B": [0.0, 1.0, 0.0, 1.0, 0.0],
-        "C": ["foo1", "foo2", "foo3", "foo4", "foo5"],
-        "D": pd.bdate_range("1/1/2009", periods=5),
+        'A': [0.0, 1.0, 2.0, 3.0, 4.0],
+        'B': [0.0, 1.0, 0.0, 1.0, 0.0],
+        'C': ['foo1', 'foo2', 'foo3', 'foo4', 'foo5'],
+        'D': pd.bdate_range('1/1/2009', periods=5),
     }
     return pd.DataFrame(data)
 
 
 def getSeriesData():
     index = makeStringIndex(_N)
     return {
@@ -54,32 +53,30 @@
 
 
 def makeDataFrame():
     data = getSeriesData()
     return pd.DataFrame(data)
 
 
-def makeDateIndex(
-    k=10, freq="B", name=None, **kwargs
-):
+def makeDateIndex(k=10, freq='B', name=None, **kwargs):
     dt = datetime(2000, 1, 1)
     dr = pd.bdate_range(dt, periods=k, freq=freq, name=name)
     return pd.DatetimeIndex(dr, name=name, **kwargs)
 
 
-def makeTimeSeries(nper=None, freq="B", name=None):
+def makeTimeSeries(nper=None, freq='B', name=None):
     if nper is None:
         nper = _N
     return pd.Series(
         np.random.default_rng(2).standard_normal(nper),
         index=makeDateIndex(nper, freq=freq),
         name=name,
     )
 
 
-def getTimeSeriesData(nper=None, freq="B"):
+def getTimeSeriesData(nper=None, freq='B'):
     return {c: makeTimeSeries(nper, freq) for c in getCols(_K)}
 
 
-def makeTimeDataFrame(nper=None, freq="B"):
+def makeTimeDataFrame(nper=None, freq='B'):
     data = getTimeSeriesData(nper, freq)
     return pd.DataFrame(data)
```

### Comparing `hvplot-0.9.2rc1/hvplot/ui.py` & `hvplot-0.9.3a1/hvplot/ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,37 +12,44 @@
 from .plotting import hvPlot as _hvPlot
 from .util import is_geodataframe, is_xarray, instantiate_crs_str
 
 # Defaults
 KINDS = {
     # these are for the kind selector
     'dataframe': sorted(
-        set(_hvConverter._kind_mapping) -
-        set(_hvConverter._gridded_types) -
-        set(_hvConverter._geom_types) |
-        set(['points'])
+        set(_hvConverter._kind_mapping)
+        - set(_hvConverter._gridded_types)
+        - set(_hvConverter._geom_types)
+        | set(['points'])
     ),
     'gridded': sorted(set(_hvConverter._gridded_types) - set(['dataset'])),
     'geom': _hvConverter._geom_types,
 }
 
-KINDS['2d'] = ['bivariate', 'heatmap', 'hexbin', 'labels', 'vectorfield', 'points'] + KINDS['gridded'] + KINDS['geom']
+KINDS['2d'] = (
+    ['bivariate', 'heatmap', 'hexbin', 'labels', 'vectorfield', 'points']
+    + KINDS['gridded']
+    + KINDS['geom']
+)
 KINDS['stats'] = ['hist', 'kde', 'boxwhisker', 'violin', 'heatmap', 'bar', 'barh']
 KINDS['all'] = sorted(set(KINDS['dataframe'] + KINDS['gridded'] + KINDS['geom']))
 
 CMAPS = [cm for cm in list_cmaps() if not cm.endswith('_r_r')]
 DEFAULT_CMAPS = _hvConverter._default_cmaps
-GEO_FEATURES = [
-    'borders', 'coastline', 'land', 'lakes', 'ocean', 'rivers',
-    'states', 'grid'
-]
+GEO_FEATURES = ['borders', 'coastline', 'land', 'lakes', 'ocean', 'rivers', 'states', 'grid']
 GEO_TILES = [None] + sorted(tile_sources)
 GEO_KEYS = [
-    'crs', 'crs_kwargs', 'projection', 'projection_kwargs',
-    'global_extent', 'project', 'features', 'feature_scale',
+    'crs',
+    'crs_kwargs',
+    'projection',
+    'projection_kwargs',
+    'global_extent',
+    'project',
+    'features',
+    'feature_scale',
 ]
 AGGREGATORS = [None, 'count', 'min', 'max', 'mean', 'sum', 'any']
 MAX_ROWS = 10000
 CONTROLS_WIDTH = 200
 
 
 def explorer(data, **kwargs):
@@ -100,15 +107,14 @@
     if parameters:
         kwargs['parameters'] = parameters
     pane = pn.Param(inst.param, **kwargs)
     return pane
 
 
 class Controls(Viewer):
-
     explorer = param.ClassSelector(class_=Viewer, precedence=-1)
 
     _widgets_kwargs = {}
 
     __abstract = True
 
     def __init__(self, df, **params):
@@ -116,46 +122,53 @@
         super().__init__(**params)
 
     def __panel__(self):
         return _create_param_pane(self, widgets_kwargs=self._widgets_kwargs)
 
     @property
     def kwargs(self):
-        return {k: v for k, v in self.param.values().items()
-                if k not in ('name', 'explorer') and v is not None and v != ''}
+        return {
+            k: v
+            for k, v in self.param.values().items()
+            if k not in ('name', 'explorer') and v is not None and v != ''
+        }
 
 
 class Colormapping(Controls):
-
-    clim = param.Range(label="Colorbar Limits (clim)", doc="""
-        Upper and lower limits of the colorbar.""")
+    clim = param.Range(
+        label='Colorbar Limits (clim)',
+        doc="""
+        Upper and lower limits of the colorbar.""",
+    )
 
     cnorm = param.Selector(
-        label="Colorbar Normalization (cnorm)",
+        label='Colorbar Normalization (cnorm)',
         default='linear',
-        objects=['linear', 'log', 'eq_hist']
+        objects=['linear', 'log', 'eq_hist'],
     )
 
     color = param.String(default=None)
 
     colorbar = param.Boolean(default=None)
 
-    cmap = param.Selector(default=DEFAULT_CMAPS['linear'],
-                          label='Colormap', objects=CMAPS)
+    cmap = param.Selector(default=DEFAULT_CMAPS['linear'], label='Colormap', objects=CMAPS)
 
     rescale_discrete_levels = param.Boolean(default=True)
 
-    symmetric = param.Boolean(default=False, doc="""
-        Whether the data are symmetric around zero.""")
+    symmetric = param.Boolean(
+        default=False,
+        doc="""
+        Whether the data are symmetric around zero.""",
+    )
 
     _widgets_kwargs = {'clim': {'placeholder': '(min, max)'}}
 
     def __init__(self, data, **params):
         super().__init__(data, **params)
-        if not 'symmetric' in params:
+        if 'symmetric' not in params:
             self.symmetric = self.explorer._converter._plot_opts.get('symmetric', False)
 
     @property
     def colormapped(self):
         if self.explorer.kind in _hvConverter._colorbar_types:
             return True
         return self.color is not None and self.color in self._data
@@ -177,20 +190,18 @@
                 key = 'linear'
         else:
             return
         self.cmap = DEFAULT_CMAPS[key]
 
 
 class Style(Controls):
-
     alpha = param.Magnitude(default=1)
 
 
 class Axes(Controls):
-
     legend = param.Selector(default='bottom_right', objects=_hvConverter._legend_positions)
 
     logx = param.Boolean(default=False)
 
     logy = param.Boolean(default=False)
 
     height = param.Integer(default=None, bounds=(0, None))
@@ -209,15 +220,15 @@
 
     logy = param.Boolean(default=False)
 
     def __init__(self, data, **params):
         super().__init__(data, **params)
         self._update_ranges()
 
-    @param.depends('explorer.xlim', 'explorer.ylim',  watch=True)
+    @param.depends('explorer.xlim', 'explorer.ylim', watch=True)
     def _update_ranges(self):
         xlim = self.explorer.xlim()
         if xlim is not None and is_number(xlim[0]) and is_number(xlim[1]) and xlim[0] != xlim[1]:
             xlim = self._convert_to_int(xlim)
             self.param.xlim.precedence = 0
             self.param.xlim.bounds = xlim
         else:
@@ -242,89 +253,129 @@
         if isinstance(val[0], datetime_types) and isinstance(val[1], datetime_types):
             val = (dt_to_int(val[0], 'ms'), dt_to_int(val[1], 'ms'))
 
         return val
 
 
 class Labels(Controls):
+    title = param.String(doc='Title for the plot')
 
-    title = param.String(doc="Title for the plot")
-
-    xlabel = param.String(doc="Axis labels for the x-axis.")
+    xlabel = param.String(doc='Axis labels for the x-axis.')
 
-    ylabel = param.String(doc="Axis labels for the y-axis.")
+    ylabel = param.String(doc='Axis labels for the y-axis.')
 
-    clabel = param.String(label="Colorbar Label (clabel)", doc="""
-        Axis labels for the colorbar.""")
+    clabel = param.String(
+        label='Colorbar Label (clabel)',
+        doc="""
+        Axis labels for the colorbar.""",
+    )
 
-    fontscale = param.Number(default=1, doc="""
+    fontscale = param.Number(
+        default=1,
+        doc="""
         Scales the size of all fonts by the same amount, e.g. fontscale=1.5
-        enlarges all fonts (title, xticks, labels etc.) by 50%.""")
+        enlarges all fonts (title, xticks, labels etc.) by 50%.""",
+    )
 
     rot = param.Integer(
-        default=0, bounds=(0, 360), label="X Tick Labels Rotation (rot)", doc="""
+        default=0,
+        bounds=(0, 360),
+        label='X Tick Labels Rotation (rot)',
+        doc="""
         Rotates the axis ticks along the x-axis by the specified
-        number of degrees.""")
+        number of degrees.""",
+    )
 
 
 class Geographic(Controls):
-
-    tiles = param.ObjectSelector(default=None, objects=GEO_TILES, doc="""
+    tiles = param.ObjectSelector(
+        default=None,
+        objects=GEO_TILES,
+        doc="""
         Whether to overlay the plot on a tile source. Tiles sources
         can be selected by name or a tiles object or class can be passed,
-        the default is 'Wikipedia'.""")
+        the default is 'Wikipedia'.""",
+    )
 
-    geo = param.Boolean(default=False, doc="""
+    geo = param.Boolean(
+        default=False,
+        doc="""
         Whether the plot should be treated as geographic (and assume
-        PlateCarree, i.e. lat/lon coordinates). Require GeoViews.""")
+        PlateCarree, i.e. lat/lon coordinates). Require GeoViews.""",
+    )
 
-    crs = param.Selector(default=None, doc="""
+    crs = param.Selector(
+        default=None,
+        doc="""
         Coordinate reference system of the data specified as Cartopy
-        CRS object, proj.4 string or EPSG code.""")
+        CRS object, proj.4 string or EPSG code.""",
+    )
 
-    crs_kwargs = param.Dict(default={}, doc="""
-        Keyword arguments to pass to selected CRS.""")
+    crs_kwargs = param.Dict(
+        default={},
+        doc="""
+        Keyword arguments to pass to selected CRS.""",
+    )
 
-    projection = param.ObjectSelector(default=None, doc="""
-        Projection to use for cartographic plots.""")
+    projection = param.ObjectSelector(
+        default=None,
+        doc="""
+        Projection to use for cartographic plots.""",
+    )
 
-    projection_kwargs = param.Dict(default={}, doc="""
-        Keyword arguments to pass to selected projection.""")
+    projection_kwargs = param.Dict(
+        default={},
+        doc="""
+        Keyword arguments to pass to selected projection.""",
+    )
 
-    global_extent = param.Boolean(default=None, doc="""
-        Whether to expand the plot extent to span the whole globe.""")
+    global_extent = param.Boolean(
+        default=None,
+        doc="""
+        Whether to expand the plot extent to span the whole globe.""",
+    )
 
-    project = param.Boolean(default=False, doc="""
+    project = param.Boolean(
+        default=False,
+        doc="""
         Whether to project the data before plotting (adds initial
         overhead but avoids projecting data when plot is dynamically
-        updated).""")
+        updated).""",
+    )
 
-    features = param.ListSelector(default=None, objects=GEO_FEATURES, doc="""
+    features = param.ListSelector(
+        default=None,
+        objects=GEO_FEATURES,
+        doc="""
         A list of features or a dictionary of features and the scale
         at which to render it. Available features include 'borders',
-        'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'.""")
+        'coastline', 'lakes', 'land', 'ocean', 'rivers' and 'states'.""",
+    )
 
-    feature_scale = param.ObjectSelector(default='110m', objects=['110m', '50m', '10m'], doc="""
-        The scale at which to render the features.""")
+    feature_scale = param.ObjectSelector(
+        default='110m',
+        objects=['110m', '50m', '10m'],
+        doc="""
+        The scale at which to render the features.""",
+    )
 
     _widgets_kwargs = {'geo': {'type': pn.widgets.Toggle}}
 
-    def __init__(self, data,  **params):
+    def __init__(self, data, **params):
         gv_available = False
         try:
             import geoviews  # noqa
+
             gv_available = True
         except ImportError:
             pass
 
         geo_params = GEO_KEYS + ['geo']
         if not gv_available and any(p in params for p in geo_params):
-            raise ImportError(
-                'GeoViews must be installed to enable the geographic options.'
-            )
+            raise ImportError('GeoViews must be installed to enable the geographic options.')
         super().__init__(data, **params)
         if not gv_available:
             for p in geo_params:
                 self.param[p].constant = True
             # Workaround: Checkbox widgets don't yet have a tooltip
             self.param['geo'].label = 'geo (require GeoViews)'
         else:
@@ -336,16 +387,18 @@
         for key in GEO_KEYS:
             self.param[key].constant = not enabled
         self.geo = enabled
         if not enabled:
             return
 
         from cartopy.crs import CRS
+
         crs_list = sorted(
-            k for k in param.concrete_descendents(CRS).keys()
+            k
+            for k in param.concrete_descendents(CRS).keys()
             if not k.startswith('_') and k != 'CRS'
         )
         crs_list.insert(0, 'GOOGLE_MERCATOR')
         crs_list.insert(0, 'PlateCarree')
         crs_list.remove('PlateCarree')
 
         self.param.crs.objects = crs_list
@@ -360,35 +413,53 @@
         if self.features is None:
             updates['features'] = ['coastline']
 
         self.param.update(**updates)
 
 
 class Operations(Controls):
-
-    datashade = param.Boolean(default=False, doc="""
+    datashade = param.Boolean(
+        default=False,
+        doc="""
         Whether to apply rasterization and shading using datashader
-        library returning an RGB object.""")
+        library returning an RGB object.""",
+    )
 
-    rasterize = param.Boolean(default=False, doc="""
+    rasterize = param.Boolean(
+        default=False,
+        doc="""
         Whether to apply rasterization using the datashader library
-        returning an aggregated Image.""")
+        returning an aggregated Image.""",
+    )
 
-    aggregator = param.Selector(default=None, objects=AGGREGATORS, doc="""
-        Aggregator to use when applying rasterize or datashade operation.""")
+    aggregator = param.Selector(
+        default=None,
+        objects=AGGREGATORS,
+        doc="""
+        Aggregator to use when applying rasterize or datashade operation.""",
+    )
 
-    dynspread = param.Boolean(default=False, doc="""
+    dynspread = param.Boolean(
+        default=False,
+        doc="""
         Allows plots generated with datashade=True or rasterize=True
-        to increase the point size to make sparse regions more visible.""")
+        to increase the point size to make sparse regions more visible.""",
+    )
 
-    x_sampling = param.Number(default=None, doc="""
-        Specifies the smallest allowed sampling interval along the x-axis.""")
+    x_sampling = param.Number(
+        default=None,
+        doc="""
+        Specifies the smallest allowed sampling interval along the x-axis.""",
+    )
 
-    y_sampling = param.Number(default=None, doc="""
-        Specifies the smallest allowed sampling interval along the y-axis.""")
+    y_sampling = param.Number(
+        default=None,
+        doc="""
+        Specifies the smallest allowed sampling interval along the y-axis.""",
+    )
 
     @param.depends('datashade', watch=True)
     def _toggle_rasterize(self):
         if self.datashade:
             self.rasterize = False
 
     @param.depends('rasterize', watch=True)
@@ -402,33 +473,36 @@
         self.param.dynspread.constant = not enabled
         self.param.x_sampling.constant = not enabled
         self.param.y_sampling.constant = not enabled
         self.param.aggregator.constant = not enabled
 
 
 class Advanced(Controls):
-
-    opts = param.Dict(label='HoloViews .opts()', doc="""
+    opts = param.Dict(
+        label='HoloViews .opts()',
+        doc="""
         Options applied via HoloViews .opts().
         Examples:
         - image: {"color_levels": 11}
         - line: {"line_dash": "dashed"}
-        - scatter: {'size': 5, 'marker': '^'}""")
+        - scatter: {'size': 5, 'marker': '^'}""",
+    )
 
     _widgets_kwargs = {'opts': {'placeholder': "{'size': 5, 'marker': '^'}"}}
 
 
 class StatusBar(param.Parameterized):
-
-    live_update = param.Boolean(default=True, doc="""
-        Whether to automatically update the plot when a param is changed""")
+    live_update = param.Boolean(
+        default=True,
+        doc="""
+        Whether to automatically update the plot when a param is changed""",
+    )
 
 
 class hvPlotExplorer(Viewer):
-
     kind = param.Selector()
 
     x = param.Selector()
 
     y = param.Selector()
 
     y_multi = param.ListSelector(default=[], label='Y')
@@ -451,16 +525,19 @@
 
     statusbar = param.ClassSelector(class_=StatusBar)
 
     style = param.ClassSelector(class_=Style)
 
     advanced = param.ClassSelector(class_=Advanced)
 
-    code = param.String(precedence=-1, doc="""
-        Code to generate the plot.""")
+    code = param.String(
+        precedence=-1,
+        doc="""
+        Code to generate the plot.""",
+    )
 
     @classmethod
     def from_data(cls, data, **params):
         if is_geodataframe(data):
             # cls = hvGeomExplorer
             raise TypeError('GeoDataFrame objects not yet supported.')
         elif is_xarray(data):
@@ -472,29 +549,20 @@
     def __panel__(self):
         return self._layout
 
     def __init__(self, df, **params):
         x, y = params.get('x'), params.get('y')
         if 'y' in params:
             params['y_multi'] = params.pop('y') if isinstance(params['y'], list) else [params['y']]
-        statusbar_params = {
-            k: params.pop(k)
-            for k in params.copy()
-            if k in StatusBar.param
-        }
+        statusbar_params = {k: params.pop(k) for k in params.copy() if k in StatusBar.param}
         converter = _hvConverter(
-            df, x, y,
-            **{k: v for k, v in params.items() if k not in ('x', 'y', 'y_multi')}
+            df, x, y, **{k: v for k, v in params.items() if k not in ('x', 'y', 'y_multi')}
         )
         # Collect kwargs passed to the constructor but meant for the controls
-        extras = {
-            k: params.pop(k)
-            for k in params.copy()
-            if k not in self.param
-        }
+        extras = {k: params.pop(k) for k in params.copy() if k not in self.param}
         super().__init__(**params)
         self._data = df
         self._converter = converter
         groups = {group: KINDS[group] for group in self._groups}
         # Create pane for the main controls as done by the Controls instances.
         self._controls = _create_param_pane(
             self,
@@ -504,66 +572,61 @@
         self.param.watch(self._toggle_controls, 'kind')
         self.param.watch(self._check_y, 'y_multi')
         self.param.watch(self._check_by, 'by')
         self._populate()
         self._control_tabs = pn.Tabs(tabs_location='left')
         self.statusbar = StatusBar(**statusbar_params)
         self._statusbar = pn.Param(
-            self.statusbar,
-            show_name=False,
-            default_layout=pn.Row,
-            margin=(5, 56, 0, 56)
+            self.statusbar, show_name=False, default_layout=pn.Row, margin=(5, 56, 0, 56)
         )
         controls = [
             p.class_
             for p in self.param.objects().values()
-            if isinstance(p, param.ClassSelector)
-            and issubclass(p.class_, Controls)
+            if isinstance(p, param.ClassSelector) and issubclass(p.class_, Controls)
         ]
         controller_params = {}
         for cls in controls:
-            controller_params[cls] = {
-                k: extras.pop(k)
-                for k in extras.copy()
-                if k in cls.param
-            }
+            controller_params[cls] = {k: extras.pop(k) for k in extras.copy() if k in cls.param}
         if extras:
-            raise TypeError(
-                f'__init__() got keyword(s) not supported by any control: {extras}'
-            )
+            raise TypeError(f'__init__() got keyword(s) not supported by any control: {extras}')
         self._controllers = {
             cls.name.lower(): cls(df, explorer=self, **cparams)
             for cls, cparams in controller_params.items()
         }
         self.param.update(**self._controllers)
         self.param.watch(self._refresh, list(self.param))
         for controller in self._controllers.values():
             controller.param.watch(self._refresh, list(controller.param))
         self.statusbar.param.watch(self._refresh, list(self.statusbar.param))
         self._alert = pn.pane.Alert(
             alert_type='danger', visible=False, sizing_mode='stretch_width'
         )
         self._hv_pane = pn.pane.HoloViews(
-            sizing_mode='stretch_both', min_height=250, margin=(5, 5, 5, 20),
-            widget_location="bottom", widget_layout=pn.Row)
+            sizing_mode='stretch_both',
+            min_height=250,
+            margin=(5, 5, 5, 20),
+            widget_location='bottom',
+            widget_layout=pn.Row,
+        )
         self._code_pane = pn.pane.Markdown(
-            sizing_mode='stretch_both', min_height=250, margin=(5, 5, 0, 20))
+            sizing_mode='stretch_both', min_height=250, margin=(5, 5, 0, 20)
+        )
         self._layout = pn.Column(
             self._alert,
             self._statusbar,
             pn.layout.Divider(),
             pn.Row(
                 self._control_tabs,
                 # Using .layout on the HoloViews pane to display the widgets
                 # https://github.com/holoviz/panel/issues/5628#issuecomment-1763443895
                 pn.Tabs(('Plot', self._hv_pane.layout), ('Code', self._code_pane)),
-                sizing_mode='stretch_both'
+                sizing_mode='stretch_both',
             ),
             sizing_mode='stretch_width',
-            height=600
+            height=600,
         )
 
         # initialize
         self.param.trigger('kind')
 
     def _populate(self):
         """
@@ -611,15 +674,17 @@
                 kwargs[key] = instantiate_crs_str(kwargs.pop(key), **crs_kwargs)
 
             feature_scale = kwargs.pop('feature_scale', None)
             kwargs['features'] = {feature: feature_scale for feature in kwargs.pop('features', [])}
 
         kwargs['min_height'] = 400
         df = self._data
-        if len(df) > MAX_ROWS and not (self.kind in KINDS['stats'] or kwargs.get('rasterize') or kwargs.get('datashade')):
+        if len(df) > MAX_ROWS and not (
+            self.kind in KINDS['stats'] or kwargs.get('rasterize') or kwargs.get('datashade')
+        ):
             df = df.sample(n=MAX_ROWS)
         self._layout.loading = True
         try:
             self._hvplot = _hvPlot(df)(
                 kind=self.kind, x=self.x, y=y, by=self.by, groupby=self.groupby, **kwargs
             )
             if opts_kwargs:
@@ -630,16 +695,15 @@
             # See https://github.com/holoviz/panel/issues/6110
             if len(self._hv_pane.widget_box) > 1:
                 for w in self._hv_pane.widget_box:
                     w.margin = (20, 5, 5, 5)
             self._alert.visible = False
         except Exception as e:
             self._alert.param.update(
-                object=f'**Rendering failed with following error**: {e}',
-                visible=True
+                object=f'**Rendering failed with following error**: {e}', visible=True
             )
         finally:
             self._layout.loading = False
 
     def _refresh(self, *events):
         if not self.statusbar.live_update:
             return
@@ -692,24 +756,28 @@
         self._control_tabs[:] = tabs
 
     def _check_y(self, event):
         if len(event.new) > 1 and self.by:
             self.y = event.old
 
     def _check_by(self, event):
-        if event.new and 'y_multi' in self._controls.parameters and self.y_multi and len(self.y_multi) > 1:
+        if (
+            event.new
+            and 'y_multi' in self._controls.parameters
+            and self.y_multi
+            and len(self.y_multi) > 1
+        ):
             self.by = []
 
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
     # Public API
-    #----------------------------------------------------------------
+    # ----------------------------------------------------------------
 
     def hvplot(self):
-        """Return the plot as a HoloViews object.
-        """
+        """Return the plot as a HoloViews object."""
         return self._hvplot.clone()
 
     def plot_code(self, var_name=None):
         """Return a string representation that can be easily copy-pasted
         in a notebook cell to create a plot from a call to the `.hvplot`
         accessor, and that includes all the customized settings of the explorer.
 
@@ -718,17 +786,17 @@
 
         Parameters
         ----------
         var_name: string
             Data variable name by which the returned string will start.
         """
         settings = self.settings()
-        if "legend" not in settings:
-            settings["legend"] = "bottom_right"
-        settings["widget_location"] = "bottom"
+        if 'legend' not in settings:
+            settings['legend'] = 'bottom_right'
+        settings['widget_location'] = 'bottom'
         settings_args = ''
         if settings:
             settings_args = self._build_kwargs_string(settings)
         snippet = f'{var_name or self._var_name}.hvplot(\n{settings_args}\n)'
         opts = self.advanced.opts
         if opts:
             opts_args = self._build_kwargs_string(opts)
@@ -780,15 +848,14 @@
             settings['y'] = settings.pop('y_multi')
         settings.pop('opts', None)
         settings = {k: v for k, v in sorted(list(settings.items()))}
         return settings
 
 
 class hvGeomExplorer(hvPlotExplorer):
-
     kind = param.Selector(default=None, objects=KINDS['all'])
 
     @property
     def _var_name(self):
         return 'gdf'
 
     @property
@@ -811,20 +878,21 @@
     def ylim(self):
         pass
 
     @property
     def _groups(self):
         return ['gridded', 'dataframe']
 
-class hvGridExplorer(hvPlotExplorer):
 
+class hvGridExplorer(hvPlotExplorer):
     kind = param.Selector(default='image', objects=KINDS['all'])
 
     def __init__(self, ds, **params):
         import xarray as xr
+
         var_name_suffix = ''
         if isinstance(ds, xr.Dataset):
             data_vars = list(ds.data_vars)
             if len(data_vars) == 1:
                 ds = ds[data_vars[0]]
                 var_name_suffix = f"['{data_vars[0]}']"
             else:
@@ -850,15 +918,15 @@
     def _y(self):
         return (self._converter.y or self._converter.indexes[1]) if self.y is None else self.y
 
     @param.depends('x')
     def xlim(self):
         try:
             values = self._data[self._x]
-        except:
+        except Exception:
             return 0, 1
         if values.dtype.kind in 'OSU':
             return None
         return (np.nanmin(values), np.nanmax(values))
 
     @param.depends('y', 'y_multi')
     def ylim(self):
@@ -887,20 +955,23 @@
                     p.objects = variables_no_index
 
                 # Setting the default value if not set
                 if pname == 'x' and getattr(self, pname, None) is None:
                     setattr(self, pname, p.objects[0])
                 elif pname == 'y' and getattr(self, pname, None) is None:
                     setattr(self, pname, p.objects[1])
-                elif pname == 'groupby' and len(getattr(self, pname, [])) == 0 and len(p.objects) > 2:
+                elif (
+                    pname == 'groupby'
+                    and len(getattr(self, pname, [])) == 0
+                    and len(p.objects) > 2
+                ):
                     setattr(self, pname, p.objects[2:])
 
 
 class hvDataFrameExplorer(hvPlotExplorer):
-
     z = param.Selector()
 
     kind = param.Selector(default='scatter', objects=KINDS['all'])
 
     @property
     def _var_name(self):
         return 'df'
@@ -935,15 +1006,15 @@
     @param.depends('x')
     def xlim(self):
         if self._x == 'index':
             values = self._data.index.values
         else:
             try:
                 values = self._data[self._x]
-            except:
+            except Exception:
                 return 0, 1
         # for dask series; else it cannot get length
         if hasattr(values, 'compute_chunk_sizes'):
             values = values.compute_chunk_sizes()
         if values.dtype.kind in 'OSU':
             return None
         elif not len(values):
```

### Comparing `hvplot-0.9.2rc1/hvplot/util.py` & `hvplot-0.9.3a1/hvplot/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,41 +11,47 @@
 from types import FunctionType
 
 import bokeh
 import numpy as np
 import pandas as pd
 import param
 import holoviews as hv
+
 try:
     import panel as pn
+
     panel_available = True
-except:
+except ImportError:
     panel_available = False
 
 hv_version = Version(hv.__version__)
 bokeh_version = Version(bokeh.__version__)
-bokeh3 = bokeh_version >= Version("3.0")
-param2 = Version(param.__version__) >= Version("2.0rc4")
+bokeh3 = bokeh_version >= Version('3.0')
+param2 = Version(param.__version__) >= Version('2.0rc4')
 _fugue_ipython = None  # To be set to True in tests to mock ipython
 
+
 def with_hv_extension(func, extension='bokeh', logo=False):
     """If hv.extension is not loaded, load before calling function"""
+
     @wraps(func)
     def wrapper(*args, **kwargs):
         if extension and not getattr(hv.extension, '_loaded', False):
             from . import hvplot_extension
+
             hvplot_extension(extension, logo=logo)
         return func(*args, **kwargs)
+
     return wrapper
 
 
 def get_ipy():
     try:
-        ip = get_ipython() # noqa
-    except:
+        ip = get_ipython()  # noqa
+    except NameError:
         ip = None
     return ip
 
 
 def check_crs(crs):
     """
     Checks if the crs represents a valid grid, projection or ESPG string.
@@ -66,16 +72,18 @@
     A valid crs if possible, otherwise None.
     """
     import pyproj
 
     try:
         crs_type = pyproj.crs.CRS
     except AttributeError:
+
         class Dummy:
             pass
+
         crs_type = Dummy
 
     if isinstance(crs, pyproj.Proj):
         out = crs
     elif isinstance(crs, crs_type):
         out = pyproj.Proj(crs.to_wkt(), preserve_units=True)
     elif isinstance(crs, dict) or isinstance(crs, str):
@@ -118,74 +126,82 @@
         the projection to convert
     Returns
     -------
     a cartopy.crs.Projection object
     """
 
     import cartopy.crs as ccrs
+
     try:
         from osgeo import osr
+
         has_gdal = True
     except ImportError:
         has_gdal = False
 
     input_proj = proj
     proj = check_crs(input_proj)
     if proj is None:
-        raise ValueError(f"Invalid proj projection {input_proj!r}")
+        raise ValueError(f'Invalid proj projection {input_proj!r}')
 
     srs = proj.srs
     if has_gdal:
         import warnings
+
         with warnings.catch_warnings():
             # Avoiding this warning could be done by setting osr.UseExceptions(),
             # except there might be a risk to break the code of users leveraging
             # GDAL on their side or through other libraries. So we just silence it.
-            warnings.filterwarnings('ignore', category=FutureWarning, message=
-                r'Neither osr\.UseExceptions\(\) nor osr\.DontUseExceptions\(\) has '
+            warnings.filterwarnings(
+                'ignore',
+                category=FutureWarning,
+                message=r'Neither osr\.UseExceptions\(\) nor osr\.DontUseExceptions\(\) has '
                 r'been explicitly called\. In GDAL 4\.0, exceptions will be enabled '
-                'by default'
+                'by default',
             )
             # this is more robust, as srs could be anything (espg, etc.)
             s1 = osr.SpatialReference()
             s1.ImportFromProj4(proj.srs)
             if s1.ExportToProj4():
                 srs = s1.ExportToProj4()
 
-    km_proj = {'lon_0': 'central_longitude',
-               'lat_0': 'central_latitude',
-               'x_0': 'false_easting',
-               'y_0': 'false_northing',
-               'lat_ts': 'latitude_true_scale',
-               'o_lon_p': 'central_rotated_longitude',
-               'o_lat_p': 'pole_latitude',
-               'k': 'scale_factor',
-               'zone': 'zone',
-               }
-    km_globe = {'a': 'semimajor_axis',
-                'b': 'semiminor_axis',
-                }
-    km_std = {'lat_1': 'lat_1',
-              'lat_2': 'lat_2',
-              }
+    km_proj = {
+        'lon_0': 'central_longitude',
+        'lat_0': 'central_latitude',
+        'x_0': 'false_easting',
+        'y_0': 'false_northing',
+        'lat_ts': 'latitude_true_scale',
+        'o_lon_p': 'central_rotated_longitude',
+        'o_lat_p': 'pole_latitude',
+        'k': 'scale_factor',
+        'zone': 'zone',
+    }
+    km_globe = {
+        'a': 'semimajor_axis',
+        'b': 'semiminor_axis',
+    }
+    km_std = {
+        'lat_1': 'lat_1',
+        'lat_2': 'lat_2',
+    }
     kw_proj = {}
     kw_globe = {}
     kw_std = {}
     for s in srs.split('+'):
         s = s.split('=')
         if len(s) != 2:
             continue
         k = s[0].strip()
         v = s[1].strip()
         try:
             v = float(v)
-        except:
+        except Exception:
             pass
         if k == 'proj':
-            if v == "longlat":
+            if v == 'longlat':
                 cl = ccrs.PlateCarree
             elif v == 'tmerc':
                 cl = ccrs.TransverseMercator
                 kw_proj['approx'] = True
             elif v == 'lcc':
                 cl = ccrs.LambertConformal
             elif v == 'merc':
@@ -213,15 +229,15 @@
     if kw_std:
         kw_proj['standard_parallels'] = (kw_std['lat_1'], kw_std['lat_2'])
 
     # mercatoooor
     if cl.__name__ == 'Mercator':
         kw_proj.pop('false_easting', None)
         kw_proj.pop('false_northing', None)
-        if "scale_factor" in kw_proj:
+        if 'scale_factor' in kw_proj:
             kw_proj.pop('latitude_true_scale', None)
     elif cl.__name__ == 'Stereographic':
         kw_proj.pop('scale_factor', None)
         if 'latitude_true_scale' in kw_proj:
             kw_proj['true_scale_latitude'] = kw_proj['latitude_true_scale']
             kw_proj.pop('latitude_true_scale', None)
     elif cl.__name__ == 'RotatedPole':
@@ -252,15 +268,15 @@
     """
     missing = []
     try:
         import cartopy.crs as ccrs
     except ImportError:
         missing.append('cartopy')
     try:
-        import geoviews as gv # noqa
+        import geoviews as gv  # noqa
     except ImportError:
         missing.append('geoviews')
     try:
         import pyproj
     except ImportError:
         missing.append('pyproj')
     if missing:
@@ -282,151 +298,183 @@
     if isinstance(crs, (str, pyproj.Proj)):  # proj4/wkt strings
         try:
             return proj_to_cartopy(crs)
         except Exception as e:
             errors.append(e)
 
     raise ValueError(
-        "Projection must be defined as a EPSG code, proj4 string, "
-        "WKT string, cartopy CRS, pyproj.Proj, or pyproj.CRS."
+        'Projection must be defined as a EPSG code, proj4 string, '
+        'WKT string, cartopy CRS, pyproj.Proj, or pyproj.CRS.'
     ) from Exception(*errors)
 
 
 def is_list_like(obj):
     """
     Adapted from pandas' is_list_like cython function.
     """
     return (
         # equiv: `isinstance(obj, abc.Iterable)`
-        hasattr(obj, "__iter__") and not isinstance(obj, type)
+        hasattr(obj, '__iter__')
+        and not isinstance(obj, type)
         # we do not count strings/unicode/bytes as list-like
         and not isinstance(obj, (str, bytes))
         # exclude zero-dimensional numpy arrays, effectively scalars
         and not (isinstance(obj, np.ndarray) and obj.ndim == 0)
     )
 
 
 def is_tabular(data):
     if check_library(data, ['dask', 'streamz', 'pandas', 'geopandas', 'cudf']):
         return True
     elif check_library(data, 'intake'):
         from intake.source.base import DataSource
+
         if isinstance(data, DataSource):
             return data.container == 'dataframe'
     else:
         return False
 
+
 def is_series(data):
     if not check_library(data, ['dask', 'streamz', 'pandas', 'cudf']):
         return False
     elif isinstance(data, pd.Series):
         return True
     elif check_library(data, 'streamz'):
         import streamz.dataframe as sdf
+
         return isinstance(data, (sdf.Series, sdf.Seriess))
     elif check_library(data, 'dask'):
         import dask.dataframe as dd
+
         return isinstance(data, dd.Series)
     elif check_library(data, 'cudf'):
         import cudf
+
         return isinstance(data, cudf.Series)
     else:
         return False
 
+
 def check_library(obj, library):
     if not isinstance(library, list):
         library = [library]
-    return any([obj.__module__.split('.')[0].startswith(l) for l in library])
+    return any([obj.__module__.split('.')[0].startswith(lib) for lib in library])
+
 
 def is_cudf(data):
     if 'cudf' in sys.modules:
         from cudf import DataFrame, Series
+
         return isinstance(data, (DataFrame, Series))
 
+
 def is_dask(data):
     if not check_library(data, 'dask'):
         return False
     import dask.dataframe as dd
+
     return isinstance(data, (dd.DataFrame, dd.Series))
 
+
 def is_polars(data):
     if not check_library(data, 'polars'):
         return False
     import polars as pl
+
     return isinstance(data, (pl.DataFrame, pl.Series, pl.LazyFrame))
 
+
 def is_intake(data):
-    if "intake" not in sys.modules:
+    if 'intake' not in sys.modules:
         return False
     from intake.source.base import DataSource
+
     return isinstance(data, DataSource)
 
+
 def is_ibis(data):
     if not check_library(data, 'ibis'):
         return False
     import ibis
+
     return isinstance(data, ibis.Expr)
 
+
 def is_streamz(data):
     if not check_library(data, 'streamz'):
         return False
     import streamz.dataframe as sdf
+
     return sdf and isinstance(data, (sdf.DataFrame, sdf.Series, sdf.DataFrames, sdf.Seriess))
 
+
 def is_xarray(data):
     if not check_library(data, 'xarray'):
         return False
     from xarray import DataArray, Dataset
+
     return isinstance(data, (DataArray, Dataset))
 
+
 def is_xarray_dataarray(data):
     if not check_library(data, 'xarray'):
         return False
     from xarray import DataArray
+
     return isinstance(data, DataArray)
 
 
 def process_intake(data, use_dask):
     if data.container not in ('dataframe', 'xarray'):
-        raise NotImplementedError('Plotting interface currently only '
-                                  'supports DataSource objects declaring '
-                                  'a dataframe or xarray container.')
+        raise NotImplementedError(
+            'Plotting interface currently only '
+            'supports DataSource objects declaring '
+            'a dataframe or xarray container.'
+        )
     if use_dask:
         data = data.to_dask()
     else:
         data = data.read()
     return data
 
 
 def is_geodataframe(data):
     if 'spatialpandas' in sys.modules:
         import spatialpandas as spd
+
         if isinstance(data, spd.GeoDataFrame):
             return True
-    return isinstance(data, pd.DataFrame) and hasattr(data, 'geom_type') and hasattr(data, 'geometry')
+    return (
+        isinstance(data, pd.DataFrame) and hasattr(data, 'geom_type') and hasattr(data, 'geometry')
+    )
 
 
-def process_xarray(data, x, y, by, groupby, use_dask, persist, gridded,
-                   label, value_label, other_dims, kind=None):
+def process_xarray(
+    data, x, y, by, groupby, use_dask, persist, gridded, label, value_label, other_dims, kind=None
+):
     import xarray as xr
+
     if isinstance(data, xr.Dataset):
         dataset = data
     else:
         name = data.name or label or value_label
         dataset = data.to_dataset(name=name)
 
     all_vars = list(other_dims) if other_dims else []
     for var in [x, y, by, groupby]:
         if isinstance(var, list):
             all_vars.extend(var)
         elif isinstance(var, str):
             all_vars.append(var)
 
     if not gridded:
-        not_found = [var for var in all_vars if var not in list(dataset.data_vars) + list(dataset.coords)]
+        not_found = [
+            var for var in all_vars if var not in list(dataset.data_vars) + list(dataset.coords)
+        ]
         _, extra_vars, extra_coords = process_derived_datetime_xarray(dataset, not_found)
         dataset = dataset.assign_coords(**{var: dataset[var] for var in extra_coords})
         dataset = dataset.assign(**{var: dataset[var] for var in extra_vars})
 
     data_vars = list(dataset.data_vars)
     ignore = (by or []) + (groupby or [])
     dims = [c for c in dataset.coords if dataset[c].shape != () and c not in ignore][::-1]
@@ -445,17 +493,19 @@
                     y = c
         if not (x or y):
             x, y = index_dims[:2] if len(index_dims) > 1 else dims[:2]
         elif x and not y:
             y = [d for d in dims if d != x][0]
         elif y and not x:
             x = [d for d in dims if d != y][0]
-        if (len(dims) > 2 and kind not in ('table', 'dataset') and not groupby):
+        if len(dims) > 2 and kind not in ('table', 'dataset') and not groupby:
             dims = list(data.coords[x].dims) + list(data.coords[y].dims)
-            groupby = [d for d in index_dims if d not in (x, y) and d not in dims and d not in other_dims]
+            groupby = [
+                d for d in index_dims if d not in (x, y) and d not in dims and d not in other_dims
+            ]
     else:
         if use_dask:
             data = dataset.to_dask_dataframe()
             data = data.persist() if persist else data
         else:
             data = dataset.to_dataframe()
             if len(data.index.names) > 1:
@@ -475,24 +525,24 @@
             elif isinstance(var, str):
                 all_vars.append(var)
 
         covered_dims = []
         for var in all_vars:
             if var in dataset.coords:
                 covered_dims.extend(dataset[var].dims)
-        leftover_dims = [dim for dim in index_dims
-                         if dim not in covered_dims + all_vars]
+        leftover_dims = [dim for dim in index_dims if dim not in covered_dims + all_vars]
 
         if groupby is None:
             groupby = [c for c in leftover_dims if c not in (by or [])]
     return data, x, y, by, groupby
 
 
 def process_derived_datetime_xarray(data, not_found):
     from pandas.api.types import is_datetime64_any_dtype as isdate
+
     extra_vars = []
     extra_coords = []
     for var in not_found:
         if '.' in var:
             derived_from = var.split('.')[0]
             if isdate(data[derived_from]):
                 if derived_from in data.coords:
@@ -501,14 +551,15 @@
                     extra_vars.append(var)
     not_found = [var for var in not_found if var not in extra_vars + extra_coords]
     return not_found, extra_vars, extra_coords
 
 
 def process_derived_datetime_pandas(data, not_found, indexes=None):
     from pandas.api.types import is_datetime64_any_dtype as isdate
+
     indexes = indexes or []
     extra_cols = {}
     for var in not_found:
         if '.' in var:
             parts = var.split('.')
             base_col = parts[0]
             dt_str = parts[-1]
@@ -550,16 +601,15 @@
             arg_names += list(k) * len(deps)
 
     return dynamic, arg_deps, arg_names
 
 
 def filter_opts(eltype, options, backend='bokeh'):
     opts = getattr(hv.Store.options(backend), eltype)
-    allowed = [k for g in opts.groups.values()
-               for k in list(g.allowed_keywords)]
+    allowed = [k for g in opts.groups.values() for k in list(g.allowed_keywords)]
     opts = {k: v for k, v in options.items() if k in allowed}
     return opts
 
 
 def _flatten(line):
     """
     Flatten an arbitrarily nested sequence.
@@ -593,24 +643,35 @@
     """
     # There's no generic way to rename columns across tabular object types.
     # `columns` could refer to anything else on the object, e.g. a dim
     # on an xarray DataArray. So this may need to be stricter.
     if not hasattr(data, 'columns') or not hasattr(data, 'rename'):
         return data
     renamed = {
-        c: str(c)
-        for c in data.columns
-        if not isinstance(c, str) and isinstance(c, Hashable)
+        c: str(c) for c in data.columns if not isinstance(c, str) and isinstance(c, Hashable)
     }
     if renamed:
         data = data.rename(columns=renamed)
     return data
 
 
 def instantiate_crs_str(crs_str: str, **kwargs):
     """
     Instantiate a cartopy.crs.Projection from a string.
     """
     import cartopy.crs as ccrs
+
     if crs_str.upper() == 'GOOGLE_MERCATOR':
         return ccrs.GOOGLE_MERCATOR
     return getattr(ccrs, crs_str)(**kwargs)
+
+
+def import_datashader():
+    datashader = None
+    try:
+        import datashader
+    except ModuleNotFoundError:
+        raise ModuleNotFoundError(
+            'The `datashader` package must be installed in order to use '
+            'datashading features. Install it with pip or conda.'
+        ) from None
+    return datashader
```

### Comparing `hvplot-0.9.2rc1/hvplot/xarray.py` & `hvplot-0.9.3a1/hvplot/xarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from panel.widgets import Widget
 
 from .interactive import Interactive
 
 
 class XArrayInteractive(Interactive):
-
     @classmethod
     def applies(cls, obj):
         return isinstance(obj, (xr.DataArray, xr.Dataset))
 
     def sel(self, **kwargs):
         processed = {}
         for k, v in kwargs.items():
@@ -40,22 +39,24 @@
 
 
 def patch(name='hvplot', interactive='interactive', extension='bokeh', logo=False):
     from . import hvPlot, post_patch
 
     try:
         import xarray as xr
-    except:
-        raise ImportError('Could not patch plotting API onto xarray. '
-                          'xarray could not be imported.')
+    except ImportError:
+        raise ImportError(
+            'Could not patch plotting API onto xarray. xarray could not be imported.'
+        )
 
     # Remove the class docstring as it very developer focused
-    XArrayInteractive.__doc__ = ""
+    XArrayInteractive.__doc__ = ''
 
     xr.register_dataset_accessor(name)(hvPlot)
     xr.register_dataarray_accessor(name)(hvPlot)
     xr.register_dataset_accessor(interactive)(XArrayInteractive)
     xr.register_dataarray_accessor(interactive)(XArrayInteractive)
 
     post_patch(extension, logo)
 
+
 patch()
```

