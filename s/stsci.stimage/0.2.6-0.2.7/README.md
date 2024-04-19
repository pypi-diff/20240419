# Comparing `tmp/stsci.stimage-0.2.6.tar.gz` & `tmp/stsci_stimage-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stsci.stimage-0.2.6.tar", last modified: Thu Nov  3 16:28:22 2022, max compression
+gzip compressed data, was "stsci_stimage-0.2.7.tar", last modified: Fri Apr 19 17:33:56 2024, max compression
```

## Comparing `stsci.stimage-0.2.6.tar` & `stsci_stimage-0.2.7.tar`

### file list

```diff
@@ -1,103 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.488483 stsci.stimage-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3207 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-11-03 16:28:22.488483 stsci.stimage-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     3132 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/doc/source/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6751 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/doc/source/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (121)      267 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/get_waf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/include/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/include/immatch/
--rw-r--r--   0 runner    (1001) docker     (121)     9102 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/immatch/geomap.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.480482 stsci.stimage-0.2.6/include/immatch/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     1709 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/immatch/lib/match_util.h
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/immatch/lib/tolerance.h
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/immatch/lib/triangles.h
--rw-r--r--   0 runner    (1001) docker     (121)     6778 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/immatch/xyxymatch.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/include/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/error.h
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/lintransform.h
--rw-r--r--   0 runner    (1001) docker     (121)     7373 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/polynomial.h
--rw-r--r--   0 runner    (1001) docker     (121)     7735 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/util.h
--rw-r--r--   0 runner    (1001) docker     (121)     3429 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/xybbox.h
--rw-r--r--   0 runner    (1001) docker     (121)     2341 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/xycoincide.h
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/lib/xysort.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/include/surface/
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/surface/cholesky.h
--rw-r--r--   0 runner    (1001) docker     (121)     3075 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/surface/fit.h
--rw-r--r--   0 runner    (1001) docker     (121)     3831 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/surface/surface.h
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/include/surface/vector.h
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-11-03 16:28:22.488483 stsci.stimage-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1064 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/immatch/
--rw-r--r--   0 runner    (1001) docker     (121)    50354 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/immatch/geomap.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/immatch/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     4005 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/immatch/lib/tolerance.c
--rw-r--r--   0 runner    (1001) docker     (121)    25905 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/immatch/lib/triangles.c
--rw-r--r--   0 runner    (1001) docker     (121)     5602 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/immatch/lib/triangles_vote.c
--rw-r--r--   0 runner    (1001) docker     (121)     7722 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/immatch/xyxymatch.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/error.c
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/lintransform.c
--rw-r--r--   0 runner    (1001) docker     (121)    16094 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/polynomial.c
--rw-r--r--   0 runner    (1001) docker     (121)     6936 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/util.c
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/xybbox.c
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/xycoincide.c
--rw-r--r--   0 runner    (1001) docker     (121)     3115 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/lib/xysort.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/surface/
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/surface/cholesky.c
--rw-r--r--   0 runner    (1001) docker     (121)     9269 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/surface/fit.c
--rw-r--r--   0 runner    (1001) docker     (121)     9375 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/surface/surface.c
--rw-r--r--   0 runner    (1001) docker     (121)     4001 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/surface/vector.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/wrap/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/src/wrap/immatch/
--rw-r--r--   0 runner    (1001) docker     (121)    13821 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wrap/immatch/py_geomap.c
--rw-r--r--   0 runner    (1001) docker     (121)     5617 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wrap/immatch/py_xyxymatch.c
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wrap/stimage_module.c
--rw-r--r--   0 runner    (1001) docker     (121)     8145 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wrap/wrap_util.c
--rw-r--r--   0 runner    (1001) docker     (121)     2794 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wrap/wrap_util.h
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/src/wscript
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/stsci/
--rw-r--r--   0 runner    (1001) docker     (121)      476 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/stsci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/stsci/stimage/
--rw-r--r--   0 runner    (1001) docker     (121)    24284 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/stsci/stimage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci/stimage/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.488483 stsci.stimage-0.2.6/stsci/stimage/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/stsci/stimage/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/stsci/stimage/tests/test_geomap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/stsci/stimage/tests/test_xyxymatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.484482 stsci.stimage-0.2.6/stsci.stimage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-03 16:28:22.000000 stsci.stimage-0.2.6/stsci.stimage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-03 16:28:22.488483 stsci.stimage-0.2.6/test_c/
--rwxr-xr-x   0 runner    (1001) docker     (121)      943 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_c.py
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_cholesky.c
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_geomap.c
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_lintransform.c
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_surface.c
--rw-r--r--   0 runner    (1001) docker     (121)     6258 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_triangles.c
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_xycoincide.c
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_xysort.c
--rw-r--r--   0 runner    (1001) docker     (121)     2932 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_xyxymatch.c
--rw-r--r--   0 runner    (1001) docker     (121)     2845 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/test_xyxymatch_triangles.c
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/test_c/wscript
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-11-03 16:28:09.000000 stsci.stimage-0.2.6/wscript
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.410848 stsci_stimage-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.github/workflows/test_devdeps.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 17:33:56.406848 stsci_stimage-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/doc/rtd_environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/doc/source/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      259 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/get_waf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.390848 stsci_stimage-0.2.7/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/include/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/immatch/geomap.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.394847 stsci_stimage-0.2.7/include/immatch/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/immatch/lib/match_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/immatch/lib/tolerance.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/immatch/lib/triangles.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/immatch/xyxymatch.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.398848 stsci_stimage-0.2.7/include/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/error.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/lintransform.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/polynomial.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/util.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/xybbox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/xycoincide.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/lib/xysort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.398848 stsci_stimage-0.2.7/include/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/surface/cholesky.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/surface/fit.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/surface/surface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/include/surface/vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 17:33:56.410848 stsci_stimage-0.2.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      950 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.398848 stsci_stimage-0.2.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.398848 stsci_stimage-0.2.7/src/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    50354 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/immatch/geomap.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.398848 stsci_stimage-0.2.7/src/immatch/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/immatch/lib/tolerance.c
+-rw-r--r--   0 runner    (1001) docker     (127)    25905 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/immatch/lib/triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/immatch/lib/triangles_vote.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/immatch/xyxymatch.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/src/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/error.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/lintransform.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16094 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/polynomial.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6936 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/xybbox.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/xycoincide.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/lib/xysort.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/src/surface/
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/surface/cholesky.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9269 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/surface/fit.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/surface/surface.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/surface/vector.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/src/wrap/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/src/wrap/immatch/
+-rw-r--r--   0 runner    (1001) docker     (127)    13821 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wrap/immatch/py_geomap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wrap/immatch/py_xyxymatch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wrap/stimage_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wrap/wrap_util.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wrap/wrap_util.h
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/src/wscript
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/stsci/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/stsci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.402848 stsci_stimage-0.2.7/stsci/stimage/
+-rw-r--r--   0 runner    (1001) docker     (127)    24284 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/stsci/stimage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.406848 stsci_stimage-0.2.7/stsci/stimage/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/stsci/stimage/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/stsci/stimage/tests/test_geomap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/stsci/stimage/tests/test_xyxymatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.406848 stsci_stimage-0.2.7/stsci.stimage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-19 17:33:56.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-19 17:33:56.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:33:56.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 17:33:55.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-19 17:33:56.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-19 17:33:56.000000 stsci_stimage-0.2.7/stsci.stimage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 17:33:56.406848 stsci_stimage-0.2.7/test_c/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      943 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_cholesky.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_geomap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_lintransform.c
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_surface.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_xycoincide.c
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_xysort.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_xyxymatch.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/test_xyxymatch_triangles.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/test_c/wscript
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 17:33:44.000000 stsci_stimage-0.2.7/wscript
```

### Comparing `stsci.stimage-0.2.6/.github/workflows/ci.yml` & `stsci_stimage-0.2.7/.github/workflows/ci.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,86 @@
-name: CI
+name: test
 
 on:
   push:
     branches:
       - master
       - '*.x'
     tags:
       - '*'
   pull_request:
   schedule:
     # Weekly Monday 7AM build
     - cron: "0 7 * * 1"
 
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
+
 env:
   CODECOV: $(codecov)
 
 jobs:
   test:
