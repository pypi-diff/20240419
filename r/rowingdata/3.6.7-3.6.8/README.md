# Comparing `tmp/rowingdata-3.6.7.tar.gz` & `tmp/rowingdata-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rowingdata-3.6.7.tar", last modified: Sat Apr 13 07:15:45 2024, max compression
+gzip compressed data, was "rowingdata-3.6.8.tar", last modified: Fri Apr 19 15:32:56 2024, max compression
```

## Comparing `rowingdata-3.6.7.tar` & `rowingdata-3.6.8.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/
--rw-r--r--   0 sander    (1000) sander    (1000)     1074 2023-06-04 14:45:11.000000 rowingdata-3.6.7/LICENSE
--rw-r--r--   0 sander    (1000) sander    (1000)      276 2023-06-04 14:45:11.000000 rowingdata-3.6.7/MANIFEST.in
--rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-13 07:15:45.993515 rowingdata-3.6.7/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)    31386 2023-06-04 14:45:11.000000 rowingdata-3.6.7/README.rst
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.960181 rowingdata-3.6.7/bin/
--rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/crewnerddata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2933658 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/crewnerddata.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    53177 2023-06-04 14:45:11.000000 rowingdata-3.6.7/bin/testdata.csv
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.953515 rowingdata-3.6.7/docs/
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.956848 rowingdata-3.6.7/docs/_build/
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.960181 rowingdata-3.6.7/docs/_build/html/
--rw-r--r--   0 sander    (1000) sander    (1000)      166 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/.buildinfo
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.963515 rowingdata-3.6.7/docs/_build/html/_images/
--rw-r--r--   0 sander    (1000) sander    (1000)   124024 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/2x20min.png
--rw-r--r--   0 sander    (1000) sander    (1000)    85796 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/editrower.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)   156560 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/greghoc.png
--rw-r--r--   0 sander    (1000) sander    (1000)   118169 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/image001.png
--rw-r--r--   0 sander    (1000) sander    (1000)    42789 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/otwlogbook.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    59925 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/otwscreenshot.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    58348 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/screenshot.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)    37995 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/screenshotlogbook.JPG
--rw-r--r--   0 sander    (1000) sander    (1000)   156147 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_images/woensdag.png
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.963515 rowingdata-3.6.7/docs/_build/html/_sources/
--rw-r--r--   0 sander    (1000) sander    (1000)      463 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/index.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       67 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/modules.txt
--rw-r--r--   0 sander    (1000) sander    (1000)     3149 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_sources/rowingdata.txt
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.966848 rowingdata-3.6.7/docs/_build/html/_static/
--rw-r--r--   0 sander    (1000) sander    (1000)      673 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/ajax-loader.gif
--rw-r--r--   0 sander    (1000) sander    (1000)    10507 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/alabaster.css
--rw-r--r--   0 sander    (1000) sander    (1000)     9740 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/basic.css
--rw-r--r--   0 sander    (1000) sander    (1000)     3500 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment-bright.png
--rw-r--r--   0 sander    (1000) sander    (1000)     3578 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment-close.png
--rw-r--r--   0 sander    (1000) sander    (1000)     3445 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/comment.png
--rw-r--r--   0 sander    (1000) sander    (1000)       42 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/custom.css
--rw-r--r--   0 sander    (1000) sander    (1000)     8166 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/doctools.js
--rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/down-pressed.png
--rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/down.png
--rw-r--r--   0 sander    (1000) sander    (1000)      358 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/file.png
--rw-r--r--   0 sander    (1000) sander    (1000)   282766 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/jquery-1.11.1.js
--rw-r--r--   0 sander    (1000) sander    (1000)    95786 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/jquery.js
--rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/minus.png
--rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/plus.png
--rw-r--r--   0 sander    (1000) sander    (1000)     4149 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/pygments.css
--rw-r--r--   0 sander    (1000) sander    (1000)    18862 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 sander    (1000) sander    (1000)    35168 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 sander    (1000) sander    (1000)    12140 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/underscore.js
--rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/up-pressed.png
--rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/up.png
--rw-r--r--   0 sander    (1000) sander    (1000)    25351 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/_static/websupport.js
--rw-r--r--   0 sander    (1000) sander    (1000)    25780 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/genindex.html
--rw-r--r--   0 sander    (1000) sander    (1000)    68960 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/index.html
--rw-r--r--   0 sander    (1000) sander    (1000)     6140 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/modules.html
--rw-r--r--   0 sander    (1000) sander    (1000)     1101 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/objects.inv
--rw-r--r--   0 sander    (1000) sander    (1000)     7330 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/py-modindex.html
--rw-r--r--   0 sander    (1000) sander    (1000)    58474 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/rowingdata.html
--rw-r--r--   0 sander    (1000) sander    (1000)     3164 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/search.html
--rw-r--r--   0 sander    (1000) sander    (1000)    17380 2023-06-04 14:45:11.000000 rowingdata-3.6.7/docs/_build/html/searchindex.js
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.970181 rowingdata-3.6.7/rowingdata/
--rw-r--r--   0 sander    (1000) sander    (1000)       27 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/__init__.py
--rw-r--r--   0 sander    (1000) sander    (1000)       36 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/__main__.py
--rw-r--r--   0 sander    (1000) sander    (1000)      303 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/boatedit.py
--rw-r--r--   0 sander    (1000) sander    (1000)     6404 2024-04-13 07:15:29.000000 rowingdata-3.6.7/rowingdata/checkdatafiles.py
--rw-r--r--   0 sander    (1000) sander    (1000)      425 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/copystats.py
--rw-r--r--   0 sander    (1000) sander    (1000)      758 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/crewnerdplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      771 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/crewnerdplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)    98961 2024-04-13 07:15:29.000000 rowingdata-3.6.7/rowingdata/csvparsers.py
--rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdataplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      610 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdataplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      623 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergdatatotcx.py
--rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergstickplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergstickplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      628 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/ergsticktotcx.py
--rw-r--r--   0 sander    (1000) sander    (1000)     1491 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/gpxtools.py
--rw-r--r--   0 sander    (1000) sander    (1000)     5327 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/gpxwrite.py
--rw-r--r--   0 sander    (1000) sander    (1000)      429 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/konkatenaadje.py
--rw-r--r--   0 sander    (1000) sander    (1000)    13014 2024-02-15 15:52:54.000000 rowingdata-3.6.7/rowingdata/laptesting.py
--rw-r--r--   0 sander    (1000) sander    (1000)    22121 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/obsolete.py
--rw-r--r--   0 sander    (1000) sander    (1000)    23514 2023-11-18 13:14:27.000000 rowingdata-3.6.7/rowingdata/otherparsers.py
--rw-r--r--   0 sander    (1000) sander    (1000)      587 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_plot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      521 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_plottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      569 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsled_desktop_toc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      508 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      522 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      441 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/painsledtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      315 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/roweredit.py
--rw-r--r--   0 sander    (1000) sander    (1000)   243331 2024-04-13 07:15:33.000000 rowingdata-3.6.7/rowingdata/rowingdata.py
--rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/rowproplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      609 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/rowproplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      613 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      691 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/speedcoachtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)      694 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplot.py
--rw-r--r--   0 sander    (1000) sander    (1000)      700 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplot_nogeo.py
--rw-r--r--   0 sander    (1000) sander    (1000)      683 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplottime.py
--rw-r--r--   0 sander    (1000) sander    (1000)      689 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxplottime_nogeo.py
--rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/tcxtoc2.py
--rw-r--r--   0 sander    (1000) sander    (1000)    14568 2023-11-21 09:46:06.000000 rowingdata-3.6.7/rowingdata/tcxtools.py
--rw-r--r--   0 sander    (1000) sander    (1000)     7714 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/trainingparser.py
--rw-r--r--   0 sander    (1000) sander    (1000)     3676 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/utils.py
--rw-r--r--   0 sander    (1000) sander    (1000)     1095 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/windcorrected.py
--rw-r--r--   0 sander    (1000) sander    (1000)    10102 2023-06-04 14:45:11.000000 rowingdata-3.6.7/rowingdata/writetcx.py
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/rowingdata.egg-info/
--rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/PKG-INFO
--rw-r--r--   0 sander    (1000) sander    (1000)     5562 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/SOURCES.txt
--rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/dependency_links.txt
--rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:56:39.000000 rowingdata-3.6.7/rowingdata.egg-info/not-zip-safe
--rw-r--r--   0 sander    (1000) sander    (1000)      185 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/requires.txt
--rw-r--r--   0 sander    (1000) sander    (1000)       11 2024-04-13 07:15:45.000000 rowingdata-3.6.7/rowingdata.egg-info/top_level.txt
--rw-r--r--   0 sander    (1000) sander    (1000)      202 2024-04-13 07:15:45.993515 rowingdata-3.6.7/setup.cfg
--rw-r--r--   0 sander    (1000) sander    (1000)     3846 2023-06-04 14:45:11.000000 rowingdata-3.6.7/setup.py
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/testdata/
--rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2016-03-25-0758.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   416618 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2016-03-25-0758_data.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    56355 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/2x20min_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    17496 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/3km_cd_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   539777 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/EUBoatCoach.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    97777 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/EmpowerSpeedCoachForce.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    72367 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NKEmporfromgreg.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   111860 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NKLiNKv130.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2827124 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/NoHR.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    70850 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/PainsledForce.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   104085 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   124341 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_interval.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    63080 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/RP_testdata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    98860 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpdCoach2_imp_inconsistent.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   159697 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpdCoachAmbiguous.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    62781 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach GPS Workout.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    17242 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2Link_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   185339 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2Linkv1.27.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    12146 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/SpeedCoach2v2.12.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     4976 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/Speedcoach2example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    53949 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/aritmo.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   459974 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc1.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   340372 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   365508 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/bc3.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    18887 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    95234 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach_fixed_distance.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   520154 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/boatcoach_otw.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    74347 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/correctedpainsled.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     5461 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/coxmate.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  1479971 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerd_interval.csv
--rw-r--r--   0 sander    (1000) sander    (1000)      381 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)  2945286 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   420603 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/crewnerddata_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)      453 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/cumvalues.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7424 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergdata_example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    11261 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergdata_example.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   462959 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   262276 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)    40411 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   231959 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ergstick_o.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   378971 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   416716 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/example_data.csv
--rw-r--r--   0 sander    (1000) sander    (1000)       17 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/faketcx.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    64254 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/float.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23400 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/herodata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   215236 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/humon.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   157127 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/impeller_empower.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   484172 2023-11-18 12:40:31.000000 rowingdata-3.6.7/testdata/invalidchar.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   115182 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/kinomap.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   397003 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/mystery.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   792595 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/nk_logbook.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    56673 2023-11-18 13:14:27.000000 rowingdata-3.6.7/testdata/painsled.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   369891 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_desktop_example.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    41434 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_out_data.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   923421 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    76485 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_left.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   366614 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_new.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   277062 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_right.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   511961 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/quiske_per_stroke_seat.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    20254 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/recover.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   106145 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/ritmointervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    14216 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowingdata_eth.csv
--rw-r--r--   0 sander    (1000) sander    (1000)  2744646 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowinginmotionexample.TCX
--rw-r--r--   0 sander    (1000) sander    (1000)   657715 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowinginmotionexample.TCX_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   184978 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowperfect.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     4490 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowpro5.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   144225 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rowpro_carrick.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   253794 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3_curve.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   420248 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3intervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   417209 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp3intervals2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    85870 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/rp_out.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    41141 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/smartrow.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    34271 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/smartrow_intervals.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    31104 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/spdcoach2noheader.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    13731 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoach2test2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7840 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoach3test3.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    28352 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoachexample.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23429 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/speedcoachexample.csv_o.CSV
--rw-r--r--   0 sander    (1000) sander    (1000)   422653 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/summarytest.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    11130 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata_part1.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     9315 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testdata_part2.csv
--rw-r--r--   0 sander    (1000) sander    (1000)     7061 2024-04-13 07:15:29.000000 rowingdata-3.6.7/testdata/testdatasummary.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    19849 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testlapidx.csv
--rw-r--r--   0 sander    (1000) sander    (1000)   427961 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testtcs_210614.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    51127 2024-04-13 07:12:19.000000 rowingdata-3.6.7/testdata/testtcx.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)   427951 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/testtcx_210614.tcx
--rw-r--r--   0 sander    (1000) sander    (1000)    74249 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/tim.csv
--rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.7/testdata/划船.csv
-drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-13 07:15:45.993515 rowingdata-3.6.7/tests/
--rw-r--r--   0 sander    (1000) sander    (1000)    27734 2024-04-13 07:15:29.000000 rowingdata-3.6.7/tests/test_rowingdata.py
--rw-r--r--   0 sander    (1000) sander    (1000)     3424 2023-06-04 14:45:11.000000 rowingdata-3.6.7/tests/testparser.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.082646 rowingdata-3.6.8/
+-rw-r--r--   0 sander    (1000) sander    (1000)     1074 2023-06-04 14:45:11.000000 rowingdata-3.6.8/LICENSE
+-rw-r--r--   0 sander    (1000) sander    (1000)      276 2023-06-04 14:45:11.000000 rowingdata-3.6.8/MANIFEST.in
+-rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-19 15:32:56.082646 rowingdata-3.6.8/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)    31386 2023-06-04 14:45:11.000000 rowingdata-3.6.8/README.rst
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.049312 rowingdata-3.6.8/bin/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.8/bin/crewnerddata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2933658 2023-06-04 14:45:11.000000 rowingdata-3.6.8/bin/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    53177 2023-06-04 14:45:11.000000 rowingdata-3.6.8/bin/testdata.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.045979 rowingdata-3.6.8/docs/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.045979 rowingdata-3.6.8/docs/_build/
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.052646 rowingdata-3.6.8/docs/_build/html/
+-rw-r--r--   0 sander    (1000) sander    (1000)      166 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/.buildinfo
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.055979 rowingdata-3.6.8/docs/_build/html/_images/
+-rw-r--r--   0 sander    (1000) sander    (1000)   124024 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/2x20min.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    85796 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/editrower.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156560 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/greghoc.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   118169 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/image001.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    42789 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/otwlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    59925 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/otwscreenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    58348 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/screenshot.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)    37995 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/screenshotlogbook.JPG
+-rw-r--r--   0 sander    (1000) sander    (1000)   156147 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_images/woensdag.png
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.055979 rowingdata-3.6.8/docs/_build/html/_sources/
+-rw-r--r--   0 sander    (1000) sander    (1000)      463 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_sources/index.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       67 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_sources/modules.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)     3149 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_sources/rowingdata.txt
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.059312 rowingdata-3.6.8/docs/_build/html/_static/
+-rw-r--r--   0 sander    (1000) sander    (1000)      673 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/ajax-loader.gif
+-rw-r--r--   0 sander    (1000) sander    (1000)    10507 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/alabaster.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     9740 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/basic.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     3500 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/comment-bright.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3578 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/comment-close.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     3445 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/comment.png
+-rw-r--r--   0 sander    (1000) sander    (1000)       42 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/custom.css
+-rw-r--r--   0 sander    (1000) sander    (1000)     8166 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/down-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      347 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/down.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      358 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/file.png
+-rw-r--r--   0 sander    (1000) sander    (1000)   282766 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/jquery-1.11.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    95786 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/minus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      173 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/plus.png
+-rw-r--r--   0 sander    (1000) sander    (1000)     4149 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 sander    (1000) sander    (1000)    18862 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    35168 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    12140 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/up-pressed.png
+-rw-r--r--   0 sander    (1000) sander    (1000)      345 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/up.png
+-rw-r--r--   0 sander    (1000) sander    (1000)    25351 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/_static/websupport.js
+-rw-r--r--   0 sander    (1000) sander    (1000)    25780 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/genindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    68960 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/index.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     6140 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/modules.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     1101 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/objects.inv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7330 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/py-modindex.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    58474 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/rowingdata.html
+-rw-r--r--   0 sander    (1000) sander    (1000)     3164 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/search.html
+-rw-r--r--   0 sander    (1000) sander    (1000)    17380 2023-06-04 14:45:11.000000 rowingdata-3.6.8/docs/_build/html/searchindex.js
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.062646 rowingdata-3.6.8/rowingdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)       27 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/__init__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)       36 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/__main__.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      303 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/boatedit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     6404 2024-04-13 07:15:29.000000 rowingdata-3.6.8/rowingdata/checkdatafiles.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      425 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/copystats.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      758 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/crewnerdplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      771 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/crewnerdplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    98962 2024-04-19 15:31:59.000000 rowingdata-3.6.8/rowingdata/csvparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergdataplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      610 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergdataplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      623 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergdatatotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergstickplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      612 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergstickplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      628 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/ergsticktotcx.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1491 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/gpxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     5327 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/gpxwrite.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      429 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/konkatenaadje.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    13014 2024-02-15 15:52:54.000000 rowingdata-3.6.8/rowingdata/laptesting.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    22121 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/obsolete.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    23514 2023-11-18 13:14:27.000000 rowingdata-3.6.8/rowingdata/otherparsers.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      587 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsled_desktop_plot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      521 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsled_desktop_plottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      569 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsled_desktop_toc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      508 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsledplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      522 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsledplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      441 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/painsledtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      315 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/roweredit.py
+-rw-r--r--   0 sander    (1000) sander    (1000)   243335 2024-04-19 15:32:04.000000 rowingdata-3.6.8/rowingdata/rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/rowproplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      609 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/rowproplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      615 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/speedcoachplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      613 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/speedcoachplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      691 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/speedcoachtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      694 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/tcxplot.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      700 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/tcxplot_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      683 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/tcxplottime.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      689 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/tcxplottime_nogeo.py
+-rw-r--r--   0 sander    (1000) sander    (1000)      585 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/tcxtoc2.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    14568 2023-11-21 09:46:06.000000 rowingdata-3.6.8/rowingdata/tcxtools.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     7714 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/trainingparser.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3676 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/utils.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     1095 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/windcorrected.py
+-rw-r--r--   0 sander    (1000) sander    (1000)    10102 2023-06-04 14:45:11.000000 rowingdata-3.6.8/rowingdata/writetcx.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.082646 rowingdata-3.6.8/rowingdata.egg-info/
+-rw-r--r--   0 sander    (1000) sander    (1000)    32218 2024-04-19 15:32:56.000000 rowingdata-3.6.8/rowingdata.egg-info/PKG-INFO
+-rw-r--r--   0 sander    (1000) sander    (1000)     5562 2024-04-19 15:32:56.000000 rowingdata-3.6.8/rowingdata.egg-info/SOURCES.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2024-04-19 15:32:56.000000 rowingdata-3.6.8/rowingdata.egg-info/dependency_links.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)        1 2023-06-04 14:56:39.000000 rowingdata-3.6.8/rowingdata.egg-info/not-zip-safe
+-rw-r--r--   0 sander    (1000) sander    (1000)      185 2024-04-19 15:32:56.000000 rowingdata-3.6.8/rowingdata.egg-info/requires.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)       11 2024-04-19 15:32:56.000000 rowingdata-3.6.8/rowingdata.egg-info/top_level.txt
+-rw-r--r--   0 sander    (1000) sander    (1000)      202 2024-04-19 15:32:56.082646 rowingdata-3.6.8/setup.cfg
+-rw-r--r--   0 sander    (1000) sander    (1000)     3846 2023-06-04 14:45:11.000000 rowingdata-3.6.8/setup.py
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.082646 rowingdata-3.6.8/testdata/
+-rw-r--r--   0 sander    (1000) sander    (1000)     3481 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/2016-03-25-0758.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   416618 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/2016-03-25-0758_data.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    56355 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/2x20min_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17496 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/3km_cd_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   539777 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/EUBoatCoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    97777 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/EmpowerSpeedCoachForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    72367 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/NKEmporfromgreg.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   111860 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/NKLiNKv130.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2827124 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/NoHR.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    70850 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/PainsledForce.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   104085 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/RP_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   124341 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/RP_interval.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    63080 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/RP_testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    98860 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpdCoach2_imp_inconsistent.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   159697 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpdCoachAmbiguous.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    62781 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpeedCoach GPS Workout.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    17242 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpeedCoach2Link_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   185339 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpeedCoach2Linkv1.27.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    12146 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/SpeedCoach2v2.12.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4976 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/Speedcoach2example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    53949 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/aritmo.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   459974 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/bc1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   340372 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/bc2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   365508 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/bc3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    18887 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/boatcoach.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    95234 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/boatcoach_fixed_distance.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   520154 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/boatcoach_otw.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    74347 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/correctedpainsled.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     5461 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/coxmate.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  1479971 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/crewnerd_interval.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)      381 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/crewnerddata.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)  2945286 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/crewnerddata.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   420603 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/crewnerddata_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)      453 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/cumvalues.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7424 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergdata_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11261 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergdata_example.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   462959 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergstick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   262276 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergstick.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)    40411 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergstick2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   231959 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ergstick_o.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   378971 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   416716 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/example_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)       17 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/faketcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    64254 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/float.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23400 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/herodata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   215236 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/humon.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   157127 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/impeller_empower.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   484172 2023-11-18 12:40:31.000000 rowingdata-3.6.8/testdata/invalidchar.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   115182 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/kinomap.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   397003 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/mystery.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   792595 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/nk_logbook.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    56673 2023-11-18 13:14:27.000000 rowingdata-3.6.8/testdata/painsled.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   369891 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/painsled_desktop_example.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41434 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/painsled_out_data.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   923421 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    76485 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/quiske_per_stroke_left.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   366614 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/quiske_per_stroke_new.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   277062 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/quiske_per_stroke_right.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   511961 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/quiske_per_stroke_seat.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    20254 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/recover.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   106145 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/ritmointervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    14216 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowingdata_eth.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)  2744646 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowinginmotionexample.TCX
+-rw-r--r--   0 sander    (1000) sander    (1000)   657715 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowinginmotionexample.TCX_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   184978 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowperfect.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     4490 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowpro5.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   144225 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rowpro_carrick.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   253794 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rp3_curve.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   420248 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rp3intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   417209 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rp3intervals2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    85870 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/rp_out.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    41141 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/smartrow.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    34271 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/smartrow_intervals.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    31104 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/spdcoach2noheader.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    13731 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/speedcoach2test2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7840 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/speedcoach3test3.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    28352 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/speedcoachexample.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23429 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/speedcoachexample.csv_o.CSV
+-rw-r--r--   0 sander    (1000) sander    (1000)   422653 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/summarytest.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testdata.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    11130 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testdata_part1.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     9315 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testdata_part2.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)     7061 2024-04-13 07:15:29.000000 rowingdata-3.6.8/testdata/testdatasummary.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    19849 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testlapidx.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)   427961 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testtcs_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    51127 2024-04-19 15:31:38.000000 rowingdata-3.6.8/testdata/testtcx.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)   427951 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/testtcx_210614.tcx
+-rw-r--r--   0 sander    (1000) sander    (1000)    74249 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/tim.csv
+-rw-r--r--   0 sander    (1000) sander    (1000)    23885 2023-06-04 14:45:11.000000 rowingdata-3.6.8/testdata/划船.csv
+drwxr-xr-x   0 sander    (1000) sander    (1000)        0 2024-04-19 15:32:56.082646 rowingdata-3.6.8/tests/
+-rw-r--r--   0 sander    (1000) sander    (1000)    27734 2024-04-13 07:15:29.000000 rowingdata-3.6.8/tests/test_rowingdata.py
+-rw-r--r--   0 sander    (1000) sander    (1000)     3424 2023-06-04 14:45:11.000000 rowingdata-3.6.8/tests/testparser.py
```

### Comparing `rowingdata-3.6.7/LICENSE` & `rowingdata-3.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/PKG-INFO` & `rowingdata-3.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowingdata
-Version: 3.6.7
+Version: 3.6.8
 Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
 Home-page: 
 Author: Sander Roosendaal
 Author-email: roosendaalsander@gmail.com
 License: MIT
 Keywords: rowing ergometer concept2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rowingdata-3.6.7/README.rst` & `rowingdata-3.6.8/README.rst`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/bin/crewnerddata.csv` & `rowingdata-3.6.8/bin/crewnerddata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/bin/crewnerddata.tcx` & `rowingdata-3.6.8/bin/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/bin/testdata.csv` & `rowingdata-3.6.8/bin/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/2x20min.png` & `rowingdata-3.6.8/docs/_build/html/_images/2x20min.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/editrower.JPG` & `rowingdata-3.6.8/docs/_build/html/_images/editrower.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/greghoc.png` & `rowingdata-3.6.8/docs/_build/html/_images/greghoc.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/image001.png` & `rowingdata-3.6.8/docs/_build/html/_images/image001.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/otwlogbook.JPG` & `rowingdata-3.6.8/docs/_build/html/_images/otwlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/otwscreenshot.JPG` & `rowingdata-3.6.8/docs/_build/html/_images/otwscreenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/screenshot.JPG` & `rowingdata-3.6.8/docs/_build/html/_images/screenshot.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/screenshotlogbook.JPG` & `rowingdata-3.6.8/docs/_build/html/_images/screenshotlogbook.JPG`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_images/woensdag.png` & `rowingdata-3.6.8/docs/_build/html/_images/woensdag.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_sources/rowingdata.txt` & `rowingdata-3.6.8/docs/_build/html/_sources/rowingdata.txt`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/ajax-loader.gif` & `rowingdata-3.6.8/docs/_build/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/alabaster.css` & `rowingdata-3.6.8/docs/_build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/basic.css` & `rowingdata-3.6.8/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/comment-bright.png` & `rowingdata-3.6.8/docs/_build/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/comment-close.png` & `rowingdata-3.6.8/docs/_build/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/comment.png` & `rowingdata-3.6.8/docs/_build/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/doctools.js` & `rowingdata-3.6.8/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/jquery-1.11.1.js` & `rowingdata-3.6.8/docs/_build/html/_static/jquery-1.11.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/jquery.js` & `rowingdata-3.6.8/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/pygments.css` & `rowingdata-3.6.8/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/searchtools.js` & `rowingdata-3.6.8/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/underscore-1.3.1.js` & `rowingdata-3.6.8/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/underscore.js` & `rowingdata-3.6.8/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/_static/websupport.js` & `rowingdata-3.6.8/docs/_build/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/genindex.html` & `rowingdata-3.6.8/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/index.html` & `rowingdata-3.6.8/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/modules.html` & `rowingdata-3.6.8/docs/_build/html/modules.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/objects.inv` & `rowingdata-3.6.8/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/py-modindex.html` & `rowingdata-3.6.8/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/rowingdata.html` & `rowingdata-3.6.8/docs/_build/html/rowingdata.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/search.html` & `rowingdata-3.6.8/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/docs/_build/html/searchindex.js` & `rowingdata-3.6.8/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/checkdatafiles.py` & `rowingdata-3.6.8/rowingdata/checkdatafiles.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/crewnerdplot.py` & `rowingdata-3.6.8/rowingdata/crewnerdplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/crewnerdplottime.py` & `rowingdata-3.6.8/rowingdata/crewnerdplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/csvparsers.py` & `rowingdata-3.6.8/rowingdata/csvparsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,14 +714,15 @@
             dxpos[index] = xvalues[index + 1]
         newvalues = np.append(0, np.cumsum(dxpos)) + xvalues[0]
     else:
         newvalues = xvalues
 
     return [newvalues, abs(lapidx)]
 
+
 def make_cumvalues(xvalues):
     """ Takes a Pandas dataframe with one column as input value.
     Tries to create a cumulative series.
 
     """
 
     newvalues = 0.0 * xvalues
```

