# Comparing `tmp/pycaputo-0.4.0.tar.gz` & `tmp/pycaputo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycaputo-0.4.0.tar", last modified: Tue Feb  6 13:23:55 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pycaputo-0.4.0.tar` & `pycaputo-0.5.0.tar`

### file list

```diff
@@ -1,109 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.580154 pycaputo-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 13:23:39.000000 pycaputo-0.4.0/.codespell-ignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.560154 pycaputo-0.4.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-06 13:23:39.000000 pycaputo-0.4.0/.reuse/dep5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.560154 pycaputo-0.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-02-06 13:23:39.000000 pycaputo-0.4.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-06 13:23:39.000000 pycaputo-0.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-06 13:23:39.000000 pycaputo-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-06 13:23:39.000000 pycaputo-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-06 13:23:55.580154 pycaputo-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-06 13:23:39.000000 pycaputo-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.568154 pycaputo-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.560154 pycaputo-0.4.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.568154 pycaputo-0.4.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    60118 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/brusselator-predictor-corrector-cycle-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    58136 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/brusselator-predictor-corrector-cycle-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    66576 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/brusselator-predictor-corrector-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    64378 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/brusselator-predictor-corrector-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    67299 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/caputo-derivative-l1-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65147 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/caputo-derivative-l1-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/controllers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/differentiation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/fode.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/operator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/quadrature.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/timestepping.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)   182839 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-eest-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)   180507 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-eest-light.svg
--rw-r--r--   0 runner    (1001) docker     (127)   233122 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-solution-dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)   230498 2024-02-06 13:23:39.000000 pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-solution-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.568154 pycaputo-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/brusselator-predictor-corrector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/caputo-derivative-l1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/caputo-derivative-quadratic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/caputo-gradient-spectral.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/example-custom-diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/example-custom-quad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/example-lipschitz-weibull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/lorenz-weighted-euler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-02-06 13:23:39.000000 pycaputo-0.4.0/examples/van-der-pol-adaptive-pece.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-02-06 13:23:39.000000 pycaputo-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-02-06 13:23:39.000000 pycaputo-0.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-06 13:23:39.000000 pycaputo-0.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.568154 pycaputo-0.4.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-02-06 13:23:39.000000 pycaputo-0.4.0/scripts/generate-doc-figures.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 13:23:55.580154 pycaputo-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-06 13:23:39.000000 pycaputo-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.560154 pycaputo-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.572154 pycaputo-0.4.0/src/pycaputo/
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/derivatives.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.572154 pycaputo-0.4.0/src/pycaputo/differentiation/
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/differentiation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/differentiation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/differentiation/caputo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/differentiation/riemann_liouville.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/finite_difference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.576154 pycaputo-0.4.0/src/pycaputo/fode/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/fode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19825 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/fode/caputo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/fode/product_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/generating_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7576 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/implicit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12371 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/jacobi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/lagrange.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/lipschitz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/mittagleffler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.576154 pycaputo-0.4.0/src/pycaputo/quadrature/
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/quadrature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/quadrature/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/quadrature/riemann_liouville.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/stepping.py
--rw-r--r--   0 runner    (1001) docker     (127)    22756 2024-02-06 13:23:39.000000 pycaputo-0.4.0/src/pycaputo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.576154 pycaputo-0.4.0/src/pycaputo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-06 13:23:55.000000 pycaputo-0.4.0/src/pycaputo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-02-06 13:23:55.000000 pycaputo-0.4.0/src/pycaputo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 13:23:55.000000 pycaputo-0.4.0/src/pycaputo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-06 13:23:55.000000 pycaputo-0.4.0/src/pycaputo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-06 13:23:55.000000 pycaputo-0.4.0/src/pycaputo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 13:23:55.576154 pycaputo-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37732 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/mittag_leffler_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_diff_caputo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_diff_riemann_liouville.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_fode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_fode_caputo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_generating_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9210 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_jacobi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_mittag_leffler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-02-06 13:23:39.000000 pycaputo-0.4.0/tests/test_quad_riemann_liouville.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.broken.gitlab-ci.yml
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.codespell-ignore
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 pycaputo-0.5.0/Makefile
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 pycaputo-0.5.0/requirements-dev.txt
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 pycaputo-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.reuse/dep5
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 pycaputo-0.5.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pycaputo-0.5.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0    60118 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-dark.svg
+-rw-r--r--   0        0        0    58136 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-light.svg
+-rw-r--r--   0        0        0    66576 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-dark.svg
+-rw-r--r--   0        0        0    64378 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/brusselator-predictor-corrector-light.svg
+-rw-r--r--   0        0        0    67299 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/caputo-derivative-l1-dark.svg
+-rw-r--r--   0        0        0    65147 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/caputo-derivative-l1-light.svg
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/changelog.rst
+-rw-r--r--   0        0        0     4882 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/controllers.rst
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/differentiation.rst
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/fode.rst
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/history.rst
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/integrate_fire.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/misc.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/operator.rst
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/quadrature.rst
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/references.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/timestepping.rst
+-rw-r--r--   0        0        0     9395 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/tutorials.rst
+-rw-r--r--   0        0        0   182839 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-dark.svg
+-rw-r--r--   0        0        0   180507 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-light.svg
+-rw-r--r--   0        0        0   233122 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-dark.svg
+-rw-r--r--   0        0        0   230498 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-light.svg
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    12881 2020-02-02 00:00:00.000000 pycaputo-0.5.0/docs/benchmarks/Linux-CPython-3.11-64bit/0001_561ba4947e7fa72377b82f411a1f0eb91929763c_20240408_123818.json
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/brusselator-predictor-corrector.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-derivative-l1.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-derivative-quadratic.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/caputo-gradient-spectral.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-custom-diff.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-custom-quad.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/example-lipschitz-weibull.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-ad-ex.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-eif.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-lif.py
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/integrate-and-fire-pif.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/lorenz-weighted-euler.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 pycaputo-0.5.0/examples/van-der-pol-adaptive-pece.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 pycaputo-0.5.0/scripts/benchmark-boxplot.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 pycaputo-0.5.0/scripts/generate-doc-figures.py
+-rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/__init__.py
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/benchmark.py
+-rw-r--r--   0        0        0    27855 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/controller.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/derivatives.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/events.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/finite_difference.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/generating_functions.py
+-rw-r--r--   0        0        0     7592 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/grid.py
+-rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/history.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/implicit.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/interpolation.py
+-rw-r--r--   0        0        0    12371 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/jacobi.py
+-rw-r--r--   0        0        0     1953 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/lagrange.py
+-rw-r--r--   0        0        0     4532 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/lipschitz.py
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/logging.py
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/mittagleffler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/py.typed
+-rw-r--r--   0        0        0     6065 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/stepping.py
+-rw-r--r--   0        0        0    25864 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/utils.py
+-rw-r--r--   0        0        0     3516 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/__init__.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/base.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/caputo.py
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/differentiation/riemann_liouville.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/__init__.py
+-rw-r--r--   0        0        0    19826 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/caputo.py
+-rw-r--r--   0        0        0     3873 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/fode/product_integration.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/__init__.py
+-rw-r--r--   0        0        0    19297 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/ad_ex.py
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/base.py
+-rw-r--r--   0        0        0    12039 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/eif.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/lif.py
+-rw-r--r--   0        0        0     9200 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/pif.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/integrate_fire/spikes.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/base.py
+-rw-r--r--   0        0        0    15259 2020-02-02 00:00:00.000000 pycaputo-0.5.0/src/pycaputo/quadrature/riemann_liouville.py
+-rw-r--r--   0        0        0    37732 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/mittag_leffler_ref.py
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_diff_caputo.py
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_diff_riemann_liouville.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_finite_difference.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_fode.py
+-rw-r--r--   0        0        0     7382 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_fode_caputo.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_generating_functions.py
+-rw-r--r--   0        0        0    13909 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_integrate_fire.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_interpolation.py
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_jacobi.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_misc.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_mittag_leffler.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_points.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/test_quad_riemann_liouville.py
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 pycaputo-0.5.0/tests/benchmarks/test_bench_diff.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pycaputo-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 pycaputo-0.5.0/README.rst
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 pycaputo-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pycaputo-0.5.0/PKG-INFO
```

### Comparing `pycaputo-0.4.0/LICENSES/CC0-1.0.txt` & `pycaputo-0.5.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/LICENSES/MIT.txt` & `pycaputo-0.5.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/Makefile` & `pycaputo-0.5.0/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 format: black isort pyproject							## Run all formatting scripts
 .PHONY: format
 
 fmt: format
 .PHONY: fmt
 
 black:			## Run ruff format over the source code
-	ruff format src tests examples docs
+	ruff format src tests examples docs scripts
 	@echo -e "\e[1;32mruff format clean!\e[0m"
 .PHONY: black
 
 isort:			## Run ruff isort fixes over the source code
 	ruff check --fix --select=I src tests examples scripts docs
 	ruff check --fix --select=RUF022 src
 	@echo -e "\e[1;32mruff isort clean!\e[0m"
 .PHONY: isort
 
 pyproject:		## Run pyproject-fmt over the configuration
 	$(PYTHON) -m pyproject_fmt --indent 4 pyproject.toml
 	@echo -e "\e[1;32mpyproject clean!\e[0m"
 .PHONY: pyproject
 