-    name: run tests (Python ${{ matrix.python }}, numpy ${{ matrix.numpy }})
+    name: test (Python ${{ matrix.python }}, numpy ${{ matrix.numpy }}, ${{ matrix.os }})
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python: [ '3.8', '3.9', '3.10' ]
+        python: [ '3.9', '3.10', '3.11', '3.12' ]
         os: [ ubuntu-latest, macos-latest ]
-        numpy: [ '1.20.*', '1.21.*', '1.*' ]
-        exclude:
-          - python: '3.10'
+        numpy: [ '1.*' ]
+        include:
+          - python: '3.9'
             numpy: '1.20.*'
+            os: ubuntu-latest
+          - python: '3.9'
+            numpy: '1.20.*'
+            os: macos-latest
+          - python: '3.9'
+            numpy: '1.21.*'
+            os: ubuntu-latest
+          - python: '3.9'
+            numpy: '1.21.*'
+            os: macos-latest
+          - python: '3.10'
+            numpy: '1.21.*'
+            os: ubuntu-latest
+          - python: '3.10'
+            numpy: '1.21.*'
+            os: macos-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
-      - uses: actions/cache@v3
-        with:
-          path: ${{ env.pythonLocation }}
-          key: test-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('**/pyproject.toml', '**/setup.*') }}
+          cache: 'pip'
+          cache-dependency-path: pyproject.toml
       - run: pip install -e ".[test]" "numpy==${{ matrix.numpy }}"
