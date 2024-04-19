# Comparing `tmp/lmfit-1.3.0.tar.gz` & `tmp/lmfit-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmfit-1.3.0.tar", last modified: Thu Apr  4 17:31:35 2024, max compression
+gzip compressed data, was "lmfit-1.3.1.tar", last modified: Fri Apr 19 16:02:50 2024, max compression
```

## Comparing `lmfit-1.3.0.tar` & `lmfit-1.3.1.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.696514 lmfit-1.3.0/
--rw-r--r--   0 Newville   (501) staff       (20)      308 2024-04-04 17:29:11.000000 lmfit-1.3.0/.codecov.yml
--rw-r--r--   0 Newville   (501) staff       (20)      393 2024-04-04 17:29:11.000000 lmfit-1.3.0/.gitattributes
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.661185 lmfit-1.3.0/.github/
--rw-r--r--   0 Newville   (501) staff       (20)     5158 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/CONTRIBUTING.md
--rw-r--r--   0 Newville   (501) staff       (20)     2901 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)     2211 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)      502 2024-04-04 17:29:11.000000 lmfit-1.3.0/.github/dependabot.yml
--rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-04 17:29:11.000000 lmfit-1.3.0/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1789 2024-04-04 17:29:11.000000 lmfit-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 Newville   (501) staff       (20)     3015 2024-04-04 17:29:11.000000 lmfit-1.3.0/AUTHORS.txt
--rw-r--r--   0 Newville   (501) staff       (20)     3670 2024-04-04 17:29:11.000000 lmfit-1.3.0/LICENSE
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.665527 lmfit-1.3.0/NIST_STRD/
--rw-r--r--   0 Newville   (501) staff       (20)     6869 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Bennett5.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1713 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/BoxBOD.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7558 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Chwirut1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3060 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Chwirut2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1990 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/DanWood.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6761 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/ENSO.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2773 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Eckerle4.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8098 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8100 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8102 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Gauss3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9276 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Hahn1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5858 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Kirby2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2945 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2601 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2574 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Lanczos3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2305 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH09.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2335 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH10.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3078 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/MGH17.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1853 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1a.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1845 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1b.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1839 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1c.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1843 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Misra1d.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6401 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Models
--rw-r--r--   0 Newville   (501) staff       (20)     7001 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Nelson.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1873 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Rat42.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2072 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Rat43.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2486 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Roszman1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3026 2024-04-04 17:29:11.000000 lmfit-1.3.0/NIST_STRD/Thurber.dat
--rw-r--r--   0 Newville   (501) staff       (20)    13054 2024-04-04 17:31:35.696052 lmfit-1.3.0/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     6229 2024-04-04 17:29:11.000000 lmfit-1.3.0/README.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.666163 lmfit-1.3.0/asv_benchmarking/
--rw-r--r--   0 Newville   (501) staff       (20)       43 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/README.md
--rw-r--r--   0 Newville   (501) staff       (20)     2793 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/asv.conf.json
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.666478 lmfit-1.3.0/asv_benchmarking/benchmarks/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/benchmarks/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     4394 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/benchmarks/benchmarks.py
--rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-04 17:29:11.000000 lmfit-1.3.0/asv_benchmarking/run_benchmark_code.py
--rw-r--r--   0 Newville   (501) staff       (20)    12203 2024-04-04 17:29:11.000000 lmfit-1.3.0/azure-pipelines.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669610 lmfit-1.3.0/doc/
--rw-r--r--   0 Newville   (501) staff       (20)     4529 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/Makefile
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669803 lmfit-1.3.0/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.669947 lmfit-1.3.0/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      756 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     3499 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/bounds.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30647 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/builtin_models.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6530 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)    16305 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/confidence.rst
--rw-r--r--   0 Newville   (501) staff       (20)     8110 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/constraints.rst
--rw-r--r--   0 Newville   (501) staff       (20)      223 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/contents.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/doc_examples_to_gallery.py
--rw-r--r--   0 Newville   (501) staff       (20)    12177 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/faq.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)      657 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/filter_spurious_link_from_html.py
--rw-r--r--   0 Newville   (501) staff       (20)    40606 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/fitting.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5143 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     9268 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/intro.rst
--rw-r--r--   0 Newville   (501) staff       (20)      941 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/make.bat
--rw-r--r--   0 Newville   (501) staff       (20)    50953 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/model.rst
--rw-r--r--   0 Newville   (501) staff       (20)     4670 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/parameters.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.670382 lmfit-1.3.0/doc/sphinx/
--rw-r--r--   0 Newville   (501) staff       (20)      460 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/ext_imgmath.py
--rw-r--r--   0 Newville   (501) staff       (20)      407 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/ext_mathjax.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.658261 lmfit-1.3.0/doc/sphinx/theme/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.670942 lmfit-1.3.0/doc/sphinx/theme/sphinx13/
--rw-r--r--   0 Newville   (501) staff       (20)     7586 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/basic_layout.html
--rw-r--r--   0 Newville   (501) staff       (20)     3080 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/layout.html
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.672040 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/
--rw-r--r--   0 Newville   (501) staff       (20)      429 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/bodybg.png
--rw-r--r--   0 Newville   (501) staff       (20)      180 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/footerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      189 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/headerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      149 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/listitem.png
--rw-r--r--   0 Newville   (501) staff       (20)     9907 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png
--rw-r--r--   0 Newville   (501) staff       (20)      183 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/relbg.png
--rw-r--r--   0 Newville   (501) staff       (20)     7978 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/sphinx13.css
--rw-r--r--   0 Newville   (501) staff       (20)       72 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/sphinx/theme/sphinx13/theme.conf
--rw-r--r--   0 Newville   (501) staff       (20)     1500 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/support.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30537 2024-04-04 17:29:11.000000 lmfit-1.3.0/doc/whatsnew.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.682089 lmfit-1.3.0/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     8195 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/NIST_Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)      419 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/README.txt
--rw-r--r--   0 Newville   (501) staff       (20)   392918 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/discuss_model_eval_uncertainty.ipynb
--rw-r--r--   0 Newville   (501) staff       (20)     1419 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_nistgauss.py
--rw-r--r--   0 Newville   (501) staff       (20)     1010 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_nistgauss2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1364 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_peakmodels.py
--rw-r--r--   0 Newville   (501) staff       (20)     1961 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_splinemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      784 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_builtinmodels_stepmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)     1964 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_advanced.py
--rw-r--r--   0 Newville   (501) staff       (20)      481 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     3795 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_confidence_chi2_maps.py
--rw-r--r--   0 Newville   (501) staff       (20)     3359 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_fitting_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)      969 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_fitting_withreport.py
--rw-r--r--   0 Newville   (501) staff       (20)     1953 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_composite.py
--rw-r--r--   0 Newville   (501) staff       (20)      651 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_gaussian.py
--rw-r--r--   0 Newville   (501) staff       (20)      774 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      531 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      537 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_loadmodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      337 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      423 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      996 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_savemodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      862 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_two_components.py
--rw-r--r--   0 Newville   (501) staff       (20)      834 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty.py
--rw-r--r--   0 Newville   (501) staff       (20)     3148 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty2.py
--rw-r--r--   0 Newville   (501) staff       (20)     5383 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_uncertainty_pred.py
--rw-r--r--   0 Newville   (501) staff       (20)     1051 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_with_iter_callback.py
--rw-r--r--   0 Newville   (501) staff       (20)      775 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_model_with_nan_policy.py
--rw-r--r--   0 Newville   (501) staff       (20)     1499 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_parameters_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     1252 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_parameters_valuesdict.py
--rw-r--r--   0 Newville   (501) staff       (20)     2417 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/doc_uvars_params.py
--rw-r--r--   0 Newville   (501) staff       (20)     7666 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1867 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)    17926 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)     4731 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_complex_resonator_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     4378 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_confidence_interval.py
--rw-r--r--   0 Newville   (501) staff       (20)     3331 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_detect_outliers.py
--rw-r--r--   0 Newville   (501) staff       (20)     1795 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_diffev.py
--rw-r--r--   0 Newville   (501) staff       (20)     4098 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_emcee_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1273 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_expression_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     2716 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_multi_datasets.py
--rw-r--r--   0 Newville   (501) staff       (20)     1417 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     2161 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)     2666 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_derivfunc.py
--rw-r--r--   0 Newville   (501) staff       (20)     2190 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_fit_with_inequality.py
--rw-r--r--   0 Newville   (501) staff       (20)     2378 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_reduce_fcn.py
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_sympy.py
--rw-r--r--   0 Newville   (501) staff       (20)     6112 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_two_dimensional_peak.py
--rw-r--r--   0 Newville   (501) staff       (20)      851 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/example_use_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)     7776 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/lmfit_emcee_model_selection.py
--rw-r--r--   0 Newville   (501) staff       (20)     2373 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/model1d_gauss.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1987 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/peak.csv
--rw-r--r--   0 Newville   (501) staff       (20)     2464 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/sinedata.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9496 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/test_peak.dat
--rw-r--r--   0 Newville   (501) staff       (20)    11611 2024-04-04 17:29:11.000000 lmfit-1.3.0/examples/test_splinepeak.dat
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.685597 lmfit-1.3.0/lmfit/
--rw-r--r--   0 Newville   (501) staff       (20)     1956 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    10016 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)    21021 2023-12-31 16:26:04.000000 lmfit-1.3.0/lmfit/conf_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)    16981 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     5251 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)    16913 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)   105588 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    91579 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/model.py
--rw-r--r--   0 Newville   (501) staff       (20)    68814 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/models.py
--rw-r--r--   0 Newville   (501) staff       (20)    40207 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    16055 2024-04-04 17:29:11.000000 lmfit-1.3.0/lmfit/printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)      411 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit/version.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.693863 lmfit-1.3.0/lmfit.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)    13054 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     5290 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)      423 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        6 2024-04-04 17:31:35.000000 lmfit-1.3.0/lmfit.egg-info/top_level.txt
--rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2024-04-04 17:29:11.000000 lmfit-1.3.0/publish_docs.sh
--rw-r--r--   0 Newville   (501) staff       (20)     3056 2024-04-04 17:29:11.000000 lmfit-1.3.0/pyproject.toml
--rw-r--r--   0 Newville   (501) staff       (20)       38 2024-04-04 17:31:35.696578 lmfit-1.3.0/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2024-04-04 17:29:11.000000 lmfit-1.3.0/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.692922 lmfit-1.3.0/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     6109 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/NISTModels.py
--rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      893 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/conftest.py
--rw-r--r--   0 Newville   (501) staff       (20)     5656 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/gauss_modelresult_lmfit100.sav
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-04 17:31:35.693390 lmfit-1.3.0/tests/saved_models/
--rw-r--r--   0 Newville   (501) staff       (20)      767 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py310_lm122.sav
--rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py311_lm122.sav
--rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/saved_models/sinemodel_py312_lm122.sav
--rw-r--r--   0 Newville   (501) staff       (20)     1374 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_1variable.py
--rw-r--r--   0 Newville   (501) staff       (20)     7097 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_NIST_Strd.py
--rw-r--r--   0 Newville   (501) staff       (20)     4008 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     4640 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1238 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_basicfit.py
--rw-r--r--   0 Newville   (501) staff       (20)     3663 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)     1900 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_bounded_jacobian.py
--rw-r--r--   0 Newville   (501) staff       (20)     1413 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)    11428 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)    11953 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_builtin_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     9251 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     9987 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_covariance_matrix.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_custom_independentvar.py
--rw-r--r--   0 Newville   (501) staff       (20)      612 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_default_kws.py
--rw-r--r--   0 Newville   (501) staff       (20)     2259 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_dual_annealing.py
--rw-r--r--   0 Newville   (501) staff       (20)     4292 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_itercb.py
--rw-r--r--   0 Newville   (501) staff       (20)     3066 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)     6266 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_least_squares.py
--rw-r--r--   0 Newville   (501) staff       (20)     4780 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)      781 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_manypeaks_speed.py
--rw-r--r--   0 Newville   (501) staff       (20)     3689 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_max_nfev.py
--rw-r--r--   0 Newville   (501) staff       (20)     2686 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    58586 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model.py
--rw-r--r--   0 Newville   (501) staff       (20)    12648 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model_saveload.py
--rw-r--r--   0 Newville   (501) staff       (20)     4354 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_model_uncertainties.py
--rw-r--r--   0 Newville   (501) staff       (20)     4965 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     2181 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_multidatasets.py
--rw-r--r--   0 Newville   (501) staff       (20)    24062 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_nose.py
--rw-r--r--   0 Newville   (501) staff       (20)     1168 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)    19779 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    21262 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_parameters.py
--rw-r--r--   0 Newville   (501) staff       (20)     4367 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_params_uvars.py
--rw-r--r--   0 Newville   (501) staff       (20)    14955 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)     3999 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_shgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1503 2024-04-04 17:29:11.000000 lmfit-1.3.0/tests/test_stepmodel.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.685166 lmfit-1.3.1/
+-rw-r--r--   0 Newville   (501) staff       (20)      308 2024-04-19 16:02:36.000000 lmfit-1.3.1/.codecov.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      393 2024-04-19 16:02:36.000000 lmfit-1.3.1/.gitattributes
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.646917 lmfit-1.3.1/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)     5158 2024-04-19 16:02:36.000000 lmfit-1.3.1/.github/CONTRIBUTING.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2901 2024-04-19 16:02:36.000000 lmfit-1.3.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2211 2024-04-19 16:02:36.000000 lmfit-1.3.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2024-04-19 16:02:36.000000 lmfit-1.3.1/.github/dependabot.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-19 16:02:36.000000 lmfit-1.3.1/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1789 2024-04-19 16:02:36.000000 lmfit-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 Newville   (501) staff       (20)     3015 2024-04-19 16:02:36.000000 lmfit-1.3.1/AUTHORS.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     3670 2024-04-19 16:02:36.000000 lmfit-1.3.1/LICENSE
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.651625 lmfit-1.3.1/NIST_STRD/
+-rw-r--r--   0 Newville   (501) staff       (20)     6869 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Bennett5.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1713 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/BoxBOD.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7558 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Chwirut1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3060 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Chwirut2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1990 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/DanWood.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6761 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/ENSO.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2773 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Eckerle4.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8098 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Gauss1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8100 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8102 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Gauss3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9276 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Hahn1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5858 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Kirby2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2945 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Lanczos1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2601 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Lanczos2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2574 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Lanczos3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2305 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/MGH09.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2335 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/MGH10.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3078 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/MGH17.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1853 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Misra1a.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1845 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Misra1b.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1839 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Misra1c.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1843 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Misra1d.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6401 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Models
+-rw-r--r--   0 Newville   (501) staff       (20)     7001 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Nelson.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1873 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Rat42.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2072 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Rat43.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2486 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Roszman1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3026 2024-04-19 16:02:36.000000 lmfit-1.3.1/NIST_STRD/Thurber.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    13093 2024-04-19 16:02:50.684708 lmfit-1.3.1/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     6229 2024-04-19 16:02:36.000000 lmfit-1.3.1/README.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.652161 lmfit-1.3.1/asv_benchmarking/
+-rw-r--r--   0 Newville   (501) staff       (20)       43 2024-04-19 16:02:36.000000 lmfit-1.3.1/asv_benchmarking/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2793 2024-04-19 16:02:36.000000 lmfit-1.3.1/asv_benchmarking/asv.conf.json
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.652730 lmfit-1.3.1/asv_benchmarking/benchmarks/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:36.000000 lmfit-1.3.1/asv_benchmarking/benchmarks/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4394 2024-04-19 16:02:36.000000 lmfit-1.3.1/asv_benchmarking/benchmarks/benchmarks.py
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2024-04-19 16:02:36.000000 lmfit-1.3.1/asv_benchmarking/run_benchmark_code.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12203 2024-04-19 16:02:36.000000 lmfit-1.3.1/azure-pipelines.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.657961 lmfit-1.3.1/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)     4529 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/Makefile
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.658137 lmfit-1.3.1/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.658284 lmfit-1.3.1/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      756 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3499 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/bounds.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30647 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/builtin_models.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6530 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16305 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/confidence.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     8110 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/constraints.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      223 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/contents.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/doc_examples_to_gallery.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12177 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/faq.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)      657 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/filter_spurious_link_from_html.py
+-rw-r--r--   0 Newville   (501) staff       (20)    40606 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/fitting.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     5143 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     9268 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/intro.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      941 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/make.bat
+-rw-r--r--   0 Newville   (501) staff       (20)    50953 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/model.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     4670 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/parameters.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.658602 lmfit-1.3.1/doc/sphinx/
+-rw-r--r--   0 Newville   (501) staff       (20)      460 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/ext_imgmath.py
+-rw-r--r--   0 Newville   (501) staff       (20)      407 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/ext_mathjax.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.644036 lmfit-1.3.1/doc/sphinx/theme/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.659104 lmfit-1.3.1/doc/sphinx/theme/sphinx13/
+-rw-r--r--   0 Newville   (501) staff       (20)     7586 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/basic_layout.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3080 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/layout.html
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.660229 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/
+-rw-r--r--   0 Newville   (501) staff       (20)      429 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/bodybg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      180 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/footerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      189 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/headerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      149 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/listitem.png
+-rw-r--r--   0 Newville   (501) staff       (20)     9907 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png
+-rw-r--r--   0 Newville   (501) staff       (20)      183 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/relbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)     7978 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/sphinx13.css
+-rw-r--r--   0 Newville   (501) staff       (20)       72 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/sphinx/theme/sphinx13/theme.conf
+-rw-r--r--   0 Newville   (501) staff       (20)     1500 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/support.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    31351 2024-04-19 16:02:36.000000 lmfit-1.3.1/doc/whatsnew.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.670052 lmfit-1.3.1/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     8195 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/NIST_Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)      419 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/README.txt
+-rw-r--r--   0 Newville   (501) staff       (20)   392918 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/discuss_model_eval_uncertainty.ipynb
+-rw-r--r--   0 Newville   (501) staff       (20)     1419 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_builtinmodels_nistgauss.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1010 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_builtinmodels_nistgauss2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1364 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_builtinmodels_peakmodels.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1961 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_builtinmodels_splinemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      784 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_builtinmodels_stepmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1964 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_confidence_advanced.py
+-rw-r--r--   0 Newville   (501) staff       (20)      481 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_confidence_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3795 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_confidence_chi2_maps.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3359 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_fitting_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)      969 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_fitting_withreport.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1953 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_composite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      651 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_gaussian.py
+-rw-r--r--   0 Newville   (501) staff       (20)      774 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_loadmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      531 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_loadmodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      537 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_loadmodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      337 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_savemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_savemodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      996 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_savemodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_two_components.py
+-rw-r--r--   0 Newville   (501) staff       (20)      834 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_uncertainty.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3148 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_uncertainty2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5383 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_uncertainty_pred.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1051 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_with_iter_callback.py
+-rw-r--r--   0 Newville   (501) staff       (20)      775 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_model_with_nan_policy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1499 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_parameters_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1252 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_parameters_valuesdict.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2417 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/doc_uvars_params.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7666 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1867 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)    17926 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4731 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_complex_resonator_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4378 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_confidence_interval.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3331 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_detect_outliers.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1795 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_diffev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4098 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_emcee_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1273 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_expression_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2716 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_fit_multi_datasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1417 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_fit_with_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2161 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_fit_with_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2666 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_fit_with_derivfunc.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2190 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_fit_with_inequality.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2378 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_reduce_fcn.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_sympy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6112 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_two_dimensional_peak.py
+-rw-r--r--   0 Newville   (501) staff       (20)      851 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/example_use_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7776 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/lmfit_emcee_model_selection.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2373 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/model1d_gauss.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1987 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/peak.csv
+-rw-r--r--   0 Newville   (501) staff       (20)     2464 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/sinedata.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9496 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/test_peak.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    11611 2024-04-19 16:02:36.000000 lmfit-1.3.1/examples/test_splinepeak.dat
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.673048 lmfit-1.3.1/lmfit/
+-rw-r--r--   0 Newville   (501) staff       (20)     1956 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10016 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21021 2023-12-31 16:26:04.000000 lmfit-1.3.1/lmfit/conf_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16981 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5258 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16913 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)   105588 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    91862 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    68838 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/models.py
+-rw-r--r--   0 Newville   (501) staff       (20)    40207 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16055 2024-04-19 16:02:36.000000 lmfit-1.3.1/lmfit/printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)      411 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit/version.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.682377 lmfit-1.3.1/lmfit.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)    13093 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     5290 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)      431 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        6 2024-04-19 16:02:50.000000 lmfit-1.3.1/lmfit.egg-info/top_level.txt
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2024-04-19 16:02:36.000000 lmfit-1.3.1/publish_docs.sh
+-rw-r--r--   0 Newville   (501) staff       (20)     3128 2024-04-19 16:02:36.000000 lmfit-1.3.1/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)       38 2024-04-19 16:02:50.685239 lmfit-1.3.1/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2024-04-19 16:02:36.000000 lmfit-1.3.1/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.681343 lmfit-1.3.1/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     6109 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/NISTModels.py
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)      893 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/conftest.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5656 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/gauss_modelresult_lmfit100.sav
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-19 16:02:50.681855 lmfit-1.3.1/tests/saved_models/
+-rw-r--r--   0 Newville   (501) staff       (20)      767 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/saved_models/sinemodel_py310_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/saved_models/sinemodel_py311_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)      863 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/saved_models/sinemodel_py312_lm122.sav
+-rw-r--r--   0 Newville   (501) staff       (20)     1374 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_1variable.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7097 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_NIST_Strd.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4008 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4640 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1238 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_basicfit.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3663 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1900 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_bounded_jacobian.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1413 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11428 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11953 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_builtin_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9251 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9987 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_covariance_matrix.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1235 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_custom_independentvar.py
+-rw-r--r--   0 Newville   (501) staff       (20)      612 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_default_kws.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2259 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_dual_annealing.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4292 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_itercb.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3066 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6266 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_least_squares.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4780 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)      781 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_manypeaks_speed.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3689 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_max_nfev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2686 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    60244 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12648 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_model_saveload.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5157 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_model_uncertainties.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4965 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2181 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_multidatasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)    24062 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_nose.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1168 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)    19779 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21262 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_parameters.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4367 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_params_uvars.py
+-rw-r--r--   0 Newville   (501) staff       (20)    14955 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3999 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_shgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1503 2024-04-19 16:02:36.000000 lmfit-1.3.1/tests/test_stepmodel.py
```

### Comparing `lmfit-1.3.0/.github/CONTRIBUTING.md` & `lmfit-1.3.1/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/.github/ISSUE_TEMPLATE.md` & `lmfit-1.3.1/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `lmfit-1.3.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/.pre-commit-config.yaml` & `lmfit-1.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/AUTHORS.txt` & `lmfit-1.3.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/LICENSE` & `lmfit-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Bennett5.dat` & `lmfit-1.3.1/NIST_STRD/Bennett5.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/BoxBOD.dat` & `lmfit-1.3.1/NIST_STRD/BoxBOD.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Chwirut1.dat` & `lmfit-1.3.1/NIST_STRD/Chwirut1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Chwirut2.dat` & `lmfit-1.3.1/NIST_STRD/Chwirut2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/DanWood.dat` & `lmfit-1.3.1/NIST_STRD/DanWood.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/ENSO.dat` & `lmfit-1.3.1/NIST_STRD/ENSO.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Eckerle4.dat` & `lmfit-1.3.1/NIST_STRD/Eckerle4.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Gauss1.dat` & `lmfit-1.3.1/NIST_STRD/Gauss1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Gauss2.dat` & `lmfit-1.3.1/NIST_STRD/Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Gauss3.dat` & `lmfit-1.3.1/NIST_STRD/Gauss3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Hahn1.dat` & `lmfit-1.3.1/NIST_STRD/Hahn1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Kirby2.dat` & `lmfit-1.3.1/NIST_STRD/Kirby2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Lanczos1.dat` & `lmfit-1.3.1/NIST_STRD/Lanczos1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Lanczos2.dat` & `lmfit-1.3.1/NIST_STRD/Lanczos2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Lanczos3.dat` & `lmfit-1.3.1/NIST_STRD/Lanczos3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/MGH09.dat` & `lmfit-1.3.1/NIST_STRD/MGH09.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/MGH10.dat` & `lmfit-1.3.1/NIST_STRD/MGH10.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/MGH17.dat` & `lmfit-1.3.1/NIST_STRD/MGH17.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Misra1a.dat` & `lmfit-1.3.1/NIST_STRD/Misra1a.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Misra1b.dat` & `lmfit-1.3.1/NIST_STRD/Misra1b.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Misra1c.dat` & `lmfit-1.3.1/NIST_STRD/Misra1c.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Misra1d.dat` & `lmfit-1.3.1/NIST_STRD/Misra1d.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Models` & `lmfit-1.3.1/NIST_STRD/Models`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Nelson.dat` & `lmfit-1.3.1/NIST_STRD/Nelson.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Rat42.dat` & `lmfit-1.3.1/NIST_STRD/Rat42.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Rat43.dat` & `lmfit-1.3.1/NIST_STRD/Rat43.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Roszman1.dat` & `lmfit-1.3.1/NIST_STRD/Roszman1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/NIST_STRD/Thurber.dat` & `lmfit-1.3.1/NIST_STRD/Thurber.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/PKG-INFO` & `lmfit-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.3.0
+Version: 1.3.1
 Summary: Least-Squares Minimization with Bounds and Constraints
 Author-email: LMFit Development Team <matt.newville@gmail.com>
 License: BSD-3
         
         Copyright 2022 Matthew Newville, The University of Chicago
                        Renee Otten, Brandeis University
                        Till Stensitzki, Freie Universitat Berlin
