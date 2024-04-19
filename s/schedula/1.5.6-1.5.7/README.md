# Comparing `tmp/schedula-1.5.6.tar.gz` & `tmp/schedula-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula-1.5.6.tar", last modified: Wed Apr  3 14:54:33 2024, max compression
+gzip compressed data, was "schedula-1.5.7.tar", last modified: Fri Apr 19 10:48:53 2024, max compression
```

## Comparing `schedula-1.5.6.tar` & `schedula-1.5.7.tar`

### file list

```diff
@@ -1,288 +1,291 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.521578 schedula-1.5.6/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2020-04-22 23:09:02.000000 schedula-1.5.6/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2020-04-22 23:09:02.000000 schedula-1.5.6/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-04-03 14:54:33.521445 schedula-1.5.6/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-03 14:51:38.000000 schedula-1.5.6/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.423327 schedula-1.5.6/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4300 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-03 14:51:38.000000 schedula-1.5.6/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-03 12:07:12.000000 schedula-1.5.6/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.425384 schedula-1.5.6/schedula/ext/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/autosummary.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.426362 schedula-1.5.6/schedula/ext/dispatcher/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/documenter.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/ext/dispatcher/graphviz.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.431119 schedula-1.5.6/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.432188 schedula-1.5.6/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17367 2024-03-30 08:05:12.000000 schedula-1.5.6/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/cst.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.432508 schedula-1.5.6/schedula/utils/des/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/des/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.433756 schedula-1.5.6/schedula/utils/drw/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/drw/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420059 schedula-1.5.6/schedula/utils/drw/index/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.435173 schedula-1.5.6/schedula/utils/drw/index/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/index/css/icon.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/css/index.css
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.436843 schedula-1.5.6/schedula/utils/drw/index/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap-treeview.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/d3-scale.v3.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/jquery-3.4.1.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/jquery.fullscreen.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2020-04-22 23:09:02.000000 schedula-1.5.6/schedula/utils/drw/index/js/sunburst-chart.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/drw/nodes.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.437245 schedula-1.5.6/schedula/utils/drw/templates/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/templates/index.html
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/drw/templates/render.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.437456 schedula-1.5.6/schedula/utils/drw/viz/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2023-11-19 09:38:55.000000 schedula-1.5.6/schedula/utils/drw/viz/viz.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/exc.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.442708 schedula-1.5.6/schedula/utils/form/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12042 2024-03-22 15:04:12.000000 schedula-1.5.6/schedula/utils/form/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/form/config.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1171 2024-03-22 15:04:12.000000 schedula-1.5.6/schedula/utils/form/json_secrets.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/form/mail.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13359 2024-03-22 16:24:55.000000 schedula-1.5.6/schedula/utils/form/server.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420478 schedula-1.5.6/schedula/utils/form/static/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420814 schedula-1.5.6/schedula/utils/form/static/schedula/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.448004 schedula-1.5.6/schedula/utils/form/static/schedula/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      837 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      185 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      251 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.448466 schedula-1.5.6/schedula/utils/form/static/schedula/forms/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2023-11-19 15:42:01.000000 schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-schema.json
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3421 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-ui.json
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.506291 schedula-1.5.6/schedula/utils/form/static/schedula/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1226 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4268 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      936 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1444 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1748.0df73428.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3521 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      311 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1831.7a4c7750.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7431 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12859 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3772 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4864 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2286.850702e1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4571 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3769 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4365 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2742.cef81b1c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468024 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10229 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19245 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11274 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10537 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11849 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7251 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4129.3e3e6e91.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5841 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6643 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      976 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5056 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3472 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4452.45bca48d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3347 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7078 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4673.aa83f5e0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16182 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5025.2850b7b4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3733 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1668 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5652.dde5ef02.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1962 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      734 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11589 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14429 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4647 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7293 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6753.e37ed964.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3702 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6836.43947ef9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   261511 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7193.528d18c4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8089 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3130 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3735 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37416 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/796.a7fc5105.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266679 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/7974.7e7de702.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      669 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8115.11a85e47.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8861 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1015 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3291 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8428.7d81c7b5.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28905 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8497.f11bc0ea.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13322 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8516.30c79314.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      336 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/853.c4b3a572.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11595 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12186 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7429 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4065 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3721 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      604 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432329 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/js/main.d401041d.js.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.512147 schedula-1.5.6/schedula/utils/form/static/schedula/media/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-04-03 12:52:57.000000 schedula-1.5.6/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.420971 schedula-1.5.6/schedula/utils/form/templates/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.512622 schedula-1.5.6/schedula/utils/form/templates/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4460 2024-03-14 10:09:53.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/base.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.513526 schedula-1.5.6/schedula/utils/form/templates/schedula/email/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-body-en.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-body-it.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2023-11-15 13:00:39.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/email/contact-subject.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2022-10-19 15:46:09.000000 schedula-1.5.6/schedula/utils/form/templates/schedula/index.html
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/imp.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.513721 schedula-1.5.6/schedula/utils/io/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/io/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.514036 schedula-1.5.6/schedula/utils/web/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-03-14 10:25:40.000000 schedula-1.5.6/schedula/utils/web/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.517130 schedula-1.5.6/schedula.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14353 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14964 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      990 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/requires.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-03 14:54:33.000000 schedula-1.5.6/schedula.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-03 14:54:33.521906 schedula-1.5.6/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7084 2024-03-14 10:25:40.000000 schedula-1.5.6/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-03 14:54:33.516773 schedula-1.5.6/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-03-14 10:25:40.000000 schedula-1.5.6/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.879416 schedula-1.5.7/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula-1.5.7/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula-1.5.7/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 10:48:53.879261 schedula-1.5.7/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 10:36:00.000000 schedula-1.5.7/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.832148 schedula-1.5.7/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula-1.5.7/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 10:36:00.000000 schedula-1.5.7/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula-1.5.7/schedula/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.833144 schedula-1.5.7/schedula/ext/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/autosummary.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.833565 schedula-1.5.7/schedula/ext/dispatcher/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/documenter.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/graphviz.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836198 schedula-1.5.7/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836636 schedula-1.5.7/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula-1.5.7/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/cst.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836757 schedula-1.5.7/schedula/utils/des/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/des/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.837103 schedula-1.5.7/schedula/utils/drw/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.829721 schedula-1.5.7/schedula/utils/drw/index/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.838232 schedula-1.5.7/schedula/utils/drw/index/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/icon.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/index.css
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839412 schedula-1.5.7/schedula/utils/drw/index/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap-treeview.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/d3-scale.v3.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/jquery-3.4.1.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/jquery.fullscreen.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/sunburst-chart.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/nodes.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839737 schedula-1.5.7/schedula/utils/drw/templates/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/templates/index.html
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/templates/render.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839894 schedula-1.5.7/schedula/utils/drw/viz/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/viz/viz.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/exc.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.842544 schedula-1.5.7/schedula/utils/form/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11497 2024-04-18 07:55:31.000000 schedula-1.5.7/schedula/utils/form/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6065 2024-04-19 10:04:16.000000 schedula-1.5.7/schedula/utils/form/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/config.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1986 2024-04-18 10:08:20.000000 schedula-1.5.7/schedula/utils/form/gapp.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1541 2024-04-18 07:56:48.000000 schedula-1.5.7/schedula/utils/form/json_secrets.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/mail.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13359 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/server.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830036 schedula-1.5.7/schedula/utils/form/static/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830413 schedula-1.5.7/schedula/utils/form/static/schedula/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.845370 schedula-1.5.7/schedula/utils/form/static/schedula/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      837 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      185 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      251 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.845641 schedula-1.5.7/schedula/utils/form/static/schedula/forms/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-schema.json
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-ui.json
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.870038 schedula-1.5.7/schedula/utils/form/static/schedula/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7227 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1224 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4265 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      936 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1441 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3519 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      329 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1831.6e43492c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7430 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12856 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3771 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4863 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4570 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4363 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468331 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10227 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19245 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11271 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10536 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11849 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5839 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6642 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      976 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5055 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3470 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3344 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7075 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16181 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3728 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1672 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1960 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      734 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11587 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4645 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7293 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3700 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8087 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3130 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37414 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266738 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14837 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8859 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1014 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3289 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28904 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13457 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      339 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/853.904196e2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11594 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12185 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7427 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4064 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3720 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      917 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      604 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432389 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873127 schedula-1.5.7/schedula/utils/form/static/schedula/media/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830564 schedula-1.5.7/schedula/utils/form/templates/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873380 schedula-1.5.7/schedula/utils/form/templates/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3610 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/base.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873777 schedula-1.5.7/schedula/utils/form/templates/schedula/email/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-body-en.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-body-it.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-subject.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/index.html
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/imp.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873909 schedula-1.5.7/schedula/utils/io/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/io/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.874037 schedula-1.5.7/schedula/utils/web/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/web/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.875069 schedula-1.5.7/schedula.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15005 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       46 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/entry_points.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1083 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/requires.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 10:48:53.879706 schedula-1.5.7/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7344 2024-04-19 10:12:23.000000 schedula-1.5.7/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.874710 schedula-1.5.7/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_setup.py
```

### Comparing `schedula-1.5.6/LICENSE.txt` & `schedula-1.5.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/PKG-INFO` & `schedula-1.5.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.6
+Version: 1.5.7
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
@@ -61,56 +61,65 @@
 Requires-Dist: docutils; extra == "form"
 Requires-Dist: flask-babel; extra == "form"
 Requires-Dist: flask-wtf; extra == "form"
 Requires-Dist: flask-principal; extra == "form"
 Requires-Dist: flask-security-too; extra == "form"
 Requires-Dist: flask-mail; extra == "form"
 Requires-Dist: stripe; extra == "form"