-lint: ruff mypy doc8 reuse codespell manifest	## Run all linting scripts
+lint: ruff mypy doc8 reuse codespell 					## Run all linting scripts
 .PHONY: lint
 
 ruff:			## Run ruff checks over the source code
 	ruff check src tests examples scripts scripts
 	@echo -e "\e[1;32mruff lint clean!\e[0m"
 .PHONY: ruff
 
@@ -60,50 +60,54 @@
 		--skip _build \
 		--uri-ignore-words-list '*' \
 		--ignore-words .codespell-ignore \
 		src tests examples docs scripts
 	@echo -e "\e[1;32mcodespell clean!\e[0m"
 .PHONY: codespell
 
-manifest:		## Update MANIFEST.in file
-	$(PYTHON) -m check_manifest
-	@echo -e "\e[1;32mMANIFEST.in is up to date!\e[0m"
-.PHONY: manifest
-
 # }}}
 
 # {{{ testing
 
 REQUIREMENTS=\
 	requirements-dev.txt \
 	requirements.txt
 
 requirements-dev.txt: pyproject.toml
-	$(PYTHON) -m piptools compile \
-		--resolver=backtracking --upgrade \
+	uv pip compile --upgrade --resolution highest \
 		--extra dev \
 		-o $@ $<
+.PHONY: requirements-dev.txt
 
 requirements.txt: pyproject.toml
-	$(PYTHON) -m piptools compile \
-		--resolver=backtracking --upgrade \
+	uv pip compile --upgrade --resolution highest \
 		-o $@ $<
+.PHONY: requirements.txt
 
 pin: $(REQUIREMENTS)	## Pin dependencies versions to requirements.txt
 .PHONY: pin
 
 pip-install:			## Install pinned depdencies from requirements.txt
-	$(PYTHON) -m pip install --upgrade pip setuptools
+	$(PYTHON) -m pip install --upgrade pip hatchling wheel
 	$(PYTHON) -m pip install -r requirements-dev.txt -e .
 .PHONY: pip-install
 
 test:					## Run pytest tests
-	$(PYTHON) -m pytest -rswx --durations=25 -v -s
+	$(PYTHON) -m pytest -m 'not benchmark'
 .PHONY: test
 
+benchmark:				## Run pytest benchmarks
+	$(PYTHON) -m pytest -m 'benchmark' \
+		--benchmark-autosave \
+		--benchmark-storage=docs/benchmarks \
+		--benchmark-name=short \
+		--benchmark-columns=min,max,mean,iqr,ops,rounds \
+		tests/benchmarks
+.PHONY: benchmark
+
 examples:				## Run examples
 	@for ex in $$(find examples -name "*.py"); do \
 		echo -e "\x1b[1;32m===> \x1b[97mRunning $${ex}\x1b[0m"; \
 		$(PYTHON) "$${ex}"; \
 		sleep 1; \
 	done
 .PHONY: examples
```

### Comparing `pycaputo-0.4.0/PKG-INFO` & `pycaputo-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pycaputo
-Version: 0.4.0
+Version: 0.5.0
 Summary: Evaluate fractional integrals and solve fractional ODEs
+Project-URL: Documentation, https://pycaputo.readthedocs.io
+Project-URL: Repository, https://github.com/alexfikl/pycaputo
 Author-email: Alexandru Fikl <alexfikl@gmail.com>
 Maintainer-email: Alexandru Fikl <alexfikl@gmail.com>
 License: MIT
-Project-URL: Documentation, https://pycaputo.readthedocs.io
-Project-URL: Repository, https://github.com/alexfikl/pycaputo
 Keywords: fractional-derivatives,fractional-integrals,quadrature,time-stepping
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
 Requires-Dist: numpy>=1.17
-Requires-Dist: rich
+Requires-Dist: rich>=13
 Requires-Dist: scipy>=1.7
-Requires-Dist: typing-extensions
+Requires-Dist: typing-extensions; python_version < '3.10'
 Provides-Extra: dev
-Requires-Dist: check-manifest; extra == "dev"
-Requires-Dist: codespell; extra == "dev"
-Requires-Dist: differint; extra == "dev"
-Requires-Dist: doc8; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pyproject-fmt; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: reuse; extra == "dev"
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: types-dataclasses; extra == "dev"
+Requires-Dist: codespell; extra == 'dev'
+Requires-Dist: differint; extra == 'dev'
+Requires-Dist: doc8; extra == 'dev'
+Requires-Dist: matplotlib; extra == 'dev'
+Requires-Dist: mypy; extra == 'dev'
+Requires-Dist: pyproject-fmt; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-benchmark; extra == 'dev'
+Requires-Dist: reuse; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Requires-Dist: types-dataclasses; extra == 'dev'
+Requires-Dist: uv; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: sphinx>=6; extra == "docs"
-Requires-Dist: sphinx-book-theme; extra == "docs"
+Requires-Dist: sphinx-book-theme; extra == 'docs'
+Requires-Dist: sphinx>=6; extra == 'docs'
 Provides-Extra: vis
-Requires-Dist: SciencePlots; extra == "vis"
+Requires-Dist: scienceplots; extra == 'vis'
+Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/alexfikl/pycaputo/workflows/CI/badge.svg
     :alt: Build Status
     :target: https://github.com/alexfikl/pycaputo/actions?query=branch%3Amain+workflow%3ACI
 
 .. image:: https://badge.fury.io/py/pycaputo.svg
     :alt: PyPI
```

### Comparing `pycaputo-0.4.0/README.rst` & `pycaputo-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/Makefile` & `pycaputo-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/brusselator-predictor-corrector-cycle-dark.svg` & `pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/brusselator-predictor-corrector-cycle-light.svg` & `pycaputo-0.5.0/docs/brusselator-predictor-corrector-cycle-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/brusselator-predictor-corrector-dark.svg` & `pycaputo-0.5.0/docs/brusselator-predictor-corrector-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/brusselator-predictor-corrector-light.svg` & `pycaputo-0.5.0/docs/brusselator-predictor-corrector-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/caputo-derivative-l1-dark.svg` & `pycaputo-0.5.0/docs/caputo-derivative-l1-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/caputo-derivative-l1-light.svg` & `pycaputo-0.5.0/docs/caputo-derivative-l1-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/changelog.rst` & `pycaputo-0.5.0/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,29 @@
 Changelog
 =========
 