### Comparing `rowingdata-3.6.7/rowingdata/ergdataplot.py` & `rowingdata-3.6.8/rowingdata/ergdataplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/ergdataplottime.py` & `rowingdata-3.6.8/rowingdata/ergdataplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/ergdatatotcx.py` & `rowingdata-3.6.8/rowingdata/ergdatatotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/ergstickplot.py` & `rowingdata-3.6.8/rowingdata/ergstickplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/ergstickplottime.py` & `rowingdata-3.6.8/rowingdata/ergstickplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/ergsticktotcx.py` & `rowingdata-3.6.8/rowingdata/ergsticktotcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/gpxtools.py` & `rowingdata-3.6.8/rowingdata/gpxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/gpxwrite.py` & `rowingdata-3.6.8/rowingdata/gpxwrite.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/laptesting.py` & `rowingdata-3.6.8/rowingdata/laptesting.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/obsolete.py` & `rowingdata-3.6.8/rowingdata/obsolete.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/otherparsers.py` & `rowingdata-3.6.8/rowingdata/otherparsers.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/painsled_desktop_plot.py` & `rowingdata-3.6.8/rowingdata/painsled_desktop_plot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/painsled_desktop_plottime.py` & `rowingdata-3.6.8/rowingdata/painsled_desktop_plottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/painsled_desktop_toc2.py` & `rowingdata-3.6.8/rowingdata/painsled_desktop_toc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/painsledplottime.py` & `rowingdata-3.6.8/rowingdata/painsledplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/rowingdata.py` & `rowingdata-3.6.8/rowingdata/rowingdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=C0103, C0303, C0325, C0413, W0403, W0611
 
 from __future__ import absolute_import
 from __future__ import print_function
 from six.moves import range
 from six.moves import input
 