+Requires-Dist: click; extra == "form"
+Requires-Dist: click_log; extra == "form"
+Requires-Dist: gunicorn; extra == "form"
 Provides-Extra: sphinx
 Requires-Dist: sphinx>=7.2; extra == "sphinx"
 Requires-Dist: requests; extra == "sphinx"
 Requires-Dist: graphviz>=0.17; extra == "sphinx"
 Requires-Dist: regex; extra == "sphinx"
 Requires-Dist: flask; extra == "sphinx"
 Requires-Dist: Pygments; extra == "sphinx"
 Requires-Dist: jinja2; extra == "sphinx"
 Requires-Dist: docutils; extra == "sphinx"
 Provides-Extra: all
 Requires-Dist: Pygments; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: click_log; extra == "all"
 Requires-Dist: dill!=0.2.7; extra == "all"
 Requires-Dist: docutils; extra == "all"
 Requires-Dist: flask; extra == "all"
 Requires-Dist: flask-babel; extra == "all"
 Requires-Dist: flask-mail; extra == "all"
 Requires-Dist: flask-principal; extra == "all"
 Requires-Dist: flask-security-too; extra == "all"
 Requires-Dist: flask-sqlalchemy; extra == "all"
 Requires-Dist: flask-wtf; extra == "all"
 Requires-Dist: graphviz>=0.17; extra == "all"
+Requires-Dist: gunicorn; extra == "all"
 Requires-Dist: itsdangerous; extra == "all"
 Requires-Dist: jinja2; extra == "all"
 Requires-Dist: multiprocess; extra == "all"
 Requires-Dist: regex; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: rst2txt; extra == "all"
 Requires-Dist: sphinx>=7.2; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: stripe; extra == "all"
 Provides-Extra: dev
 Requires-Dist: Pygments; extra == "dev"
+Requires-Dist: click; extra == "dev"
+Requires-Dist: click_log; extra == "dev"
 Requires-Dist: dill!=0.2.7; extra == "dev"
 Requires-Dist: docutils; extra == "dev"
 Requires-Dist: flask; extra == "dev"
 Requires-Dist: flask-babel; extra == "dev"
 Requires-Dist: flask-mail; extra == "dev"
 Requires-Dist: flask-principal; extra == "dev"
 Requires-Dist: flask-security-too; extra == "dev"
 Requires-Dist: flask-sqlalchemy; extra == "dev"
 Requires-Dist: flask-wtf; extra == "dev"
 Requires-Dist: graphviz>=0.17; extra == "dev"
+Requires-Dist: gunicorn; extra == "dev"
 Requires-Dist: itsdangerous; extra == "dev"
 Requires-Dist: jinja2; extra == "dev"
 Requires-Dist: multiprocess; extra == "dev"
 Requires-Dist: regex; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: rst2txt; extra == "dev"
 Requires-Dist: sphinx>=7.2; extra == "dev"
@@ -126,14 +135,15 @@
 Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: polib; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: readthedocs-sphinx-ext; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ddt; extra == "dev"
 Requires-Dist: translators; extra == "dev"
+Requires-Dist: livereload>=2.6.3; extra == "dev"
 
 
 About schedula
 **************
 
 **schedula** is a dynamic flow-based programming environment for
 python, that handles automatically the control flow of the program.
```

### Comparing `schedula-1.5.6/README.rst` & `schedula-1.5.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.6
-:date:          2024-04-03 15:00:00
+:release:       1.5.7
+:date:          2024-04-19 12:30:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula-1.5.6/schedula/__init__.py` & `schedula-1.5.7/schedula/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 .. autosummary::
     :nosignatures:
     :toctree: toctree/schedula
 
     ~dispatcher
     ~utils
     ~ext