@@ -114,14 +114,15 @@
 Requires-Dist: corner; extra == "doc"
 Requires-Dist: emcee>=3.0.0; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: jupyter_sphinx>=0.2.4; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: numdifftools; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
+Requires-Dist: numexpr; extra == "doc"
 Requires-Dist: Pillow; extra == "doc"
 Requires-Dist: pycairo; platform_system == "Windows" and extra == "doc"
 Requires-Dist: Sphinx; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.10; extra == "doc"
 Requires-Dist: sphinxcontrib-svg2pdfconverter; extra == "doc"
 Requires-Dist: sympy; extra == "doc"
 Provides-Extra: test
```

### Comparing `lmfit-1.3.0/README.rst` & `lmfit-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/asv_benchmarking/asv.conf.json` & `lmfit-1.3.1/asv_benchmarking/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/asv_benchmarking/benchmarks/benchmarks.py` & `lmfit-1.3.1/asv_benchmarking/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/azure-pipelines.yml` & `lmfit-1.3.1/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/Makefile` & `lmfit-1.3.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/_templates/indexsidebar.html` & `lmfit-1.3.1/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/bounds.rst` & `lmfit-1.3.1/doc/bounds.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/builtin_models.rst` & `lmfit-1.3.1/doc/builtin_models.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/conf.py` & `lmfit-1.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/confidence.rst` & `lmfit-1.3.1/doc/confidence.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/constraints.rst` & `lmfit-1.3.1/doc/constraints.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/doc_examples_to_gallery.py` & `lmfit-1.3.1/doc/doc_examples_to_gallery.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/faq.rst` & `lmfit-1.3.1/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/filter_spurious_link_from_html.py` & `lmfit-1.3.1/doc/filter_spurious_link_from_html.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/fitting.rst` & `lmfit-1.3.1/doc/fitting.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/index.rst` & `lmfit-1.3.1/doc/index.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/installation.rst` & `lmfit-1.3.1/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/intro.rst` & `lmfit-1.3.1/doc/intro.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/make.bat` & `lmfit-1.3.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/model.rst` & `lmfit-1.3.1/doc/model.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/parameters.rst` & `lmfit-1.3.1/doc/parameters.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/sphinx/theme/sphinx13/basic_layout.html` & `lmfit-1.3.1/doc/sphinx/theme/sphinx13/basic_layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/sphinx/theme/sphinx13/layout.html` & `lmfit-1.3.1/doc/sphinx/theme/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png` & `lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/lmfitheader.png`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/sphinx/theme/sphinx13/static/sphinx13.css` & `lmfit-1.3.1/doc/sphinx/theme/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/support.rst` & `lmfit-1.3.1/doc/support.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/doc/whatsnew.rst` & `lmfit-1.3.1/doc/whatsnew.rst`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,38 @@
 .. _lmfit GitHub repository: https://github.com/lmfit/lmfit-py
 
 This section discusses changes between versions, especially changes
 significant to the use and behavior of the library. This is not meant
 to be a comprehensive list of changes. For such a complete record,
 consult the `lmfit GitHub repository`_.
 
