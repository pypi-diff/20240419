# Comparing `tmp/plothist-1.2.2.tar.gz` & `tmp/plothist-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plothist-1.2.2.tar", last modified: Fri Apr 19 07:12:32 2024, max compression
+gzip compressed data, was "plothist-1.2.3.tar", last modified: Fri Apr 19 07:13:07 2024, max compression
```

## Comparing `plothist-1.2.2.tar` & `plothist-1.2.3.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0      363 2024-04-19 00:12:45.212523 plothist-1.2.2/.github/ISSUE_TEMPLATE/user-story.md
--rw-r--r--   0        0        0     1031 2024-04-18 00:01:09.624927 plothist-1.2.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      217 2024-04-18 00:01:09.624927 plothist-1.2.2/.gitignore
--rw-r--r--   0        0        0      853 2024-02-27 12:31:06.447939 plothist-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      367 2024-02-27 12:31:06.447939 plothist-1.2.2/.readthedocs.yaml
--rw-r--r--   0        0        0      111 2024-01-24 11:19:08.106954 plothist-1.2.2/AUTHORS.md
--rw-r--r--   0        0        0     1523 2024-02-01 10:13:39.803203 plothist-1.2.2/LICENSE
--rw-r--r--   0        0        0     2495 2024-04-19 07:12:22.709929 plothist-1.2.2/README.rst
--rw-r--r--   0        0        0    10493 2024-03-27 04:27:38.576554 plothist-1.2.2/docs/advanced/model_examples.rst
--rw-r--r--   0        0        0     1970 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/advanced/other_advanced.rst
--rw-r--r--   0        0        0    10309 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/basics/1d_hist.rst
--rw-r--r--   0        0        0     2838 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/basics/2d_hist.rst
--rw-r--r--   0        0        0     8175 2024-04-18 00:01:09.624927 plothist-1.2.2/docs/basics/variable_registry.rst
--rw-r--r--   0        0        0     6958 2024-04-19 07:12:22.709929 plothist-1.2.2/docs/conf.py
--rw-r--r--   0        0        0      585 2024-04-18 00:01:09.624927 plothist-1.2.2/docs/documentation/documentation.rst
--rw-r--r--   0        0        0      834 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/documentation/statistics.rst
--rw-r--r--   0        0        0      786 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_asymmetry.py
--rw-r--r--   0        0        0      914 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_difference.py
--rw-r--r--   0        0        0      865 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_efficiency.py
--rw-r--r--   0        0        0      831 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_only_efficiency.py
--rw-r--r--   0        0        0      719 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_pull.py
--rw-r--r--   0        0        0      724 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_ratio.py
--rw-r--r--   0        0        0      823 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_relative_difference.py
--rw-r--r--   0        0        0      803 2024-02-28 09:38:28.691495 plothist-1.2.2/docs/examples/1d_hist/1d_comparison_split_ratio.py
--rw-r--r--   0        0        0      795 2024-01-25 11:39:29.527978 plothist-1.2.2/docs/examples/1d_hist/1d_elt1.py
--rw-r--r--   0        0        0      810 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/1d_hist/1d_elt1_stacked.py
--rw-r--r--   0        0        0      558 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_elt2.py
--rw-r--r--   0        0        0      455 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/1d_hist/1d_fct.py
--rw-r--r--   0        0        0      687 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/1d_hist/1d_fct_stacked.py
--rw-r--r--   0        0        0      418 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/1d_hist/1d_hist_simple.py
--rw-r--r--   0        0        0      883 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_int_category.py
--rw-r--r--   0        0        0      661 2024-03-15 05:56:03.521542 plothist-1.2.2/docs/examples/1d_hist/1d_profile.py
--rw-r--r--   0        0        0      882 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/examples/1d_hist/1d_str_category.py
--rw-r--r--   0        0        0       96 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/1d_hist/README.rst
--rw-r--r--   0        0        0     1495 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/2d_hist/2d_hist_correlations.py
--rw-r--r--   0        0        0      534 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/2d_hist/2d_hist_simple.py
--rw-r--r--   0        0        0     1040 2024-01-24 11:19:08.106954 plothist-1.2.2/docs/examples/2d_hist/2d_hist_simple_discrete_colormap.py
--rw-r--r--   0        0        0      650 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/2d_hist/2d_hist_uneven.py
--rw-r--r--   0        0        0      744 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/2d_hist/2d_hist_with_projections.py
--rw-r--r--   0        0        0      116 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/2d_hist/README.rst
--rw-r--r--   0        0        0      147 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/README.rst
--rw-r--r--   0        0        0     2702 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/advanced/1d_comparison_advanced.py
--rw-r--r--   0        0        0      112 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/advanced/README.rst
--rw-r--r--   0        0        0     2598 2024-04-18 00:01:09.624927 plothist-1.2.2/docs/examples/advanced/asymmetry_comparison_advanced.py
--rw-r--r--   0        0        0     3066 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/advanced/model_examples_flatten2D.py
--rw-r--r--   0        0        0      103 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/model_ex/README.rst
--rw-r--r--   0        0        0     2816 2024-02-28 09:38:28.691495 plothist-1.2.2/docs/examples/model_ex/model_all_comparisons.py
--rw-r--r--   0        0        0     3423 2024-02-28 09:38:28.691495 plothist-1.2.2/docs/examples/model_ex/model_all_comparisons_no_model_unc.py
--rw-r--r--   0        0        0     1654 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_examples_pull.py
--rw-r--r--   0        0        0     1879 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_examples_pull_no_model_unc.py
--rw-r--r--   0        0        0     1943 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_examples_stacked.py
--rw-r--r--   0        0        0     1947 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_examples_stacked_unstacked.py
--rw-r--r--   0        0        0     1744 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_examples_unstacked.py
--rw-r--r--   0        0        0     1355 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_with_stacked_and_unstacked_function_components.py
--rw-r--r--   0        0        0     1991 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/model_with_stacked_and_unstacked_histograms_components.py
--rw-r--r--   0        0        0     1413 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/model_ex/ratio_data_vs_model_with_stacked_and_unstacked_function_components.py
--rw-r--r--   0        0        0       77 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/utility/README.rst
--rw-r--r--   0        0        0     2359 2023-12-11 08:11:42.957778 plothist-1.2.2/docs/examples/utility/color_palette_hists.py
--rw-r--r--   0        0        0     2729 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/utility/color_palette_squares.py
--rw-r--r--   0        0        0     1820 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/examples/utility/matplotlib_vs_plothist_style.py
--rw-r--r--   0        0        0   115640 2024-03-26 03:06:19.637708 plothist-1.2.2/docs/img/1d_comparison_advanced.svg
--rw-r--r--   0        0        0    53814 2024-03-27 05:59:25.694889 plothist-1.2.2/docs/img/1d_comparison_asymmetry.svg
--rw-r--r--   0        0        0    67200 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_difference.svg
--rw-r--r--   0        0        0    70322 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_efficiency.svg
--rw-r--r--   0        0        0    45998 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_only_efficiency.svg
--rw-r--r--   0        0        0    47754 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_pull.svg
--rw-r--r--   0        0        0    50549 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_ratio.svg
--rw-r--r--   0        0        0    53545 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_relative_difference.svg
--rw-r--r--   0        0        0    62167 2024-03-27 05:59:25.698889 plothist-1.2.2/docs/img/1d_comparison_split_ratio.svg
--rw-r--r--   0        0        0    31035 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_elt1.svg
--rw-r--r--   0        0        0    40167 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_elt1_stacked.svg
--rw-r--r--   0        0        0    37991 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_elt2.svg
--rw-r--r--   0        0        0    25927 2024-03-26 03:06:51.502231 plothist-1.2.2/docs/img/1d_fct.svg
--rw-r--r--   0        0        0   118828 2024-03-26 03:06:59.702372 plothist-1.2.2/docs/img/1d_fct_stacked.svg
--rw-r--r--   0        0        0    41618 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_hist_simple.svg
--rw-r--r--   0        0        0    22944 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_int_category.svg
--rw-r--r--   0        0        0    28474 2024-03-26 03:07:10.026554 plothist-1.2.2/docs/img/1d_profile.svg
--rw-r--r--   0        0        0    23667 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/1d_str_category.svg
--rw-r--r--   0        0        0   551253 2024-03-26 03:06:49.342194 plothist-1.2.2/docs/img/2d_hist_correlations_0.svg
--rw-r--r--   0        0        0   521575 2024-03-26 03:06:49.786202 plothist-1.2.2/docs/img/2d_hist_correlations_1.svg
--rw-r--r--   0        0        0   518776 2024-03-26 03:06:50.290211 plothist-1.2.2/docs/img/2d_hist_correlations_2.svg
--rw-r--r--   0        0        0    60974 2024-03-26 03:06:47.578164 plothist-1.2.2/docs/img/2d_hist_simple.svg
--rw-r--r--   0        0        0   555885 2024-03-27 05:59:25.702889 plothist-1.2.2/docs/img/2d_hist_simple_discrete_colormap.svg
--rw-r--r--   0        0        0    48903 2024-03-26 03:06:42.858085 plothist-1.2.2/docs/img/2d_hist_uneven.svg
--rw-r--r--   0        0        0   578843 2024-03-27 05:59:25.706888 plothist-1.2.2/docs/img/2d_hist_with_projections.svg
--rw-r--r--   0        0        0   107898 2024-03-26 03:06:20.817726 plothist-1.2.2/docs/img/asymmetry_comparison_advanced.svg
--rw-r--r--   0        0        0    35065 2024-03-26 03:06:25.469801 plothist-1.2.2/docs/img/matplotlib_example.svg
--rw-r--r--   0        0        0   210630 2024-03-26 03:06:39.762034 plothist-1.2.2/docs/img/model_all_comparisons.svg
--rw-r--r--   0        0        0   198568 2024-03-26 03:06:30.609883 plothist-1.2.2/docs/img/model_all_comparisons_no_model_unc.svg
--rw-r--r--   0        0        0    65977 2024-03-26 03:06:21.989745 plothist-1.2.2/docs/img/model_examples_flatten2D.svg
--rw-r--r--   0        0        0    94412 2024-03-26 03:06:36.137974 plothist-1.2.2/docs/img/model_examples_pull.svg
--rw-r--r--   0        0        0    93502 2024-03-26 03:06:33.537931 plothist-1.2.2/docs/img/model_examples_pull_no_model_unc.svg
--rw-r--r--   0        0        0   122943 2024-03-26 03:06:41.382060 plothist-1.2.2/docs/img/model_examples_stacked.svg
--rw-r--r--   0        0        0   103269 2024-03-26 03:06:28.561850 plothist-1.2.2/docs/img/model_examples_stacked_unstacked.svg
--rw-r--r--   0        0        0   102567 2024-03-26 03:06:27.177828 plothist-1.2.2/docs/img/model_examples_unstacked.svg
--rw-r--r--   0        0        0   141571 2024-03-26 03:06:37.177991 plothist-1.2.2/docs/img/model_with_stacked_and_unstacked_function_components.svg
--rw-r--r--   0        0        0    72038 2024-03-26 03:06:34.729951 plothist-1.2.2/docs/img/model_with_stacked_and_unstacked_histograms_components.svg
--rw-r--r--   0        0        0    49322 2024-03-26 03:06:25.773805 plothist-1.2.2/docs/img/plothist_example.svg
--rw-r--r--   0        0        0    42928 2024-02-20 15:43:53.653134 plothist-1.2.2/docs/img/pyhf_example.svg
--rw-r--r--   0        0        0   170416 2024-03-26 03:06:31.881904 plothist-1.2.2/docs/img/ratio_data_vs_model_with_stacked_and_unstacked_function_components.svg
--rw-r--r--   0        0        0   436516 2023-12-11 08:11:42.973778 plothist-1.2.2/docs/img/savefig_comparisons.gif
--rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.373783 plothist-1.2.2/docs/img/usage_YlGnBu_r_palette.svg
--rw-r--r--   0        0        0   270554 2024-03-26 03:06:23.429768 plothist-1.2.2/docs/img/usage_colorpalette_examples.svg
--rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.317782 plothist-1.2.2/docs/img/usage_coolwarm_palette.svg
--rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.213780 plothist-1.2.2/docs/img/usage_cubehelix.svg
--rw-r--r--   0        0        0    16297 2024-03-26 03:06:24.133779 plothist-1.2.2/docs/img/usage_style_cycle.svg
--rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.269781 plothist-1.2.2/docs/img/usage_viridis_palette.svg
--rw-r--r--   0        0        0      646 2024-02-27 12:31:06.447939 plothist-1.2.2/docs/index.rst
--rw-r--r--   0        0        0     2062 2024-03-15 05:54:51.299588 plothist-1.2.2/docs/usage/font_installation.rst
--rw-r--r--   0        0        0     2407 2024-01-24 11:19:08.110954 plothist-1.2.2/docs/usage/installation.rst
--rw-r--r--   0        0        0     9801 2024-04-18 00:01:09.624927 plothist-1.2.2/docs/usage/plot_fitting_results.rst
--rw-r--r--   0        0        0     3483 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/usage/style.rst
--rw-r--r--   0        0        0     3457 2024-02-27 13:16:21.606387 plothist-1.2.2/docs/usage/utilities.rst
--rw-r--r--   0        0        0     1322 2024-03-13 11:52:28.304522 plothist-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3314 2024-04-19 07:12:22.709929 plothist-1.2.2/src/plothist/__init__.py
--rw-r--r--   0        0        0    17431 2024-03-15 05:54:51.299588 plothist-1.2.2/src/plothist/comparison.py
--rw-r--r--   0        0        0     1574 2024-02-29 11:43:44.793823 plothist-1.2.2/src/plothist/default_style.mplstyle
--rw-r--r--   0        0        0  5936219 2024-02-29 11:43:44.821823 plothist-1.2.2/src/plothist/dummy_data.csv
--rw-r--r--   0        0        0      434 2024-02-29 11:43:44.821823 plothist-1.2.2/src/plothist/get_dummy_data.py
--rw-r--r--   0        0        0    10201 2024-03-27 05:59:25.706888 plothist-1.2.2/src/plothist/histogramming.py
--rw-r--r--   0        0        0    12282 2024-04-18 00:01:09.624927 plothist-1.2.2/src/plothist/plothist_style.py
--rw-r--r--   0        0        0    41526 2024-04-18 00:01:09.624927 plothist-1.2.2/src/plothist/plotters.py
--rw-r--r--   0        0        0      108 2024-03-13 11:52:28.304522 plothist-1.2.2/src/plothist/scripts/__init__.py
--rw-r--r--   0        0        0     7272 2024-04-18 00:01:09.624927 plothist-1.2.2/src/plothist/scripts/install_latin_modern_fonts.py
--rw-r--r--   0        0        0     6779 2024-04-18 00:01:09.624927 plothist-1.2.2/src/plothist/scripts/make_examples.py
--rw-r--r--   0        0        0    10207 2024-03-27 05:59:25.706888 plothist-1.2.2/src/plothist/variable_registry.py
--rw-r--r--   0        0        0     1828 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_asymmetry.py
--rw-r--r--   0        0        0     3543 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_difference.py
--rw-r--r--   0        0        0     4662 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_efficiency.py
--rw-r--r--   0        0        0     4080 2024-03-27 05:59:25.706888 plothist-1.2.2/tests/test_histogramming.py
--rw-r--r--   0        0        0      832 2024-02-28 09:38:28.695495 plothist-1.2.2/tests/test_install_fonts.py
--rw-r--r--   0        0        0      161 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_make_examples.py
--rw-r--r--   0        0        0     2952 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_pull.py
--rw-r--r--   0        0        0     7303 2024-03-13 11:52:28.304522 plothist-1.2.2/tests/test_ratio.py
--rw-r--r--   0        0        0     8444 2024-04-18 00:01:09.624927 plothist-1.2.2/tests/test_variable_registry.py
--rw-r--r--   0        0        0     3507 1970-01-01 00:00:00.000000 plothist-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      363 2024-04-19 00:12:45.212523 plothist-1.2.3/.github/ISSUE_TEMPLATE/user-story.md
+-rw-r--r--   0        0        0     1031 2024-04-18 00:01:09.624927 plothist-1.2.3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      217 2024-04-18 00:01:09.624927 plothist-1.2.3/.gitignore
+-rw-r--r--   0        0        0      853 2024-02-27 12:31:06.447939 plothist-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2024-02-27 12:31:06.447939 plothist-1.2.3/.readthedocs.yaml
+-rw-r--r--   0        0        0      111 2024-01-24 11:19:08.106954 plothist-1.2.3/AUTHORS.md
+-rw-r--r--   0        0        0     1523 2024-02-01 10:13:39.803203 plothist-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2644 2024-04-19 07:13:01.245893 plothist-1.2.3/README.rst
+-rw-r--r--   0        0        0    10493 2024-03-27 04:27:38.576554 plothist-1.2.3/docs/advanced/model_examples.rst
+-rw-r--r--   0        0        0     1970 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/advanced/other_advanced.rst
+-rw-r--r--   0        0        0    10309 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/basics/1d_hist.rst
+-rw-r--r--   0        0        0     2838 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/basics/2d_hist.rst
+-rw-r--r--   0        0        0     8175 2024-04-18 00:01:09.624927 plothist-1.2.3/docs/basics/variable_registry.rst
+-rw-r--r--   0        0        0     6958 2024-04-19 07:13:01.245893 plothist-1.2.3/docs/conf.py
+-rw-r--r--   0        0        0      585 2024-04-18 00:01:09.624927 plothist-1.2.3/docs/documentation/documentation.rst
+-rw-r--r--   0        0        0      834 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/documentation/statistics.rst
+-rw-r--r--   0        0        0      786 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_asymmetry.py
+-rw-r--r--   0        0        0      914 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_difference.py
+-rw-r--r--   0        0        0      865 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_efficiency.py
+-rw-r--r--   0        0        0      831 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_only_efficiency.py
+-rw-r--r--   0        0        0      719 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_pull.py
+-rw-r--r--   0        0        0      724 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_ratio.py
+-rw-r--r--   0        0        0      823 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_relative_difference.py
+-rw-r--r--   0        0        0      803 2024-02-28 09:38:28.691495 plothist-1.2.3/docs/examples/1d_hist/1d_comparison_split_ratio.py
+-rw-r--r--   0        0        0      795 2024-01-25 11:39:29.527978 plothist-1.2.3/docs/examples/1d_hist/1d_elt1.py
+-rw-r--r--   0        0        0      810 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/1d_hist/1d_elt1_stacked.py
+-rw-r--r--   0        0        0      558 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_elt2.py
+-rw-r--r--   0        0        0      455 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/1d_hist/1d_fct.py
+-rw-r--r--   0        0        0      687 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/1d_hist/1d_fct_stacked.py
+-rw-r--r--   0        0        0      418 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/1d_hist/1d_hist_simple.py
+-rw-r--r--   0        0        0      883 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_int_category.py
+-rw-r--r--   0        0        0      661 2024-03-15 05:56:03.521542 plothist-1.2.3/docs/examples/1d_hist/1d_profile.py
+-rw-r--r--   0        0        0      882 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/examples/1d_hist/1d_str_category.py
+-rw-r--r--   0        0        0       96 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/1d_hist/README.rst
+-rw-r--r--   0        0        0     1495 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/2d_hist/2d_hist_correlations.py
+-rw-r--r--   0        0        0      534 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/2d_hist/2d_hist_simple.py
+-rw-r--r--   0        0        0     1040 2024-01-24 11:19:08.106954 plothist-1.2.3/docs/examples/2d_hist/2d_hist_simple_discrete_colormap.py
+-rw-r--r--   0        0        0      650 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/2d_hist/2d_hist_uneven.py
+-rw-r--r--   0        0        0      744 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/2d_hist/2d_hist_with_projections.py
+-rw-r--r--   0        0        0      116 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/2d_hist/README.rst
+-rw-r--r--   0        0        0      147 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/README.rst
+-rw-r--r--   0        0        0     2702 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/advanced/1d_comparison_advanced.py
+-rw-r--r--   0        0        0      112 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/advanced/README.rst
+-rw-r--r--   0        0        0     2598 2024-04-18 00:01:09.624927 plothist-1.2.3/docs/examples/advanced/asymmetry_comparison_advanced.py
+-rw-r--r--   0        0        0     3066 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/advanced/model_examples_flatten2D.py
+-rw-r--r--   0        0        0      103 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/model_ex/README.rst
+-rw-r--r--   0        0        0     2816 2024-02-28 09:38:28.691495 plothist-1.2.3/docs/examples/model_ex/model_all_comparisons.py
+-rw-r--r--   0        0        0     3423 2024-02-28 09:38:28.691495 plothist-1.2.3/docs/examples/model_ex/model_all_comparisons_no_model_unc.py
+-rw-r--r--   0        0        0     1654 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_examples_pull.py
+-rw-r--r--   0        0        0     1879 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_examples_pull_no_model_unc.py
+-rw-r--r--   0        0        0     1943 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_examples_stacked.py
+-rw-r--r--   0        0        0     1947 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_examples_stacked_unstacked.py
+-rw-r--r--   0        0        0     1744 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_examples_unstacked.py
+-rw-r--r--   0        0        0     1355 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_with_stacked_and_unstacked_function_components.py
+-rw-r--r--   0        0        0     1991 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/model_with_stacked_and_unstacked_histograms_components.py
+-rw-r--r--   0        0        0     1413 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/model_ex/ratio_data_vs_model_with_stacked_and_unstacked_function_components.py
+-rw-r--r--   0        0        0       77 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/utility/README.rst
+-rw-r--r--   0        0        0     2359 2023-12-11 08:11:42.957778 plothist-1.2.3/docs/examples/utility/color_palette_hists.py
+-rw-r--r--   0        0        0     2729 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/utility/color_palette_squares.py
+-rw-r--r--   0        0        0     1820 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/examples/utility/matplotlib_vs_plothist_style.py
+-rw-r--r--   0        0        0   115640 2024-03-26 03:06:19.637708 plothist-1.2.3/docs/img/1d_comparison_advanced.svg
+-rw-r--r--   0        0        0    53814 2024-03-27 05:59:25.694889 plothist-1.2.3/docs/img/1d_comparison_asymmetry.svg
+-rw-r--r--   0        0        0    67200 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_difference.svg
+-rw-r--r--   0        0        0    70322 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_efficiency.svg
+-rw-r--r--   0        0        0    45998 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_only_efficiency.svg
+-rw-r--r--   0        0        0    47754 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_pull.svg
+-rw-r--r--   0        0        0    50549 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_ratio.svg
+-rw-r--r--   0        0        0    53545 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_relative_difference.svg
+-rw-r--r--   0        0        0    62167 2024-03-27 05:59:25.698889 plothist-1.2.3/docs/img/1d_comparison_split_ratio.svg
+-rw-r--r--   0        0        0    31035 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_elt1.svg
+-rw-r--r--   0        0        0    40167 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_elt1_stacked.svg
+-rw-r--r--   0        0        0    37991 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_elt2.svg
+-rw-r--r--   0        0        0    25927 2024-03-26 03:06:51.502231 plothist-1.2.3/docs/img/1d_fct.svg
+-rw-r--r--   0        0        0   118828 2024-03-26 03:06:59.702372 plothist-1.2.3/docs/img/1d_fct_stacked.svg
+-rw-r--r--   0        0        0    41618 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_hist_simple.svg
+-rw-r--r--   0        0        0    22944 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_int_category.svg
+-rw-r--r--   0        0        0    28474 2024-03-26 03:07:10.026554 plothist-1.2.3/docs/img/1d_profile.svg
+-rw-r--r--   0        0        0    23667 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/1d_str_category.svg
+-rw-r--r--   0        0        0   551253 2024-03-26 03:06:49.342194 plothist-1.2.3/docs/img/2d_hist_correlations_0.svg
+-rw-r--r--   0        0        0   521575 2024-03-26 03:06:49.786202 plothist-1.2.3/docs/img/2d_hist_correlations_1.svg
+-rw-r--r--   0        0        0   518776 2024-03-26 03:06:50.290211 plothist-1.2.3/docs/img/2d_hist_correlations_2.svg
+-rw-r--r--   0        0        0    60974 2024-03-26 03:06:47.578164 plothist-1.2.3/docs/img/2d_hist_simple.svg
+-rw-r--r--   0        0        0   555885 2024-03-27 05:59:25.702889 plothist-1.2.3/docs/img/2d_hist_simple_discrete_colormap.svg
+-rw-r--r--   0        0        0    48903 2024-03-26 03:06:42.858085 plothist-1.2.3/docs/img/2d_hist_uneven.svg
+-rw-r--r--   0        0        0   578843 2024-03-27 05:59:25.706888 plothist-1.2.3/docs/img/2d_hist_with_projections.svg
+-rw-r--r--   0        0        0   107898 2024-03-26 03:06:20.817726 plothist-1.2.3/docs/img/asymmetry_comparison_advanced.svg
+-rw-r--r--   0        0        0    35065 2024-03-26 03:06:25.469801 plothist-1.2.3/docs/img/matplotlib_example.svg
+-rw-r--r--   0        0        0   210630 2024-03-26 03:06:39.762034 plothist-1.2.3/docs/img/model_all_comparisons.svg
+-rw-r--r--   0        0        0   198568 2024-03-26 03:06:30.609883 plothist-1.2.3/docs/img/model_all_comparisons_no_model_unc.svg
+-rw-r--r--   0        0        0    65977 2024-03-26 03:06:21.989745 plothist-1.2.3/docs/img/model_examples_flatten2D.svg
+-rw-r--r--   0        0        0    94412 2024-03-26 03:06:36.137974 plothist-1.2.3/docs/img/model_examples_pull.svg
+-rw-r--r--   0        0        0    93502 2024-03-26 03:06:33.537931 plothist-1.2.3/docs/img/model_examples_pull_no_model_unc.svg
+-rw-r--r--   0        0        0   122943 2024-03-26 03:06:41.382060 plothist-1.2.3/docs/img/model_examples_stacked.svg
+-rw-r--r--   0        0        0   103269 2024-03-26 03:06:28.561850 plothist-1.2.3/docs/img/model_examples_stacked_unstacked.svg
+-rw-r--r--   0        0        0   102567 2024-03-26 03:06:27.177828 plothist-1.2.3/docs/img/model_examples_unstacked.svg
+-rw-r--r--   0        0        0   141571 2024-03-26 03:06:37.177991 plothist-1.2.3/docs/img/model_with_stacked_and_unstacked_function_components.svg
+-rw-r--r--   0        0        0    72038 2024-03-26 03:06:34.729951 plothist-1.2.3/docs/img/model_with_stacked_and_unstacked_histograms_components.svg
+-rw-r--r--   0        0        0    49322 2024-03-26 03:06:25.773805 plothist-1.2.3/docs/img/plothist_example.svg
+-rw-r--r--   0        0        0    42928 2024-02-20 15:43:53.653134 plothist-1.2.3/docs/img/pyhf_example.svg
+-rw-r--r--   0        0        0   170416 2024-03-26 03:06:31.881904 plothist-1.2.3/docs/img/ratio_data_vs_model_with_stacked_and_unstacked_function_components.svg
+-rw-r--r--   0        0        0   436516 2023-12-11 08:11:42.973778 plothist-1.2.3/docs/img/savefig_comparisons.gif
+-rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.373783 plothist-1.2.3/docs/img/usage_YlGnBu_r_palette.svg
+-rw-r--r--   0        0        0   270554 2024-03-26 03:06:23.429768 plothist-1.2.3/docs/img/usage_colorpalette_examples.svg
+-rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.317782 plothist-1.2.3/docs/img/usage_coolwarm_palette.svg
+-rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.213780 plothist-1.2.3/docs/img/usage_cubehelix.svg
+-rw-r--r--   0        0        0    16297 2024-03-26 03:06:24.133779 plothist-1.2.3/docs/img/usage_style_cycle.svg
+-rw-r--r--   0        0        0     2384 2024-03-26 03:06:24.269781 plothist-1.2.3/docs/img/usage_viridis_palette.svg
+-rw-r--r--   0        0        0      646 2024-02-27 12:31:06.447939 plothist-1.2.3/docs/index.rst
+-rw-r--r--   0        0        0     2062 2024-03-15 05:54:51.299588 plothist-1.2.3/docs/usage/font_installation.rst
+-rw-r--r--   0        0        0     2407 2024-01-24 11:19:08.110954 plothist-1.2.3/docs/usage/installation.rst
+-rw-r--r--   0        0        0     9801 2024-04-18 00:01:09.624927 plothist-1.2.3/docs/usage/plot_fitting_results.rst
+-rw-r--r--   0        0        0     3483 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/usage/style.rst
+-rw-r--r--   0        0        0     3457 2024-02-27 13:16:21.606387 plothist-1.2.3/docs/usage/utilities.rst
+-rw-r--r--   0        0        0     1322 2024-03-13 11:52:28.304522 plothist-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3314 2024-04-19 07:13:01.245893 plothist-1.2.3/src/plothist/__init__.py
+-rw-r--r--   0        0        0    17431 2024-03-15 05:54:51.299588 plothist-1.2.3/src/plothist/comparison.py
+-rw-r--r--   0        0        0     1574 2024-02-29 11:43:44.793823 plothist-1.2.3/src/plothist/default_style.mplstyle
+-rw-r--r--   0        0        0  5936219 2024-02-29 11:43:44.821823 plothist-1.2.3/src/plothist/dummy_data.csv
+-rw-r--r--   0        0        0      434 2024-02-29 11:43:44.821823 plothist-1.2.3/src/plothist/get_dummy_data.py
+-rw-r--r--   0        0        0    10201 2024-03-27 05:59:25.706888 plothist-1.2.3/src/plothist/histogramming.py
+-rw-r--r--   0        0        0    12282 2024-04-18 00:01:09.624927 plothist-1.2.3/src/plothist/plothist_style.py
+-rw-r--r--   0        0        0    41526 2024-04-18 00:01:09.624927 plothist-1.2.3/src/plothist/plotters.py
+-rw-r--r--   0        0        0      108 2024-03-13 11:52:28.304522 plothist-1.2.3/src/plothist/scripts/__init__.py
+-rw-r--r--   0        0        0     7272 2024-04-18 00:01:09.624927 plothist-1.2.3/src/plothist/scripts/install_latin_modern_fonts.py
+-rw-r--r--   0        0        0     6779 2024-04-18 00:01:09.624927 plothist-1.2.3/src/plothist/scripts/make_examples.py
+-rw-r--r--   0        0        0    10207 2024-03-27 05:59:25.706888 plothist-1.2.3/src/plothist/variable_registry.py
+-rw-r--r--   0        0        0     1828 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_asymmetry.py
+-rw-r--r--   0        0        0     3543 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_difference.py
+-rw-r--r--   0        0        0     4662 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_efficiency.py
+-rw-r--r--   0        0        0     4080 2024-03-27 05:59:25.706888 plothist-1.2.3/tests/test_histogramming.py
+-rw-r--r--   0        0        0      832 2024-02-28 09:38:28.695495 plothist-1.2.3/tests/test_install_fonts.py
+-rw-r--r--   0        0        0      161 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_make_examples.py
+-rw-r--r--   0        0        0     2952 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_pull.py
+-rw-r--r--   0        0        0     7303 2024-03-13 11:52:28.304522 plothist-1.2.3/tests/test_ratio.py
+-rw-r--r--   0        0        0     8444 2024-04-18 00:01:09.624927 plothist-1.2.3/tests/test_variable_registry.py
+-rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 plothist-1.2.3/PKG-INFO
```

### Comparing `plothist-1.2.2/.github/workflows/python-package.yml` & `plothist-1.2.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/.pre-commit-config.yaml` & `plothist-1.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/LICENSE` & `plothist-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/README.rst` & `plothist-1.2.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    :width: 320
 
 .. |img2| image:: https://raw.githubusercontent.com/cyrraz/plothist/main/docs/img/model_examples_stacked.svg
    :alt: Example
    :width: 320
 
 