+    ~cli
 """
 import os
 import sys
 from ._version import *
 
 _all = {
     'Dispatcher': '.dispatcher',
```

### Comparing `schedula-1.5.6/schedula/dispatcher.py` & `schedula-1.5.7/schedula/dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/ext/autosummary.py` & `schedula-1.5.7/schedula/ext/autosummary.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/ext/dispatcher/__init__.py` & `schedula-1.5.7/schedula/ext/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/ext/dispatcher/documenter.py` & `schedula-1.5.7/schedula/ext/dispatcher/documenter.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/ext/dispatcher/graphviz.py` & `schedula-1.5.7/schedula/ext/dispatcher/graphviz.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/__init__.py` & `schedula-1.5.7/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/alg.py` & `schedula-1.5.7/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/asy/__init__.py` & `schedula-1.5.7/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/asy/executors.py` & `schedula-1.5.7/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/asy/factory.py` & `schedula-1.5.7/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/base.py` & `schedula-1.5.7/schedula/utils/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,17 +113,14 @@
             sites.add(webmap.site(view=run))
         elif run:
             return webmap.site(view=run)
         return webmap
 
     def form(self, depth=1, node_data=NONE, node_function=NONE, directory=None,
              sites=None, run=True, view=True, get_context=NONE, get_data=NONE,
-             edit_on_change='static/schedula/onChange/*.js',
-             pre_submit='static/schedula/preSubmit/*.js',
-             post_submit='static/schedula/postSubmit/*.js',
              subsite_idle_timeout=600, basic_app_config=None,
              stripe_event_handler=lambda event: None):
         """
         Creates a dispatcher Form Flask app.
 
         :param depth:
             Depth of sub-dispatch API. If negative all levels are configured.
@@ -158,26 +155,14 @@
             Function to pass extra data as form context.
         :type get_context: function | dict, optional
 
         :param get_data:
             Function to initialize the formdata.
         :type get_data: function | dict, optional
 
-        :param edit_on_change:
-            JS function to edit on the browser the formdata when value change.
-        :type edit_on_change: str | dict[str], optional
-
-        :param pre_submit:
-            JS function to edit on the browser the formdata before submitting.
-        :type pre_submit: str | dict[str], optional
-
-        :param post_submit:
-            JS function to edit on the browser server response after submision.
-        :type post_submit: str | dict[str], optional
-
         :param subsite_idle_timeout:
             Idle timeout of a debug subsite in seconds.
         :type subsite_idle_timeout: int, optional
 
         :param basic_app_config:
             Flask app config object.
         :type basic_app_config: object, optional
@@ -201,33 +186,17 @@
         formmap = FormMap()
         formmap.add_items(obj, workflow=False, depth=depth, **options)
         formmap.directory = directory
         formmap.idle_timeout = subsite_idle_timeout
         formmap.basic_app_config = basic_app_config
         formmap.stripe_event_handler = stripe_event_handler
         methods = {
-            'get_edit_on_change_func': edit_on_change,
-            'get_pre_submit_func': pre_submit,
-            'get_post_submit_func': post_submit
-        }
-        for k, v in methods.items():
-            if isinstance(v, str):
-                methods[k] = d = {}
-                v = osp.join(directory or '.', *v.replace('\\', '/').split('/'))
-                for fpath in glob.glob(v):
-                    with open(fpath) as f:
-                        d[f'/{osp.splitext(osp.basename(fpath))[0]}'] = f.read()
-                if '/' not in d and '/index' in d:
-                    d['/'] = d['/index']
-                elif not d:
-                    methods[k] = NONE
-        methods.update({
             'get_form_context': get_context,
             'get_form_data': get_data
-        })
+        }
         for k, v in methods.items():
             if v is not NONE:
                 setattr(formmap, f'_{k}', v)
         if sites is not None or run or view:
             site = formmap.site(view=view)
             site = run and not view and site.run() or site
             if sites is None:
```

### Comparing `schedula-1.5.6/schedula/utils/blue.py` & `schedula-1.5.7/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/cst.py` & `schedula-1.5.7/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/des/__init__.py` & `schedula-1.5.7/schedula/utils/des/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/__init__.py` & `schedula-1.5.7/schedula/utils/drw/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css` & `schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/css/bootstrap.min.css.map` & `schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/css/icon.css` & `schedula-1.5.7/schedula/utils/drw/index/css/icon.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/css/index.css` & `schedula-1.5.7/schedula/utils/drw/index/css/index.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap-treeview.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/bootstrap.min.js.map` & `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/d3-scale.v3.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/d3-scale.v3.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/jquery-3.4.1.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/jquery.fullscreen.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/jquery.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/index/js/sunburst-chart.min.js` & `schedula-1.5.7/schedula/utils/drw/index/js/sunburst-chart.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/nodes.py` & `schedula-1.5.7/schedula/utils/drw/nodes.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/templates/index.html` & `schedula-1.5.7/schedula/utils/drw/templates/index.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/templates/render.html` & `schedula-1.5.7/schedula/utils/drw/templates/render.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/drw/viz/viz.js` & `schedula-1.5.7/schedula/utils/drw/viz/viz.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/dsp.py` & `schedula-1.5.7/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/exc.py` & `schedula-1.5.7/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/form/__init__.py` & `schedula-1.5.7/schedula/utils/form/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 
 .. currentmodule:: schedula.utils.form
 
 .. autosummary::
     :nosignatures:
     :toctree: form/
 
+    cli
     config