-      - run: |
-          python get_waf.py
-          python waf configure build
+      - run: python get_waf.py
+      - run: python waf configure build
       - run: pip freeze
       - run: pytest -rsv
   test_with_coverage:
     name: run tests with coverage
     needs: [ test ]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: '3.10'
-      - uses: actions/cache@v3
-        with:
-          path: ${{ env.pythonLocation }}
-          key: test-${{ runner.os }}-${{ env.pythonLocation }}-${{ hashFiles('**/pyproject.toml', '**/setup.*') }}
+          cache: 'pip'
+          cache-dependency-path: pyproject.toml
       - run: pip install -e ".[test]"
-      - run: |
-          python get_waf.py
-          python waf configure build
+      - run: python get_waf.py
+      - run: python waf configure build
       - run: pip freeze
       - run: pytest -rsv --cov=./ --cov-report=xml --cov-report term-missing
-      - uses: codecov/codecov-action@v3
+      - uses: codecov/codecov-action@v4
         with:
           file: ./coverage.xml
           fail_ci_if_error: true
```

### Comparing `stsci.stimage-0.2.6/CODE_OF_CONDUCT.md` & `stsci_stimage-0.2.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/LICENSE` & `stsci_stimage-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/README.md` & `stsci_stimage-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/doc/Makefile` & `stsci_stimage-0.2.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/doc/source/conf.py` & `stsci_stimage-0.2.7/doc/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,24 +6,29 @@
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
+from datetime import datetime
+from pathlib import Path
 
-import sys, os
+import sys
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-#sys.path.append(os.path.abspath('.'))
+# sys.path.append(os.path.abspath('.'))
 
 # -- General configuration -----------------------------------------------------
-
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.imgmath',
     'sphinx.ext.napoleon',
     'sphinx.ext.intersphinx',
     'sphinx.ext.autosummary',
     'sphinx_automodapi.automodapi']
@@ -39,16 +44,19 @@
 # The encoding of source files.
 #source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'stimage'
-copyright = u'2010-2020, STScI'
+with open(Path(__file__).parent.parent.parent / "pyproject.toml", "rb") as metadata_file:
+    metadata = tomllib.load(metadata_file)['project']
+project = metadata['name']
+author = metadata["authors"][0]["name"]
+copyright = f'2010-{datetime.now().year}, {author}'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '0.2'
@@ -121,15 +129,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-# html_static_path = ['_static']
+#html_static_path = ['_static']
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 #html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -172,16 +180,16 @@
 
 # The font size ('10pt', '11pt' or '12pt').
 #latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'stimage.tex', u'stimage Documentation',