-|GitHub Project| |PyPI version| |Docs from latest| |Docs from main| |Code style: black|
+|GitHub Project| |PyPI version| |Docs from main| |Discussion| |DOI| |Code style: black|
 
 
 **Advantages of the package**: scalability, style and user-friendly way of managing variables and a stunning `image gallery <https://plothist.readthedocs.io/en/latest/example_gallery/>`_.
 
 1. **First idea**: default style is already presentation-ready and/or publication-ready (with no effort).
 
 2. **Second idea**: separate the histogram creation from its plotting. This allows to easily manage histogram objects (defined in the ``boost_histogram`` `package <https://boost-histogram.readthedocs.io/>`_) and plot large amount of variables and data really fast.
@@ -41,13 +41,15 @@
 
 
 
 .. |GitHub Project| image:: https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub
    :target: https://github.com/cyrraz/plothist
 .. |PyPI version| image:: https://badge.fury.io/py/plothist.svg
    :target: https://badge.fury.io/py/plothist
-.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-.. |Docs from latest| image:: https://img.shields.io/badge/docs-v1.2.2-blue.svg
-   :target: https://plothist.readthedocs.io/en/latest/
 .. |Docs from main| image:: https://img.shields.io/badge/docs-main-blue.svg
    :target: https://plothist.readthedocs.io/en/main/