-__version__ = "3.6.7"
+__version__ = "3.6.8"
 
 from collections import Counter
 
 from matplotlib import figure
 import matplotlib
 try:
     matplotlib.use('TkCairo')
@@ -2092,15 +2092,15 @@
                             sled_df = sled_df.with_columns((spm).alias(name))
                         except KeyError: # pragma: no cover
                             pass
 
         sled_df = sled_df.drop([c for c in sled_df.columns if c not in self.defaultnames])
 
         # add drive energy
-        sled_df = sled_df.with_columns((pl.col(" Power (watts)")/pl.col(" Cadence (stokes/min)")).alias("driveenergy"))
+        sled_df = sled_df.with_columns((60.*pl.col(" Power (watts)")/pl.col(" Cadence (stokes/min)")).alias("driveenergy"))
 
         self.duration = 0
         
         if not sled_df.is_empty():
             sled_df = addzones_pl(
                 sled_df,
                 self.rwr.ut2,
```

### Comparing `rowingdata-3.6.7/rowingdata/rowproplot.py` & `rowingdata-3.6.8/rowingdata/rowproplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/rowproplottime.py` & `rowingdata-3.6.8/rowingdata/rowproplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/speedcoachplot.py` & `rowingdata-3.6.8/rowingdata/speedcoachplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/speedcoachplottime.py` & `rowingdata-3.6.8/rowingdata/speedcoachplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/speedcoachtoc2.py` & `rowingdata-3.6.8/rowingdata/speedcoachtoc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxplot.py` & `rowingdata-3.6.8/rowingdata/tcxplot.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxplot_nogeo.py` & `rowingdata-3.6.8/rowingdata/tcxplot_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxplottime.py` & `rowingdata-3.6.8/rowingdata/tcxplottime.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxplottime_nogeo.py` & `rowingdata-3.6.8/rowingdata/tcxplottime_nogeo.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxtoc2.py` & `rowingdata-3.6.8/rowingdata/tcxtoc2.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/tcxtools.py` & `rowingdata-3.6.8/rowingdata/tcxtools.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/trainingparser.py` & `rowingdata-3.6.8/rowingdata/trainingparser.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/utils.py` & `rowingdata-3.6.8/rowingdata/utils.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/windcorrected.py` & `rowingdata-3.6.8/rowingdata/windcorrected.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata/writetcx.py` & `rowingdata-3.6.8/rowingdata/writetcx.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/rowingdata.egg-info/PKG-INFO` & `rowingdata-3.6.8/rowingdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rowingdata
-Version: 3.6.7
+Version: 3.6.8
 Summary: The rowingdata library to create colorful plots from CrewNerd, Painsled and other rowing data tools
 Home-page: 
 Author: Sander Roosendaal
 Author-email: roosendaalsander@gmail.com
 License: MIT
 Keywords: rowing ergometer concept2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rowingdata-3.6.7/rowingdata.egg-info/SOURCES.txt` & `rowingdata-3.6.8/rowingdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/setup.py` & `rowingdata-3.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/2016-03-25-0758.CSV` & `rowingdata-3.6.8/testdata/2016-03-25-0758.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/2016-03-25-0758_data.CSV` & `rowingdata-3.6.8/testdata/2016-03-25-0758_data.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/2x20min_o.csv` & `rowingdata-3.6.8/testdata/2x20min_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/3km_cd_o.csv` & `rowingdata-3.6.8/testdata/3km_cd_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/EUBoatCoach.csv` & `rowingdata-3.6.8/testdata/EUBoatCoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/EmpowerSpeedCoachForce.csv` & `rowingdata-3.6.8/testdata/EmpowerSpeedCoachForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/NKEmporfromgreg.csv` & `rowingdata-3.6.8/testdata/NKEmporfromgreg.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/NKLiNKv130.csv` & `rowingdata-3.6.8/testdata/NKLiNKv130.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/NoHR.tcx` & `rowingdata-3.6.8/testdata/NoHR.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/PainsledForce.csv` & `rowingdata-3.6.8/testdata/PainsledForce.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/RP_interval.csv` & `rowingdata-3.6.8/testdata/RP_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/RP_interval.csv_o.CSV` & `rowingdata-3.6.8/testdata/RP_interval.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/RP_testdata.csv` & `rowingdata-3.6.8/testdata/RP_testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpdCoach2_imp_inconsistent.csv` & `rowingdata-3.6.8/testdata/SpdCoach2_imp_inconsistent.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpdCoachAmbiguous.csv` & `rowingdata-3.6.8/testdata/SpdCoachAmbiguous.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpeedCoach GPS Workout.csv` & `rowingdata-3.6.8/testdata/SpeedCoach GPS Workout.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpeedCoach2Link_interval.csv` & `rowingdata-3.6.8/testdata/SpeedCoach2Link_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpeedCoach2Linkv1.27.csv` & `rowingdata-3.6.8/testdata/SpeedCoach2Linkv1.27.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/SpeedCoach2v2.12.csv` & `rowingdata-3.6.8/testdata/SpeedCoach2v2.12.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/Speedcoach2example.csv` & `rowingdata-3.6.8/testdata/Speedcoach2example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/aritmo.csv` & `rowingdata-3.6.8/testdata/aritmo.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/bc1.csv` & `rowingdata-3.6.8/testdata/bc1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/bc2.csv` & `rowingdata-3.6.8/testdata/bc2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/bc3.csv` & `rowingdata-3.6.8/testdata/bc3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/boatcoach.csv` & `rowingdata-3.6.8/testdata/boatcoach.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/boatcoach_fixed_distance.csv` & `rowingdata-3.6.8/testdata/boatcoach_fixed_distance.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/boatcoach_otw.csv` & `rowingdata-3.6.8/testdata/boatcoach_otw.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/correctedpainsled.csv` & `rowingdata-3.6.8/testdata/correctedpainsled.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/coxmate.csv` & `rowingdata-3.6.8/testdata/coxmate.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/crewnerd_interval.csv` & `rowingdata-3.6.8/testdata/crewnerd_interval.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/crewnerddata.tcx` & `rowingdata-3.6.8/testdata/crewnerddata.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/crewnerddata_o.CSV` & `rowingdata-3.6.8/testdata/crewnerddata_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergdata_example.csv` & `rowingdata-3.6.8/testdata/ergdata_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergdata_example.csv_o.CSV` & `rowingdata-3.6.8/testdata/ergdata_example.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergstick.csv` & `rowingdata-3.6.8/testdata/ergstick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergstick.csv_o.CSV` & `rowingdata-3.6.8/testdata/ergstick.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergstick2.csv` & `rowingdata-3.6.8/testdata/ergstick2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ergstick_o.csv` & `rowingdata-3.6.8/testdata/ergstick_o.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/example.csv` & `rowingdata-3.6.8/testdata/example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/example_data.csv` & `rowingdata-3.6.8/testdata/example_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/float.csv` & `rowingdata-3.6.8/testdata/float.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/herodata.csv` & `rowingdata-3.6.8/testdata/herodata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/humon.csv` & `rowingdata-3.6.8/testdata/humon.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/impeller_empower.csv` & `rowingdata-3.6.8/testdata/impeller_empower.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/invalidchar.tcx` & `rowingdata-3.6.8/testdata/invalidchar.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/kinomap.csv` & `rowingdata-3.6.8/testdata/kinomap.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/mystery.csv` & `rowingdata-3.6.8/testdata/mystery.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/nk_logbook.csv` & `rowingdata-3.6.8/testdata/nk_logbook.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/painsled.tcx` & `rowingdata-3.6.8/testdata/painsled.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/painsled_desktop_example.csv` & `rowingdata-3.6.8/testdata/painsled_desktop_example.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/painsled_out_data.csv` & `rowingdata-3.6.8/testdata/painsled_out_data.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv` & `rowingdata-3.6.8/testdata/painsled_to_csv_20160221-105218_erg-400150318_760465m.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/quiske_per_stroke_left.csv` & `rowingdata-3.6.8/testdata/quiske_per_stroke_left.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/quiske_per_stroke_new.csv` & `rowingdata-3.6.8/testdata/quiske_per_stroke_new.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/quiske_per_stroke_right.csv` & `rowingdata-3.6.8/testdata/quiske_per_stroke_right.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/quiske_per_stroke_seat.csv` & `rowingdata-3.6.8/testdata/quiske_per_stroke_seat.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/recover.tcx` & `rowingdata-3.6.8/testdata/recover.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/ritmointervals.csv` & `rowingdata-3.6.8/testdata/ritmointervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowingdata_eth.csv` & `rowingdata-3.6.8/testdata/rowingdata_eth.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowinginmotionexample.TCX` & `rowingdata-3.6.8/testdata/rowinginmotionexample.TCX`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowinginmotionexample.TCX_o.CSV` & `rowingdata-3.6.8/testdata/rowinginmotionexample.TCX_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowperfect.csv` & `rowingdata-3.6.8/testdata/rowperfect.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowpro5.csv` & `rowingdata-3.6.8/testdata/rowpro5.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rowpro_carrick.csv` & `rowingdata-3.6.8/testdata/rowpro_carrick.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rp3_curve.csv` & `rowingdata-3.6.8/testdata/rp3_curve.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rp3intervals.csv` & `rowingdata-3.6.8/testdata/rp3intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rp3intervals2.csv` & `rowingdata-3.6.8/testdata/rp3intervals2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/rp_out.csv` & `rowingdata-3.6.8/testdata/rp_out.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/smartrow.csv` & `rowingdata-3.6.8/testdata/smartrow.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/smartrow_intervals.csv` & `rowingdata-3.6.8/testdata/smartrow_intervals.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/spdcoach2noheader.csv` & `rowingdata-3.6.8/testdata/spdcoach2noheader.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/speedcoach2test2.csv` & `rowingdata-3.6.8/testdata/speedcoach2test2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/speedcoach3test3.csv` & `rowingdata-3.6.8/testdata/speedcoach3test3.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/speedcoachexample.csv` & `rowingdata-3.6.8/testdata/speedcoachexample.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/speedcoachexample.csv_o.CSV` & `rowingdata-3.6.8/testdata/speedcoachexample.csv_o.CSV`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/summarytest.csv` & `rowingdata-3.6.8/testdata/summarytest.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testdata.csv` & `rowingdata-3.6.8/testdata/testdata.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testdata_part1.csv` & `rowingdata-3.6.8/testdata/testdata_part1.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testdata_part2.csv` & `rowingdata-3.6.8/testdata/testdata_part2.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testdatasummary.csv` & `rowingdata-3.6.8/testdata/testdatasummary.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testlapidx.csv` & `rowingdata-3.6.8/testdata/testlapidx.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testtcs_210614.tcx` & `rowingdata-3.6.8/testdata/testtcs_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/testtcx.tcx` & `rowingdata-3.6.8/testdata/testtcx.tcx`

 * *Files 0% similar despite different names*

#### Comparing `rowingdata-3.6.7/testdata/testtcx.tcx` & `rowingdata-3.6.8/testdata/testtcx.tcx`

```diff
@@ -1276,15 +1276,15 @@
               <TPX xmlns="http://www.garmin.com/xmlschemas/ActivityExtension/v2">
                 <Watts>0</Watts>
               </TPX>
             </Extensions>
           </Trackpoint>
         </Track>
       </Lap>
-      <Notes>&lt;Element 'Notes' at 0x7f7e54795680&gt;</Notes>
+      <Notes>&lt;Element 'Notes' at 0x7f51820df9f0&gt;</Notes>
     </Activity>
   </Activities>
   <Creator>
     <Name>rowsandall.com/rowingdata</Name>
   </Creator>
   <Author xsi:type="Application_t">
     <Name>rowingdata</Name>
```

### Comparing `rowingdata-3.6.7/testdata/testtcx_210614.tcx` & `rowingdata-3.6.8/testdata/testtcx_210614.tcx`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/tim.csv` & `rowingdata-3.6.8/testdata/tim.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/testdata/划船.csv` & `rowingdata-3.6.8/testdata/划船.csv`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/tests/test_rowingdata.py` & `rowingdata-3.6.8/tests/test_rowingdata.py`

 * *Files identical despite different names*

### Comparing `rowingdata-3.6.7/tests/testparser.py` & `rowingdata-3.6.8/tests/testparser.py`

 * *Files identical despite different names*