+pycaputo 0.5.0 (April 19, 2024)
+-------------------------------
+
+Features
+^^^^^^^^
+
+* Implement an implicit adaptive L1 type method for Integrate-and-Fire models
+  in :mod:`pycaputo.integrate_fire`.
+* Implement PIF, LIF, EIF and AdEx models explicitly. These can be used to model
+  neurons using fractional dynamics.
+
+Maintenance
+^^^^^^^^^^^
+
+* Use [uv](https://github.com/astral-sh/uv) to handled pinning dependencies.
+* Use [hatchling](https://hatch.pypa.io) as the build backend instead of ``setuptools``.
+* Start using [pytest-benchmark](https://pytest-benchmark.readthedocs.io) to
+  benchmark the code. This still needs a lot of work.
+
 pycaputo 0.4.0 (February 6, 2024)
 ---------------------------------
 
 Features
 ^^^^^^^^
 
 * Implement an implicit L1 method in :class:`pycaputo.fode.caputo.L1`.
```

### Comparing `pycaputo-0.4.0/docs/conf.py` & `pycaputo-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/differentiation.rst` & `pycaputo-0.5.0/docs/differentiation.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/history.rst` & `pycaputo-0.5.0/docs/history.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/index.rst` & `pycaputo-0.5.0/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     operator
     quadrature
     differentiation
     history
     controllers
     timestepping
     fode
+    integrate_fire
     misc
     references
     changelog
 
 .. warning::
 
    This package is currently in development and very experimental (the API
```

### Comparing `pycaputo-0.4.0/docs/misc.rst` & `pycaputo-0.5.0/docs/misc.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/quadrature.rst` & `pycaputo-0.5.0/docs/quadrature.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/references.rst` & `pycaputo-0.5.0/docs/references.rst`

 * *Files 4% similar despite different names*

```diff
@@ -79,7 +79,12 @@
     *Solving Ordinary Differential Equations II - Stiff and Differential-Algebraic Problems*,
     Springer, 2010.
 
 .. [Jannelli2020] A. Jannelli,
     *A Novel Adaptive Procedure for Solving Fractional Differential Equations*,
     Journal of Computational Science, Vol. 47, pp. 101220--101220, 2020,
     `DOI <https://doi.org/10.1016/j.jocs.2020.101220>`__.
+
+.. [Naud2008] R. Naud, N. Marcille, C. Clopath, W. Gerstner,
+    *Firing Patterns in the Adaptive Exponential Integrate-and-Fire Model*,
+    Biological Cybernetics, Vol. 99, pp. 335--347, 2008,
+    `DOI <https://doi.org/10.1007/s00422-008-0264-7>`__.
```

### Comparing `pycaputo-0.4.0/docs/tutorials.rst` & `pycaputo-0.5.0/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-eest-dark.svg` & `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-eest-light.svg` & `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-eest-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-solution-dark.svg` & `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-dark.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/docs/van-der-pol-adaptive-pece-solution-light.svg` & `pycaputo-0.5.0/docs/van-der-pol-adaptive-pece-solution-light.svg`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/brusselator-predictor-corrector.py` & `pycaputo-0.5.0/examples/brusselator-predictor-corrector.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/caputo-derivative-l1.py` & `pycaputo-0.5.0/examples/caputo-derivative-l1.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/caputo-derivative-quadratic.py` & `pycaputo-0.5.0/examples/caputo-derivative-quadratic.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/caputo-gradient-spectral.py` & `pycaputo-0.5.0/examples/caputo-gradient-spectral.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/example-custom-diff.py` & `pycaputo-0.5.0/examples/example-custom-diff.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/example-custom-quad.py` & `pycaputo-0.5.0/examples/example-custom-quad.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/example-lipschitz-weibull.py` & `pycaputo-0.5.0/examples/example-lipschitz-weibull.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/lorenz-weighted-euler.py` & `pycaputo-0.5.0/examples/lorenz-weighted-euler.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/examples/van-der-pol-adaptive-pece.py` & `pycaputo-0.5.0/examples/van-der-pol-adaptive-pece.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/pyproject.toml` & `pycaputo-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [build-system]
-build-backend = "setuptools.build_meta"
+build-backend = "hatchling.build"
 requires = [
-    "setuptools>=61",
-    "wheel",
+    "hatchling>=1.10",
 ]
 
 [project]
 name = "pycaputo"
-version = "0.4.0"
+version = "0.5.0"
 description = "Evaluate fractional integrals and solve fractional ODEs"
 readme = "README.rst"
 keywords = [
     "fractional-derivatives",
     "fractional-integrals",
     "quadrature",
     "time-stepping",
@@ -35,50 +34,49 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
     "Topic :: Utilities",
 ]
 dependencies = [
     "numpy>=1.17",
-    "rich",
+    "rich>=13",
     "scipy>=1.7",
-    "typing-extensions",
+    'typing-extensions; python_version < "3.10"',
 ]
 [project.optional-dependencies]
 dev = [
-    "check-manifest",
     "codespell",
     "differint",
     "doc8",
     "matplotlib",
     "mypy",
-    "pip-tools",
     "pyproject-fmt",
     "pytest",
+    "pytest-benchmark",
     "reuse",
     "ruff",
     "types-dataclasses",
+    "uv",
 ]
 docs = [
     "sphinx>=6",
     "sphinx-book-theme",
 ]
 vis = [
     "SciencePlots",
 ]
 [project.urls]
 Documentation = "https://pycaputo.readthedocs.io"
 Repository = "https://github.com/alexfikl/pycaputo"
 
-[tool.setuptools]
-package-dir = { "" = "src" }
-packages = { find = { where = ["src"] } }
+[tool.hatch.build.targets.sdist]
+exclude = [".github", ".ci", "docs/_build"]
 
-[tool.setuptools.package-data]
-pycaputo = ["py.typed"]
+[tool.hatch.build.targets.wheel]
+packages = ["src/pycaputo"]
 
 [tool.ruff]
 preview = true
 target-version = "py38"
 line-length = 88
 
 [tool.ruff.lint]
@@ -114,47 +112,53 @@
     "PLR0911",  # too-many-return-statements
     "PLR0912",  # too-many-branches
     "PLR0913",  # too-many-arguments
     "PLR0914",  # too-many-locals
     "PLR0915",  # too-many-statements
     "PLR0917",  # too-many-positional
     "PLR6301",  # no-self-use
+    "PLR6104",  # non-augmented-assignment
     "PLR2004",  # magic-value-comparison
     "S101",     # assert
     "S102",     # exec-builtin
     "UP037",    # quoted-annotation
 ]
 
 [tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 inline-quotes = "double"
 multiline-quotes = "double"
 
 [tool.ruff.lint.isort]
 known-first-party = ["pycaputo"]
+force-wrap-aliases = true
 
-[tool.check-manifest]
-ignore = [
-    "*.yml",
-    "*.yaml",
-    ".ci/*",
+[tool.pytest.ini_options]
+testpaths = "tests"
+addopts = [
+    "-rswx",
+    "--durations=25",
+    "--capture=no",
+    "--verbose",
 ]
 
 [tool.mypy]
 strict = true
 hide_error_codes = false
 warn_unused_ignores = true
+local_partial_types = true
 plugins = "numpy.typing.mypy_plugin"
 
 [[tool.mypy.overrides]]
 module = [
+    "SciencePlots.*",
     "differint.*",
     "mittleff.*",
-    "scipy.*",
-    "SciencePlots.*",
+    "pytest_benchmark.*",
     "scienceplots.*",
+    "scipy.*",
 ]
 ignore_missing_imports = true
 
 [tool.doc8]
 max-line-length = 88
 ignore-path = "src/*.egg-info"
```

### Comparing `pycaputo-0.4.0/scripts/generate-doc-figures.py` & `pycaputo-0.5.0/scripts/generate-doc-figures.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/__init__.py` & `pycaputo-0.5.0/src/pycaputo/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/controller.py` & `pycaputo-0.5.0/src/pycaputo/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,32 +215,37 @@
 
     A controller is used to decide if a time step can be accepted and give an
     estimate for the next time step. If the controller is adaptive, it should
     also give guarantees that the next time step will be accepted with high
     probability.
     """
 
-    #: Start of the time interval.
     tstart: float
-    #: End of the time interval (leave *None* for infinite time stepping).
+    """Start of the time interval."""
     tfinal: float | None
-    #: Number of time steps (leave *None* for infinite time stepping).
+    """End of the time interval (leave *None* for infinite time stepping)."""
     nsteps: int | None
+    """Number of time steps (leave *None* for infinite time stepping)."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if self.tfinal is not None and self.tstart > self.tfinal:
                 raise ValueError("Invalid time interval: 'tstart' > 'tfinal'")
 
             if self.nsteps is not None and self.nsteps <= 0:
                 raise ValueError(
                     f"Number of iterations must be positive: {self.nsteps}"
                 )
 
+    @property
+    def is_adaptive(self) -> bool:
+        """*True* if the controller is adaptive."""
+        return True
+
     def finished(self, n: int, t: float) -> bool:
         """Check if the evolution should finish at iteration *n* and time *t*."""
         # fmt: off
         return (
             (self.tfinal is not None and t >= self.tfinal)
             or (self.nsteps is not None and n >= self.nsteps))
         # fmt: on
@@ -330,20 +335,27 @@
 
 # }}}
 
 
 # {{{ non-adaptive controller
 
 
+# {{{ FixedController
+
+
 @dataclass(frozen=True)
 class FixedController(Controller):
     """A fake controller with a fixed time step."""
 
-    #: Fixed time step used by the controller.
     dt: float
+    """Fixed time step used by the controller."""
+
+    @property
+    def is_adaptive(self) -> bool:
+        return False
 
 
 @evaluate_error_estimate.register(FixedController)
 def _evaluate_error_estimate_fixed(
     c: FixedController,
     m: FractionalDifferentialEquationMethod[StateFunctionT],
     trunc: Array,
@@ -374,14 +386,20 @@
     if c.tfinal is not None:
         eps = 5.0 * np.finfo(m.y0[0].dtype).eps
         dt = min(dt, c.tfinal - state["t"]) + eps
 
     return dt
 
 
+# }}}
+
+
+# {{{ GradedController
+
+
 @dataclass(frozen=True)
 class GradedController(Controller):
     r"""A :class:`Controller` with a variable graded time step.
 
     This graded grid of time steps is described in [Garrappa2015b]_. It
     essentially takes the form
 
@@ -391,17 +409,18 @@
 
     where the time interval is :math:`[t_s, t_f]` and :math:`N` time steps are
     taken. This graded grid can give full second-order convergence for certain
     methods such as the Predictor-Corrector method (e.g. implemented by
     :class:`~pycaputo.fode.caputo.PECE`).
     """
 
-    #: A grading exponent that controls the clustering of points at
-    #: :attr:`~Controller.tstart`.
     r: float
+    """A grading exponent that controls the clustering of points at
+    :attr:`~Controller.tstart`.
+    """
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if self.tfinal is None:
                 raise ValueError("'tfinal' must be given for the graded estimate.")
 
@@ -409,23 +428,17 @@
                 raise ValueError("'nsteps' must be given for the graded estimate")
 
             if self.r < 1:
                 raise ValueError(f"Exponent must be >= 1: {self.r}")
 
             super().__post_init__()
 
-    def estimate_initial_time_step(
-        self,
-        m: FractionalDifferentialEquationMethod[StateFunctionT],
-        t: float,
-        y: Array,
-    ) -> float:
-        assert self.tfinal is not None
-        assert self.nsteps is not None
-        return float((self.tfinal - self.tstart) / self.nsteps**self.r)
+    @property
+    def is_adaptive(self) -> bool:
+        return False
 
 
 @evaluate_error_estimate.register(GradedController)
 def _evaluate_error_estimate_graded(
     c: GradedController,
     m: FractionalDifferentialEquationMethod[StateFunctionT],
     trunc: Array,
@@ -464,14 +477,16 @@
         dt = min(dt, c.tfinal - state["t"]) + eps
 
     return float(dt)
 
 
 # }}}
 
+# }}}
+
 
 # {{{ adaptive controller
 
 
 @dataclass(frozen=True)
 class AdaptiveController(Controller):
     r"""An adaptive time step controller.
@@ -499,28 +514,30 @@
         \sqrt{\frac{1}{M} \sum_{i = 0}^{M - 1} \left(\mathcal{E}^{n + 1}_i\right)^2}
 
     The time step is rejected if :math:`E^{n + 1}_{\text{scaled}} > 1` and
     accepted otherwise. Each controller decides the manner in which the time
     step is updated for each of these cases.
     """
 
-    #: Smallest allowable time step by the controller.
     dtmin: float
+    """Smallest allowable time step by the controller."""
 
-    #: Smallest allowable step change factor. If the factor is larger than this,
-    #: no change in the time step will be added.
     qmin: float
-    #: Largest allowable step change factor. If the factor is smaller than this,
-    #: no change in the time step will be added.
+    """Smallest allowable step change factor. If the factor is larger than this,
+    no change in the time step will be added.
+    """
     qmax: float
+    """Largest allowable step change factor. If the factor is smaller than this,
+    no change in the time step will be added.
+    """
 
-    #: Absolute tolerance used by the controller to compute a scaled norm.
     abstol: float
-    #: Relative tolerance used by the controller to compute a scaled norm.
+    """Absolute tolerance used by the controller to compute a scaled norm."""
     reltol: float
+    """Relative tolerance used by the controller to compute a scaled norm."""
 
     nrejects: int = field(default=0, init=False)
 
     @property
     def max_rejects(self) -> int:
         return 16
 
@@ -560,14 +577,15 @@
         raise StepEstimateError("Scaled error estimate is not finite")
 
     return eest
 
 
 # }}}
 
+
 # {{{ integral controller
 
 
 @dataclass(frozen=True)
 class IntegralController(AdaptiveController):
     r"""A standard integral controller.
 
@@ -741,15 +759,15 @@
 
     return dt
 
 
 # }}}
 
 
-# {{{ Jannelli integral controller
+# {{{ Jannelli error controller
 
 
 def make_jannelli_controller(
     tstart: float = 0.0,
     tfinal: float | None = None,
     nsteps: int | None = None,
     *,
@@ -758,15 +776,21 @@
     rho: float = 1.5,
     chimin: float | None = None,
     chimax: float | None = None,
     abstol: float = 1.0e-8,
 ) -> JannelliIntegralController:
     r"""Construct a :class:`JannelliIntegralController`.
 
-    This functions simply provides some useful defaults
+    This functions simply provides some useful defaults. The main parameters
+    for the model are the :math:`\chi_{min}` and :math:`\chi_{max}`, which
+    effectively determine the error thresholds at which the step size should
+    change. In general, the rule of thumb is:
+
+    * :math:`\chi_{min}`: smaller values make it harder to increase the step size.
+    * :math:`\chi_{max}`: larger values make it harder to decrease the step size.
 
     :arg sigma: factor by which the time step will be decreased in the case the
         step is rejected. A default value of ``0.5`` will half the time step
         each time, but smaller increments are possible.
     :arg rho: factor by which the time step will be increased in the case the
         step is accepted. A default value of ``1.5`` with increase the time
         step by half each time, but smaller increments are possible.
@@ -816,18 +840,18 @@
 
     The time step is then adapted using a fixed factor, based on
     :attr:`~AdaptiveController.qmin` (denoted by :math:`\sigma`) as a decrease
     factor and :attr:`~AdaptiveController.qmax` (denoted by :math:`\rho`) as
     the amplification factor.
     """
 
-    #: Minimum limit of the error estimate.
     chimin: float
-    #: Maximum limit of the error estimate.
+    """Minimum limit of the error estimate."""
     chimax: float
+    """Maximum limit of the error estimate."""
 
 
 @evaluate_error_estimate.register(JannelliIntegralController)
 def _evaluate_error_estimate_jannelli(
     c: JannelliIntegralController,
     m: FractionalDifferentialEquationMethod[StateFunctionT],
     trunc: Array,
```

### Comparing `pycaputo-0.4.0/src/pycaputo/derivatives.py` & `pycaputo-0.5.0/src/pycaputo/derivatives.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 import math
 from dataclasses import dataclass
 
 
 class Side(enum.Enum):
     """Side of a fractional derivative, if any."""
 
-    #: Denotes the left side, e.g. :math:`[a, x]` for intervals around :math:`x`.
     Left = enum.auto()
-    #: Denotes the right side, e.g. :math:`[x, b]` for intervals around :math:`x`.
+    """Denotes the left side, e.g. :math:`[a, x]` for intervals around :math:`x`."""
     Right = enum.auto()
+    """Denotes the right side, e.g. :math:`[x, b]` for intervals around :math:`x`."""
 
 
 @dataclass(frozen=True)
 class FractionalOperator:
     """Generic type of a fractional order operator.
 
     Subclasses can define any form of a fractional order derivative or integral.
     This includes classic derivatives, such as the Riemann-Liouville derivative,
     or more modern operators that do not necessarily satisfy all the fractional
     derivative axioms (or can even be reduced to integer order derivatives).
 
     For a recent review of these operators see [SalesTeodoro2019]_.
     """
 
-    #: Order of the fractional operator, as a real number
-    #: :math:`\alpha \in \mathbb{R}`. A positive number would denote a derivative,
-    #: while a negative number would denote a fractional integral, as supported.
     order: float
+    r"""Order of the fractional operator, as a real number
+    :math:`\alpha \in \mathbb{R}`. A positive number would denote a derivative,
+    while a negative number would denote a fractional integral, as supported.
+    """
 
     @property
     def n(self) -> int:
         raise NotImplementedError
 
 
 @dataclass(frozen=True)
@@ -53,16 +54,16 @@
             \frac{\mathrm{d}^n}{\mathrm{d} x^n} \int_a^x
             \frac{f(s)}{(x - s)^{\alpha + 1 - n}} \,\mathrm{d}s,
 
     while the upper Riemann-Liouville fractional derivative is integrated on
     :math:`[x, b]` with a factor of :math:`(-1)^n`.
     """
 
-    #: Side on which to compute the derivative.
     side: Side
+    """Side on which to compute the derivative."""
 
     @property
     def n(self) -> int:
         r"""Integer part of the :attr:`~FractionalOperator.order`, i.e.
         :math:`n - 1 \le \text{order} < n`.
         """
         return math.floor(self.order + 1)
@@ -82,16 +83,16 @@
             \frac{f^{(n)}(s)}{(x - s)^{\alpha + 1 - n}} \,\mathrm{d}s,
 
     while the upper Caputo fractional derivative is integrated on :math:`[x, b]`.
     Note that for negative orders, the Caputo derivative is defined as the
     Riemann-Liouville integral.
     """
 
-    #: Side on which to compute the derivative.
     side: Side
+    """Side on which to compute the derivative."""
 
     @property
     def n(self) -> int:
         r"""Integer part of the :attr:`~FractionalOperator.order`, i.e.
         :math:`n - 1 < \text{order} \le n`.
         """
         return math.ceil(self.order)
@@ -111,16 +112,16 @@
             \sum_{k = 0}^{N(h)} (-1)^k
             \frac{\Gamma(\alpha + 1)}{\Gamma(k + 1) \Gamma(\alpha + 1 - k)}
             f(x - k h),
 
     where :math:`N(h) = (x - a) / h`. The upper derivative is similarly defined.
     """
 
-    #: Side on which to compute the derivative.
     side: Side
+    """Side on which to compute the derivative."""
 
     @property
     def n(self) -> int:
         r"""Integer part of the :attr:`~FractionalOperator.order`, i.e.
         :math:`n - 1 \le \text{order} < n`.
         """
         return math.floor(self.order + 1)
@@ -137,9 +138,9 @@
     .. math::
 
         D_{H}^\alpha[f](x) = \frac{\alpha}{\Gamma(1 - \alpha)}
             \frac{\mathrm{d}^n}{\mathrm{d} x^n}
             \int_a^x (\log x - \log s)^{2 + n - \alpha} \frac{f(s)}{s} \,\mathrm{d}s.
     """
 
-    #: Side on which to compute the derivative.
     side: Side
+    """Side on which to compute the derivative."""
```

### Comparing `pycaputo-0.4.0/src/pycaputo/differentiation/__init__.py` & `pycaputo-0.5.0/src/pycaputo/differentiation/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/differentiation/base.py` & `pycaputo-0.5.0/src/pycaputo/differentiation/base.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/differentiation/caputo.py` & `pycaputo-0.5.0/src/pycaputo/differentiation/caputo.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 logger = get_logger(__name__)
 
 
 @dataclass(frozen=True)
 class CaputoDerivativeMethod(DerivativeMethod):
     """A method used to evaluate a :class:`~pycaputo.derivatives.CaputoDerivative`."""
 
-    #: A Caputo derivative to discretize.
     d: CaputoDerivative
+    """A Caputo derivative to discretize."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             super().__post_init__()
             if not isinstance(self.d, CaputoDerivative):
                 raise TypeError(
```

### Comparing `pycaputo-0.4.0/src/pycaputo/differentiation/riemann_liouville.py` & `pycaputo-0.5.0/src/pycaputo/differentiation/riemann_liouville.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 
 @dataclass(frozen=True)
 class RiemannLiouvilleDerivativeMethod(DerivativeMethod):
     """A method used to evaluate a
     :class:`~pycaputo.derivatives.RiemannLiouvilleDerivative`."""
 
-    #: A Riemann-Liouville derivative to discretize.
     d: RiemannLiouvilleDerivative
+    """A Riemann-Liouville derivative to discretize."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             super().__post_init__()
             if not isinstance(self.d, RiemannLiouvilleDerivative):
                 raise TypeError(
@@ -55,16 +55,16 @@
                 f^{(k)}(a).
 
     so any method approximating the Caputo derivative can be repurposed to
     also approximate the Riemann-Liouville derivative with the addition of
     initial terms.
     """
 
-    #: A Riemann-Liouville derivative to discretize
     d: RiemannLiouvilleDerivative
+    """A Riemann-Liouville derivative to discretize"""
 
     @property
     def caputo(self) -> CaputoDerivativeMethod:
         raise AttributeError
 
     @property
     def order(self) -> float:
@@ -139,24 +139,24 @@
 
     if 0.0 < alpha <= 1.0:
         # NOTE: handled above
         pass
     elif 1.0 < alpha <= 2.0:
         # NOTE: this is a 3rd order approximation of the derivative at f(a)
         # that works on non-uniform grids too (derived by Mathematica)
-        # fmt: off
         dfx = (
+            # fmt: off
             (fx[0] - fx[1]) / (x[0] - x[1])
             + (fx[0] - fx[2]) / (x[0] - x[2])
             + (fx[0] - fx[3]) / (x[0] - x[3])
             - (fx[1] - fx[2]) / (x[1] - x[2])
             - (fx[1] - fx[3]) * (x[0] - x[2]) / ((x[1] - x[2]) * (x[1] - x[3]))
             + (fx[2] - fx[3]) * (x[0] - x[1]) / ((x[1] - x[2]) * (x[2] - x[3]))
+            # fmt: on
         )
-        # fmt: on
 
         df[1:] += dfx / (x[1:] - x[0]) ** (alpha - 1) / math.gamma(2 - alpha)
     else:
         raise AssertionError
 
     return df
```

### Comparing `pycaputo-0.4.0/src/pycaputo/finite_difference.py` & `pycaputo-0.5.0/src/pycaputo/finite_difference.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 from pycaputo.utils import Array
 
 
 class Truncation(NamedTuple):
     """A representation of the truncation error of a :class:`DiffStencil`."""
 
-    #: Order of the approximation.
     order: int
-    #: Truncation error coefficient (without the function derivative).
+    """Order of the approximation."""
     error: float
+    """Truncation error coefficient (without the function derivative)."""
 
 
 @dataclass(frozen=True)
 class DiffStencil:
     r"""Approximation of a derivative by finite difference on a uniform grid.
 
     .. math::
@@ -32,20 +32,20 @@
         \approx \frac{1}{h^n} \sum_{k \in \text{offsets}} a_k f_{m + k}
 
     where :math:`a_k` are the given coefficients :attr:`coeffs` and :math:`f_m`
     are the point function evaluations. The approximation is to an order and
     truncation error can be retrieved from :attr:`trunc`.
     """
 
-    #: Order of the derivative approximated by the stencil.
+    """Order of the derivative approximated by the stencil."""
     derivative: int
-    #: Coefficients used in the stencil.
     coeffs: Array
-    #: Offsets around the centered :math:`0` used in the stencil.
+    """Coefficients used in the stencil."""
     offsets: Array
+    """Offsets around the centered :math:`0` used in the stencil."""
 
     @cached_property
     def padded_coeffs(self) -> Array:
         """Padded coefficients that are symmetric around the :math:`0`
         index and can be easily applied as a convolution.
         """
         n = np.max(np.abs(self.offsets))
```

### Comparing `pycaputo-0.4.0/src/pycaputo/fode/caputo.py` & `pycaputo-0.5.0/src/pycaputo/fode/caputo.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,23 +145,25 @@
     Note that for :math:`\theta = 0` we get the forward Euler method, which
     is first order, for :math:`\theta = 1` we get the backward Euler method,
     which is first order, and for :math:`\theta = 1/2` we get the Crank-Nicolson
     method, which is order :math:`1 + \alpha`. This method only becomes second
     order in the limit of :math:`\alpha \to 1`.
     """
 
-    #: Parameter weight between the forward and backward Euler methods. The value
-    #: of :math:`\theta = 1/2` gives the standard Crank-Nicolson method.
     theta: float
+    r"""Parameter weight between the forward and backward Euler methods. The value
+    of :math:`\theta = 1/2` gives the standard Crank-Nicolson method.
+    """
 
-    #: Jacobian of
-    #: :attr:`~pycaputo.stepping.FractionalDifferentialEquationMethod.source`.
-    #: By default, implicit methods use :mod:`scipy` for their root finding,
-    #: which defines the Jacobian as :math:`J_{ij} = \partial f_i / \partial y_j`.
     source_jac: StateFunctionT | None
+    r"""Jacobian of
+    :attr:`~pycaputo.stepping.FractionalDifferentialEquationMethod.source`.
+    By default, implicit methods use :mod:`scipy` for their root finding,
+    which defines the Jacobian as :math:`J_{ij} = \partial f_i / \partial y_j`.
+    """
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if not 0.0 <= self.theta <= 1.0:
                 raise ValueError(
                     f"'theta' parameter must be in [0, 1]: got {self.theta}"
@@ -283,16 +285,16 @@
 
     Note that using a high number of corrector iterations is not recommended, as
     the fixed point iteration is not guaranteed to converge, e.g. for very stiff
     problems. In that case it is better to use an implicit method and, e.g.,
     a Newton iteration to solve the root finding problem.
     """
 
-    #: Number of repetitions of the corrector step.
     corrector_iterations: int
+    """Number of repetitions of the corrector step."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if self.corrector_iterations < 1:
                 raise ValueError(
                     "More than one corrector iteration is required:"
@@ -494,21 +496,20 @@
         dy, _ = _update_caputo_adams_bashforth2(dy, history, alpha, n=n)
 
         # compute predictor
         yp = np.copy(dy)
 
         k = n - 1
 
-        # fmt: off
         omega = (
-            ts[k] ** (alpha + 1) / gamma2 / ds[k]
-            + ts[k] ** alpha / gamma1
-            )
+            # fmt: off
+            ts[k] ** (alpha + 1) / gamma2 / ds[k] + ts[k] ** alpha / gamma1
+            # fmt: on
+        )
         yp += omega * history.storage[k - 1]
-        # fmt: on
 
         omega = -(ts[k] ** (alpha + 1)) / gamma2 / ds[k]
         yp += omega * history.storage[k]
 
     # compute corrector
     ynext = np.copy(dy)
 
@@ -547,19 +548,20 @@
     """The first-order implicit L1 discretization of the Caputo derivative.
 
     Note that, unlike the :class:`ForwardEuler` method, the L1 method discretizes
     the Caputo derivative directly and does not use the Volterra formulation of
     the equation.
     """
 
-    #: Jacobian of
-    #: :attr:`~pycaputo.stepping.FractionalDifferentialEquationMethod.source`.
-    #: By default, implicit methods use :mod:`scipy` for their root finding,
-    #: which defines the Jacobian as :math:`J_{ij} = \partial f_i / \partial y_j`.
     source_jac: StateFunctionT | None
+    r"""Jacobian of
+    :attr:`~pycaputo.stepping.FractionalDifferentialEquationMethod.source`.
+    By default, implicit methods use :mod:`scipy` for their root finding,
+    which defines the Jacobian as :math:`J_{ij} = \partial f_i / \partial y_j`.
+    """
 
     @property
     def order(self) -> float:
         return 2.0 - self.largest_derivative_order
 
     def _get_kwargs(self, *, scalar: bool = True) -> dict[str, object]:
         """
```

### Comparing `pycaputo-0.4.0/src/pycaputo/fode/product_integration.py` & `pycaputo-0.5.0/src/pycaputo/fode/product_integration.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 logger = get_logger(__name__)
 
 
 class AdvanceResult(NamedTuple):
     """Result of :func:`~pycaputo.stepping.advance` for
     :class:`ProductIntegrationMethod` subclasses."""
 
-    #: Estimated solution at the next time step.
     y: Array
-    #: Estimated truncation error at the next time step.
+    """Estimated solution at the next time step."""
     trunc: Array
-    #: Array to add to the history storage.
+    """Estimated truncation error at the next time step."""
     storage: Array
+    """Array to add to the history storage."""
 
 
 @dataclass(frozen=True)
 class ProductIntegrationMethod(FractionalDifferentialEquationMethod[StateFunctionT]):
     """A generic class of methods based on Product Integration.
 
     In general, these methods support a variable time step.
```

### Comparing `pycaputo-0.4.0/src/pycaputo/generating_functions.py` & `pycaputo-0.5.0/src/pycaputo/generating_functions.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/grid.py` & `pycaputo-0.5.0/src/pycaputo/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 # {{{ non-uniform points
 
 
 @dataclass(frozen=True)
 class Points:
     """A collection of points in an interval :math:`[a, b]`."""
 
-    #: The left boundary of the interval.
     a: float
-    #: The right boundary of the interval.
+    """The left boundary of the interval."""
     b: float
-    #: The array of points.
+    """The right boundary of the interval."""
     x: Array
+    """The array of points."""
 
     def __len__(self) -> int:
         return len(self.x)
 
     @property
-    def dtype(self) -> "np.dtype[Any]":
+    def dtype(self) -> np.dtype[Any]:
         """The :class:`numpy.dtype` of the points in the set."""
         return np.dtype(self.x.dtype)
 
     @property
     def size(self) -> int:
         """The number of points in the set."""
         return self.x.size
@@ -178,20 +178,20 @@
     """A set of Jacobi-Gauss-Lobatto points on :math:`[a, b]`.
 
     See :func:`scipy.special.roots_jacobi`. This can also be used for quadrature
     using :attr:`w` and is accurate for polynomials of degreen up to
     :math:`2 n - 3`.
     """
 
-    #: Parameter of the Jacobi polynomials.
     alpha: float
-    #: Parameter of the Jacobi poylnomials.
+    """Parameter of the Jacobi polynomials."""
     beta: float
-    #: Jacobi-Gauss-Lobatto quadrature weights on :math:`[a, b]`.
+    """Parameter of the Jacobi poylnomials."""
     w: Array
+    """Jacobi-Gauss-Lobatto quadrature weights on :math:`[a, b]`."""
 
     def translate(self, a: float, b: float) -> Points:
         """Linearly translate the set of points to the new interval :math:`[a, b]`."""
         # translate from [a', b'] to [0, 1] to [a, b]
         r = (b - a) / (self.b - self.a)
         x = a - r * self.a + r * self.x
         w = r * self.w
```

### Comparing `pycaputo-0.4.0/src/pycaputo/history.py` & `pycaputo-0.5.0/src/pycaputo/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     """
 
     def __iter__(self) -> Iterable[Any]:
         for f in fields(self):
             yield getattr(self, f.name)
 
 
-#: Invariant type variable bound to :class:`State`.
 T = TypeVar("T", bound=State)
+"""Invariant type variable bound to :class:`State`."""
 
 
 class History(ABC, Generic[T]):
     """A class handling the history checkpointing of an evolution equation.
 
     It essentially acts as a queue from which the items cannot be removed. For
     inspiration check out :class:`collections.deque`.
@@ -89,20 +89,21 @@
     This storage automatically grows when it exceeds its capacity and allows
     for easy retrieval of specific time steps. Note that, to resize the arrays
     no external references to them must exist. For example,
     ``ts = history.ts[:n]`` will create such a reference and a copy should be
     made instead if absolutely necessary.
     """
 
-    #: An array of shape ``(n, ...)`` containing the stored values. Note that
-    #: this is not necessarily the solution itself, but can be any data that is
-    #: required for storage in the method.
     storage: Array = field(repr=False)
-    #: An array of shape ``(n,)`` containing the fixed time steps.
+    """An array of shape ``(n, ...)`` containing the stored values. Note that
+    this is not necessarily the solution itself, but can be any data that is
+    required for storage in the method.
+    """
     ts: Array = field(repr=False)
+    """An array of shape ``(n,)`` containing the fixed time steps."""
 
     filled: int = field(default=0, repr=False, init=False)
 
     @property
     def capacity(self) -> int:
         """The maximum size currently available for storage."""
         return self.ts.size
@@ -175,27 +176,27 @@
 
 @dataclass(frozen=True)
 class ProductIntegrationState(State):
     """A state history that holds the right-hand side evaluations used by
     standard Product Integration methods.
     """
 
-    #: Time of the evaluation.
     t: float
-    #: Evaluation of the right-hand side.
+    """Time of the evaluation."""
     f: Array
+    """Evaluation of the right-hand side."""
 
 
 @dataclass(frozen=True)
 class ProductIntegrationHistory(InMemoryHistory[ProductIntegrationState]):
     """A history for Product Integration methods with variable time step."""
 
     def __getitem__(self, k: int) -> ProductIntegrationState:
-        if k == -1:
-            k = self.filled - 1
+        if k <= -1:
+            k = self.filled + k
 
         if not 0 <= k < self.filled:
             raise IndexError(f"History index out of range: 0 <= {k} < {self.filled}")
 
         return ProductIntegrationState(self.ts[k], self.storage[k])
```

### Comparing `pycaputo-0.4.0/src/pycaputo/implicit.py` & `pycaputo-0.5.0/src/pycaputo/implicit.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/interpolation.py` & `pycaputo-0.5.0/src/pycaputo/interpolation.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,20 +24,20 @@
     where :math:`\ell_k` is the :math:`k`-th Lagrange polynomial. The approximation
     is of the :attr:`order` of the Lagrange polynomials.
 
     Note that Lagrange polynomials are notoriously ill-conditioned on uniform
     grids (Runge phenomenon), so they should not be used with high-order.
     """
 
-    #: Coefficients used in the stencil.
     coeffs: Array
-    #: Offsets around the centered :math:`0` used in the stencil.
+    """Coefficients used in the stencil."""
     offsets: Array
-    #: Point at which the interpolation was evaluated.
+    """Offsets around the centered :math:`0` used in the stencil."""
     x: float
+    """Point at which the interpolation was evaluated."""
 
     @property
     def order(self) -> int:
         """Order of the Lagrange polynomial."""
         return self.coeffs.size
 
     @cached_property
```

### Comparing `pycaputo-0.4.0/src/pycaputo/jacobi.py` & `pycaputo-0.5.0/src/pycaputo/jacobi.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/lagrange.py` & `pycaputo-0.5.0/src/pycaputo/lagrange.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/lipschitz.py` & `pycaputo-0.5.0/src/pycaputo/lipschitz.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/logging.py` & `pycaputo-0.5.0/src/pycaputo/logging.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/mittagleffler.py` & `pycaputo-0.5.0/src/pycaputo/mittagleffler.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 logger = get_logger(__name__)
 
 
 @enum.unique
 class Algorithm(enum.Enum):
     """Algorithm used to compute the Mittag-Leffler function."""
 
-    #: The standard series definition is used to compute the function. This
-    #: choice can be very slow to converge for certain arguments and parameters.
-    #: It is not recommended for production use.
     Series = enum.auto()
+    """The standard series definition is used to compute the function. This
+    choice can be very slow to converge for certain arguments and parameters.
+    It is not recommended for production use.
+    """
 
-    #: Algorithm by [Diethelm2005]_.
     Diethelm = enum.auto()
+    """Algorithm by [Diethelm2005]_."""
 
-    #: Algorithm by [Garrappa2015]_.
     Garrappa = enum.auto()
+    """Algorithm by [Garrappa2015]_."""
 
-    #: Algorithm by [Ortigueira2019]_.
     Ortigueira = enum.auto()
+    """Algorithm by [Ortigueira2019]_."""
 
 
 # {{{ series
 
 
 def mittag_leffler_series(
     z: complex,
@@ -47,14 +48,20 @@
 ) -> complex:
     if eps is None:
         eps = 2 * float(np.finfo(np.array(z).dtype).eps)
 
     if kmax is None:
         kmax = 2048
 
+    if abs(z) >= 1.0:
+        raise ValueError(
+            "The series expansion of the Mittag-Leffler function "
+            "only converges for |z| < 1"
+        )
+
     result, term = 0j, 1j
     k = 0
     while abs(term) > eps and k <= kmax:
         term = z**k / math.gamma(alpha * k + beta)
         result += term
         k += 1
 
@@ -239,15 +246,15 @@
         #   https://sistemas.fc.unesp.br/ojs/index.php/revistacqd/article/view/306
         K = _ml_quad_k(zabs + 1, chi0, alpha, beta, z, eps=eps)
         P = _ml_quad_p(-api, api, alpha, beta, zabs + 1, z, eps=eps)
 
         return K + P
 
     k0 = math.floor(-math.log(eps) / math.log(zabs))
-    result = -sum((z**-k / math.gamma(beta - alpha * k) for k in range(k0)), 0.0)
+    result = -sum((z**-k / math.gamma(beta - alpha * k + eps) for k in range(k0)), 0.0)
 
     if zarg < 0.75 * alpha * np.pi:
         result += z ** ((1 - beta) / alpha) * cmath.exp(z ** (1 / alpha)) / alpha
 
     return result
```

### Comparing `pycaputo-0.4.0/src/pycaputo/quadrature/__init__.py` & `pycaputo-0.5.0/src/pycaputo/quadrature/__init__.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/src/pycaputo/quadrature/base.py` & `pycaputo-0.5.0/src/pycaputo/quadrature/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pycaputo.utils import Array, ArrayOrScalarFunction
 
 
 @dataclass(frozen=True)
 class QuadratureMethod(ABC):
     """A generic method used to evaluate a fractional integral."""
 
-    #: Description of the integral that is approximated.
     d: FractionalOperator
+    """Description of the integral that is approximated."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if self.d.order >= 0:
                 raise ValueError(
                     f"Integral requires a negative order: order is '{self.d.order}'"
```

### Comparing `pycaputo-0.4.0/src/pycaputo/quadrature/riemann_liouville.py` & `pycaputo-0.5.0/src/pycaputo/quadrature/riemann_liouville.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from .base import QuadratureMethod, quad
 
 
 @dataclass(frozen=True)
 class RiemannLiouvilleMethod(QuadratureMethod):
     """Quadrature method for the Riemann-Liouville integral."""
 
-    #: Description of the integral that is approximated.
     d: RiemannLiouvilleDerivative
+    """Description of the integral that is approximated."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             super().__post_init__()
             if not isinstance(self.d, RiemannLiouvilleDerivative):
                 raise TypeError(
@@ -43,16 +43,16 @@
     uses a piecewise constant approximation on each subinterval and cannot
     be used to evaluate the value at the starting point, i.e.
     :math:`I_{RL}^\alpha[f](a)` is not defined.
 
     This method is of order :math:`\mathcal{O}(h)` and supports arbitrary grids.
     """
 
-    #: Weight used in the approximation :math:`\theta f_k + (1 - \theta) f_{k + 1}`.
     theta: float = 0.5
+    r"""Weight used in the approximation :math:`\theta f_k + (1 - \theta) f_{k + 1}`."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             super().__post_init__()
             if not 0.0 <= self.theta <= 1.0:
                 raise ValueError(
@@ -440,24 +440,25 @@
 
     These quadrature methods are modelled on the Backward Differencing Formulas
     (BDF) and only support orders up to :math:`6`.
 
     This quadrature method only supports on uniform grids.
     """
 
-    #: The order of the convolution quadrature method. Only orders up to 6 are
-    #: currently supported, see
-    #: :func:`~pycaputo.generating_functions.lubich_bdf_weights` for additional
-    #: details.
     quad_order: int
-    #: An exponent used in constructing the starting weights of the quadrature.
-    #: Negative values will allow for certain singularities at the origin, while
-    #: a default of :math:`\beta = 1` will benefit a smooth function. Setting
-    #: this to ``float("inf")`` will disable the starting weights.
+    """The order of the convolution quadrature method. Only orders up to 6 are
+    currently supported, see :func:`~pycaputo.generating_functions.lubich_bdf_weights`
+    for additional details.
+    """
     beta: float
+    r"""An exponent used in constructing the starting weights of the quadrature.
+    Negative values will allow for certain singularities at the origin, while
+    a default of :math:`\beta = 1` will benefit a smooth function. Setting
+    this to ``float("inf")`` will disable the starting weights.
+    """
 
     if __debug__:
 
         def __post_init__(self) -> None:
             super().__post_init__()
 
             if not 1 <= self.quad_order <= 6:
```

### Comparing `pycaputo-0.4.0/src/pycaputo/stepping.py` & `pycaputo-0.5.0/src/pycaputo/stepping.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,23 @@
 
     where the Caputo derivative :math:`D_C^\alpha` is used with
     :math:`\alpha \in (0, 1)`. In this case, only :math:`y(0)` is required
     as an initial condition. Different derivatives or higher-order derivatives
     will required additional initial data.
     """
 
-    #: The fractional derivative order used for the derivative.
     derivative_order: tuple[float, ...]
-    #: An instance describing the discrete time being simulated.
+    """The fractional derivative order used for the derivative."""
     control: Controller
+    """An instance describing the discrete time being simulated."""
 
-    #: Right-hand side source term.
     source: StateFunctionT
-    #: Values used to reconstruct the required initial conditions.
+    """Right-hand side source term."""
     y0: tuple[Array, ...]
+    """Values used to reconstruct the required initial conditions."""
 
     if __debug__:
 
         def __post_init__(self) -> None:
             if not self.y0:
                 raise ValueError("No initial conditions given")
```

### Comparing `pycaputo-0.4.0/src/pycaputo/utils.py` & `pycaputo-0.5.0/src/pycaputo/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,48 +13,55 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     ClassVar,
     Iterable,
     Iterator,
+    Literal,
     NamedTuple,
     Protocol,
     TypeVar,
     Union,
     runtime_checkable,
 )
 
 import numpy as np
-from typing_extensions import Concatenate, ParamSpec, TypeAlias
+
+try:
+    # NOTE: available in Python >=3.10
+    from typing import Concatenate, ParamSpec
+except ImportError:
+    from typing_extensions import Concatenate, ParamSpec  # type: ignore[assignment]
 
 from pycaputo.logging import get_logger
 
 logger = get_logger(__name__)
 
 
 # {{{ typing
 
-#: A generic invariant :class:`typing.TypeVar`.
 T = TypeVar("T")
-#: A generic invariant :class:`typing.TypeVar`.
+"""A generic invariant :class:`typing.TypeVar`."""
 R = TypeVar("R")
+"""A generic invariant :class:`typing.TypeVar`."""
 P = ParamSpec("P")
+"""A generic invariant :class:`typing.ParamSpec`."""
 
-#: A union of types supported as paths.
 PathLike = Union[pathlib.Path, str]
+"""A union of types supported as paths."""
 
 if TYPE_CHECKING:
-    Array: TypeAlias = np.ndarray[Any, Any]
-    Scalar: TypeAlias = Union[np.generic, Array]
+    Array = np.ndarray[Any, Any]
+    Scalar = Union[np.generic, Array]
 else:
-    #: Array type alias for :class:`numpy.ndarray`.
-    Array: TypeAlias = np.ndarray
-    #: Scalar type alias (generally a value convertible to a :class:`float`).
-    Scalar: TypeAlias = Union[np.generic, Array]
+    Array = np.ndarray
+    """Array type alias for :class:`numpy.ndarray`."""
+    Scalar = Union[np.generic, Array]
+    """Scalar type alias (generally a value convertible to a :class:`float`)."""
 
 
 class DataclassInstance(Protocol):
     """Dataclass protocol from
     `typeshed <https://github.com/python/typeshed/blob/770724013de34af6f75fa444cdbb76d187b41875/stdlib/_typeshed/__init__.pyi#L329-L334>`__."""
 
     __dataclass_fields__: ClassVar[dict[str, Field[Any]]]
@@ -68,15 +75,14 @@
 
     def __call__(self, x: Array, /) -> Array:
         """
         :arg x: a scalar or array at which to evaluate the function.
         """
 
 
-@runtime_checkable
 class StateFunction(Protocol):
     r"""A generic callable for right-hand side functions
     :math:`\mathbf{f}(t, \mathbf{y})`.
 
     .. automethod:: __call__
     """
 
@@ -130,19 +136,19 @@
         """Evaluate the function or any of its derivatives.
 
         :arg x: a scalar or array at which to evaluate the function.
         :arg d: order of the derivative.
         """
 
 
-#: A invaraint :class:`~typing.TypeVar` bound to :class:`StateFunction`.
 StateFunctionT = TypeVar("StateFunctionT", bound=StateFunction)
+"""An invariant :class:`~typing.TypeVar` bound to :class:`StateFunction`."""
 
-#: A union of scalar functions.
 ArrayOrScalarFunction = Union[Array, ScalarFunction, DifferentiableScalarFunction]
+"""A union of scalar functions."""
 
 # fmt: off
 BOOLEAN_STATES = {
     1: True, "1": True, "yes": True, "true": True, "on": True, "y": True,
     0: False, "0": False, "no": False, "false": False, "off": False, "n": False,
 }
 # fmt: on
@@ -153,21 +159,31 @@
 # {{{ Estimated Order of Convergence (EOC)
 
 
 @dataclass(frozen=True)
 class EOCRecorder:
     """Keep track of all your *estimated order of convergence* needs."""
 
-    #: A string identifier for the value which is estimated.
     name: str = "Error"
-    #: An expected order of convergence, if any.
+    """A string identifier for the value which is estimated."""
     order: float | None = None
+    """An expected order of convergence, if any."""
 
-    #: A list of ``(h, error)`` entries added from :meth:`add_data_point`.
     history: list[tuple[float, float]] = field(default_factory=list, repr=False)
+    """A list of ``(h, error)`` entries added from :meth:`add_data_point`."""
+
+    @classmethod
+    def from_data(
+        cls, name: str, h: Array, error: Array, *, order: float | None = None
+    ) -> EOCRecorder:
+        eoc = cls(name=name, order=order)
+        for i in range(h.size):
+            eoc.add_data_point(h[i], error[i])
+
+        return eoc
 
     def add_data_points(self, h: Array, error: Array) -> None:
         """Add multiple data points using :meth:`add_data_point`."""
         for h_i, e_i in zip(h, error):
             self.add_data_point(h_i, e_i)
 
     def add_data_point(self, h: Any, error: Any) -> None:
@@ -298,14 +314,91 @@
 
     return "\n".join([
         " | ".join(fmt.format(value) for fmt, value in zip(formats, line))
         for line in lines
     ])
 
 
+def visualize_eoc(
+    filename: pathlib.Path,
+    *eocs: EOCRecorder,
+    order: float | None = None,
+    abscissa: str | Literal[False] = "h",
+    ylabel: str | Literal[False] = "Error",
+    olabel: str | Literal[False] | None = None,
+    enable_legend: bool = True,
+    overwrite: bool = True,
+) -> None:
+    """Plot the given :class:`EOCRecorder` instances in a loglog plot.
+
+    :arg filename: output file name for the figure.
+    :arg order: expected order for all the errors recorded in *eocs*.
+    :arg abscissa: name for the abscissa.
+    """
+    if not eocs:
+        raise ValueError("no EOCRecorders are provided")
+
+    if order is not None and order <= 0.0:
+        raise ValueError(f"The 'order' should be a non-negative real number: {order}")
+
+    markers = ["o", "v", "^", "<", ">", "x", "+", "d", "D"]
+    with figure(filename, overwrite=overwrite) as fig:
+        ax = fig.gca()
+
+        # {{{ plot eocs
+
+        line = None
+        for eoc, marker in zip(eocs, markers):
+            h, error = np.array(eoc.history).T
+            ax.loglog(h, error, marker=marker, label=eoc.name)
+
+            imax = np.argmax(h)
+            max_h = h[imax]
+            max_e = error[imax]
+            min_e = np.min(error)
+
+            if eoc.order is not None:
+                order = eoc.order
+                min_h = np.exp(np.log(max_h) + np.log(min_e / max_e) / eoc.order)
+                (line,) = ax.loglog(
+                    [max_h, min_h],
+                    [max_e, min_e],
+                    "k--",
+                )
+
+        if abscissa and line is not None:
+            if olabel is None:
+                hname = abscissa.strip("$")
+                if order == 1:
+                    olabel = rf"$\mathcal{{O}}({hname})$"
+                else:
+                    olabel = rf"$\mathcal{{O}}({hname}^{{{order:g}}})$"
+
+            if olabel:
+                line.set_label(olabel)
+
+        # }}}
+
+        # {{{ plot order
+
+        # }}}
+
+        ax.grid(visible=True, which="major", linestyle="-", alpha=0.75)
+        ax.grid(visible=True, which="minor", linestyle="--", alpha=0.5)
+
+        if abscissa:
+            ax.set_xlabel(abscissa)
+
+        if ylabel:
+            ax.set_ylabel(ylabel)
+
+        if enable_legend and (len(eocs) > 1 or (line and olabel)):
+            ax.legend()
+
+
 # }}}
 
 
 # {{{ matplotlib helpers
 
 
 def check_usetex(*, s: bool) -> bool:
@@ -324,25 +417,26 @@
 
         if not shutil.which("tex"):
             return False
 
         if not shutil.which("dvipng"):
             return False
 
-        if not shutil.which("gs"):
+        if not shutil.which("gs"):  # noqa: SIM103
             return False
 
         return True
 
 
 def set_recommended_matplotlib(
     *,
     use_tex: bool | None = None,
     dark: bool | None = None,
     savefig_format: str | None = None,
+    overrides: dict[str, Any] | None = None,
 ) -> None:
     """Set custom :mod:`matplotlib` parameters.
 
     These are mainly used in the tests and examples to provide a uniform style
     to the results using `SciencePlots <https://github.com/garrettj403/SciencePlots>`__.
     For other applications, it is recommended to use local settings (e.g. in
     `matplotlibrc`).
@@ -352,52 +446,58 @@
     :arg dark: if *True*, a dark default theme is selected instead of the
         default light one (see the ``dark_background`` theme of the ``SciencePlots``
         package). If *None*, this takes its values from the ``PYCAPUTO_DARK``
         boolean environment variable.
     :arg savefig_format: the format used when saving figures. By default, this
         uses the ``PYCAPUTO_SAVEFIG`` environment variable and falls back to
         the :mod:`matplotlib` parameter ``savefig.format``.
+    :arg overrides: a mapping of parameters to override the defaults. These
+        can also be set separately after this function was called.
     """
     try:
         import matplotlib.pyplot as mp
     except ImportError:
         return
 
     if use_tex is None:
         use_tex = "GITHUB_REPOSITORY" not in os.environ and check_usetex(s=True)
 
+    if not use_tex:
+        logger.warning("'use_tex' is disabled on this system.")
+
     if dark is None:
         tmp = os.environ.get("PYCAPUTO_DARK", "off").lower()
         dark = BOOLEAN_STATES.get(tmp, False)
 
     if savefig_format is None:
         savefig_format = os.environ.get(
             "PYCAPUTO_SAVEFIG", mp.rcParams["savefig.format"]
         ).lower()
 
     defaults: dict[str, dict[str, Any]] = {
         "figure": {
             "figsize": (8, 8),
             "dpi": 300,
-            "constrained_layout": {"use": True},
+            "constrained_layout.use": True,
         },
         "savefig": {"format": savefig_format},
         "text": {"usetex": use_tex},
         "legend": {"fontsize": 32},
         "lines": {"linewidth": 2, "markersize": 10},
         "axes": {
-            "labelsize": 32,
-            "titlesize": 32,
+            "labelsize": 28,
+            "titlesize": 28,
             "grid": True,
+            "grid.axis": "both",
+            "grid.which": "both",
             # NOTE: preserve existing colors (the ones in "science" are ugly)
             "prop_cycle": mp.rcParams["axes.prop_cycle"],
         },
-        "xtick": {"labelsize": 24, "direction": "inout"},
-        "ytick": {"labelsize": 24, "direction": "inout"},
-        "axes.grid": {"axis": "both", "which": "both"},
+        "xtick": {"labelsize": 20, "direction": "inout"},
+        "ytick": {"labelsize": 20, "direction": "inout"},
         "xtick.major": {"size": 6.5, "width": 1.5},
         "ytick.major": {"size": 6.5, "width": 1.5},
         "xtick.minor": {"size": 4.0},
         "ytick.minor": {"size": 4.0},
     }
 
     with suppress(ImportError):
@@ -415,15 +515,18 @@
         # NOTE: matplotlib v3.6 deprecated all the seaborn styles
         mp.style.use("seaborn-v0_8-dark" if dark else "seaborn-v0_8-white")
     elif "seaborn" in mp.style.library:
         # NOTE: for older versions of matplotlib
         mp.style.use("seaborn-dark" if dark else "seaborn-white")
 
     for group, params in defaults.items():
-        with suppress(KeyError):
+        mp.rc(group, **params)
+
+    if overrides:
+        for group, params in overrides.items():
             mp.rc(group, **params)
 
 
 @contextmanager
 def figure(
     filename: PathLike | None = None,
     nrows: int = 1,
@@ -484,35 +587,33 @@
         ext = mp.rcParams["savefig.format"]
         filename = filename.with_suffix(f".{ext}").resolve()
 
     if not overwrite and filename.exists():
         raise FileExistsError(f"Output file '{filename}' already exists")
 
     logger.info("Saving '%s'", filename)
-
-    fig.tight_layout()
     fig.savefig(filename, **kwargs)
 
 
 # }}}
 
 
 # {{{ timing
 
 
 @dataclass(frozen=True)
 class TimingResult:
     """Statistics for a set of runs (see :func:`timeit`)."""
 
-    #: Minimum walltime for a set of runs.
     walltime: float
-    #: Mean walltime for a set of runs.
+    """Minimum walltime for a set of runs."""
     mean: float
-    #: Standard derivation for a set of runs.
+    """Mean walltime for a set of runs."""
     std: float
+    """Standard derivation for a set of runs."""
 
     @classmethod
     def from_results(cls, results: list[float]) -> TimingResult:
         """Gather statistics from a set of runs."""
         rs = np.array(results)
 
         return TimingResult(
@@ -557,26 +658,28 @@
 
         with BlockTimer("my-code-block") as bt:
             # do some code
 
         print(bt)
     """
 
-    #: An identifier used to differentiate the timer.
     name: str = "block"
+    """An identifier used to differentiate the timer."""
 
-    #: Total wall time (set after ``__exit__``), obtained from
-    #: :func:`time.perf_counter`.
-    t_wall: float = field(init=False)
     t_wall_start: float = field(init=False)
+    t_wall: float = field(init=False)
+    """Total wall time (set after ``__exit__``), obtained from
+    :func:`time.perf_counter`.
+    """
 
-    #: Total process time (set after ``__exit__``), obtained from
-    #: :func:`time.process_time`.
-    t_proc: float = field(init=False)
     t_proc_start: float = field(init=False)
+    t_proc: float = field(init=False)
+    """Total process time (set after ``__exit__``), obtained from
+    :func:`time.process_time`.
+    """
 
     @property
     def t_cpu(self) -> float:
         """Total CPU time, obtained from ``t_proc / t_wall``."""
         return self.t_proc / self.t_wall
 
     def __enter__(self) -> BlockTimer:
```

### Comparing `pycaputo-0.4.0/tests/mittag_leffler_ref.py` & `pycaputo-0.5.0/tests/mittag_leffler_ref.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_diff_caputo.py` & `pycaputo-0.5.0/tests/test_diff_caputo.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_diff_riemann_liouville.py` & `pycaputo-0.5.0/tests/test_diff_riemann_liouville.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_finite_difference.py` & `pycaputo-0.5.0/tests/test_finite_difference.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
             sign = part(1.0j**s.derivative)
 
             ax = fig.gca()
             ax.plot(k, km)
             ax.plot(k, sign * k**s.derivative, "k--")
 
             ax.set_xlabel("$k h$")
-            ax.set_ylabel(r"$\tilde{k} h$")
+            ax.set_ylabel(r"$\tilde{k} h$")  # noqa: RUF027
             ax.set_xlim(0.0, float(np.pi))
             ax.set_ylim(0.0, float(sign * np.pi**s.derivative))
 
             dirname = pathlib.Path(__file__).parent
             filename = f"test_diff_fd_{s.derivative}_{s.trunc.order}"
             savefig(fig, dirname / filename)
```

### Comparing `pycaputo-0.4.0/tests/test_fode.py` & `pycaputo-0.5.0/tests/test_fode.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_fode_caputo.py` & `pycaputo-0.5.0/tests/test_fode_caputo.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_generating_functions.py` & `pycaputo-0.5.0/tests/test_generating_functions.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_interpolation.py` & `pycaputo-0.5.0/tests/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_jacobi.py` & `pycaputo-0.5.0/tests/test_jacobi.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_misc.py` & `pycaputo-0.5.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_mittag_leffler.py` & `pycaputo-0.5.0/tests/test_mittag_leffler.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_points.py` & `pycaputo-0.5.0/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `pycaputo-0.4.0/tests/test_quad_riemann_liouville.py` & `pycaputo-0.5.0/tests/test_quad_riemann_liouville.py`

 * *Files identical despite different names*