+.. |Discussion| image:: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+   :target: https://github.com/cyrraz/plothist/discussions
+.. |DOI| image:: https://zenodo.org/badge/647069945.svg
+   :target: https://zenodo.org/doi/10.5281/zenodo.10995667
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
```

### Comparing `plothist-1.2.2/docs/advanced/model_examples.rst` & `plothist-1.2.3/docs/advanced/model_examples.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/advanced/other_advanced.rst` & `plothist-1.2.3/docs/advanced/other_advanced.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/basics/1d_hist.rst` & `plothist-1.2.3/docs/basics/1d_hist.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/basics/2d_hist.rst` & `plothist-1.2.3/docs/basics/2d_hist.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/basics/variable_registry.rst` & `plothist-1.2.3/docs/basics/variable_registry.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/conf.py` & `plothist-1.2.3/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 from sphinx_gallery.sorting import FileNameSortKey
 
 project = "plothist"
 copyright = "2023-2024, Cyrille Praz, Tristan Fillinger"
 author = "Cyrille Praz, Tristan Fillinger"
 
 # The short X.Y version
-version = "1.2.2"
+version = "1.2.3"
 # The full version, including alpha/beta/rc tags
-release = "1.2.2"
+release = "1.2.3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `plothist-1.2.2/docs/documentation/documentation.rst` & `plothist-1.2.3/docs/documentation/documentation.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/documentation/statistics.rst` & `plothist-1.2.3/docs/documentation/statistics.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_asymmetry.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_asymmetry.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_difference.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_difference.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_efficiency.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_efficiency.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_only_efficiency.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_only_efficiency.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_pull.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_pull.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_ratio.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_ratio.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_relative_difference.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_relative_difference.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_comparison_split_ratio.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_comparison_split_ratio.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_elt1.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_elt1.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_elt1_stacked.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_elt1_stacked.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_elt2.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_elt2.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_fct_stacked.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_fct_stacked.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_int_category.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_int_category.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_profile.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_profile.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/1d_hist/1d_str_category.py` & `plothist-1.2.3/docs/examples/1d_hist/1d_str_category.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/2d_hist/2d_hist_correlations.py` & `plothist-1.2.3/docs/examples/2d_hist/2d_hist_correlations.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/2d_hist/2d_hist_simple.py` & `plothist-1.2.3/docs/examples/2d_hist/2d_hist_simple.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/2d_hist/2d_hist_simple_discrete_colormap.py` & `plothist-1.2.3/docs/examples/2d_hist/2d_hist_simple_discrete_colormap.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/2d_hist/2d_hist_uneven.py` & `plothist-1.2.3/docs/examples/2d_hist/2d_hist_uneven.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/2d_hist/2d_hist_with_projections.py` & `plothist-1.2.3/docs/examples/2d_hist/2d_hist_with_projections.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/advanced/1d_comparison_advanced.py` & `plothist-1.2.3/docs/examples/advanced/1d_comparison_advanced.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/advanced/asymmetry_comparison_advanced.py` & `plothist-1.2.3/docs/examples/advanced/asymmetry_comparison_advanced.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/advanced/model_examples_flatten2D.py` & `plothist-1.2.3/docs/examples/advanced/model_examples_flatten2D.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_all_comparisons.py` & `plothist-1.2.3/docs/examples/model_ex/model_all_comparisons.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_all_comparisons_no_model_unc.py` & `plothist-1.2.3/docs/examples/model_ex/model_all_comparisons_no_model_unc.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_examples_pull.py` & `plothist-1.2.3/docs/examples/model_ex/model_examples_pull.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_examples_pull_no_model_unc.py` & `plothist-1.2.3/docs/examples/model_ex/model_examples_pull_no_model_unc.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_examples_stacked.py` & `plothist-1.2.3/docs/examples/model_ex/model_examples_stacked.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_examples_stacked_unstacked.py` & `plothist-1.2.3/docs/examples/model_ex/model_examples_stacked_unstacked.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_examples_unstacked.py` & `plothist-1.2.3/docs/examples/model_ex/model_examples_unstacked.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_with_stacked_and_unstacked_function_components.py` & `plothist-1.2.3/docs/examples/model_ex/model_with_stacked_and_unstacked_function_components.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/model_with_stacked_and_unstacked_histograms_components.py` & `plothist-1.2.3/docs/examples/model_ex/model_with_stacked_and_unstacked_histograms_components.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/model_ex/ratio_data_vs_model_with_stacked_and_unstacked_function_components.py` & `plothist-1.2.3/docs/examples/model_ex/ratio_data_vs_model_with_stacked_and_unstacked_function_components.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/utility/color_palette_hists.py` & `plothist-1.2.3/docs/examples/utility/color_palette_hists.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/utility/color_palette_squares.py` & `plothist-1.2.3/docs/examples/utility/color_palette_squares.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/examples/utility/matplotlib_vs_plothist_style.py` & `plothist-1.2.3/docs/examples/utility/matplotlib_vs_plothist_style.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_advanced.svg` & `plothist-1.2.3/docs/img/1d_comparison_advanced.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_asymmetry.svg` & `plothist-1.2.3/docs/img/1d_comparison_asymmetry.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_difference.svg` & `plothist-1.2.3/docs/img/1d_comparison_difference.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_efficiency.svg` & `plothist-1.2.3/docs/img/1d_comparison_efficiency.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_only_efficiency.svg` & `plothist-1.2.3/docs/img/1d_comparison_only_efficiency.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_pull.svg` & `plothist-1.2.3/docs/img/1d_comparison_pull.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_ratio.svg` & `plothist-1.2.3/docs/img/1d_comparison_ratio.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_relative_difference.svg` & `plothist-1.2.3/docs/img/1d_comparison_relative_difference.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_comparison_split_ratio.svg` & `plothist-1.2.3/docs/img/1d_comparison_split_ratio.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_elt1.svg` & `plothist-1.2.3/docs/img/1d_elt1.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_elt1_stacked.svg` & `plothist-1.2.3/docs/img/1d_elt1_stacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_elt2.svg` & `plothist-1.2.3/docs/img/1d_elt2.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_fct.svg` & `plothist-1.2.3/docs/img/1d_fct.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_fct_stacked.svg` & `plothist-1.2.3/docs/img/1d_fct_stacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_hist_simple.svg` & `plothist-1.2.3/docs/img/1d_hist_simple.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_int_category.svg` & `plothist-1.2.3/docs/img/1d_int_category.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_profile.svg` & `plothist-1.2.3/docs/img/1d_profile.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/1d_str_category.svg` & `plothist-1.2.3/docs/img/1d_str_category.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_correlations_0.svg` & `plothist-1.2.3/docs/img/2d_hist_correlations_0.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_correlations_1.svg` & `plothist-1.2.3/docs/img/2d_hist_correlations_1.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_correlations_2.svg` & `plothist-1.2.3/docs/img/2d_hist_correlations_2.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_simple.svg` & `plothist-1.2.3/docs/img/2d_hist_simple.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_simple_discrete_colormap.svg` & `plothist-1.2.3/docs/img/2d_hist_simple_discrete_colormap.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_uneven.svg` & `plothist-1.2.3/docs/img/2d_hist_uneven.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/2d_hist_with_projections.svg` & `plothist-1.2.3/docs/img/2d_hist_with_projections.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/asymmetry_comparison_advanced.svg` & `plothist-1.2.3/docs/img/asymmetry_comparison_advanced.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/matplotlib_example.svg` & `plothist-1.2.3/docs/img/matplotlib_example.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_all_comparisons.svg` & `plothist-1.2.3/docs/img/model_all_comparisons.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_all_comparisons_no_model_unc.svg` & `plothist-1.2.3/docs/img/model_all_comparisons_no_model_unc.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_flatten2D.svg` & `plothist-1.2.3/docs/img/model_examples_flatten2D.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_pull.svg` & `plothist-1.2.3/docs/img/model_examples_pull.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_pull_no_model_unc.svg` & `plothist-1.2.3/docs/img/model_examples_pull_no_model_unc.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_stacked.svg` & `plothist-1.2.3/docs/img/model_examples_stacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_stacked_unstacked.svg` & `plothist-1.2.3/docs/img/model_examples_stacked_unstacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_examples_unstacked.svg` & `plothist-1.2.3/docs/img/model_examples_unstacked.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_with_stacked_and_unstacked_function_components.svg` & `plothist-1.2.3/docs/img/model_with_stacked_and_unstacked_function_components.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/model_with_stacked_and_unstacked_histograms_components.svg` & `plothist-1.2.3/docs/img/model_with_stacked_and_unstacked_histograms_components.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/plothist_example.svg` & `plothist-1.2.3/docs/img/plothist_example.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/pyhf_example.svg` & `plothist-1.2.3/docs/img/pyhf_example.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/ratio_data_vs_model_with_stacked_and_unstacked_function_components.svg` & `plothist-1.2.3/docs/img/ratio_data_vs_model_with_stacked_and_unstacked_function_components.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/savefig_comparisons.gif` & `plothist-1.2.3/docs/img/savefig_comparisons.gif`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_YlGnBu_r_palette.svg` & `plothist-1.2.3/docs/img/usage_YlGnBu_r_palette.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_colorpalette_examples.svg` & `plothist-1.2.3/docs/img/usage_colorpalette_examples.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_coolwarm_palette.svg` & `plothist-1.2.3/docs/img/usage_coolwarm_palette.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_cubehelix.svg` & `plothist-1.2.3/docs/img/usage_cubehelix.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_style_cycle.svg` & `plothist-1.2.3/docs/img/usage_style_cycle.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/img/usage_viridis_palette.svg` & `plothist-1.2.3/docs/img/usage_viridis_palette.svg`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/index.rst` & `plothist-1.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/usage/font_installation.rst` & `plothist-1.2.3/docs/usage/font_installation.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/usage/installation.rst` & `plothist-1.2.3/docs/usage/installation.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/usage/plot_fitting_results.rst` & `plothist-1.2.3/docs/usage/plot_fitting_results.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/usage/style.rst` & `plothist-1.2.3/docs/usage/style.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/docs/usage/utilities.rst` & `plothist-1.2.3/docs/usage/utilities.rst`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/pyproject.toml` & `plothist-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/__init__.py` & `plothist-1.2.3/src/plothist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Plot histograms in a scalable way and a beautiful style."""
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 from .plotters import (
     create_comparison_figure,
     plot_hist,
     plot_2d_hist,
     plot_2d_hist_with_projections,
     plot_error_hist,
```

### Comparing `plothist-1.2.2/src/plothist/comparison.py` & `plothist-1.2.3/src/plothist/comparison.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/default_style.mplstyle` & `plothist-1.2.3/src/plothist/default_style.mplstyle`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/dummy_data.csv` & `plothist-1.2.3/src/plothist/dummy_data.csv`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/histogramming.py` & `plothist-1.2.3/src/plothist/histogramming.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/plothist_style.py` & `plothist-1.2.3/src/plothist/plothist_style.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/plotters.py` & `plothist-1.2.3/src/plothist/plotters.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/scripts/install_latin_modern_fonts.py` & `plothist-1.2.3/src/plothist/scripts/install_latin_modern_fonts.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/scripts/make_examples.py` & `plothist-1.2.3/src/plothist/scripts/make_examples.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/src/plothist/variable_registry.py` & `plothist-1.2.3/src/plothist/variable_registry.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_asymmetry.py` & `plothist-1.2.3/tests/test_asymmetry.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_difference.py` & `plothist-1.2.3/tests/test_difference.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_efficiency.py` & `plothist-1.2.3/tests/test_efficiency.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_histogramming.py` & `plothist-1.2.3/tests/test_histogramming.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_install_fonts.py` & `plothist-1.2.3/tests/test_install_fonts.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_pull.py` & `plothist-1.2.3/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_ratio.py` & `plothist-1.2.3/tests/test_ratio.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/tests/test_variable_registry.py` & `plothist-1.2.3/tests/test_variable_registry.py`

 * *Files identical despite different names*

### Comparing `plothist-1.2.2/PKG-INFO` & `plothist-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plothist
-Version: 1.2.2
+Version: 1.2.3
 Summary: Plot histograms in a scalable way and a beautiful style.
 Author-email: Cyrille Praz <cyrraz.code@protonmail.com>, Tristan Fillinger <tristan.github@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -39,15 +39,15 @@
    :width: 320
 
 .. |img2| image:: https://raw.githubusercontent.com/cyrraz/plothist/main/docs/img/model_examples_stacked.svg
    :alt: Example
    :width: 320
 
 
-|GitHub Project| |PyPI version| |Docs from latest| |Docs from main| |Code style: black|
+|GitHub Project| |PyPI version| |Docs from main| |Discussion| |DOI| |Code style: black|
 
 
 **Advantages of the package**: scalability, style and user-friendly way of managing variables and a stunning `image gallery <https://plothist.readthedocs.io/en/latest/example_gallery/>`_.
 
 1. **First idea**: default style is already presentation-ready and/or publication-ready (with no effort).
 
 2. **Second idea**: separate the histogram creation from its plotting. This allows to easily manage histogram objects (defined in the ``boost_histogram`` `package <https://boost-histogram.readthedocs.io/>`_) and plot large amount of variables and data really fast.
@@ -65,14 +65,16 @@
 
 
 
 .. |GitHub Project| image:: https://img.shields.io/badge/GitHub--blue?style=social&logo=GitHub
    :target: https://github.com/cyrraz/plothist
 .. |PyPI version| image:: https://badge.fury.io/py/plothist.svg
    :target: https://badge.fury.io/py/plothist
-.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-.. |Docs from latest| image:: https://img.shields.io/badge/docs-v1.2.2-blue.svg
-   :target: https://plothist.readthedocs.io/en/latest/
 .. |Docs from main| image:: https://img.shields.io/badge/docs-main-blue.svg
    :target: https://plothist.readthedocs.io/en/main/
+.. |Discussion| image:: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
+   :target: https://github.com/cyrraz/plothist/discussions
+.. |DOI| image:: https://zenodo.org/badge/647069945.svg
+   :target: https://zenodo.org/doi/10.5281/zenodo.10995667
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
```