-   u'STScI', 'manual'),
+    ('index', 'stimage.tex', u'stimage Documentation',
+     u'STScI', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
```

### Comparing `stsci.stimage-0.2.6/include/immatch/geomap.h` & `stsci_stimage-0.2.7/include/immatch/geomap.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/immatch/lib/match_util.h` & `stsci_stimage-0.2.7/include/immatch/lib/match_util.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/immatch/lib/tolerance.h` & `stsci_stimage-0.2.7/include/immatch/lib/tolerance.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/immatch/lib/triangles.h` & `stsci_stimage-0.2.7/include/immatch/lib/triangles.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/immatch/xyxymatch.h` & `stsci_stimage-0.2.7/include/immatch/xyxymatch.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/error.h` & `stsci_stimage-0.2.7/include/lib/error.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/lintransform.h` & `stsci_stimage-0.2.7/include/lib/lintransform.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/polynomial.h` & `stsci_stimage-0.2.7/include/lib/polynomial.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/util.h` & `stsci_stimage-0.2.7/include/lib/util.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/xybbox.h` & `stsci_stimage-0.2.7/include/lib/xybbox.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/xycoincide.h` & `stsci_stimage-0.2.7/include/lib/xycoincide.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/lib/xysort.h` & `stsci_stimage-0.2.7/include/lib/xysort.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/surface/cholesky.h` & `stsci_stimage-0.2.7/include/surface/cholesky.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/surface/fit.h` & `stsci_stimage-0.2.7/include/surface/fit.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/surface/surface.h` & `stsci_stimage-0.2.7/include/surface/surface.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/include/surface/vector.h` & `stsci_stimage-0.2.7/include/surface/vector.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/setup.py` & `stsci_stimage-0.2.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import os
 from fnmatch import fnmatch
-from setuptools import setup, find_packages, Extension
+
 from numpy import get_include as numpy_includes
+from setuptools import setup, Extension
 
 
 def c_sources(parent):
     sources = []
     for root, _, files in os.walk(parent):
         for f in files:
             fn = os.path.join(root, f)
@@ -26,19 +27,18 @@
             includes.append(dn)
     return includes
 
 
 SOURCES = c_sources('src')
 INCLUDES = c_includes('include') + c_includes('src') + [numpy_includes()]
 
+ext_modules = [
+    Extension(
+        'stsci.stimage._stimage',
+        sources=SOURCES,
+        include_dirs=INCLUDES,
+    ),
+]
 
 setup(
-    use_scm_version={"write_to": "stsci/stimage/_version.py"},
-    setup_requires=['setuptools_scm'],
-    ext_modules=[
-        Extension(
-            'stsci.stimage._stimage',
-            sources=SOURCES,
-            include_dirs=INCLUDES,
-        ),
-    ],
+    ext_modules=ext_modules,
 )
```

### Comparing `stsci.stimage-0.2.6/src/immatch/geomap.c` & `stsci_stimage-0.2.7/src/immatch/geomap.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/immatch/lib/tolerance.c` & `stsci_stimage-0.2.7/src/immatch/lib/tolerance.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/immatch/lib/triangles.c` & `stsci_stimage-0.2.7/src/immatch/lib/triangles.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/immatch/lib/triangles_vote.c` & `stsci_stimage-0.2.7/src/immatch/lib/triangles_vote.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/immatch/xyxymatch.c` & `stsci_stimage-0.2.7/src/immatch/xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/error.c` & `stsci_stimage-0.2.7/src/lib/error.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/lintransform.c` & `stsci_stimage-0.2.7/src/lib/lintransform.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/polynomial.c` & `stsci_stimage-0.2.7/src/lib/polynomial.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/util.c` & `stsci_stimage-0.2.7/src/lib/util.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/xybbox.c` & `stsci_stimage-0.2.7/src/lib/xybbox.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/xycoincide.c` & `stsci_stimage-0.2.7/src/lib/xycoincide.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/lib/xysort.c` & `stsci_stimage-0.2.7/src/lib/xysort.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/surface/cholesky.c` & `stsci_stimage-0.2.7/src/surface/cholesky.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/surface/fit.c` & `stsci_stimage-0.2.7/src/surface/fit.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/surface/surface.c` & `stsci_stimage-0.2.7/src/surface/surface.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/surface/vector.c` & `stsci_stimage-0.2.7/src/surface/vector.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wrap/immatch/py_geomap.c` & `stsci_stimage-0.2.7/src/wrap/immatch/py_geomap.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wrap/immatch/py_xyxymatch.c` & `stsci_stimage-0.2.7/src/wrap/immatch/py_xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wrap/stimage_module.c` & `stsci_stimage-0.2.7/src/wrap/stimage_module.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wrap/wrap_util.c` & `stsci_stimage-0.2.7/src/wrap/wrap_util.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wrap/wrap_util.h` & `stsci_stimage-0.2.7/src/wrap/wrap_util.h`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/src/wscript` & `stsci_stimage-0.2.7/src/wscript`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/stsci/stimage/__init__.py` & `stsci_stimage-0.2.7/stsci/stimage/__init__.py`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/stsci/stimage/tests/test_geomap.py` & `stsci_stimage-0.2.7/stsci/stimage/tests/test_geomap.py`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/stsci/stimage/tests/test_xyxymatch.py` & `stsci_stimage-0.2.7/stsci/stimage/tests/test_xyxymatch.py`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/stsci.stimage.egg-info/SOURCES.txt` & `stsci_stimage-0.2.7/stsci.stimage.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 .coveragerc
 .gitignore
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 get_waf.py
 pyproject.toml
-setup.cfg
 setup.py
 wscript
+.github/CODEOWNERS
+.github/dependabot.yml
+.github/workflows/build.yml
 .github/workflows/ci.yml
-.github/workflows/publish-to-pypi.yml
+.github/workflows/test_devdeps.yml
 doc/Makefile
+doc/rtd_environment.yaml
 doc/source/api.rst
 doc/source/conf.py
 doc/source/index.rst
 include/immatch/geomap.h
 include/immatch/xyxymatch.h
 include/immatch/lib/match_util.h
 include/immatch/lib/tolerance.h
@@ -54,20 +57,18 @@
 src/wrap/wrap_util.h
 src/wrap/immatch/py_geomap.c
 src/wrap/immatch/py_xyxymatch.c
 stsci/__init__.py
 stsci.stimage.egg-info/PKG-INFO
 stsci.stimage.egg-info/SOURCES.txt
 stsci.stimage.egg-info/dependency_links.txt
-stsci.stimage.egg-info/namespace_packages.txt
 stsci.stimage.egg-info/not-zip-safe
 stsci.stimage.egg-info/requires.txt
 stsci.stimage.egg-info/top_level.txt
 stsci/stimage/__init__.py
-stsci/stimage/_version.py
 stsci/stimage/tests/__init__.py
 stsci/stimage/tests/test_geomap.py
 stsci/stimage/tests/test_xyxymatch.py
 test_c/test_c.py
 test_c/test_cholesky.c
 test_c/test_geomap.c
 test_c/test_lintransform.c
```

### Comparing `stsci.stimage-0.2.6/test_c/test_c.py` & `stsci_stimage-0.2.7/test_c/test_c.py`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_geomap.c` & `stsci_stimage-0.2.7/test_c/test_geomap.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_lintransform.c` & `stsci_stimage-0.2.7/test_c/test_lintransform.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_surface.c` & `stsci_stimage-0.2.7/test_c/test_surface.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_triangles.c` & `stsci_stimage-0.2.7/test_c/test_triangles.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_xycoincide.c` & `stsci_stimage-0.2.7/test_c/test_xycoincide.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_xysort.c` & `stsci_stimage-0.2.7/test_c/test_xysort.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_xyxymatch.c` & `stsci_stimage-0.2.7/test_c/test_xyxymatch.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/test_xyxymatch_triangles.c` & `stsci_stimage-0.2.7/test_c/test_xyxymatch_triangles.c`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/test_c/wscript` & `stsci_stimage-0.2.7/test_c/wscript`

 * *Files identical despite different names*

### Comparing `stsci.stimage-0.2.6/wscript` & `stsci_stimage-0.2.7/wscript`

 * *Files identical despite different names*