+.. _whatsnew_131_label:
+
+Version 1.3.1 Release Notes (April 19, 2024)
+====================================================
+
+Mostly fixes for bugs introduced in 1.3.0
+
+- allow ``Model.eval_uncertainty`` to be performed with single points for ``x``
+  independent variables (PR #952, Issue #951)
+
+-  allow ``Model._parse_param`` to handle older-style passed-in 'argnames' and
+   'kwargs' as for variadic function, add test  (PR #950)
+
+- better allow (or re-allow) Model function independent variables / keyword
+  argumentss to be given non-default values at model creation time
+
+- add ``form`` as independent variable for builtin Step, Rectangle, Thermal
+  Distribution models.
+
+- use a copy of ``sys.modules`` when iterating over it. (#949)
+
+-  use ``Model._reprstring(long=True)`` for model ``Model.__repr__()``.
+
+
 .. _whatsnew_130_label:
 
 Version 1.3.0 Release Notes (April 4, 2024)
 ===========================================
 
 New features:
```

### Comparing `lmfit-1.3.0/examples/NIST_Gauss2.dat` & `lmfit-1.3.1/examples/NIST_Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/discuss_model_eval_uncertainty.ipynb` & `lmfit-1.3.1/examples/discuss_model_eval_uncertainty.ipynb`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_builtinmodels_nistgauss.py` & `lmfit-1.3.1/examples/doc_builtinmodels_nistgauss.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_builtinmodels_nistgauss2.py` & `lmfit-1.3.1/examples/doc_builtinmodels_nistgauss2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_builtinmodels_peakmodels.py` & `lmfit-1.3.1/examples/doc_builtinmodels_peakmodels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_builtinmodels_splinemodel.py` & `lmfit-1.3.1/examples/doc_builtinmodels_splinemodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_builtinmodels_stepmodel.py` & `lmfit-1.3.1/examples/doc_builtinmodels_stepmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_confidence_advanced.py` & `lmfit-1.3.1/examples/doc_confidence_advanced.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_confidence_chi2_maps.py` & `lmfit-1.3.1/examples/doc_confidence_chi2_maps.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_fitting_emcee.py` & `lmfit-1.3.1/examples/doc_fitting_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_fitting_withreport.py` & `lmfit-1.3.1/examples/doc_fitting_withreport.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_composite.py` & `lmfit-1.3.1/examples/doc_model_composite.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_gaussian.py` & `lmfit-1.3.1/examples/doc_model_gaussian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_loadmodel.py` & `lmfit-1.3.1/examples/doc_model_loadmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_loadmodelresult.py` & `lmfit-1.3.1/examples/doc_model_loadmodelresult.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_loadmodelresult2.py` & `lmfit-1.3.1/examples/doc_model_loadmodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_savemodelresult2.py` & `lmfit-1.3.1/examples/doc_model_savemodelresult2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_two_components.py` & `lmfit-1.3.1/examples/doc_model_two_components.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_uncertainty.py` & `lmfit-1.3.1/examples/doc_model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_uncertainty2.py` & `lmfit-1.3.1/examples/doc_model_uncertainty2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_uncertainty_pred.py` & `lmfit-1.3.1/examples/doc_model_uncertainty_pred.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_with_iter_callback.py` & `lmfit-1.3.1/examples/doc_model_with_iter_callback.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_model_with_nan_policy.py` & `lmfit-1.3.1/examples/doc_model_with_nan_policy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_parameters_basic.py` & `lmfit-1.3.1/examples/doc_parameters_basic.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_parameters_valuesdict.py` & `lmfit-1.3.1/examples/doc_parameters_valuesdict.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/doc_uvars_params.py` & `lmfit-1.3.1/examples/doc_uvars_params.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_Model_interface.py` & `lmfit-1.3.1/examples/example_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_basinhopping.py` & `lmfit-1.3.1/examples/example_basinhopping.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_brute.py` & `lmfit-1.3.1/examples/example_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_complex_resonator_model.py` & `lmfit-1.3.1/examples/example_complex_resonator_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_confidence_interval.py` & `lmfit-1.3.1/examples/example_confidence_interval.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_detect_outliers.py` & `lmfit-1.3.1/examples/example_detect_outliers.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_diffev.py` & `lmfit-1.3.1/examples/example_diffev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_emcee_Model_interface.py` & `lmfit-1.3.1/examples/example_emcee_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_expression_model.py` & `lmfit-1.3.1/examples/example_expression_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_fit_multi_datasets.py` & `lmfit-1.3.1/examples/example_fit_multi_datasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_fit_with_algebraic_constraint.py` & `lmfit-1.3.1/examples/example_fit_with_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_fit_with_bounds.py` & `lmfit-1.3.1/examples/example_fit_with_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_fit_with_derivfunc.py` & `lmfit-1.3.1/examples/example_fit_with_derivfunc.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_fit_with_inequality.py` & `lmfit-1.3.1/examples/example_fit_with_inequality.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_reduce_fcn.py` & `lmfit-1.3.1/examples/example_reduce_fcn.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_sympy.py` & `lmfit-1.3.1/examples/example_sympy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_two_dimensional_peak.py` & `lmfit-1.3.1/examples/example_two_dimensional_peak.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/example_use_pandas.py` & `lmfit-1.3.1/examples/example_use_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/lmfit_emcee_model_selection.py` & `lmfit-1.3.1/examples/lmfit_emcee_model_selection.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/model1d_gauss.dat` & `lmfit-1.3.1/examples/model1d_gauss.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/peak.csv` & `lmfit-1.3.1/examples/peak.csv`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/sinedata.dat` & `lmfit-1.3.1/examples/sinedata.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/test_peak.dat` & `lmfit-1.3.1/examples/test_peak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/examples/test_splinepeak.dat` & `lmfit-1.3.1/examples/test_splinepeak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/__init__.py` & `lmfit-1.3.1/lmfit/__init__.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/_ampgo.py` & `lmfit-1.3.1/lmfit/_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/conf_emcee.py` & `lmfit-1.3.1/lmfit/conf_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/confidence.py` & `lmfit-1.3.1/lmfit/confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/jsonutils.py` & `lmfit-1.3.1/lmfit/jsonutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 pyvers = f'{sys.version_info.major}.{sys.version_info.minor}'
 
 
 def find_importer(obj):
     """Find importer of an object."""
     oname = obj.__name__
-    for modname, module in sys.modules.items():
+    for modname, module in sys.modules.copy().items():
         if modname.startswith('__main__'):
             continue
         t = getattr(module, oname, None)
         if t is obj:
             return modname
     return None
```

### Comparing `lmfit-1.3.0/lmfit/lineshapes.py` & `lmfit-1.3.1/lmfit/lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/minimizer.py` & `lmfit-1.3.1/lmfit/minimizer.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/model.py` & `lmfit-1.3.1/lmfit/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         self._parse_params()
         if self.independent_vars is None:
             self.independent_vars = []
         if name is None and hasattr(self.func, '__name__'):
             name = self.func.__name__
         self._name = name
 
-    def _reprstring(self, long=False):
+    def _reprstring(self, long=True):
         out = self._name
         opts = []
         if len(self._prefix) > 0:
             opts.append(f"prefix='{self._prefix}'")
         if long:
             for k, v in self.opts.items():
                 opts.append(f"{k}='{v}'")
@@ -464,15 +464,15 @@
 
         """
         return self.loads(fp.read(), funcdefs=funcdefs, **kws)
 
     @property
     def name(self):
         """Return Model name."""
-        return self._reprstring(long=False)
+        return self._reprstring(long=True)
 
     @name.setter
     def name(self, value):
         self._name = value
 
     @property
     def prefix(self):
@@ -493,40 +493,42 @@
     @property
     def param_names(self):
         """Return the parameter names of the Model."""
         return self._param_names
 
     def __repr__(self):
         """Return representation of Model."""
-        return f"<lmfit.Model: {self.name}>"
+        return self._reprstring(long=True)
 
     def copy(self, **kwargs):
         """DOES NOT WORK."""
         raise NotImplementedError("Model.copy does not work. Make a new Model")
 
     def _parse_params(self):
         """Build parameters from function arguments."""
         if self.func is None:
             return
         kw_args = {}
         keywords_ = None
+        indep_vars = []
+        default_vals = {}
         # need to fetch the following from the function signature:
         #   pos_args: list of positional argument names
         #   kw_args: dict of keyword arguments with default values
         #   keywords_:  name of **kws argument or None
         # 1. limited support for asteval functions as the model functions:
         if hasattr(self.func, 'argnames') and hasattr(self.func, 'kwargs'):
             pos_args = self.func.argnames[:]
+            default_vals = {v: inspect._empty for v in pos_args}
             for name, defval in self.func.kwargs:
                 kw_args[name] = defval
+                default_vals[name] = defval
         # 2. modern, best-practice approach: use inspect.signature
         else:
             pos_args = []
-            default_vals = {}
-            indep_vars = []
             sig = inspect.signature(self.func)
             for fnam, fpar in sig.parameters.items():
                 if fpar.kind == fpar.VAR_KEYWORD:
                     keywords_ = fnam
                 elif fpar.kind in (fpar.POSITIONAL_ONLY, fpar.POSITIONAL_OR_KEYWORD):
                     default_vals[fnam] = fpar.default
                     if (isinstance(fpar.default, (float, int, complex))
@@ -900,14 +902,15 @@
     def make_funcargs(self, params=None, kwargs=None, strip=True):
         """Convert parameter values and keywords to function arguments."""
         if params is None:
             params = {}
         if kwargs is None:
             kwargs = {}
         out = {}
+        out.update(self.opts)
         for key, val in self.independent_vars_defvals.items():
             if val is not inspect._empty:
                 out[key] = val
         # 0: if a keyword argument is going to overwrite a parameter,
         #    save that value so it can be restored before returning
         saved_values = {}
         for name, val in kwargs.items():
@@ -1146,15 +1149,15 @@
                 data = data[mask]
             if weights is not None:
                 weights = _align(weights, mask, data)
 
         # If independent_vars and data are alignable (pandas), align them,
         # and apply the mask from above if there is one.
         for var in self.independent_vars:
-            if var not in params:
+            if var not in params and var not in self.opts:
                 if var not in kwargs:
                     raise ValueError(f"'Missing independent variable '{var}'")
                 if not np.isscalar(kwargs[var]):
                     kwargs[var] = _align(kwargs[var], mask, data)
 
         if coerce_farray:
             # coerce data and independent variable(s) that are 'array-like' (list,
@@ -1267,15 +1270,15 @@
         self._func_allargs = (self.left._func_allargs +
                               self.right._func_allargs)
         self.def_vals = deepcopy(self.right.def_vals)
         self.def_vals.update(self.left.def_vals)
         self.opts = deepcopy(self.right.opts)
         self.opts.update(self.left.opts)
 
-    def _reprstring(self, long=False):
+    def _reprstring(self, long=True):
         return (f"({self.left._reprstring(long=long)} "
                 f"{self._known_ops.get(self.op, self.op)} "
                 f"{self.right._reprstring(long=long)})")
 
     def eval(self, params=None, **kwargs):
         """Evaluate model function for composite model."""
         return self.op(self.left.eval(params=params, **kwargs),
@@ -1682,15 +1685,15 @@
         userkws.update(kwargs)
         if params is None:
             params = self.params
 
         nvarys = self.nvarys
         # ensure fjac and df2 are correct size if independent var updated by kwargs
         feval = self.model.eval(params, **userkws)
-        ndata = len(feval.view('float64'))        # allows feval to be complex
+        ndata = np.atleast_1d(feval).view('float64').ravel().size  # allows feval to be complex
         covar = self.covar
         if any(p.stderr is None for p in params.values()):
             return np.zeros(ndata)
 
         # '0' would be an invalid prefix, here signifying 'Full'
         fjac = {'0': np.zeros((nvarys, ndata), dtype='float64')}
         df2 = {'0': np.zeros(ndata, dtype='float64')}
@@ -1713,16 +1716,16 @@
 
             pars[pname].value = val0 - dval
             res2 = {'0': self.model.eval(pars, **userkws)}
             res2.update(self.model.eval_components(params=pars, **userkws))
 
             pars[pname].value = val0
             for key in fjac:
-                fjac[key][i] = (res1[key].view('float64')
-                                - res2[key].view('float64')) / (2*dval)
+                fjac[key][i] = (np.atleast_1d(res1[key]).view('float64').ravel()
+                                - np.atleast_1d(res2[key]).view('float64').ravel()) / (2*dval)
 
         for i in range(nvarys):
             for j in range(nvarys):
                 for key in fjac:
                     df2[key] += fjac[key][i] * fjac[key][j] * covar[i, j]
 
         if sigma < 1.0:
@@ -1731,15 +1734,18 @@
             prob = erf(sigma/np.sqrt(2))
 
         scale = t.ppf((prob+1)/2.0, self.ndata-nvarys)
 
         # for complex data, convert back to real/imag pairs
         if feval.dtype in ('complex64', 'complex128'):
             for key in fjac:
-                df2[key] = df2[key][0::2] + 1j * df2[key][1::2]
+                df2[key] = df2[key].view(feval.dtype)
+
+        for key in fjac:
+            df2[key] = df2[key].reshape(feval.shape)
 
         df2_total = df2.pop('0')
         self.dely = scale * np.sqrt(df2_total)
         self.dely_predicted = scale * np.sqrt(df2_total + self.redchi)
 
         self.dely_comps = {}
         for key in df2:
```

### Comparing `lmfit-1.3.0/lmfit/models.py` & `lmfit-1.3.1/lmfit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1379,16 +1379,16 @@
     For more information, see:
     http://hyperphysics.phy-astr.gsu.edu/hbase/quantum/disfcn.html
 
     """
 
     valid_forms = ('bose', 'maxwell', 'fermi')
 
-    def __init__(self, independent_vars=['x'], prefix='', nan_policy='raise',
-                 form='bose', **kwargs):
+    def __init__(self, independent_vars=['x', 'form'], prefix='',
+                 nan_policy='raise', form='bose', **kwargs):
         kwargs.update({'prefix': prefix, 'nan_policy': nan_policy,
                        'form': form, 'independent_vars': independent_vars})
         super().__init__(thermal_distribution, **kwargs)
         self._set_paramhints_prefix()
 
     def guess(self, data, x, negative=False, **kwargs):
         """Estimate initial model parameter values from data."""
@@ -1540,16 +1540,16 @@
 
     where :math:`\alpha = (x - \mu)/{\sigma}`.
 
     """
 
     valid_forms = ('linear', 'atan', 'arctan', 'erf', 'logistic')
 
-    def __init__(self, independent_vars=['x'], prefix='', nan_policy='raise',
-                 form='linear', **kwargs):
+    def __init__(self, independent_vars=['x', 'form'], prefix='',
+                 nan_policy='raise', form='linear', **kwargs):
         kwargs.update({'prefix': prefix, 'nan_policy': nan_policy,
                        'form': form, 'independent_vars': independent_vars})
         super().__init__(step, **kwargs)
 
     def guess(self, data, x, **kwargs):
         """Estimate initial model parameter values from data."""
         ymin, ymax = min(data), max(data)
@@ -1600,16 +1600,16 @@
     where :math:`\alpha_1 = (x - \mu_1)/{\sigma_1}` and
     :math:`\alpha_2 = -(x - \mu_2)/{\sigma_2}`.
 
     """
 
     valid_forms = ('linear', 'atan', 'arctan', 'erf', 'logistic')
 
-    def __init__(self, independent_vars=['x'], prefix='', nan_policy='raise',
-                 form='linear', **kwargs):
+    def __init__(self, independent_vars=['x', 'form'], prefix='',
+                 nan_policy='raise', form='linear', **kwargs):
         kwargs.update({'prefix': prefix, 'nan_policy': nan_policy,
                        'form': form, 'independent_vars': independent_vars})
         super().__init__(rectangle, **kwargs)
 
         self._set_paramhints_prefix()
 
     def _set_paramhints_prefix(self):
```

### Comparing `lmfit-1.3.0/lmfit/parameter.py` & `lmfit-1.3.1/lmfit/parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit/printfuncs.py` & `lmfit-1.3.1/lmfit/printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/lmfit.egg-info/PKG-INFO` & `lmfit-1.3.1/lmfit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.3.0
+Version: 1.3.1
 Summary: Least-Squares Minimization with Bounds and Constraints
 Author-email: LMFit Development Team <matt.newville@gmail.com>
 License: BSD-3
         
         Copyright 2022 Matthew Newville, The University of Chicago
                        Renee Otten, Brandeis University
                        Till Stensitzki, Freie Universitat Berlin
@@ -114,14 +114,15 @@
 Requires-Dist: corner; extra == "doc"
 Requires-Dist: emcee>=3.0.0; extra == "doc"
 Requires-Dist: ipykernel; extra == "doc"
 Requires-Dist: jupyter_sphinx>=0.2.4; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: numdifftools; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
+Requires-Dist: numexpr; extra == "doc"
 Requires-Dist: Pillow; extra == "doc"
 Requires-Dist: pycairo; platform_system == "Windows" and extra == "doc"
 Requires-Dist: Sphinx; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.10; extra == "doc"
 Requires-Dist: sphinxcontrib-svg2pdfconverter; extra == "doc"
 Requires-Dist: sympy; extra == "doc"
 Provides-Extra: test
```

### Comparing `lmfit-1.3.0/lmfit.egg-info/SOURCES.txt` & `lmfit-1.3.1/lmfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/publish_docs.sh` & `lmfit-1.3.1/publish_docs.sh`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/pyproject.toml` & `lmfit-1.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "corner",
     "emcee>=3.0.0",
     "ipykernel",
     "jupyter_sphinx>=0.2.4",
     "matplotlib",
     "numdifftools",
     "pandas",
+    "numexpr", # note: Pandas appears to need numexpr to build our docs
     "Pillow",
     "pycairo;platform_system=='Windows'",
     "Sphinx",
     "sphinx-gallery>=0.10",
     "sphinxcontrib-svg2pdfconverter",
     "sympy",
 ]
```

### Comparing `lmfit-1.3.0/tests/NISTModels.py` & `lmfit-1.3.1/tests/NISTModels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/conftest.py` & `lmfit-1.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/gauss_modelresult_lmfit100.sav` & `lmfit-1.3.1/tests/gauss_modelresult_lmfit100.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/saved_models/sinemodel_py310_lm122.sav` & `lmfit-1.3.1/tests/saved_models/sinemodel_py310_lm122.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/saved_models/sinemodel_py311_lm122.sav` & `lmfit-1.3.1/tests/saved_models/sinemodel_py311_lm122.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/saved_models/sinemodel_py312_lm122.sav` & `lmfit-1.3.1/tests/saved_models/sinemodel_py312_lm122.sav`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_1variable.py` & `lmfit-1.3.1/tests/test_1variable.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_NIST_Strd.py` & `lmfit-1.3.1/tests/test_NIST_Strd.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_algebraic_constraint.py` & `lmfit-1.3.1/tests/test_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_ampgo.py` & `lmfit-1.3.1/tests/test_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_basicfit.py` & `lmfit-1.3.1/tests/test_basicfit.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_basinhopping.py` & `lmfit-1.3.1/tests/test_basinhopping.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_bounded_jacobian.py` & `lmfit-1.3.1/tests/test_bounded_jacobian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_bounds.py` & `lmfit-1.3.1/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_brute.py` & `lmfit-1.3.1/tests/test_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_builtin_models.py` & `lmfit-1.3.1/tests/test_builtin_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_confidence.py` & `lmfit-1.3.1/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_covariance_matrix.py` & `lmfit-1.3.1/tests/test_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_custom_independentvar.py` & `lmfit-1.3.1/tests/test_custom_independentvar.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_default_kws.py` & `lmfit-1.3.1/tests/test_default_kws.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_dual_annealing.py` & `lmfit-1.3.1/tests/test_dual_annealing.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_itercb.py` & `lmfit-1.3.1/tests/test_itercb.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_jsonutils.py` & `lmfit-1.3.1/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_least_squares.py` & `lmfit-1.3.1/tests/test_least_squares.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_lineshapes.py` & `lmfit-1.3.1/tests/test_lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_manypeaks_speed.py` & `lmfit-1.3.1/tests/test_manypeaks_speed.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_max_nfev.py` & `lmfit-1.3.1/tests/test_max_nfev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_minimizer.py` & `lmfit-1.3.1/tests/test_minimizer.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_model.py` & `lmfit-1.3.1/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,15 +277,15 @@
 def test_Model_getter_param_names(gmodel):
     """Test for Model class getter function for param_names."""
     assert gmodel.param_names == ['amplitude', 'center', 'sigma']
 
 
 def test_Model__repr__(gmodel):
     """Test for Model class __repr__ method."""
-    assert gmodel.__repr__() == '<lmfit.Model: Model(gaussian)>'
+    assert 'Model(gaussian)' in gmodel.__repr__()
 
 
 def test_Model_copy(gmodel):
     """Test for Model class copy method."""
     msg = 'Model.copy does not work. Make a new Model'
     with pytest.raises(NotImplementedError, match=msg):
         gmodel.copy()
@@ -880,18 +880,31 @@
     def test_independent_var_parsing(self):
         """test the parsing of independent variables for model functions
         with keyword arguments
 
         step:  form='linear'
         voigt: gamma=None,     can become a variable!!
         """
-        stepmod = Model(step)
-        assert 'x' in stepmod.independent_vars
-        assert 'form' in stepmod.independent_vars
-        assert 'linear' == stepmod.independent_vars_defvals.get('form', None)
+        stepmod1 = Model(step)
+        assert 'x' in stepmod1.independent_vars
+        assert 'form' in stepmod1.independent_vars
+        assert 'linear' == stepmod1.independent_vars_defvals.get('form', None)
+
+        stepmod2 = Model(step, form='arctan')
+        assert 'x' in stepmod2.independent_vars
+        assert 'form' in stepmod2.independent_vars
+        assert 'arctan' == stepmod2.independent_vars_defvals.get('form', None)
+
+        x = np.linspace(0, 30, 301)
+        pars = stepmod1.make_params(amplitude=10, center=14, sigma=2.5)
+        yline = stepmod1.eval(pars, x=x)
+        yatan = stepmod2.eval(pars, x=x)
+
+        assert (yatan-yline).std() > 0.1
+        assert (yatan-yline).ptp() > 1.0
 
         voigtmod = Model(voigt)
         assert 'x' in voigtmod.independent_vars
         assert 'gamma' in voigtmod.independent_vars
         assert voigtmod.independent_vars_defvals['gamma'] is None
 
         pars1 = voigtmod.make_params(amplitude=25, center=9.5, sigma=1)
@@ -1588,7 +1601,50 @@
 
     mod = Model(func)
     params = mod.make_params()
     result = mod.fit(y, params, x=x, weights=1.0/yerr)
 
     assert result.rsquared < 1.00
     assert result.rsquared > 0.95
+
+
+# based on Github #953
+class PolynomialFunction:
+    def __init__(self, degree=1):
+        self.degree = degree
+
+    @property
+    def __name__(self):
+        return self.__class__.__name__
+
+    @property
+    def argnames(self):
+        return ["x"] + [f"c{i}" for i in range(self.degree + 1)]
+
+    @property
+    def kwargs(self):
+        return {}
+
+    def __call__(self, x, *coeffs, **params):
+        if len(coeffs) != self.degree + 1:
+            coeffs = [params[f"c{d}"] for d in range(self.degree + 1)]
+        return np.polynomial.polynomial.polyval(x, coeffs)
+
+
+def test_custom_variadic_model():
+    """Github #953"""
+    model = Model(PolynomialFunction(degree=3))
+    params = model.make_params(c0=5, c1=3.6, c2=-0.2, c3=0)
+
+    assert 'x' in model.independent_vars
+
+    np.random.seed(0)
+    x1 = np.linspace(-10, 10, 201)
+    y1 = 5 + 3.3*x1 + 0.17*x1**2 - 0.004*x1**3
+    y1 += np.random.normal(size=201, scale=0.1)
+
+    result = model.fit(y1, params, x=x1)
+
+    assert result.chisqr < 15.0
+    assert result.nfev > 7
+    assert_allclose(result.values['c0'], 5.0, 0.02, 0.02, '', True)
+    assert_allclose(result.values['c1'], 3.3, 0.02, 0.02, '', True)
```

### Comparing `lmfit-1.3.0/tests/test_model_saveload.py` & `lmfit-1.3.1/tests/test_model_saveload.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_model_uncertainties.py` & `lmfit-1.3.1/tests/test_model_uncertainties.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests of ModelResult.eval_uncertainty()"""
 import os
 
 import numpy as np
 from numpy.testing import assert_allclose
 
 from lmfit.lineshapes import gaussian
+from lmfit.model import Model
 from lmfit.models import ExponentialModel, GaussianModel, LinearModel
 
 
 def get_linearmodel(slope=0.8, intercept=0.5, noise=1.5):
     # create data to be fitted
     np.random.seed(88)
     x = np.linspace(0, 10, 101)
@@ -123,7 +124,27 @@
     assert dely.mean() < 2.0
     assert result.dely_comps['g1_'].mean() > 0.5
     assert result.dely_comps['g1_'].mean() < 1.5
     assert result.dely_comps['g2_'].mean() > 0.5
     assert result.dely_comps['g2_'].mean() < 1.5
     assert result.dely_comps['bkg_'].mean() > 0.5
     assert result.dely_comps['bkg_'].mean() < 1.5
+
+
+def test_scalar_independent_vars():
+    """Github #951"""
+    mr = LinearModel().fit(data=[1, 2, 4], x=[1, 2, 3])
+
+    assert_allclose(mr.eval_uncertainty(x=1.2), np.array([0.60629034]))
+    assert_allclose(mr.eval_uncertainty(x=np.array(1.2j)), np.array([1.15903153+0.17475665j]))
+
+
+def test_multidim_model():
+    """test models that return a multi-dimension output"""
+    def fit(x, p=2):
+        return np.array([x, p*x])
+    model = Model(fit)
+
+    mr = model.fit(data=np.array([[1, 2, 3], [2, 3, 5]]), x=np.array([1, 2, 3]))
+
+    assert_allclose(mr.eval_uncertainty(x=np.array([3, 4])), np.array([[0, 0], [0.18432744, 0.24576991]]))
+    assert_allclose(mr.eval_uncertainty(x=np.array([3j, 4j])), np.array([[0, 0], [0.13033918+0.13033918j, 0.17378557+0.17378557j]]))
```

### Comparing `lmfit-1.3.0/tests/test_models.py` & `lmfit-1.3.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_multidatasets.py` & `lmfit-1.3.1/tests/test_multidatasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_nose.py` & `lmfit-1.3.1/tests/test_nose.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_pandas.py` & `lmfit-1.3.1/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_parameter.py` & `lmfit-1.3.1/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_parameters.py` & `lmfit-1.3.1/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_params_uvars.py` & `lmfit-1.3.1/tests/test_params_uvars.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_printfuncs.py` & `lmfit-1.3.1/tests/test_printfuncs.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_shgo.py` & `lmfit-1.3.1/tests/test_shgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.3.0/tests/test_stepmodel.py` & `lmfit-1.3.1/tests/test_stepmodel.py`

 * *Files identical despite different names*