+    gapp
+    json_secrets
     mail
     server
 """
 import io
 import os
 import gzip
 import glob
@@ -58,46 +61,15 @@
 }
 static_context = {
     k: v[:-3] if v.endswith('.gz') else v for k, v in static_context.items()
 }
 
 
 class FormMap(WebMap):
-    _get_edit_on_change_func = """
-    ({
-         formData,
-         formContext,
-         schema,
-         uiSchema,
-         csrf_token,
-         setFormData,
-         ...props
-    }) => (formData)
-    """
-    _get_pre_submit_func = """
-    ({
-         input,
-         formContext,
-         schema,
-         uiSchema,
-         csrf_token,
-         ...props
-    }) => (input)
-    """
-    _get_post_submit_func = """
-    ({
-         data,
-         input,
-         formContext,
-         schema,
-         uiSchema,
-         csrf_token,
-         ...props
-    }) => ({data})
-    """
+
     _get_basic_app_config = Config
 
     def get_form_context(self):
         context = default_get_form_context().copy()
         if hasattr(self, '_get_form_context'):
             context.update(self._get_form_context())
         return context
```

### Comparing `schedula-1.5.6/schedula/utils/form/config.py` & `schedula-1.5.7/schedula/utils/form/config.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/form/mail.py` & `schedula-1.5.7/schedula/utils/form/mail.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/form/server.py` & `schedula-1.5.7/schedula/utils/form/server.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1362.038687f8.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1362.038687f8.chunk.css", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz`

 * *Files 12% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1737.87abdd03.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1737.87abdd03.chunk.css", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2286.6e5fc492.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2286.6e5fc492.chunk.css", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9003.d2d6266b.chunk.css", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9003.d2d6266b.chunk.css", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/forms/index-schema.json` & `schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-schema.json`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz`

 * *Files 25% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1165.ff804d16.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1165.ff804d16.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1362.0594020f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1362.0594020f.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1431.780747e9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1431.780747e9.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1432.f3b34f42.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1432.f3b34f42.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1465.edd9ba38.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1465.edd9ba38.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1583.fbdd1527.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1583.fbdd1527.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1641.cc9646e9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1641.cc9646e9.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1642.5186d671.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1642.5186d671.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1656.c5fbd8dc.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1656.c5fbd8dc.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1678.b278cefb.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1678.b278cefb.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1724.d97efc34.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1724.d97efc34.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1737.13089dbe.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "1737.13089dbe.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2055.204f9b8c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2055.204f9b8c.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2128.9a07d096.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2128.9a07d096.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "218.37c2a3e8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "218.37c2a3e8.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "24.5f2a5395.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "24.5f2a5395.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2506.47c8c058.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2506.47c8c058.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2556.ab2f7391.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2556.ab2f7391.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz`

 * *Files 6% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2698.09529134.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2698.09529134.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2706.a995f39e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2706.a995f39e.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2742.cef81b1c.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz`

 * *Files 26% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2742.cef81b1c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2742.e2a045d8.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

#### Comparing `2742.cef81b1c.chunk.js` & `2742.e2a045d8.chunk.js`

##### js-beautify {}

```diff
@@ -162,15 +162,15 @@
                             d: "M942.2 486.2C847.4 286.5 704.1 186 512 186c-192.2 0-335.4 100.5-430.2 300.3a60.3 60.3 0 000 51.5C176.6 737.5 319.9 838 512 838c192.2 0 335.4-100.5 430.2-300.3 7.7-16.2 7.7-35 0-51.5zM512 766c-161.3 0-279.4-81.8-362.7-254C232.6 339.8 350.7 258 512 258c161.3 0 279.4 81.8 362.7 254C791.5 684.2 673.4 766 512 766zm-4-430c-97.2 0-176 78.8-176 176s78.8 176 176 176 176-78.8 176-176-78.8-176-176-176zm0 288c-61.9 0-112-50.1-112-112s50.1-112 112-112 112 50.1 112 112-50.1 112-112 112z"
                         }
                     }]
                 },
                 name: "eye",
                 theme: "outlined"
             };
-            var a = n(54291),
+            var a = n(8711),
                 i = function(e, t) {
                     return o.createElement(a.Z, (0, s.Z)({}, e, {
                         ref: t,
                         icon: r
                     }))
                 };
             const c = o.forwardRef(i)
@@ -194,15 +194,15 @@
                             d: "M928 160H96c-17.7 0-32 14.3-32 32v640c0 17.7 14.3 32 32 32h832c17.7 0 32-14.3 32-32V192c0-17.7-14.3-32-32-32zm-40 632H136V232h752v560zM610.3 476h123.4c1.3 0 2.3-3.6 2.3-8v-48c0-4.4-1-8-2.3-8H610.3c-1.3 0-2.3 3.6-2.3 8v48c0 4.4 1 8 2.3 8zm4.8 144h185.7c3.9 0 7.1-3.6 7.1-8v-48c0-4.4-3.2-8-7.1-8H615.1c-3.9 0-7.1 3.6-7.1 8v48c0 4.4 3.2 8 7.1 8zM224 673h43.9c4.2 0 7.6-3.3 7.9-7.5 3.8-50.5 46-90.5 97.2-90.5s93.4 40 97.2 90.5c.3 4.2 3.7 7.5 7.9 7.5H522a8 8 0 008-8.4c-2.8-53.3-32-99.7-74.6-126.1a111.8 111.8 0 0029.1-75.5c0-61.9-49.9-112-111.4-112s-111.4 50.1-111.4 112c0 29.1 11 55.5 29.1 75.5a158.09 158.09 0 00-74.6 126.1c-.4 4.6 3.2 8.4 7.8 8.4zm149-262c28.5 0 51.7 23.3 51.7 52s-23.2 52-51.7 52-51.7-23.3-51.7-52 23.2-52 51.7-52z"
                         }
                     }]
                 },
                 name: "idcard",
                 theme: "outlined"
             };
-            var a = n(54291),
+            var a = n(8711),
                 i = function(e, t) {
                     return o.createElement(a.Z, (0, s.Z)({}, e, {
                         ref: t,
                         icon: r
                     }))
                 };
             const c = o.forwardRef(i)
@@ -226,15 +226,15 @@
                             d: "M893.3 293.3L730.7 130.7c-7.5-7.5-16.7-13-26.7-16V112H144c-17.7 0-32 14.3-32 32v736c0 17.7 14.3 32 32 32h736c17.7 0 32-14.3 32-32V338.5c0-17-6.7-33.2-18.7-45.2zM384 184h256v104H384V184zm456 656H184V184h136v136c0 17.7 14.3 32 32 32h320c17.7 0 32-14.3 32-32V205.8l136 136V840zM512 442c-79.5 0-144 64.5-144 144s64.5 144 144 144 144-64.5 144-144-64.5-144-144-144zm0 224c-44.2 0-80-35.8-80-80s35.8-80 80-80 80 35.8 80 80-35.8 80-80 80z"
                         }
                     }]
                 },
                 name: "save",
                 theme: "outlined"
             };
-            var a = n(54291),
+            var a = n(8711),
                 i = function(e, t) {
                     return o.createElement(a.Z, (0, s.Z)({}, e, {
                         ref: t,
                         icon: r
                     }))
                 };
             const c = o.forwardRef(i)
@@ -295,15 +295,15 @@
                             d: "M508 624c-3.46 0-6.87-.16-10.25-.47l-52.82 52.82a176.09 176.09 0 00227.42-227.42l-52.82 52.82c.31 3.38.47 6.79.47 10.25a111.94 111.94 0 01-112 112z"
                         }
                     }]
                 },
                 name: "eye-invisible",
                 theme: "outlined"
             };
-            var f = n(54291),
+            var f = n(8711),
                 p = function(e, t) {
                     return s.createElement(f.Z, (0, d.Z)({}, e, {
                         ref: t,
                         icon: m
                     }))
                 };
             const v = s.forwardRef(p);
@@ -490,8 +490,8 @@
             var k = n(35583);
             const N = u.Z;
             N.Group = l, N.Search = S, N.TextArea = k.Z, N.Password = j;
             const B = N
         }
     }
 ]);
-//# sourceMappingURL=2742.cef81b1c.chunk.js.map
+//# sourceMappingURL=2742.e2a045d8.chunk.js.map
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz`

 * *Files 16% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "287.053696ba.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "287.053696ba.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "2894.d8c25e8b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "2894.d8c25e8b.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3052.40fbeb2c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3052.40fbeb2c.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3281.a4f1ba69.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3281.a4f1ba69.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3327.f5840c2f.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3327.f5840c2f.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3333.3da6381e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3333.3da6381e.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3457.a6f7a355.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3457.a6f7a355.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3642.27ee29bf.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3642.27ee29bf.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3676.1ee61f29.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3676.1ee61f29.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz`

 * *Files 12% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "3850.689e0ff9.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "3850.689e0ff9.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4093.1b358dc3.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4093.1b358dc3.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4095.87cc9b62.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4095.87cc9b62.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4337.8da858ce.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4337.8da858ce.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4452.45bca48d.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz`

 * *Files 14% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4452.45bca48d.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4452.ae121668.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

#### Comparing `4452.45bca48d.chunk.js` & `4452.ae121668.chunk.js`

##### js-beautify {}

```diff
@@ -173,15 +173,15 @@
                             d: "M942.2 486.2C847.4 286.5 704.1 186 512 186c-192.2 0-335.4 100.5-430.2 300.3a60.3 60.3 0 000 51.5C176.6 737.5 319.9 838 512 838c192.2 0 335.4-100.5 430.2-300.3 7.7-16.2 7.7-35 0-51.5zM512 766c-161.3 0-279.4-81.8-362.7-254C232.6 339.8 350.7 258 512 258c161.3 0 279.4 81.8 362.7 254C791.5 684.2 673.4 766 512 766zm-4-430c-97.2 0-176 78.8-176 176s78.8 176 176 176 176-78.8 176-176-78.8-176-176-176zm0 288c-61.9 0-112-50.1-112-112s50.1-112 112-112 112 50.1 112 112-50.1 112-112 112z"
                         }
                     }]
                 },
                 name: "eye",
                 theme: "outlined"
             };
-            var c = o(54291),
+            var c = o(8711),
                 s = function(e, t) {
                     return a.createElement(c.Z, (0, n.Z)({}, e, {
                         ref: t,
                         icon: r
                     }))
                 };
             const i = a.forwardRef(s)
@@ -205,15 +205,15 @@
                             d: "M400 317.7h73.9V656c0 4.4 3.6 8 8 8h60c4.4 0 8-3.6 8-8V317.7H624c6.7 0 10.4-7.7 6.3-12.9L518.3 163a8 8 0 00-12.6 0l-112 141.7c-4.1 5.3-.4 13 6.3 13zM878 626h-60c-4.4 0-8 3.6-8 8v154H214V634c0-4.4-3.6-8-8-8h-60c-4.4 0-8 3.6-8 8v198c0 17.7 14.3 32 32 32h684c17.7 0 32-14.3 32-32V634c0-4.4-3.6-8-8-8z"
                         }
                     }]
                 },
                 name: "upload",
                 theme: "outlined"
             };
-            var c = o(54291),
+            var c = o(8711),
                 s = function(e, t) {
                     return a.createElement(c.Z, (0, n.Z)({}, e, {
                         ref: t,
                         icon: r
                     }))
                 };
             const i = a.forwardRef(s)
@@ -391,8 +391,8 @@
             }), e.exports = function(e) {
                 for (var t = arguments.length, o = new Array(t > 1 ? t - 1 : 0), n = 1; n < t; n++) o[n - 1] = arguments[n];
                 return e.format(...o)
             }
         }
     }
 ]);
-//# sourceMappingURL=4452.45bca48d.chunk.js.map
+//# sourceMappingURL=4452.ae121668.chunk.js.map
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4459.6704ca6e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4459.6704ca6e.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4587.5ff7f02e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4587.5ff7f02e.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz`

 * *Files 10% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4672.f1f003ed.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4672.f1f003ed.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz`

 * *Files 6% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4786.f0dbe7a4.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4786.f0dbe7a4.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz`

 * *Files 10% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4906.d6a6dad2.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4906.d6a6dad2.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "4925.6cb145d6.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "4925.6cb145d6.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5255.baba9ad1.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5255.baba9ad1.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5349.d6abdf80.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5349.d6abdf80.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5415.96511657.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5415.96511657.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5459.ab6195a8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5459.ab6195a8.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5784.aa6dfd10.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5784.aa6dfd10.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz`

 * *Files 15% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5880.5ad7e40e.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5880.5ad7e40e.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "5959.d5ebe3fe.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "5959.d5ebe3fe.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6043.6bea23a4.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "6043.6bea23a4.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "654.98d33eb8.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "654.98d33eb8.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6855.c4d51fc1.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "6855.c4d51fc1.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz`

 * *Files 12% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6925.228697fa.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "6925.228697fa.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6938.c8986bc2.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "6938.c8986bc2.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz`

 * *Files 9% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "6984.ab1ec70c.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "6984.ab1ec70c.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7035.5a8c5d98.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7035.5a8c5d98.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7101.48b6eb7a.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7101.48b6eb7a.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7106.0babb553.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7106.0babb553.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz`

 * *Files 5% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7450.d618087b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7450.d618087b.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7522.bc15dd2d.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7522.bc15dd2d.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "78.d0c28d0b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "78.d0c28d0b.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "7828.8fdd74db.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "7828.8fdd74db.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8007.cbee9608.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "8007.cbee9608.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz`

 * *Files 10% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8119.038d4e91.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "8119.038d4e91.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "8703.743baf71.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "8703.743baf71.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "875.2593b9db.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "875.2593b9db.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9235.b2714593.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9235.b2714593.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9238.8ae8b0d0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9238.8ae8b0d0.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz`

 * *Files 2% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9367.127331a0.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9367.127331a0.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9419.1497cff3.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9419.1497cff3.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9517.d6983e61.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9517.d6983e61.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9665.8425fb6b.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9665.8425fb6b.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "9919.f339f893.chunk.js", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "9919.f339f893.chunk.js", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Black.cf56c1b149d0a5e8d7c6.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Black.cf56c1b149d0a5e8d7c6.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Bold.f80816a5455d171f948d.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Bold.f80816a5455d171f948d.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Italic.87f3afe16a8c3c370634.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Italic.87f3afe16a8c3c370634.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Light.333da16a3f3cc391d087.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Light.333da16a3f3cc391d087.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-LightItalic.c590382422f2742d788b.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-LightItalic.c590382422f2742d788b.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Medium.7c8d04cd831df3033c8a.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Medium.7c8d04cd831df3033c8a.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-MediumItalic.82736aaa11c64709055f.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-MediumItalic.82736aaa11c64709055f.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Regular.fc2b5060f7accec5cf74.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Regular.fc2b5060f7accec5cf74.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz`

 * *Files 0% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-Thin.a732a12eb07742232407.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-Thin.a732a12eb07742232407.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz`

 * *Files 1% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz` & `schedula-1.5.7/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz`

 * *Files 4% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "index.42119833dddefe38a9fa.cjs", last modified: Wed Apr  3 12:52:57 2024, from Unix
+gzip compressed data, was "index.42119833dddefe38a9fa.cjs", last modified: Thu Apr 18 21:33:38 2024, from Unix
```

### Comparing `schedula-1.5.6/schedula/utils/form/templates/schedula/base.html` & `schedula-1.5.7/schedula/utils/form/templates/schedula/base.html`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     {% block title %}
     <title>{% block title_name %}{{ name }}{% endblock %}</title>
     <link rel="shortcut icon"
           href="{{ url_for('static', filename='favicon.ico') }}"/>
     {% endblock %}
     {% block js %}
     <script src="{{ url_for('schedula.static', filename=main_js) }}"></script>
+    <script src="{{ url_for('schedula.static', filename='props/js/' + form_id + '.js') }}"></script>
     {% endblock %}
     {% block css %}
     <link href="{{ url_for('schedula.static', filename=main_css) }}"
           rel="stylesheet">
     {% endblock %}
 
     {% block alive_func %}
@@ -41,70 +42,28 @@
         }
 
         imAlive();
     </script>
     {% endif %}
     {% endblock %}
 
-    {% block edit_on_change_func %}
-    <script>
-        const editOnChange = {{ form.get_edit_on_change_func() | safe }};
-        /*({
-             formData,
-             formContext,
-             schema,
-             uiSchema,
-             csrf_token,
-             setFormData,
-             ...props
-         }) => (formData)
-        */
-    </script>
-    {% endblock %}
-
-    {% block pre_submit_func %}
-    <script>
-        const preSubmit = {{ form.get_pre_submit_func() | safe }};
-        /*({
-             input,
-             formContext,
-             schema,
-             uiSchema,
-             csrf_token,
-             ...props
-         }) => (input)
-        */
-    </script>
-    {% endblock %}
-
-    {% block post_submit_func %}
-    <script>
-        const postSubmit = {{ form.get_post_submit_func() | safe }};
-        /*({
-             data,
-             input,
-             formContext,
-             schema,
-             uiSchema,
-             csrf_token,
-             ...props
-         }) => (data)
-        */
-    </script>
-    {% endblock %}
     {% block js_onload %}
     <script defer="defer">
         function onLoad() {
             let name = "{{ form_id or 'index' }}",
                 url = "{{ url_for('api') }}",
+                {formContext: _formContext, ..._schedulaProps} = window.schedulaProps || {},
                 element = document.getElementById('root'),
                 forms_url = "{{ url_for('schedula.static', filename='forms') }}",
                 csrf_token = "{{ form.generate_csrf() }}",
-                formContext = JSON.parse('{{ form.get_form_context() | tojson | safe}}'),
                 formData = JSON.parse('{{ form.get_form_data() | tojson | safe}}');
+            let formContext = {
+                ..._formContext,
+                ...JSON.parse('{{ form.get_form_context() | tojson | safe}}')
+            }
             Promise.all([
                 fetch(`${forms_url}/${name}-schema.json`, {
                     headers: {
                         'Content-Type': 'application/json',
                         'Content-Encoding': 'gzip',
                         'Accept-Encoding': 'gzip'
                     }
@@ -120,19 +79,17 @@
                 schedula.renderForm({
                     element,
                     url,
                     name,
                     schema,
                     uiSchema,
                     csrf_token,
-                    formContext,
                     formData,
-                    editOnChange,
-                    preSubmit,
-                    postSubmit
+                    formContext,
+                    ..._schedulaProps
                 })
             });
         }
     </script>
     {% endblock %}
     {% endblock %}
 </head>
```

#### html2text {}

```diff
@@ -1,12 +1,9 @@
 {% block head %}
 {% block title %}
 {% endblock %} {% block js %}
 {% endblock %} {% block css %}
 {% endblock %} {% block alive_func %} {% if 'alive' in app.view_functions %}
-{% endif %} {% endblock %} {% block edit_on_change_func %}
-{% endblock %} {% block pre_submit_func %}
-{% endblock %} {% block post_submit_func %}
-{% endblock %} {% block js_onload %}
+{% endif %} {% endblock %} {% block js_onload %}
 {% endblock %} {% endblock %}
 {% block content %}
 {% endblock %}
```

### Comparing `schedula-1.5.6/schedula/utils/gen.py` & `schedula-1.5.7/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/graph.py` & `schedula-1.5.7/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/imp.py` & `schedula-1.5.7/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/io/__init__.py` & `schedula-1.5.7/schedula/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/sol.py` & `schedula-1.5.7/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/utl.py` & `schedula-1.5.7/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula/utils/web/__init__.py` & `schedula-1.5.7/schedula/utils/web/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/schedula.egg-info/PKG-INFO` & `schedula-1.5.7/schedula.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.6
+Version: 1.5.7
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.6
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
@@ -61,56 +61,65 @@
 Requires-Dist: docutils; extra == "form"
 Requires-Dist: flask-babel; extra == "form"
 Requires-Dist: flask-wtf; extra == "form"
 Requires-Dist: flask-principal; extra == "form"
 Requires-Dist: flask-security-too; extra == "form"
 Requires-Dist: flask-mail; extra == "form"
 Requires-Dist: stripe; extra == "form"
+Requires-Dist: click; extra == "form"
+Requires-Dist: click_log; extra == "form"
+Requires-Dist: gunicorn; extra == "form"
 Provides-Extra: sphinx
 Requires-Dist: sphinx>=7.2; extra == "sphinx"
 Requires-Dist: requests; extra == "sphinx"
 Requires-Dist: graphviz>=0.17; extra == "sphinx"
 Requires-Dist: regex; extra == "sphinx"
 Requires-Dist: flask; extra == "sphinx"
 Requires-Dist: Pygments; extra == "sphinx"
 Requires-Dist: jinja2; extra == "sphinx"
 Requires-Dist: docutils; extra == "sphinx"
 Provides-Extra: all
 Requires-Dist: Pygments; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: click_log; extra == "all"
 Requires-Dist: dill!=0.2.7; extra == "all"
 Requires-Dist: docutils; extra == "all"
 Requires-Dist: flask; extra == "all"
 Requires-Dist: flask-babel; extra == "all"
 Requires-Dist: flask-mail; extra == "all"
 Requires-Dist: flask-principal; extra == "all"
 Requires-Dist: flask-security-too; extra == "all"
 Requires-Dist: flask-sqlalchemy; extra == "all"
 Requires-Dist: flask-wtf; extra == "all"
 Requires-Dist: graphviz>=0.17; extra == "all"
+Requires-Dist: gunicorn; extra == "all"
 Requires-Dist: itsdangerous; extra == "all"
 Requires-Dist: jinja2; extra == "all"
 Requires-Dist: multiprocess; extra == "all"
 Requires-Dist: regex; extra == "all"
 Requires-Dist: requests; extra == "all"
 Requires-Dist: rst2txt; extra == "all"
 Requires-Dist: sphinx>=7.2; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
 Requires-Dist: stripe; extra == "all"
 Provides-Extra: dev
 Requires-Dist: Pygments; extra == "dev"
+Requires-Dist: click; extra == "dev"
+Requires-Dist: click_log; extra == "dev"
 Requires-Dist: dill!=0.2.7; extra == "dev"
 Requires-Dist: docutils; extra == "dev"
 Requires-Dist: flask; extra == "dev"
 Requires-Dist: flask-babel; extra == "dev"
 Requires-Dist: flask-mail; extra == "dev"
 Requires-Dist: flask-principal; extra == "dev"
 Requires-Dist: flask-security-too; extra == "dev"
 Requires-Dist: flask-sqlalchemy; extra == "dev"
 Requires-Dist: flask-wtf; extra == "dev"
 Requires-Dist: graphviz>=0.17; extra == "dev"
+Requires-Dist: gunicorn; extra == "dev"
 Requires-Dist: itsdangerous; extra == "dev"
 Requires-Dist: jinja2; extra == "dev"
 Requires-Dist: multiprocess; extra == "dev"
 Requires-Dist: regex; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: rst2txt; extra == "dev"
 Requires-Dist: sphinx>=7.2; extra == "dev"
@@ -126,14 +135,15 @@
 Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: polib; extra == "dev"
 Requires-Dist: requests; extra == "dev"
 Requires-Dist: readthedocs-sphinx-ext; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ddt; extra == "dev"
 Requires-Dist: translators; extra == "dev"
+Requires-Dist: livereload>=2.6.3; extra == "dev"
 
 
 About schedula
 **************
 
 **schedula** is a dynamic flow-based programming environment for
 python, that handles automatically the control flow of the program.
```

### Comparing `schedula-1.5.6/schedula.egg-info/SOURCES.txt` & `schedula-1.5.7/schedula.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 AUTHORS.rst
 LICENSE.txt
 README.rst
 setup.cfg
 setup.py
 schedula/__init__.py
 schedula/_version.py
+schedula/cli.py
 schedula/dispatcher.py
 schedula.egg-info/PKG-INFO
 schedula.egg-info/SOURCES.txt
 schedula.egg-info/dependency_links.txt
+schedula.egg-info/entry_points.txt
 schedula.egg-info/requires.txt
 schedula.egg-info/top_level.txt
 schedula/ext/__init__.py
 schedula/ext/autosummary.py
 schedula/ext/dispatcher/__init__.py
 schedula/ext/dispatcher/documenter.py
 schedula/ext/dispatcher/graphviz.py
@@ -45,15 +47,17 @@
 schedula/utils/drw/index/js/jquery-3.4.1.min.js
 schedula/utils/drw/index/js/jquery.fullscreen.min.js
 schedula/utils/drw/index/js/sunburst-chart.min.js
 schedula/utils/drw/templates/index.html
 schedula/utils/drw/templates/render.html
 schedula/utils/drw/viz/viz.js
 schedula/utils/form/__init__.py
+schedula/utils/form/cli.py
 schedula/utils/form/config.py
+schedula/utils/form/gapp.py
 schedula/utils/form/json_secrets.py
 schedula/utils/form/mail.py
 schedula/utils/form/server.py
 schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
 schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
 schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
 schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
@@ -71,171 +75,170 @@
 schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
 schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
 schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
 schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
 schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
 schedula/utils/form/static/schedula/forms/index-schema.json
 schedula/utils/form/static/schedula/forms/index-ui.json
+schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz
 schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
-schedula/utils/form/static/schedula/js/1177.950ebcc8.chunk.js.gz
+schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz
 schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
-schedula/utils/form/static/schedula/js/1320.8d42e1b4.chunk.js.gz
+schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz
 schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
 schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
 schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
 schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
 schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
 schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
 schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
 schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
 schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
 schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
 schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
 schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
 schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
 schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
-schedula/utils/form/static/schedula/js/1748.0df73428.chunk.js.gz
-schedula/utils/form/static/schedula/js/183.76a6294f.chunk.js.gz
-schedula/utils/form/static/schedula/js/1831.7a4c7750.chunk.js.gz
-schedula/utils/form/static/schedula/js/1973.bcd66253.chunk.js.gz
+schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz
+schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz
+schedula/utils/form/static/schedula/js/1831.6e43492c.chunk.js.gz
+schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz
 schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
 schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
-schedula/utils/form/static/schedula/js/2120.8ea1a31a.chunk.js.gz
+schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz
 schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
 schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
-schedula/utils/form/static/schedula/js/2256.c3de48fa.chunk.js.gz
-schedula/utils/form/static/schedula/js/2286.850702e1.chunk.js.gz
+schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz
+schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz
 schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
 schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
 schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
 schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
 schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
 schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
-schedula/utils/form/static/schedula/js/268.deedefec.chunk.js.gz
+schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz
 schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
 schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
-schedula/utils/form/static/schedula/js/2723.e492696d.chunk.js.gz
-schedula/utils/form/static/schedula/js/2742.cef81b1c.chunk.js.gz
-schedula/utils/form/static/schedula/js/2768.93ab5524.chunk.js.gz
+schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz
+schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz
+schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz
 schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
 schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
-schedula/utils/form/static/schedula/js/3070.25639b4f.chunk.js.gz
+schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
 schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
 schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
 schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
 schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
 schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
 schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
 schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
 schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
 schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
 schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
 schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
-schedula/utils/form/static/schedula/js/368.9a0bfb9a.chunk.js.gz
+schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz
 schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
 schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
-schedula/utils/form/static/schedula/js/4048.6f416a19.chunk.js.gz
+schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz
 schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
 schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
-schedula/utils/form/static/schedula/js/4129.3e3e6e91.chunk.js.gz
-schedula/utils/form/static/schedula/js/414.56817ff7.chunk.js.gz
+schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
-schedula/utils/form/static/schedula/js/4279.d5144a2b.chunk.js.gz
+schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz
 schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
 schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
-schedula/utils/form/static/schedula/js/4438.acbb2994.chunk.js.gz
-schedula/utils/form/static/schedula/js/4452.45bca48d.chunk.js.gz
+schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz
+schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz
 schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
 schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
 schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
-schedula/utils/form/static/schedula/js/4596.53d31027.chunk.js.gz
+schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz
 schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
-schedula/utils/form/static/schedula/js/4673.aa83f5e0.chunk.js.gz
+schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz
 schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
 schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
 schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
 schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
-schedula/utils/form/static/schedula/js/5025.2850b7b4.chunk.js.gz
+schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz
 schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
 schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
-schedula/utils/form/static/schedula/js/5097.04da753b.chunk.js.gz
+schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz
 schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
 schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
 schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
 schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
 schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
-schedula/utils/form/static/schedula/js/5652.dde5ef02.chunk.js.gz
-schedula/utils/form/static/schedula/js/5672.d78485cb.chunk.js.gz
+schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz
+schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz
 schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
 schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
-schedula/utils/form/static/schedula/js/5836.722242c0.chunk.js.gz
+schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz
 schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
 schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
 schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
 schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
-schedula/utils/form/static/schedula/js/608.60f30d1f.chunk.js.gz
-schedula/utils/form/static/schedula/js/6085.d41a2240.chunk.js.gz
+schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz
 schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
-schedula/utils/form/static/schedula/js/6474.6af0dc33.chunk.js.gz
+schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz
 schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
-schedula/utils/form/static/schedula/js/6753.e37ed964.chunk.js.gz
+schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz
 schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
-schedula/utils/form/static/schedula/js/6836.43947ef9.chunk.js.gz
+schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz
 schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
 schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
 schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
 schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
 schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
 schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
 schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
 schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
-schedula/utils/form/static/schedula/js/7193.528d18c4.chunk.js.gz
-schedula/utils/form/static/schedula/js/7435.8ac4b848.chunk.js.gz
+schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz
 schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
 schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
 schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
-schedula/utils/form/static/schedula/js/7565.867674bc.chunk.js.gz
+schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz
 schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
 schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
-schedula/utils/form/static/schedula/js/796.a7fc5105.chunk.js.gz
-schedula/utils/form/static/schedula/js/7974.7e7de702.chunk.js.gz
+schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz
+schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz
 schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
-schedula/utils/form/static/schedula/js/8115.11a85e47.chunk.js.gz
+schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz
 schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
-schedula/utils/form/static/schedula/js/8148.e27d34a2.chunk.js.gz
-schedula/utils/form/static/schedula/js/8191.a6547494.chunk.js.gz
-schedula/utils/form/static/schedula/js/8259.439eef4a.chunk.js.gz
+schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz
+schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz
+schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz
 schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
-schedula/utils/form/static/schedula/js/8428.7d81c7b5.chunk.js.gz
-schedula/utils/form/static/schedula/js/8497.f11bc0ea.chunk.js.gz
-schedula/utils/form/static/schedula/js/8516.30c79314.chunk.js.gz
-schedula/utils/form/static/schedula/js/853.c4b3a572.chunk.js.gz
-schedula/utils/form/static/schedula/js/8531.1c721013.chunk.js.gz
-schedula/utils/form/static/schedula/js/8583.baa4f5a0.chunk.js.gz
-schedula/utils/form/static/schedula/js/8698.5bb1b696.chunk.js.gz
+schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz
+schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz
+schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz
+schedula/utils/form/static/schedula/js/853.904196e2.chunk.js.gz
+schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz
+schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz
+schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz
 schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
 schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
 schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
 schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
 schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
-schedula/utils/form/static/schedula/js/9009.78b5479a.chunk.js.gz
+schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz
 schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
-schedula/utils/form/static/schedula/js/9196.312a3d80.chunk.js.gz
+schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz
 schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
 schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
 schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
 schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
 schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
 schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
+schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz
 schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
 schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
 schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
-schedula/utils/form/static/schedula/js/main.d401041d.js.gz
+schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz
 schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
```

### Comparing `schedula-1.5.6/schedula.egg-info/requires.txt` & `schedula-1.5.7/schedula.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 
 [all]
 Pygments
+click
+click_log
 dill!=0.2.7
 docutils
 flask
 flask-babel
 flask-mail
 flask-principal
 flask-security-too
 flask-sqlalchemy
 flask-wtf
 graphviz>=0.17
+gunicorn
 itsdangerous
 jinja2
 multiprocess
 regex
 requests
 rst2txt
 sphinx>=7.2
 sqlalchemy
 stripe
 
 [dev]
 Pygments
+click
+click_log
 dill!=0.2.7
 docutils
 flask
 flask-babel
 flask-mail
 flask-principal
 flask-security-too
 flask-sqlalchemy
 flask-wtf
 graphviz>=0.17
+gunicorn
 itsdangerous
 jinja2
 multiprocess
 regex
 requests
 rst2txt
 sphinx>=7.2
@@ -50,14 +56,15 @@
 sphinxcontrib-restbuilder
 coveralls
 polib
 readthedocs-sphinx-ext
 twine
 ddt
 translators
+livereload>=2.6.3
 
 [form]
 requests
 regex
 flask
 itsdangerous
 rst2txt
@@ -66,14 +73,17 @@
 docutils
 flask-babel
 flask-wtf
 flask-principal
 flask-security-too
 flask-mail
 stripe
+click
+click_log
+gunicorn
 
 [io]
 dill!=0.2.7
 
 [parallel]
 multiprocess
```

### Comparing `schedula-1.5.6/setup.py` & `schedula-1.5.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,41 +87,49 @@
             'requests', 'graphviz>=0.17', 'regex', 'flask', 'Pygments',
             'jinja2', 'docutils'
         ]
     }
     extras['form'] = extras['web'] + [
         'itsdangerous', 'rst2txt', 'flask-sqlalchemy', 'sqlalchemy', 'docutils',
         'flask-babel', 'flask-wtf', 'flask-principal', 'flask-security-too',
-        'flask-mail', 'stripe'
+        'flask-mail', 'stripe', 'click', 'click_log', 'gunicorn'
     ]
     extras['sphinx'] = ['sphinx>=7.2'] + extras['plot']
     extras['all'] = sorted(functools.reduce(set.union, extras.values(), set()))
     extras['dev'] = extras['all'] + [
         'wheel', 'sphinx>=7.2', 'gitchangelog', 'mako', 'sphinx_rtd_theme',
         'setuptools>=36.0.1', 'sphinxcontrib-restbuilder', 'coveralls', 'polib',
         'requests', 'readthedocs-sphinx-ext', 'twine', 'ddt', 'translators',
+        'livereload>=2.6.3'
     ]
     exclude = [
         'doc', 'doc.*',
         'tests', 'tests.*',
         'examples', 'examples.*',
         'micropython', 'micropython.*',
         'requirements', 'binder', 'bin'
     ]
+    kw = {'entry_points': {
+        'console_scripts': [
+            '%(p)s = %(p)s.cli:cli' % {'p': name},
+        ]
+    }}
     if core:
         exclude.extend([
             'schedula.ext', 'schedula.ext.*',
             'schedula.utils.io', 'schedula.utils.io.*',
             'schedula.utils.drw', 'schedula.utils.drw.*',
             'schedula.utils.web', 'schedula.utils.web.*',
             'schedula.utils.form', 'schedula.utils.form.*',
             'schedula.utils.des', 'schedula.utils.des.*',
+            'schedula.cli',
         ])
         name = '%s-core' % name
         extras = {}
+        kw.pop('entry_points')
     long_description = ''
     if os.environ.get('ENABLE_SETUP_LONG_DESCRIPTION') == 'TRUE':
         try:
             long_description = get_long_description(core=core)
             print('LONG DESCRIPTION ENABLED!')
         except Exception as ex:
             print('LONG DESCRIPTION ERROR:\n %r', ex)
@@ -179,9 +187,10 @@
                 'templates/schedula/*', 'static/schedula/js/*.js.gz',
                 'static/schedula/css/*.css.gz',
                 'static/schedula/media/*.gz',
                 'static/schedula/forms/*',
                 'templates/schedula/*',
                 'templates/schedula/email/*'
             ]
-        }
+        },
+        **kw
     )
```

### Comparing `schedula-1.5.6/tests/test_dispatcher.py` & `schedula-1.5.7/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/tests/test_import.py` & `schedula-1.5.7/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/tests/test_micropython.py` & `schedula-1.5.7/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/tests/test_readme.py` & `schedula-1.5.7/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.6/tests/test_setup.py` & `schedula-1.5.7/tests/test_setup.py`

 * *Files identical despite different names*

