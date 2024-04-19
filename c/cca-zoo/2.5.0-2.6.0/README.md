# Comparing `tmp/cca_zoo-2.5.0.tar.gz` & `tmp/cca_zoo-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cca_zoo-2.5.0.tar", max compression
+gzip compressed data, was "cca_zoo-2.6.0.tar", max compression
```

## Comparing `cca_zoo-2.5.0.tar` & `cca_zoo-2.6.0.tar`

### file list

```diff
@@ -1,92 +1,87 @@
--rw-r--r--   0        0        0     1069 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/LICENSE
--rw-r--r--   0        0        0     4469 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/README.md
--rw-r--r--   0        0        0      261 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/__init__.py
--rw-r--r--   0        0        0    17234 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/_base.py
--rw-r--r--   0        0        0        0 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/_utils/__init__.py
--rw-r--r--   0        0        0     7543 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/_utils/_checks.py
--rw-r--r--   0        0        0     1437 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/_utils/_cross_correlation.py
--rw-r--r--   0        0        0     4838 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/_utils/_splitter.py
--rw-r--r--   0        0        0      418 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/datasets/__init__.py
--rw-r--r--   0        0        0    15048 2023-12-04 12:30:59.106374 cca_zoo-2.5.0/cca_zoo/datasets/simulated.py
--rw-r--r--   0        0        0     9792 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/datasets/toy.py
--rw-r--r--   0        0        0     1201 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/__init__.py
--rw-r--r--   0        0        0     5835 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_base.py
--rw-r--r--   0        0        0        0 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0        0        0     2514 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_barlow_twins.py
--rw-r--r--   0        0        0     1874 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0        0        0      976 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0        0        0      616 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_gha.py
--rw-r--r--   0        0        0     5943 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0        0        0     1939 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0        0        0      625 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0        0        0      568 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0        0        0      568 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dmcca.py
--rw-r--r--   0        0        0      749 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dtcca.py
--rw-r--r--   0        0        0     4875 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_vicreg.py
--rw-r--r--   0        0        0        0 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0        0        0     1449 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0        0        0     2446 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0        0        0     5385 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0        0        0     2079 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0        0        0      180 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/_utils.py
--rw-r--r--   0        0        0     7467 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/architectures.py
--rw-r--r--   0        0        0     3321 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/data.py
--rw-r--r--   0        0        0    10990 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/deep/objectives.py
--rw-r--r--   0        0        0     1061 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/__init__.py
--rw-r--r--   0        0        0     1645 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_dummy.py
--rw-r--r--   0        0        0     3085 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gcca.py
--rw-r--r--   0        0        0        0 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/__init__.py
--rw-r--r--   0        0        0     7720 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_base.py
--rw-r--r--   0        0        0     3554 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_ey.py
--rw-r--r--   0        0        0     2015 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_gha.py
--rw-r--r--   0        0        0     1480 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_objectives.py
--rw-r--r--   0        0        0     1170 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_stochasticpls.py
--rw-r--r--   0        0        0     2021 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_svd.py
--rw-r--r--   0        0        0      153 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_gradient/_tracenorm.py
--rw-r--r--   0        0        0     6686 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_grcca.py
--rw-r--r--   0        0        0        0 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/__init__.py
--rw-r--r--   0        0        0     8216 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_altmaxvar.py
--rw-r--r--   0        0        0     5584 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_base.py
--rw-r--r--   0        0        0     2135 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_deflation.py
--rw-r--r--   0        0        0     8821 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_elastic.py
--rw-r--r--   0        0        0     4130 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_incrementalpls.py
--rw-r--r--   0        0        0     1655 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_pls_als.py
--rw-r--r--   0        0        0     7276 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_admm.py
--rw-r--r--   0        0        0     2250 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py
--rw-r--r--   0        0        0     3765 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_span.py
--rw-r--r--   0        0        0     3798 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_spls.py
--rw-r--r--   0        0        0     3983 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_iterative/_swcca.py
--rw-r--r--   0        0        0    12998 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_mcca.py
--rw-r--r--   0        0        0     2959 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_partialcca.py
--rw-r--r--   0        0        0     2303 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_pcacca.py
--rw-r--r--   0        0        0     2627 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_pls.py
--rw-r--r--   0        0        0      491 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_plsregression.py
--rw-r--r--   0        0        0     4358 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_prcca.py
--rw-r--r--   0        0        0     2681 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_search.py
--rw-r--r--   0        0        0     5213 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/linear/_tcca.py
--rw-r--r--   0        0        0      327 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/model_selection/__init__.py
--rw-r--r--   0        0        0     3930 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/model_selection/_search.py
--rw-r--r--   0        0        0    15820 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/model_selection/_validation.py
--rw-r--r--   0        0        0      158 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/nonparametric/__init__.py
--rw-r--r--   0        0        0    13019 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/nonparametric/_kcca.py
--rw-r--r--   0        0        0     6418 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/nonparametric/_ncca.py
--rw-r--r--   0        0        0     5775 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/nonparametric/_scca_hsic.py
--rw-r--r--   0        0        0     1891 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/preprocessing/__init__.py
--rw-r--r--   0        0        0      511 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0        0        0     7697 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/probabilistic/_cca.py
--rw-r--r--   0        0        0     3520 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/probabilistic/_pls.py
--rw-r--r--   0        0        0     7898 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/probabilistic/_plsregression.py
--rw-r--r--   0        0        0     4816 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/probabilistic/_rcca.py
--rw-r--r--   0        0        0     5049 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/sequential.py
--rw-r--r--   0        0        0     1282 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/__init__.py
--rw-r--r--   0        0        0     3304 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/correlation.py
--rw-r--r--   0        0        0     3111 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/covariance.py
--rw-r--r--   0        0        0     5206 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/explained_covariance.py
--rw-r--r--   0        0        0     7085 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/explained_variance.py
--rw-r--r--   0        0        0     3627 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/inference.py
--rw-r--r--   0        0        0    10897 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/scores.py
--rw-r--r--   0        0        0     1285 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/tsne_scores.py
--rw-r--r--   0        0        0     1303 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/umap_scores.py
--rw-r--r--   0        0        0     1680 2023-12-04 12:30:59.110374 cca_zoo-2.5.0/cca_zoo/visualisation/weights.py
--rw-r--r--   0        0        0     1491 2023-12-04 12:30:59.178374 cca_zoo-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     6006 1970-01-01 00:00:00.000000 cca_zoo-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-19 10:57:24.885313 cca_zoo-2.6.0/LICENSE
+-rw-r--r--   0        0        0     4754 2024-04-19 10:57:24.885313 cca_zoo-2.6.0/README.md
+-rw-r--r--   0        0        0      261 2024-04-19 10:57:24.885313 cca_zoo-2.6.0/cca_zoo/__init__.py
+-rw-r--r--   0        0        0    14105 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/_base.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/_utils/__init__.py
+-rw-r--r--   0        0        0     7543 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/_utils/_checks.py
+-rw-r--r--   0        0        0     1437 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/_utils/_cross_correlation.py
+-rw-r--r--   0        0        0     4837 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/_utils/_splitter.py
+-rw-r--r--   0        0        0      419 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/datasets/__init__.py
+-rw-r--r--   0        0        0    14735 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/datasets/simulated.py
+-rw-r--r--   0        0        0     9792 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/datasets/toy.py
+-rw-r--r--   0        0        0     1188 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/__init__.py
+-rw-r--r--   0        0        0     5905 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_base.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0        0        0     2587 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_barlow_twins.py
+-rw-r--r--   0        0        0     1435 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0        0        0      939 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0        0        0     1154 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_gha.py
+-rw-r--r--   0        0        0     5270 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0        0        0     1649 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0        0        0     1182 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0        0        0     1204 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0        0        0     1843 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dmcca.py
+-rw-r--r--   0        0        0     3872 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dtcca.py
+-rw-r--r--   0        0        0     4971 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_vicreg.py
+-rw-r--r--   0        0        0     1449 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0        0        0     2464 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0        0        0     5736 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0        0        0     1571 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/_utils.py
+-rw-r--r--   0        0        0     7467 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/architectures.py
+-rw-r--r--   0        0        0     3321 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/deep/data.py
+-rw-r--r--   0        0        0     1062 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_dummy.py
+-rw-r--r--   0        0        0     3085 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gcca.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/__init__.py
+-rw-r--r--   0        0        0     7721 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_base.py
+-rw-r--r--   0        0        0     3556 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_ey.py
+-rw-r--r--   0        0        0     2015 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_gha.py
+-rw-r--r--   0        0        0     1481 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_objectives.py
+-rw-r--r--   0        0        0     1170 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_stochasticpls.py
+-rw-r--r--   0        0        0     2021 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_svd.py
+-rw-r--r--   0        0        0      154 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_gradient/_tracenorm.py
+-rw-r--r--   0        0        0     6686 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_grcca.py
+-rw-r--r--   0        0        0        0 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/__init__.py
+-rw-r--r--   0        0        0     8226 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_altmaxvar.py
+-rw-r--r--   0        0        0     5659 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_base.py
+-rw-r--r--   0        0        0     2135 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_deflation.py
+-rw-r--r--   0        0        0     8821 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_elastic.py
+-rw-r--r--   0        0        0     4130 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_incrementalpls.py
+-rw-r--r--   0        0        0     1655 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_pls_als.py
+-rw-r--r--   0        0        0     7276 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_admm.py
+-rw-r--r--   0        0        0     2250 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0        0        0     3765 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_span.py
+-rw-r--r--   0        0        0     3798 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_spls.py
+-rw-r--r--   0        0        0     3983 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_iterative/_swcca.py
+-rw-r--r--   0        0        0    14097 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_mcca.py
+-rw-r--r--   0        0        0     2959 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_partialcca.py
+-rw-r--r--   0        0        0     2303 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_pcacca.py
+-rw-r--r--   0        0        0     2507 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_pls.py
+-rw-r--r--   0        0        0      491 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_plsregression.py
+-rw-r--r--   0        0        0     4358 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_prcca.py
+-rw-r--r--   0        0        0     2681 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_search.py
+-rw-r--r--   0        0        0     5213 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/linear/_tcca.py
+-rw-r--r--   0        0        0      328 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0        0        0     3930 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/model_selection/_search.py
+-rw-r--r--   0        0        0    15820 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/model_selection/_validation.py
+-rw-r--r--   0        0        0      159 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/nonparametric/__init__.py
+-rw-r--r--   0        0        0    12996 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/nonparametric/_kcca.py
+-rw-r--r--   0        0        0     6418 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/nonparametric/_ncca.py
+-rw-r--r--   0        0        0     5775 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/nonparametric/_scca_hsic.py
+-rw-r--r--   0        0        0     1892 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/preprocessing/__init__.py
+-rw-r--r--   0        0        0      512 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0        0        0     7783 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/probabilistic/_cca.py
+-rw-r--r--   0        0        0     3534 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/probabilistic/_pls.py
+-rw-r--r--   0        0        0     7898 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/probabilistic/_plsregression.py
+-rw-r--r--   0        0        0     4888 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/probabilistic/_rcca.py
+-rw-r--r--   0        0        0     5050 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/sequential.py
+-rw-r--r--   0        0        0     1312 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0        0        0     3304 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/visualisation/correlation.py
+-rw-r--r--   0        0        0     3111 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/visualisation/covariance.py
+-rw-r--r--   0        0        0     5206 2024-04-19 10:57:24.889313 cca_zoo-2.6.0/cca_zoo/visualisation/explained_covariance.py
+-rw-r--r--   0        0        0     7085 2024-04-19 10:57:24.893313 cca_zoo-2.6.0/cca_zoo/visualisation/explained_variance.py
+-rw-r--r--   0        0        0     3627 2024-04-19 10:57:24.893313 cca_zoo-2.6.0/cca_zoo/visualisation/inference.py
+-rw-r--r--   0        0        0    13462 2024-04-19 10:57:24.893313 cca_zoo-2.6.0/cca_zoo/visualisation/representations.py
+-rw-r--r--   0        0        0     1680 2024-04-19 10:57:24.893313 cca_zoo-2.6.0/cca_zoo/visualisation/weights.py
+-rw-r--r--   0        0        0     1441 2024-04-19 10:57:24.973314 cca_zoo-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 cca_zoo-2.6.0/PKG-INFO
```

### Comparing `cca_zoo-2.5.0/LICENSE` & `cca_zoo-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/README.md` & `cca_zoo-2.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
 Note that `deep` requires `torch` and `lightning` which may be better installed separately following the [PyTorch installation guide](https://pytorch.org/get-started/locally/).
 
 `probabilistic` requires `numpyro` which may be better installed separately following the [NumPyro installation guide](https://num.pyro.ai/en/stable/getting_started.html#installation).
 
 `visualisation` requires `matplotlib` and `seaborn`
 
+## Plug into the Machine Learning Ecosystem
+
+CCA-Zoo is designed to be compatible with the machine learning ecosystem. It is built on top of `scikit-learn`, `tensorly`, `torch`, `pytorch-lightning`, and `numpyro`.
+
+<img src="docs/_static/CCA_Zoo_map.svg" alt="drawing" width="1000"/>
+
 ## 🏎️ Performance Highlights
 CCA-Zoo shines when it comes to high-dimensional data analysis. It significantly outperforms scikit-learn, particularly as dimensionality increases. For comprehensive benchmarks, see our [script](benchmark/cca_high_dimensions.py) and the graph below.
 
 ![Benchmark Plot CCA](benchmark/CCA_Speed_Benchmark.svg)
 ![Benchmark Plot PLS](benchmark/PLS_Speed_Benchmark.svg)
 
 ## 📚 Detailed Documentation
```

### Comparing `cca_zoo-2.5.0/cca_zoo/_utils/_checks.py` & `cca_zoo-2.6.0/cca_zoo/_utils/_checks.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/_utils/_cross_correlation.py` & `cca_zoo-2.6.0/cca_zoo/_utils/_cross_correlation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/_utils/_splitter.py` & `cca_zoo-2.6.0/cca_zoo/_utils/_splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-
 from sklearn.base import TransformerMixin
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
 
 from cca_zoo._utils._checks import check_Xs
```

### Comparing `cca_zoo-2.5.0/cca_zoo/datasets/simulated.py` & `cca_zoo-2.6.0/cca_zoo/datasets/simulated.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import itertools
 from abc import ABC, abstractmethod
 from typing import List, Union
 
 import numpy as np
 import scipy
 from scipy.sparse import block_diag
-from sklearn.datasets import make_spd_matrix
 from sklearn.utils.validation import check_random_state
 
 from cca_zoo._utils._checks import _process_parameter
 
 
 def cov_eigvals(X):
     S = np.linalg.svd(X, compute_uv=False) ** 2
@@ -27,73 +26,46 @@
     ):
         self.view_features = view_features
         self.latent_dimensions = latent_dimensions
         self.random_state = check_random_state(random_state)
         self.rank = min(view_features) if rank is None else rank
         self.density = density
 
-    def _generate_covariance_matrix(self, features: int, structure: str):
-        """
-        Generates a covariance matrix for a view based on the specified structure.
-
-        :param features: Number of features in the view.
-        :param structure: Structure type of the covariance matrix.
-        :return: A covariance matrix for the view.
-        """
-        if structure == "identity":
-            return np.eye(features)
-        else:
-            covariance_matrix = make_spd_matrix(
-                features, random_state=self.random_state
-            )
-            return self._scale_covariance_matrix(covariance_matrix)
-
-    @staticmethod
-    def _scale_covariance_matrix(covariance_matrix):
-        """
-        Scales a covariance matrix so that its diagonal elements are 1, effectively
-        converting it to a correlation matrix.
-
-        :param cov_matrix: A numpy array representing the covariance matrix.
-        :return: Scaled covariance matrix with 1s on the diagonal.
-        """
-        # Extract the standard deviations from the diagonal of the covariance matrix
-        std_devs = np.sqrt(np.diag(covariance_matrix))
-
-        # Scale the covariance matrix
-        scaled_cov_matrix = covariance_matrix / np.outer(std_devs, std_devs)
-
-        return scaled_cov_matrix
-
     def _covariance_factor(self, features, structure):
         """
         Generates a covariance factor matrix based on the specified structure. For a large number of
         features, it generates a sparse representation to reduce memory and computational demands.
 
         :param features: Number of features in the view.
         :param structure: Structure type of the covariance matrix.
         :return: A covariance factor matrix for the view.
         """
         if structure == "identity":
             factor = scipy.sparse.eye(features, features)
-            factor /= np.sqrt(features)
-            return factor
-        else:
+            factor /= features
+        elif structure == "correlated":
+            factor = scipy.sparse.csr_matrix(
+                self.random_state.uniform(-1, 1, size=(features, self.rank))
+            )
+            s = scipy.linalg.svdvals(factor.toarray())
+            factor /= s.sum()
+        elif structure == "random":
             factor = scipy.sparse.random(
                 features,
                 self.rank,
                 density=self.density,
                 random_state=self.random_state,
             )
             s = scipy.linalg.svdvals(factor.toarray())
-            factor /= np.sqrt(s.sum())
-            return factor
-
-    def covariance_matrices(self):
-        return [factor @ factor.T for factor in self.covariance_factors]
+            factor /= s.sum()
+        else:
+            raise ValueError(
+                "Invalid covariance structure. Must be one of 'identity', 'correlated', or 'random'."
+            )
+        return factor
 
     @abstractmethod
     def sample(self, n_samples: int):
         pass
 
 
 class LatentVariableData(_BaseData):
@@ -149,14 +121,51 @@
         ]
         self.covariance_factors = [
             self._covariance_factor(features, structure)
             for features, structure in zip(
                 self.view_features, self.covariance_structure
             )
         ]
+        self._true_features = None
+
+    @property
+    def true_features(self):
+        if self._true_features is None:
+            self._true_features = []
+            for loading, cov_factor in zip(self.true_loadings, self.covariance_factors):
+                if self.rank is None:
+                    self._true_features.append(loading)
+                else:
+                    cov = (
+                        loading @ loading.T
+                        + (cov_factor @ cov_factor.T).toarray()
+                        / self.signal_to_noise_ratio
+                    )
+                    inv_cov = np.linalg.inv(cov)
+                    self._true_features.append(inv_cov @ loading)
+
+                    # U_l, S_l, Vt_l = np.linalg.svd(loading, full_matrices=False)
+                    # U_c, S_c, Vt_c = np.linalg.svd(
+                    #     cov_factor.toarray(), full_matrices=False
+                    # )
+                    #
+                    # M = np.hstack((U_l, U_c))
+                    # V, R = np.linalg.qr(M)
+                    #
+                    # A_prime = (
+                    #     (V.T @ cov_factor.toarray())
+                    #     @ (cov_factor.toarray().T @ V)
+                    #     / self.signal_to_noise_ratio
+                    # )
+                    # B_prime = (V.T @ loading) @ (loading.T @ V)
+                    # C = A_prime + B_prime
+                    # inv_matrix = np.linalg.inv(C)
+                    # self._true_features.append(V @ (inv_matrix @ (V.T @ loading)))
+
+        return self._true_features
 
     def _generate_loading_matrix(
         self, features: int, sparsity: float, positivity: bool
     ):
         """
         Generates a loading matrix for a view based on the specified sparsity and positivity.
 
@@ -191,15 +200,14 @@
         :return: Generated views and optionally the latent variables.
         """
         latent_variables = self.random_state.multivariate_normal(
             np.zeros(self.latent_dimensions),
             np.eye(self.latent_dimensions),
             num_samples,
         )
-
         views = [
             latent_variables @ loading.T
             + self.random_state.standard_normal(
                 size=(num_samples, covariance_factor.shape[1])
             )
             @ covariance_factor.T
             / np.sqrt(self.signal_to_noise_ratio)
@@ -214,39 +222,28 @@
         Computes the joint covariance matrix for all views.
 
         :return: The joint covariance matrix.
         """
         joint_cov = np.zeros((sum(self.view_features), sum(self.view_features)))
         joint_cov[: self.view_features[0], : self.view_features[0]] = (
             self.true_loadings[0] @ self.true_loadings[0].T
-            + self.covariance_matrices[0]
+            + self.covariance_factors[0] @ self.covariance_factors[0].T
         )
         joint_cov[self.view_features[0] :, self.view_features[0] :] = (
             self.true_loadings[1] @ self.true_loadings[1].T
-            + self.covariance_matrices[1]
+            + self.covariance_factors[1] @ self.covariance_factors[1].T
         )
         joint_cov[: self.view_features[0], self.view_features[0] :] = (
             self.true_loadings[0] @ self.true_loadings[1].T
         )
         joint_cov[self.view_features[0] :, : self.view_features[0]] = (
             self.true_loadings[1] @ self.true_loadings[0].T
         )
         return joint_cov
 
-    def true_features(self):
-        """
-        Estimates the true features based on the loading matrices and covariance matrices.
-
-        :return: List of estimated true features for each view.
-        """
-        return [
-            np.linalg.inv(cov + loading.T @ loading) @ loading
-            for cov, loading in zip(self.covariance_matrices, self.true_loadings)
-        ]
-
 
 class JointData(_BaseData):
     """
     Class for generating simulated data for a linear model with multiple representations.
     """
 
     def __init__(
@@ -292,15 +289,16 @@
         self.true_loadings = [
             covariance_factor @ (covariance_factor.T @ weight)
             for weight, covariance_factor in zip(
                 self.true_features, self.covariance_factors
             )
         ]
         U, S, Vt = np.linalg.svd(
-            self._generate_joint_covariance(self.covariance_factors), full_matrices=True
+            self._generate_joint_covariance(self.covariance_factors),
+            full_matrices=False,
         )
         self.US = U * np.sqrt(S)
 
     def _generate_true_weight(
         self, view_features, sparsity_levels, is_positive, covariance_factor
     ):
         loadings = self.random_state.randn(view_features, self.latent_dimensions)
@@ -310,68 +308,56 @@
             1
         ] * sparsity_levels
         mask = np.stack([mask_elements] * loadings.shape[1]).T
         self.random_state.shuffle(mask)
         loadings *= mask
         if is_positive:
             loadings = np.abs(loadings)
-        loadings = self._decorrelate_weights(loadings, covariance_factor)
         return loadings / np.sqrt(
-            np.diag(loadings.T @ covariance_factor @ covariance_factor.T @ loadings)
+            np.diag((loadings.T @ covariance_factor) @ (covariance_factor.T @ loadings))
         )
 
     def _generate_joint_covariance(self, covariance_factors):
         """Generates a joint covariance matrix for all representations."""
         joint_covariance = block_diag(
             [
                 covariance_factor @ covariance_factor.T
                 for covariance_factor in covariance_factors
             ]
         ).toarray()
         split_points = np.concatenate(([0], np.cumsum(self.view_features)))
-
         for i, j in itertools.combinations(range(len(split_points) - 1), 2):
             cross_cov = self._compute_cross_covariance(covariance_factors, i, j)
             joint_covariance[
                 split_points[i] : split_points[i + 1],
                 split_points[j] : split_points[j + 1],
             ] = cross_cov
             joint_covariance[
                 split_points[j] : split_points[j + 1],
                 split_points[i] : split_points[i + 1],
             ] = cross_cov.T
         return joint_covariance
 
     def _compute_cross_covariance(self, cov_factors, i, j):
         """Computes the cross-covariance matrix for a pair of representations."""
-        cross_cov = np.zeros((self.view_features[i], self.view_features[j]))
+        cross_cov = scipy.zeros((self.view_features[i], self.view_features[j]))
 
         for _ in range(self.latent_dimensions):
-            outer_product = np.outer(
+            outer_product = scipy.outer(
                 self.true_features[i][:, _], self.true_features[j][:, _]
             )
             cross_cov += (
                 cov_factors[i]
                 @ cov_factors[i].T
                 @ (self.correlation[_] * outer_product)
                 @ cov_factors[j]
                 @ cov_factors[j].T
             )
 
         return cross_cov
 
-    @staticmethod
-    def _decorrelate_weights(weights, covariance_factor):
-        product = (weights.T @ covariance_factor) @ (covariance_factor.T @ weights)
-        for k in range(1, product.shape[0]):
-            weights[:, k:] -= np.outer(
-                weights[:, k - 1], product[k - 1, k:] / product[k - 1, k - 1]
-            )
-            product = (weights.T @ covariance_factor) @ (covariance_factor.T @ weights)
-        return weights
-
     def sample(self, n_samples: int):
         random_data = self.random_state.standard_normal(
             size=(n_samples, self.US.shape[0])
         )
         samples = random_data @ self.US.T
         return np.split(samples, np.cumsum(self.view_features)[:-1], axis=1)
```

### Comparing `cca_zoo-2.5.0/cca_zoo/datasets/toy.py` & `cca_zoo-2.6.0/cca_zoo/datasets/toy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/__init__.py` & `cca_zoo-2.6.0/cca_zoo/deep/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 """
 The :mod:`cca_zoo.deep` module includes a variety of deep CCA algorithms.
 """
+
 import importlib.util
 
 if (
     importlib.util.find_spec("torch") is None
     or importlib.util.find_spec("lightning") is None
 ):
     print(
         "Warning: torch or lightning are not installed. Some functionality in cca_zoo.deep may be limited."
     )
-from . import architectures, objectives
+from . import architectures
 from ._discriminative._dcca import DCCA
 from ._discriminative._barlow_twins import BarlowTwins
 from ._discriminative._dcca_ey import DCCA_EY
 from ._discriminative._dcca_gha import DCCA_GHA
 from ._discriminative._dcca_noi import DCCA_NOI
 from ._discriminative._dcca_sdl import DCCA_SDL
 from ._discriminative._dcca_svd import DCCA_SVD
+from ._discriminative._dmcca import DMCCA
 from ._discriminative._dgcca import DGCCA
 from ._discriminative._dtcca import DTCCA
 from ._discriminative._vicreg import VICReg
 from ._generative._dccae import DCCAE
 from ._generative._dvcca import DVCCA
-from ._generative._splitae import SplitAE
 
 __all__ = [
     "DCCA",
     "DCCA_GHA",
     "DCCA_SVD",
+    "DMCCA",
     "DGCCA",
     "DCCAE",
     "DCCA_NOI",
     "DCCA_SDL",
     "DVCCA",
     "BarlowTwins",
     "VICReg",
     "DTCCA",
     "DCCA_EY",
-    "SplitAE",
     "architectures",
     "objectives",
 ]
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_barlow_twins.py` & `cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_barlow_twins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import torch
 
 from ._dcca import DCCA
 
 
 class BarlowTwins(DCCA):
     """
@@ -20,40 +22,42 @@
     ----------
     Zbontar, Jure, et al. "Barlow twins: Self-supervised learning via redundancy reduction." arXiv preprint arXiv:2103.03230 (2021).
 
     """
 
     def __init__(
         self,
-        latent_dimensions: int,
-        encoders=None,
+        *args,
         lamb=5e-3,
         **kwargs,
     ):
-        super().__init__(
-            latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
-        )
+        super().__init__(*args, **kwargs)
         self.lamb = lamb  # the lambda parameter for the off-diagonal terms of the cross-covariance matrix
         self.bns = torch.nn.ModuleList(
             [
-                torch.nn.BatchNorm1d(latent_dimensions, affine=False)
+                torch.nn.BatchNorm1d(self.latent_dimensions, affine=False)
                 for _ in self.encoders
             ]
         )  # a list of batch normalization layers for each encoder
 
     def forward(self, views, **kwargs):
-        z = []
+        representations = []
         for i, (encoder, bn) in enumerate(zip(self.encoders, self.bns)):
-            z.append(bn(encoder(views[i])))  # encode and normalize each view
-        return z  # return a list of normalized latent representations
+            representations.append(
+                bn(encoder(views[i]))
+            )  # encode and normalize each view
+        return representations  # return a list of normalized latent representations
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"])  # get the latent representations
+    def loss(
+        self,
+        representations: List[torch.Tensor],
+        independent_representations: List[torch.Tensor] = None,
+    ):
         cross_cov = (
-            z[0].T @ z[1] / z[0].shape[0]
+            representations[0].T @ representations[1] / representations[0].shape[0]
         )  # compute the cross-covariance matrix between the two representations
         invariance = torch.sum(
             torch.pow(1 - torch.diag(cross_cov), 2)
         )  # compute the invariance term as the sum of squared differences from 1 on the diagonal
         covariance = torch.sum(
             torch.triu(torch.pow(cross_cov, 2), diagonal=1)
         ) + torch.sum(
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from typing import Optional
+from typing import Optional, List
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 
 from ._dcca import DCCA
+from .._utils import inv_sqrtm
 
 
 class BatchWhiten(Module):
     def __init__(
         self,
         num_features: int,
-        eps: float = 1e-5,
         momentum: float = 0.1,
         track_running_stats: bool = True,
         device=None,
         dtype=None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super(BatchWhiten, self).__init__()
 
         self.num_features = num_features
-        self.eps = eps
         self.momentum = momentum
         self.track_running_stats = track_running_stats
 
         if self.track_running_stats:
             self.register_buffer(
                 "running_covar", torch.eye(num_features, **factory_kwargs)
             )
@@ -97,73 +96,58 @@
                     running_covar.mul_(exponential_average_factor).add_(
                         covar, alpha=1 - exponential_average_factor
                     )
 
                 # Calculate whitened input
                 if running_covar is not None:
                     covar = running_covar
-                # Enforce positive definite by taking a torch max() with eps
-                covar = torch.max(covar, torch.tensor(self.eps, device=covar.device))
                 # Calculate inverse square-root matrix
-                B = inv_sqrtm(covar, self.eps)
+                B = inv_sqrtm(covar)
                 # Calculate whitened input
                 input = torch.matmul(input, B)
                 return input
         else:
             return input
 
 
-def inv_sqrtm(A, eps=1e-9):
-    """Compute the inverse square-root of a positive definite matrix."""
-    # Perform eigendecomposition of covariance matrix
-    U, S, V = torch.svd(A)
-    # Enforce positive definite by taking a torch max() with eps
-    S = torch.max(S, torch.tensor(eps, device=S.device))
-    # Calculate inverse square-root
-    inv_sqrt_S = torch.diag_embed(torch.pow(S, -0.5))
-    # Calculate inverse square-root matrix
-    B = torch.matmul(torch.matmul(U, inv_sqrt_S), V.transpose(-1, -2))
-    return B
-
-
 class DCCA_NOI(DCCA):
     """
     A class used to fit a DCCA model by non-linear orthogonal iterations
 
 
     References
     ----------
     Wang, Weiran, et al. "Stochastic optimization for deep CCA via nonlinear orthogonal iterations." 2015 53rd Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2015.
 
     """
 
     def __init__(
         self,
-        latent_dimensions: int,
-        encoders=None,
-        r: float = 0,
+        *args,
         rho: float = 0.1,
-        eps: float = 1e-9,
         **kwargs,
     ):
         super().__init__(
-            latent_dimensions=latent_dimensions,
-            encoders=encoders,
-            r=r,
-            eps=eps,
+            *args,
             **kwargs,
         )
         if rho < 0 or rho > 1:
             raise ValueError(f"rho should be between 0 and 1. rho={rho}")
-        self.eps = eps
         self.rho = rho
         self.mse = torch.nn.MSELoss(reduction="sum")
         # Replace BatchNorm1d with BatchWhiten
         self.bws = torch.nn.ModuleList(
-            [BatchWhiten(latent_dimensions, momentum=rho) for _ in self.encoders]
+            [BatchWhiten(self.latent_dimensions, momentum=rho) for _ in self.encoders]
         )
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"])
-        z_w = [bw(z_) for z_, bw in zip(z, self.bws)]
-        loss = self.mse(z[0], z_w[1].detach()) + self.mse(z[1], z_w[0].detach())
+    def loss(
+        self,
+        representations: List[torch.Tensor],
+        independent_representations: List[torch.Tensor] = None,
+    ) -> torch.Tensor:
+        representations_w = [
+            bw(representation) for representation, bw in zip(representations, self.bws)
+        ]
+        loss = self.mse(representations[0], representations_w[1].detach()) + self.mse(
+            representations[1], representations_w[0].detach()
+        )
         return {"objective": loss}
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from typing import List
+
 import torch
 import torch.nn.functional as F
 
 from ._dcca import DCCA
 
 
 def sdl_loss(view):
-    """Calculate SDL loss."""
+    """Calculate SDL minibatch_loss."""
     cov = torch.cov(view.T)
     sgn = torch.sign(cov)
     sgn.fill_diagonal_(0)
     return torch.mean(cov * sgn)
 
 
 class DCCA_SDL(DCCA):
@@ -18,54 +20,36 @@
 
     References
     ----------
     Chang, Xiaobin, Tao Xiang, and Timothy M. Hospedales. "Scalable and effective deep _CCALoss via soft decorrelation." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018.
 
     """
 
-    def __init__(
-        self,
-        latent_dimensions: int,
-        encoders=None,
-        r: float = 0,
-        eps: float = 1e-5,
-        shared_target: bool = False,
-        lam=0.5,
-        **kwargs
-    ):
-        super().__init__(
-            latent_dimensions=latent_dimensions,
-            encoders=encoders,
-            r=r,
-            eps=eps,
-            shared_target=shared_target,
-            **kwargs
-        )
-        self.c = None
+    def __init__(self, *args, lam=0.5, **kwargs):
+        super().__init__(*args, **kwargs)
         self.lam = lam
         self.bns = torch.nn.ModuleList(
             [
-                torch.nn.BatchNorm1d(latent_dimensions, affine=False)
+                torch.nn.BatchNorm1d(self.latent_dimensions, affine=False)
                 for _ in self.encoders
             ]
         )
 
     def forward(self, views, **kwargs):
-        z = []
+        representations = []
         for i, (encoder, bn) in enumerate(zip(self.encoders, self.bns)):
-            z.append(bn(encoder(views[i])))
-        return z
+            representations.append(bn(encoder(views[i])))
+        return representations
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"])
-        l2_loss = F.mse_loss(z[0], z[1])
-        SDL_loss = torch.sum(torch.stack([sdl_loss(z_) for z_ in z]))
+    def loss(
+        self,
+        representations: List[torch.Tensor],
+        independent_representations: List[torch.Tensor] = None,
+    ):
+        l2_loss = F.mse_loss(representations[0], representations[1])
+        SDL_loss = torch.sum(
+            torch.stack(
+                [sdl_loss(representation) for representation in representations]
+            )
+        )
         loss = l2_loss + self.lam * SDL_loss
         return {"objective": loss, "l2": l2_loss, "sdl": SDL_loss}
-
-    def _sdl_loss(self, covs):
-        loss = 0
-        for cov in covs:
-            sgn = torch.sign(cov)
-            sgn.fill_diagonal_(0)
-            loss += torch.mean(cov * sgn)
-        return loss
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_discriminative/_vicreg.py` & `cca_zoo-2.6.0/cca_zoo/deep/_discriminative/_vicreg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import torch
 import torch.nn.functional as F
 
 from ._dcca import DCCA
 
 
 class VICReg(DCCA):
@@ -11,54 +13,54 @@
     VICReg is a self-supervised learning method that applies redundancy-reduction
     to learn representations that are invariant to distortions of the input sample.
 
     Parameters
     ----------
 
     sim_loss_weight : float, optional
-        weight of the similarity loss. Defaults to 25.0.
+        weight of the similarity minibatch_loss. Defaults to 25.0.
     var_loss_weight : float, optional
-        weight of the variance loss. Defaults to 25.0.
+        weight of the variance minibatch_loss. Defaults to 25.0.
     cov_loss_weight : float, optional
-        weight of the covariance loss. Defaults to 1.0.
+        weight of the covariance minibatch_loss. Defaults to 1.0.
 
     References
     ----------
     .. [1] Bardes, A., Ponce, J. and LeCun, Y., 2021. Vicreg: Variance-invariance-covariance regularization for self-supervised learning. arXiv preprint arXiv:2105.04906.
 
     """
 
     def __init__(
         self,
-        latent_dimensions: int,
-        encoders=None,
+        *args,
         sim_loss_weight: float = 25.0,
         var_loss_weight: float = 25.0,
         cov_loss_weight: float = 1.0,
         **kwargs,
     ):
-        super().__init__(
-            latent_dimensions=latent_dimensions, encoders=encoders, **kwargs
-        )
+        super().__init__(*args, **kwargs)
         self.sim_loss_weight = sim_loss_weight
         self.var_loss_weight = var_loss_weight
         self.cov_loss_weight = cov_loss_weight
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"])  # get the latent representations
-        sim_loss = invariance_loss(*z)
-        var_loss = variance_loss(*z)
-        cov_loss = covariance_loss(*z)
+    def loss(
+        self,
+        representations: List[torch.Tensor],
+        independent_representations: List[torch.Tensor] = None,
+    ):
+        sim_loss = invariance_loss(*representations)
+        var_loss = variance_loss(*representations)
+        cov_loss = covariance_loss(*representations)
         loss = (
             self.sim_loss_weight * sim_loss
             + self.var_loss_weight * var_loss
             + self.cov_loss_weight * cov_loss
         )
         return {
-            "objective": loss,  # return the loss
+            "objective": loss,  # return the minibatch_loss
             "sim_loss": sim_loss,
             "var_loss": var_loss,
             "cov_loss": cov_loss,
         }
 
 
 # Copyright 2023 solo-learn development team.
@@ -78,57 +80,57 @@
 # PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE
 # FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
 # OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 # DEALINGS IN THE SOFTWARE.
 
 
 def invariance_loss(z1: torch.Tensor, z2: torch.Tensor) -> torch.Tensor:
-    """Computes mse loss given batch of projected features z1 from view 1 and
+    """Computes mse minibatch_loss given batch of projected features z1 from view 1 and
     projected features z2 from view 2.
 
     Args:
         z1 (torch.Tensor): NxD Tensor containing projected features from view 1.
         z2 (torch.Tensor): NxD Tensor containing projected features from view 2.
 
     Returns:
-        torch.Tensor: invariance loss (mean squared error).
+        torch.Tensor: invariance minibatch_loss (mean squared error).
     """
 
     return F.mse_loss(z1, z2)
 
 
 def variance_loss(z1: torch.Tensor, z2: torch.Tensor) -> torch.Tensor:
-    """Computes variance loss given batch of projected features z1 from view 1 and
+    """Computes variance minibatch_loss given batch of projected features z1 from view 1 and
     projected features z2 from view 2.
 
     Args:
         z1 (torch.Tensor): NxD Tensor containing projected features from view 1.
         z2 (torch.Tensor): NxD Tensor containing projected features from view 2.
 
     Returns:
-        torch.Tensor: variance regularization loss.
+        torch.Tensor: variance regularization minibatch_loss.
     """
 
     eps = 1e-4
     std_z1 = torch.sqrt(z1.var(dim=0) + eps)
     std_z2 = torch.sqrt(z2.var(dim=0) + eps)
     std_loss = torch.mean(F.relu(1 - std_z1)) + torch.mean(F.relu(1 - std_z2))
     return std_loss
 
 
 def covariance_loss(z1: torch.Tensor, z2: torch.Tensor) -> torch.Tensor:
-    """Computes covariance loss given batch of projected features z1 from view 1 and
+    """Computes covariance minibatch_loss given batch of projected features z1 from view 1 and
     projected features z2 from view 2.
 
     Args:
         z1 (torch.Tensor): NxD Tensor containing projected features from view 1.
         z2 (torch.Tensor): NxD Tensor containing projected features from view 2.
 
     Returns:
-        torch.Tensor: covariance regularization loss.
+        torch.Tensor: covariance regularization minibatch_loss.
     """
 
     N, D = z1.size()
 
     z1 = z1 - z1.mean(dim=0)
     z2 = z2 - z2.mean(dim=0)
     cov_z1 = (z1.T @ z1) / (N - 1)
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.6.0/cca_zoo/deep/_generative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.6.0/cca_zoo/deep/_generative/_dccae.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,44 @@
+from typing import List
+
 import torch
 
-from .. import objectives
-from .._discriminative._dcca import DCCA
-from .._generative._base import _GenerativeMixin
+from . import _GenerativeMixin
+from .. import DMCCA
 
 
-class DCCAE(DCCA, _GenerativeMixin):
+class DCCAE(DMCCA, _GenerativeMixin):
     """
     A class used to fit a DCCAE model.
 
     References
     ----------
     Wang, Weiran, et al. "On deep multi-view representation learning." International conference on machine learning. PMLR, 2015.
 
     """
 
     def __init__(
         self,
-        latent_dimensions: int,
-        objective=objectives._MCCALoss,
-        encoders=None,
+        *args,
         decoders=None,
-        eps: float = 1e-5,
         lam=0.5,
         latent_dropout=0,
         img_dim=None,
         recon_loss_type="mse",
         **kwargs,
     ):
         super().__init__(
-            latent_dimensions=latent_dimensions,
-            objective=objective,
-            encoders=encoders,
-            eps=eps,
+            *args,
             **kwargs,
         )
         self.img_dim = img_dim
         self.decoders = torch.nn.ModuleList(decoders)
         if lam < 0 or lam > 1:
             raise ValueError(f"lam should be between 0 and 1. rho={lam}")
         self.lam = lam
-        self.objective = objective(eps=eps)
         self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
         self.recon_loss_type = recon_loss_type
 
     def forward(self, views, **kwargs):
         """
         Forward method for the model. Outputs latent encoding for each view
 
@@ -53,32 +47,36 @@
         :return:
         """
         z = []
         for i, encoder in enumerate(self.encoders):
             z.append(encoder(views[i]))
         return z
 
-    def _decode(self, z, **kwargs):
+    def _decode(self, representations, **kwargs):
         """
         This method is used to decode from the latent space to the best prediction of the original representations
 
         """
         recon = []
         for i, decoder in enumerate(self.decoders):
-            recon.append(decoder(self.latent_dropout(z[i])))
+            recon.append(decoder(self.latent_dropout(representations[i])))
         return recon
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"])
-        recons = self._decode(z)
-        loss = dict()
+    def minibatch_loss(self, batch, **kwargs):
+        # Encoding the representations with the forward method
+        representations = self(batch["views"])
+        if batch.get("independent_views") is None:
+            independent_representations = None
+        else:
+            independent_representations = self(batch["independent_views"])
+        recons = self._decode(representations)
+        loss = DMCCA.loss(self, representations, independent_representations)
         loss["reconstruction"] = torch.stack(
             [
                 self.recon_loss(x, recon, loss_type=self.recon_loss_type)
                 for x, recon in zip(batch["views"], recons)
             ]
         ).sum()
-        loss["correlation"] = self.objective(z)
         loss["objective"] = (
-            self.lam * loss["reconstruction"] + (1 - self.lam) * loss["correlation"]
+            self.lam * loss["reconstruction"] + (1 - self.lam) * loss["objective"]
         )
         return loss
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.6.0/cca_zoo/deep/_generative/_dvcca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 from typing import Iterable
 
 import torch
 
+from . import _GenerativeMixin
 from .._base import BaseDeep
-from .._generative._base import _GenerativeMixin
 
 
 class DVCCA(BaseDeep, _GenerativeMixin):
     """
     A class used to fit a DVCCA model.
 
     References
     ----------
-    Wang, Weiran, et al. 'Deep variational canonical correlation analysis.' arXiv preprint arXiv:1610.03454 (2016).
+    Wang, Weiran, et al. 'Deep variational canonical correlation analysis.' arXiv
+    preprint arXiv:1610.03454 (2016).
     https: // arxiv.org / pdf / 1610.03454.pdf
     https: // github.com / pytorch / examples / blob / master / vae / main.py
 
     """
 
     def __init__(
         self,
-        latent_dimensions: int,
-        encoders=None,
+        *args,
         decoders=None,
         private_encoders: Iterable = None,
         latent_dropout=0,
         img_dim=None,
         recon_loss_type="mse",
         **kwargs,
     ):
-        super().__init__(latent_dimensions=latent_dimensions, **kwargs)
+        super().__init__(*args, **kwargs)
         self.img_dim = img_dim
         self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
-        self.encoders = torch.nn.ModuleList(encoders)
         self.decoders = torch.nn.ModuleList(decoders)
         if private_encoders:
             self.private_encoders = torch.nn.ModuleList(private_encoders)
         else:
             self.private_encoders = None
         self.recon_loss_type = recon_loss_type
 
@@ -61,15 +60,16 @@
         return z
 
     def _sample(self, mu, logvar, mle):
         """
 
         :param mu:
         :param logvar:
-        :param mle: whether to return the maximum likelihood (i.e. mean) or whether to sample
+        :param mle: whether to return the maximum likelihood (i.e. mean) or whether
+        to sample
         :return: a sample from latent vector
         """
         if mle:
             return mu
         else:
             return mu + torch.randn_like(logvar) * torch.exp(0.5 * logvar)
 
@@ -109,51 +109,61 @@
                     )
                 )
             else:
                 x_i = decoder(self.latent_dropout(z["shared"]))
             x.append(x_i)
         return x
 
-    def loss(self, batch, **kwargs):
-        z = self(batch["views"], mle=False)
-        recons = self._decode(z)
+    def minibatch_loss(self, batch, **kwargs):
+        representations = self(batch["views"], mle=False)
+        recons = self._decode(representations)
         loss = dict()
         loss["reconstruction"] = torch.stack(
             [
                 self.recon_loss(x, recon, loss_type=self.recon_loss_type)
                 for x, recon in zip(batch["views"], recons)
             ]
         ).sum()
         loss["kl shared"] = (
-            self.kl_loss(z["mu_shared"], z["logvar_shared"]) / batch["views"][0].numel()
+            self.kl_loss(representations["mu_shared"], representations["logvar_shared"])
+            / batch["views"][0].numel()
         )
-        if "private" in z:
+        if "private" in representations:
             loss["kl private"] = torch.stack(
                 [
                     self.kl_loss(mu_, logvar_) / batch["views"][0].numel()
-                    for mu_, logvar_ in zip(z["mu_private"], z["logvar_private"])
+                    for mu_, logvar_ in zip(
+                        representations["mu_private"], representations["logvar_private"]
+                    )
                 ]
             ).sum()
         loss["objective"] = torch.stack(tuple(loss.values())).sum()
         return loss
 
+    @torch.no_grad()
     def transform(
         self,
         loader: torch.utils.data.DataLoader,
     ):
-        """
-        :param loader: a dataloader that matches the structure of that used for training
-        :return: transformed representations
-        """
-        with torch.no_grad():
-            z_shared = []
-            z_private = []
-            for batch_idx, batch in enumerate(loader):
-                views = [view.to(self.device) for view in batch["views"]]
-                z_ = self(views)
-                z_shared.append(z_["shared"].cpu())
-                if "private" in z_:
-                    z_private.append(self.detach_all(z_["private"]))
-        z = {"shared": torch.vstack(z_shared).cpu().numpy()}
-        if "private" in z_:
-            z["private"] = [torch.vstack(i).cpu().numpy() for i in zip(*z_private)]
-        return z
+        self.eval()  # Ensure the model is in evaluation mode
+        representations_shared = []
+        representations_private = []
+        for batch_idx, batch in enumerate(loader):
+            views = [view.to(self.device) for view in batch["views"]]
+            representations = self(views)
+            representations_shared.append(representations["shared"].cpu().detach())
+            if "private" in representations:
+                representations_private.append(
+                    [
+                        representation.cpu().detach()
+                        for representation in representations["private"]
+                    ]
+                )
+        representations_shared = {
+            "shared": torch.vstack(representations_shared).numpy()
+        }
+        if representations_private:
+            representations_private = [
+                torch.vstack(representation).numpy()
+                for representation in representations_private
+            ]
+        return representations_shared, representations_private
```

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/architectures.py` & `cca_zoo-2.6.0/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/deep/data.py` & `cca_zoo-2.6.0/cca_zoo/deep/data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/__init__.py` & `cca_zoo-2.6.0/cca_zoo/linear/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 The :mod:`cca_zoo.linear` module includes a variety of linear CCA algorithms.
 """
+
 from ._gcca import GCCA
-from ._grcca import GRCCA
-from ._mcca import CCA, MCCA, rCCA
-from ._partialcca import PartialCCA
-from ._pcacca import PCACCA
-from ._pls import MPLS, PLS
-from ._prcca import PRCCA
-from ._tcca import TCCA
 from ._gradient._ey import CCA_EY, PLS_EY
 from ._gradient._gha import CCA_GHA
-from ._gradient._svd import CCA_SVD
 from ._gradient._stochasticpls import PLSStochasticPower
+from ._gradient._svd import CCA_SVD
+from ._grcca import GRCCA
 from ._iterative._elastic import SCCA_IPLS, ElasticCCA
 from ._iterative._pls_als import PLS_ALS
 from ._iterative._scca_parkhomenko import SCCA_Parkhomenko
 from ._iterative._scca_span import SCCA_Span
 from ._iterative._spls import SPLS
+from ._mcca import CCA, MCCA, rCCA
+from ._partialcca import PartialCCA
+from ._pcacca import PCACCA
+from ._pls import MPLS, PLS
+from ._prcca import PRCCA
+from ._tcca import TCCA
 
 __all__ = [
     "MCCA",
     "CCA",
     "rCCA",
     "PLS",
     "MPLS",
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_dummy.py` & `cca_zoo-2.6.0/cca_zoo/linear/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def fit(self, views: Iterable[np.ndarray], y=None, K=None, **kwargs):
         return super().fit(views, y=y, K=K, **kwargs)
 
     def _check_params(self):
         self.c = _process_parameter("c", self.c, 0, self.n_views_)
 
-    def _C(self, views, K=None):
+    def _A(self, views, K=None):
         if K is None:
             # just use identity when all rows are observed in all representations.
             K = np.ones((len(views), views[0].shape[0]))
         Q = []
         self.view_weights = _process_parameter(
             "view_weights", self.view_weights, 1, self.n_views_
         )
@@ -83,15 +83,15 @@
         Q = (
             np.diag(np.sqrt(np.sum(K, axis=0)))
             @ Q
             @ np.diag(np.sqrt(np.sum(K, axis=0)))
         )
         return Q
 
-    def _D(self, views, **kwargs):
+    def _B(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
         self.weights_ = [
             np.linalg.pinv(view) @ eigvecs[:, : self.latent_dimensions]
             for view in views
         ]
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_base.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Iterable, List, Union, Optional
 
 import numpy as np
+
 from cca_zoo._base import _BaseModel
 from cca_zoo.linear._iterative._base import _default_initializer
 from cca_zoo.linear._mcca import MCCA
 
 DEFAULT_OPTIMIZER_KWARGS = dict(optimizer="SGD", nesterov=True, momentum=0.9)
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_ey.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_ey.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,53 @@
+from typing import List, Optional
+
+import numpy as np
+
 from cca_zoo._utils._cross_correlation import cross_cov
 from cca_zoo.linear._gradient._base import BaseGradientModel
-from cca_zoo.linear._gradient._objectives import CCA_AB, PLS_AB
-import numpy as np
-from typing import List, Optional
+from cca_zoo.linear._gradient._objectives import CCA_CV, PLS_AB
 
 
 class CCA_EY(BaseGradientModel):
     def loss(
         self,
         representations: List[np.ndarray],
         independent_representations: Optional[List[np.ndarray]] = None,
     ):
-        A, B = CCA_AB(representations)
+        A, B = CCA_CV(representations)
         rewards = np.trace(2 * A)
         if independent_representations is None:
             penalties = np.trace(B @ B)
         else:
-            independent_A, independent_B = CCA_AB(independent_representations)
+            independent_A, independent_B = CCA_CV(independent_representations)
             penalties = np.trace(B @ independent_B)
         return {
             "objective": -rewards + penalties,
             "rewards": rewards,
             "penalties": penalties,
         }
 
     def derivative(
         self,
         views: List[np.ndarray],
         representations: List[np.ndarray],
         independent_views: Optional[List[np.ndarray]] = None,
         independent_representations: Optional[List[np.ndarray]] = None,
     ):
-        A, B = CCA_AB(representations)
+        A, B = CCA_CV(representations)
         sum_representations = np.sum(np.stack(representations), axis=0)
         n = sum_representations.shape[0]
         rewards = [2 * view.T @ sum_representations / (n - 1) for view in views]
         if independent_representations is None:
             penalties = [
                 2 * view.T @ representation @ B / (n - 1)
                 for view, representation in zip(views, representations)
             ]
         else:
-            _, independent_B = CCA_AB(independent_representations)
+            _, independent_B = CCA_CV(independent_representations)
             penalties = [
                 view.T @ representation @ B / (n - 1)
                 + independent_view.T
                 @ independent_representation
                 @ independent_B
                 / (n - 1)
                 for view, representation, independent_view, independent_representation in zip(
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_gha.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_gha.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import List, Optional
 
 import numpy as np
 
 from cca_zoo.linear._gradient._ey import CCA_EY
-from cca_zoo.linear._gradient._objectives import CCA_AB
+from cca_zoo.linear._gradient._objectives import CCA_CV
 
 
 class CCA_GHA(CCA_EY):
     def loss(
         self,
         representations: List[np.ndarray],
         independent_representations: Optional[List[np.ndarray]] = None,
     ):
-        A, B = CCA_AB(representations)
+        A, B = CCA_CV(representations)
         rewards = np.trace(A)
         if independent_representations is None:
             rewards += np.trace(A)
             penalties = np.trace(A @ B)
         else:
-            independent_A, independent_B = CCA_AB(independent_representations)
+            independent_A, independent_B = CCA_CV(independent_representations)
             rewards += np.trace(independent_A)
             penalties = np.trace(independent_A @ B)
         return {
             "objective": -rewards + penalties,
             "rewards": rewards,
             "penalties": penalties,
         }
@@ -30,24 +30,24 @@
     def derivative(
         self,
         views: List[np.ndarray],
         representations: List[np.ndarray],
         independent_views: Optional[List[np.ndarray]] = None,
         independent_representations: Optional[List[np.ndarray]] = None,
     ):
-        A, B = CCA_AB(representations)
+        A, B = CCA_CV(representations)
         sum_representations = np.sum(np.stack(representations), axis=0)
         n = sum_representations.shape[0]
         if independent_representations is None:
             rewards = [2 * view.T @ sum_representations / (n - 1) for view in views]
             penalties = [
                 2 * view.T @ representation @ A / (n - 1)
                 for view, representation in zip(views, representations)
             ]
         else:
-            independent_A, independent_B = CCA_AB(independent_representations)
+            independent_A, independent_B = CCA_CV(independent_representations)
             rewards = [2 * view.T @ sum_representations / (n - 1) for view in views]
             penalties = [
                 2 * view.T @ representation @ independent_A / (n - 1)
                 for view, representation in zip(views, representations)
             ]
         return [2 * (-reward + penalty) for reward, penalty in zip(rewards, penalties)]
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_objectives.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_objectives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import List
+
 import numpy as np
 
 from cca_zoo._utils._cross_correlation import cross_cov
 
 
-def CCA_AB(representations: List[np.ndarray]):
+def CCA_CV(representations: List[np.ndarray]):
     latent_dimensions = representations[0].shape[1]
-    A = np.zeros(
+    C = np.zeros(
         (latent_dimensions, latent_dimensions)
     )  # initialize the cross-covariance matrix
-    B = np.zeros(
+    V = np.zeros(
         (latent_dimensions, latent_dimensions)
     )  # initialize the auto-covariance matrix
     for i, zi in enumerate(representations):
-        B += np.cov(zi.T)  # In-place addition
+        V += np.cov(zi.T)  # In-place addition
         for j, zj in enumerate(representations):
-            A += cross_cov(zi, zj, rowvar=False)  # In-place addition
+            C += cross_cov(zi, zj, rowvar=False)  # In-place addition
 
-    A /= len(representations)  # In-place division
-    B /= len(representations)  # In-place division
-    return A, B
+    C /= len(representations)  # In-place division
+    V /= len(representations)  # In-place division
+    return C, V
 
 
 def PLS_AB(representations: List[np.ndarray], weights: List[np.ndarray]):
     latent_dimensions = representations[0].shape[1]
     A = np.zeros(
         (latent_dimensions, latent_dimensions)
     )  # initialize the cross-covariance matrix
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_stochasticpls.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_stochasticpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_gradient/_svd.py` & `cca_zoo-2.6.0/cca_zoo/linear/_gradient/_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_grcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_altmaxvar.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_altmaxvar.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 #                     [
 #                         np.max(np.abs(old_weights[i] - self.weights_[i]))
 #                         / np.max(np.abs(self.weights_[i]))
 #                         for i in range(len(self.weights_))
 #                     ]
 #                 )
 #             )
-#             return {"loss": torch.tensor(objective), "weights_change": weights_change}
+#             return {"minibatch_loss": torch.tensor(objective), "weights_change": weights_change}
 #
 #
 # from pyproximal import (
 #     L0,
 #     L1,
 #     L2,
 #     L21,
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_base.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             copy_data=copy_data,
             random_state=random_state,
             accept_sparse=accept_sparse,
         )
         self.tol = tol
         self.epochs = epochs
         # validate the initialization method
-        if initialization not in ["random", "uniform", "unregularized", "pls"]:
+        if initialization not in ["random", "uniform", "unregularized", "pls", "cca"]:
             raise ValueError(
-                "Initialization method must be one of ['random', 'uniform', 'unregularized', 'pls']"
+                "Initialization method must be one of ['random', 'uniform', 'unregularized', 'pls', 'cca']"
             )
         else:
             self.initialization = initialization
         # validate the callbacks
         self.verbose = verbose
         # validate the convergence checking
         self.early_stopping = early_stopping
@@ -147,14 +147,15 @@
         ),
         "unregularized": (MPLS if pls else MCCA)(
             latent_dims, random_state=random_state
         ),
         "pls": MPLS(
             latent_dims, random_state=random_state
         ),  # Assuming PLS initialization can be used for both pls=True/False
+        "cca": MCCA(latent_dims, random_state=random_state),
     }
 
     initializer = initializer_map.get(initialization)
 
     if not initializer:
         raise ValueError(
             f"Initialization {initialization} not supported. Pass a generator implementing this method"
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_deflation.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_deflation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_elastic.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_elastic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_incrementalpls.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_pls_als.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_pls_als.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_admm.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_parkhomenko.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_scca_span.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_scca_span.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_spls.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_spls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_iterative/_swcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_mcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_mcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,17 @@
 from cca_zoo._base import _BaseModel
 from cca_zoo._utils._checks import _process_parameter
 from cca_zoo._utils._cross_correlation import cross_cov
 
 
 class MCCA(_BaseModel):
     r"""
-    A class used to fit a Regularised CCA (canonical ridge) model. This model adds a regularization term to the CCA objective function to avoid overfitting and improve stability. It uses PCA to perform the optimization efficiently for high dimensional data.
-
-    The objective function of regularised CCA is:
-
-    .. math::
-
-        w_{opt}=\underset{w}{\mathrm{argmax}}\{ w_1^TX_1^TX_2w_2  \}\\
-
-        \text{subject to:}
-
-        (1-c_1)w_1^TX_1^TX_1w_1+c_1w_1^Tw_1=n
-
-        (1-c_2)w_2^TX_2^TX_2w_2+c_2w_2^Tw_2=n
+    A class used to fit a Multiview Ridge CCA model.
+    This model adds a regularization term to the MCCA objective function to avoid overfitting and improve stability.
+    It uses PCA to perform the optimization efficiently for high dimensional data.
 
     where :math:`c_i` are the regularization parameters for each view.
 
     Parameters
     ----------
     latent_dimensions : int, optional
         Number of latent dimensions to use, by default 1
@@ -47,15 +37,15 @@
     >>> X1 = rng.random((10,5))
     >>> X2 = rng.random((10,5))
     >>> model = MCCA()
     >>> model.fit((X1,X2)).score((X1,X2))
 
     References
     --------
-    Vinod, Hrishikesh _D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
+    Vinod, Hrishikesh _B. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
     """
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state=None,
@@ -88,44 +78,41 @@
         views = self._validate_data(views)
         # Check the parameters
         self._check_params()
         views = self._process_data(views, **kwargs)
         eigvals, eigvecs = self._solve_gevp(views, y=y, **kwargs)
         # Compute the weights_ for each view
         self._weights(eigvals, eigvecs, views, **kwargs)
-        # delete pca to save memory
-        if self.pca:
-            del self.pca_models
         return self
 
     def _process_data(self, views, **kwargs):
         if self.pca:
             views = self._apply_pca(views)
         return views
 
     def _solve_gevp(self, views: Iterable[np.ndarray], y=None, **kwargs):
         # Setup the eigenvalue problem
-        C = self._C(views, **kwargs)
-        D = self._D(views, **kwargs)
+        A = self._A(views, **kwargs)
+        B = self._B(views, **kwargs)
         self.splits = np.cumsum([view.shape[1] for view in views])
         # Solve the eigenvalue problem
-        # Get the dimension of _C
-        p = C.shape[0]
+        # Get the dimension of _A
+        p = A.shape[0]
         # Solve the generalized eigenvalue problem Cx=lambda Dx using a subset of eigenvalues and eigenvectors
         [eigvals, eigvecs] = eigh(
-            C,
-            D,
+            A,
+            B,
             subset_by_index=[p - self.latent_dimensions, p - 1],
         )
         # Sort the eigenvalues and eigenvectors in descending order
         idx = np.argsort(eigvals, axis=0)[::-1]
         if eigvals.shape[0] < self.latent_dimensions:
             [eigvals, eigvecs] = eigh(
-                C,
-                D,
+                A,
+                B,
             )
             # Sort the eigenvalues and eigenvectors in descending order
             idx = np.argsort(eigvals, axis=0)[::-1][: self.latent_dimensions]
         eigvecs = eigvecs[:, idx].real
         eigvals = eigvals[idx].real
         return eigvals, eigvecs
 
@@ -134,49 +121,88 @@
         self.weights_ = np.split(eigvecs, self.splits[:-1], axis=0)
         if self.pca:
             # go from weights_ in PCA space to weights_ in original space
             self.weights_ = [
                 pca.components_.T @ self.weights_[i]
                 for i, pca in enumerate(self.pca_models)
             ]
+            del self.pca_models
 
     def _apply_pca(self, views):
         """
         Do data driven PCA on each view
         """
         self.pca_models = [PCA() for _ in views]
         # Fit PCA on each view
         return [self.pca_models[i].fit_transform(view) for i, view in enumerate(views)]
 
-    def _C(self, views, **kwargs):
+    def _A(self, views, **kwargs):
+        """
+        Constructs the matrix A for the generalized eigenvalue problem in MCCA.
+
+        Matrix A represents the between-view covariance matrix, capturing the
+        covariance among all different views. It is calculated as the covariance
+        matrix of the stacked views, from which the within-view covariance matrices
+        are subtracted.
+
+        Parameters
+        ----------
+        views : list of numpy.ndarray
+            The input views, where each view is a numpy array.
+
+        Returns
+        -------
+        numpy.ndarray
+            The matrix A, representing the between-view covariance matrix.
+        """
         all_views = np.hstack(views)
-        C = np.cov(all_views, rowvar=False)
-        C -= block_diag(*[np.cov(view, rowvar=False) for view in views])
-        return C / len(views)
+        A = np.cov(all_views, rowvar=False)
+        A -= block_diag(*[np.cov(view, rowvar=False) for view in views])
+        return A / len(views)
 
-    def _D(self, views, **kwargs):
+    def _B(self, views, **kwargs):
+        """
+        Constructs the matrix B for the generalized eigenvalue problem in MCCA.
+
+        Matrix B represents the within-view covariance matrix with regularization.
+        In the PCA case, it is constructed using the explained variance of each view
+        with regularization terms added to the diagonal. Without PCA, it is the
+        block diagonal matrix of each view's covariance matrix adjusted by the
+        regularization parameter.
+
+        The regularization improves numerical stability and controls overfitting.
+
+        Parameters
+        ----------
+        views : list of numpy.ndarray
+            The input views, where each view is a numpy array.
+
+        Returns
+        -------
+        numpy.ndarray
+            The matrix B, representing the regularized within-view covariance matrix.
+        """
         if self.pca:
-            # Can regularise by adding to diagonal
-            D = block_diag(
+            B = block_diag(
                 *[
                     np.diag((1 - self.c[i]) * pc.explained_variance_ + self.c[i])
                     for i, pc in enumerate(self.pca_models)
                 ]
             )
         else:
-            D = block_diag(
+            B = block_diag(
                 *[
                     (1 - self.c[i]) * np.cov(view, rowvar=False)
                     + self.c[i] * np.eye(view.shape[1])
                     for i, view in enumerate(views)
                 ]
             )
-        D_smallest_eig = min(0, np.linalg.eigvalsh(D).min()) - self.eps
-        D = D - D_smallest_eig * np.eye(D.shape[0])
-        return D / len(views)
+        B_smallest_eig = min(0, np.linalg.eigvalsh(B).min()) - self.eps
+        B = B - B_smallest_eig * np.eye(B.shape[0])
+        return B / len(views)
 
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"multiview": True}
 
 
 class rCCA(MCCA):
@@ -205,18 +231,18 @@
     >>> X2 = rng.random((10,5))
     >>> model = rCCA(c=0.1)
     >>> model.fit((X1,X2)).score((X1,X2))
 
 
     References
     --------
-    Vinod, Hrishikesh _D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
+    Vinod, Hrishikesh _B. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
     """
 
-    def _C(self, views, **kwargs):
+    def _A(self, views, **kwargs):
         if len(views) != 2:
             raise ValueError(
                 f"Model can only be used with two representations, but {len(views)} were given. Use MCCA or GCCA instead for CCA or MPLS for PLS."
             )
         if self.pca:
             # Compute the B matrices for each view
             B = [
@@ -248,15 +274,15 @@
                 self.T = self.L0 @ C @ self.L1 @ self.L1.T @ C.T @ self.L0.T
                 return self.T
             else:
                 self.primary_view = 1
                 self.T = self.L1 @ C.T @ self.L0 @ self.L0.T @ C @ self.L1.T
                 return self.T
 
-    def _D(self, views, **kwargs):
+    def _B(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views):
         self.weights_ = [None] * 2
         if self.pca:
             B = [
                 (1 - self.c[i]) * pc.singular_values_**2 / self.n_samples_ + self.c[i]
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_partialcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_pcacca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_pcacca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_pls.py` & `cca_zoo-2.6.0/cca_zoo/linear/_pls.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,10 @@
-import numpy as np
-
 from cca_zoo.linear._mcca import MCCA, rCCA
 
 
-def reduce_dims(x):
-    U, S, _ = np.linalg.svd(x, full_matrices=False)
-    return U @ np.diag(S)
-
-
 class PLSMixin:
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"pls": True}
 
 
 class PLS(rCCA, PLSMixin):
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_prcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_prcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,21 @@
         self.p = [X_i.shape[1] for X_i in X_1]
         X_2 = [np.delete(view, idx, axis=1) for view, idx in zip(views, idxs)]
         self.B = [np.linalg.pinv(X_2) @ X_1 for X_1, X_2 in zip(X_1, X_2)]
         X_1 = [X_1 - X_2 @ B for X_1, X_2, B in zip(X_1, X_2, self.B)]
         views = [np.hstack((X_1, X_2)) for X_1, X_2 in zip(X_1, X_2)]
         return views
 
-    def _C(self, views, **kwargs):
+    def _A(self, views, **kwargs):
         all_views = np.concatenate(views, axis=1)
         C = np.cov(all_views, rowvar=False)
         C -= block_diag(*[np.cov(view, rowvar=False) for view in views])
         return C
 
-    def _D(self, views: Iterable[np.ndarray], idxs=None, **kwargs):
+    def _B(self, views: Iterable[np.ndarray], idxs=None, **kwargs):
         penalties = [np.zeros((view.shape[1])) for view in views]
         for i, idx in enumerate(idxs):
             penalties[i][idx] = self.c[i]
         D = block_diag(
             *[
                 (1 - self.c[i]) * np.cov(view, rowvar=False) + np.diag(penalties[i])
                 for i, view in enumerate(views)
```

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_search.py` & `cca_zoo-2.6.0/cca_zoo/linear/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/linear/_tcca.py` & `cca_zoo-2.6.0/cca_zoo/linear/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/model_selection/_search.py` & `cca_zoo-2.6.0/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.6.0/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/nonparametric/_kcca.py` & `cca_zoo-2.6.0/cca_zoo/nonparametric/_kcca.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,35 +35,33 @@
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         return kernels
 
     def transform(self, views: Iterable[np.ndarray], **kwargs):
-        check_is_fitted(self, attributes=["alphas"])
+        check_is_fitted(self, attributes=["alphas_"])
         Ktest = [
             pairwise_kernels(
                 self.train_views[i],
                 Y=view,
                 metric=self.kernel[i],
                 gamma=self.gamma[i],
                 degree=self.degree[i],
                 coef0=self.coef0[i],
                 filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(views)
         ]
-        transformed_views = [
-            kernel.T @ self.alphas[i] for i, kernel in enumerate(Ktest)
-        ]
-        return transformed_views
+        representations = [kernel.T @ self.alphas_[i] for i, kernel in enumerate(Ktest)]
+        return representations
 
     @property
-    def alphas(self):
+    def alphas_(self):
         check_is_fitted(self)
         return self.weights_
 
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"kernel": True}
 
@@ -145,15 +143,15 @@
         # Store the kernel parameters
         self.kernel_params = kernel_params
         self.gamma = gamma
         self.coef0 = coef0
         self.kernel = kernel
         self.degree = degree
 
-    def _D(self, views, **kwargs):
+    def _B(self, views, **kwargs):
         D = block_diag(
             *[
                 (1 - self.c[i]) * np.cov(view, rowvar=False) + self.c[i] * view
                 for i, view in enumerate(views)
             ]
         )
         D_smallest_eig = min(0, np.linalg.eigvalsh(D).min()) - self.eps
```

### Comparing `cca_zoo-2.5.0/cca_zoo/nonparametric/_ncca.py` & `cca_zoo-2.6.0/cca_zoo/nonparametric/_ncca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/nonparametric/_scca_hsic.py` & `cca_zoo-2.6.0/cca_zoo/nonparametric/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/preprocessing/__init__.py` & `cca_zoo-2.6.0/cca_zoo/preprocessing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Preprocessing methods for multi-view data.
 """
+
 from sklearn.base import TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 
 from cca_zoo._utils._checks import check_Xs
 
 
 class MultiViewPreprocessing(TransformerMixin):
```

### Comparing `cca_zoo-2.5.0/cca_zoo/probabilistic/_cca.py` & `cca_zoo-2.6.0/cca_zoo/probabilistic/_cca.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     References
     ----------
     [1] Bach, Francis R., and Michael I. Jordan. "A probabilistic interpretation of canonical correlation analysis." (2005).
     [2] Wang, Chong. "Variational Bayesian approach to canonical correlation analysis." IEEE Transactions on Neural Networks 18.3 (2007): 905-910.
 
     """
 
-    return_sites = ["z"]
+    return_sites = ["representations"]
 
     def __init__(
         self,
         latent_dimensions: int = 1,
         copy_data=True,
         random_state: int = 0,
         learning_rate=1e-1,
@@ -165,15 +165,15 @@
                     self.n_features_in_[1],
                 ),
             ),
         )
 
         with numpyro.plate("n", self.n_samples_):
             z = numpyro.sample(
-                "z",
+                "representations",
                 dist.MultivariateNormal(
                     jnp.zeros(self.latent_dimensions), jnp.eye(self.latent_dimensions)
                 ),
             )
 
             numpyro.sample(
                 "X1",
@@ -198,26 +198,28 @@
 
         Parameters
         ----------
         views: tuple of np.ndarray
             A tuple containing the first and second representations, X1 and X2, each as a numpy array.
         """
 
-        # Variational parameters for the approximate posterior of z
+        # Variational parameters for the approximate posterior of representations
         z_loc = numpyro.param(
             "z_loc", jnp.zeros((self.n_samples_, self.latent_dimensions))
         )
         z_scale = numpyro.param(
             "z_scale",
             jnp.ones((self.n_samples_, self.latent_dimensions)),
             constraint=dist.constraints.positive,
         )
 
         with numpyro.plate("n", self.n_samples_):
-            numpyro.sample("z", dist.MultivariateNormal(z_loc, jnp.diag(z_scale)))
+            numpyro.sample(
+                "representations", dist.MultivariateNormal(z_loc, jnp.diag(z_scale))
+            )
 
     def render(self, views):
         check_graphviz_support("ProbabilisticCCA")
         self.rendering = numpyro.render_model(
             self._model, model_args=(views,), filename="model.pdf"
         )
```

### Comparing `cca_zoo-2.5.0/cca_zoo/probabilistic/_pls.py` & `cca_zoo-2.6.0/cca_zoo/probabilistic/_pls.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     self.n_features_in_[1],
                 ),
             ),
         )
 
         with numpyro.plate("n", self.n_samples_):
             z = numpyro.sample(
-                "z",
+                "representations",
                 dist.MultivariateNormal(
                     jnp.zeros(self.latent_dimensions), jnp.eye(self.latent_dimensions)
                 ),
             )
 
             numpyro.sample(
                 "X1",
```

### Comparing `cca_zoo-2.5.0/cca_zoo/probabilistic/_plsregression.py` & `cca_zoo-2.6.0/cca_zoo/probabilistic/_plsregression.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/probabilistic/_rcca.py` & `cca_zoo-2.6.0/cca_zoo/probabilistic/_rcca.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,15 @@
                     self.n_features_in_[1],
                 ),
             ),
         )
 
         with numpyro.plate("n", self.n_samples_):
             z = numpyro.sample(
-                "z",
+                "representations",
                 dist.MultivariateNormal(
                     jnp.zeros(self.latent_dimensions), jnp.eye(self.latent_dimensions)
                 ),
             )
 
             numpyro.sample(
                 "X1",
@@ -118,26 +118,28 @@
 
         Parameters
         ----------
         views: tuple of np.ndarray
             A tuple containing the first and second representations, X1 and X2, each as a numpy array.
         """
 
-        # Variational parameters for the approximate posterior of z
+        # Variational parameters for the approximate posterior of representations
         z_loc = numpyro.param(
             "z_loc", jnp.zeros((self.n_samples_, self.latent_dimensions))
         )
         z_scale = numpyro.param(
             "z_scale",
             jnp.ones((self.n_samples_, self.latent_dimensions)),
             constraint=dist.constraints.positive,
         )
 
         with numpyro.plate("n", self.n_samples_):
-            numpyro.sample("z", dist.MultivariateNormal(z_loc, jnp.diag(z_scale)))
+            numpyro.sample(
+                "representations", dist.MultivariateNormal(z_loc, jnp.diag(z_scale))
+            )
 
     def joint(self):
         psi1 = jnp.eye(self.n_features_in_[0]) * self.params["sigma_1"]
         psi2 = jnp.eye(self.n_features_in_[1]) * self.params["sigma_2"]
         # Calculate the individual matrix blocks
         top_left = self.params["W_1"] @ self.params["W_1"].T + psi1
         bottom_right = self.params["W_2"] @ self.params["W_2"].T + psi2
```

### Comparing `cca_zoo-2.5.0/cca_zoo/sequential.py` & `cca_zoo-2.6.0/cca_zoo/sequential.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Module for finding _CCALoss effects sequentially by deflation.
 
 Check if each effect is significant, and if so, remove it from the data and repeat.
 """
+
 from abc import ABCMeta
 from typing import Iterable
 
 import numpy as np
 from sklearn.base import MetaEstimatorMixin
 
 from cca_zoo._base import _BaseModel
```

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/correlation.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/correlation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/covariance.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/covariance.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/explained_covariance.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/explained_covariance.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/explained_variance.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/explained_variance.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/inference.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/inference.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/scores.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/representations.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
-from cca_zoo._utils._checks import check_seaborn_support
+from cca_zoo._utils._checks import (
+    check_seaborn_support,
+    check_tsne_support,
+    check_umap_support,
+)
 from cca_zoo._utils._cross_correlation import cross_corrcoef
 
 
-class ScoreScatterDisplay:
+class RepresentationScatterDisplay:
     """
     Display the scores of a model.
 
     Args:
         scores (tuple): Tuple of two arrays representing training scores for two representations.
         test_scores (tuple, optional): Tuple of two arrays representing test scores for two representations. Default is None.
         labels (array-like, optional): Labels for training data. Default is None.
@@ -81,15 +85,15 @@
             )
         return train_corrs, test_corrs
 
     def _validate_plot_params(self):
         """
         Validate plot parameters and check Seaborn support.
         """
-        check_seaborn_support("ScoreScatterDisplay")
+        check_seaborn_support("RepresentationScatterDisplay")
 
     @classmethod
     def from_estimator(
         cls,
         model,
         train_views,
         test_views=None,
@@ -105,15 +109,15 @@
         Args:
             model: The estimator model.
             train_views (tuple): Tuple of two arrays representing training data representations.
             test_views (tuple, optional): Tuple of two arrays representing test data representations. Default is None.
             **kwargs: Additional keyword arguments passed to the ScoreDisplay constructor.
 
         Returns:
-            ScoreScatterDisplay: An instance of ScoreDisplay.
+            RepresentationScatterDisplay: An instance of ScoreDisplay.
         """
         train_scores = model.transform(train_views)
         test_scores = model.transform(test_views) if test_views is not None else None
         return cls.from_scores(
             train_scores,
             test_scores,
             labels=labels,
@@ -139,15 +143,15 @@
 
         Args:
             train_scores (tuple): Tuple of two arrays representing training scores for two representations.
             test_scores (tuple, optional): Tuple of two arrays representing test scores for two representations. Default is None.
             **kwargs: Additional keyword arguments passed to the ScoreDisplay constructor.
 
         Returns:
-            ScoreScatterDisplay: An instance of ScoreDisplay.
+            RepresentationScatterDisplay: An instance of ScoreDisplay.
         """
 
         return cls(
             train_scores,
             test_scores,
             labels=labels,
             test_labels=test_labels,
@@ -176,17 +180,19 @@
         dimensions = self.scores[0].shape[1]
         self.figures_ = []
 
         for i in range(dimensions):
             g, fig, ax = self._create_plot(
                 x=self.combined_scores_x[:, i],
                 y=self.combined_scores_y[:, i],
-                hue=self.combined_labels
-                if self.combined_labels is not None
-                else self.mode_labels,
+                hue=(
+                    self.combined_labels
+                    if self.combined_labels is not None
+                    else self.mode_labels
+                ),
             )
             if self.ax_labels is not None:
                 ax.set_xlabel(self.ax_labels[0])
                 ax.set_ylabel(self.ax_labels[1])
             # if g is a jointplot, get the underlying figure
             plt.suptitle(f"{title} Latent Dimension {i + 1}")
 
@@ -210,26 +216,26 @@
             # if there is a legend, move it to the bottom right
             if ax.get_legend() is not None:
                 sns.move_legend(ax, "lower right")
             plt.tight_layout()
             self.figures_.append(fig)
 
 
-class JointScoreScatterDisplay(ScoreScatterDisplay):
+class JointRepresentationScatterDisplay(RepresentationScatterDisplay):
     def _create_plot(self, x, y, hue=None, palette=None):
         g = sns.jointplot(
             x=x,
             y=y,
             hue=hue,
             **self.kwargs,
         )
         return g, g.fig, g.ax_joint
 
 
-class SeparateScoreScatterDisplay(ScoreScatterDisplay):
+class SeparateRepresentationScatterDisplay(RepresentationScatterDisplay):
     def plot(self, title=""):
         dimensions = self.scores[0].shape[1]
         self.train_figures_ = []
         self.test_figures_ = []
 
         for i in range(dimensions):
             g, fig, ax = self._create_plot(
@@ -275,26 +281,26 @@
                 )
             plt.suptitle(f"{title} Test - Latent Dimension {i + 1}")
             self.test_figures_.append(g)
         plt.tight_layout()
         return self
 
 
-class SeparateJointScoreDisplay(SeparateScoreScatterDisplay):
+class SeparateJointRepresentationDisplay(SeparateRepresentationScatterDisplay):
     def _create_plot(self, x, y, hue=None, palette=None):
         g = sns.jointplot(
             x=x,
             y=y,
             hue=hue,
             **self.kwargs,
         )
         return g, g.fig, g.ax_joint
 
 
-class PairScoreScatterDisplay(ScoreScatterDisplay):
+class PairRepresentationScatterDisplay(RepresentationScatterDisplay):
     def plot(self):
         # Put the combined scores into a dataframe with dimension as column names
         x_vars = [f"X{i}" for i in range(self.combined_scores_x.shape[1])]
         y_vars = [f"Y{i}" for i in range(self.combined_scores_y.shape[1])]
         df = pd.DataFrame(self.combined_scores_x, columns=x_vars)
         df = df.join(pd.DataFrame(self.combined_scores_y, columns=y_vars))
         df["Mode"] = self.mode_labels
@@ -309,7 +315,81 @@
                 0.95,
                 f"Corr: {self.train_corrs[i]:.2f}",
                 transform=g.axes[i, i].transAxes,
                 verticalalignment="top",
             )
         self.figure_ = g.fig
         return self
+
+
+class TSNERepresentationDisplay(RepresentationScatterDisplay):
+    def _validate_plot_params(self):
+        check_tsne_support("TSNERepresentationDisplay")
+        check_seaborn_support("TSNERepresentationDisplay")
+
+    def plot(self):
+        self._validate_plot_params()
+        import openTSNE
+        import matplotlib.pyplot as plt
+
+        reducer = openTSNE.TSNE()
+        embedding = reducer.fit(self.scores[0])
+        fig, ax = plt.subplots()
+        sns.scatterplot(
+            x=embedding[:, 0],
+            y=embedding[:, 1],
+            hue=self.labels,
+            ax=ax,
+            alpha=0.1 if self.test_scores is not None else 1.0,
+            label="Train" if self.test_scores is not None else None,
+            **self.kwargs,
+        )
+        if self.test_scores is not None:
+            embedding = reducer.fit(self.test_scores[0])
+            sns.scatterplot(
+                x=embedding[:, 0],
+                y=embedding[:, 1],
+                hue=self.test_labels,
+                ax=ax,
+                label="Test",
+                **self.kwargs,
+            )
+        plt.tight_layout()
+        self.figure_ = fig
+        return self
+
+
+class UMAPRepresentationDisplay(RepresentationScatterDisplay):
+    def _validate_plot_params(self):
+        check_umap_support("UMAPRepresentationDisplay")
+        check_seaborn_support("TSNERepresentationDisplay")
+
+    def plot(self, **kwargs):
+        self._validate_plot_params()
+        import umap
+        import matplotlib.pyplot as plt
+
+        reducer = umap.UMAP()
+        embedding = reducer.fit_transform(self.scores[0])
+        fig, ax = plt.subplots()
+        sns.scatterplot(
+            x=embedding[:, 0],
+            y=embedding[:, 1],
+            hue=self.labels,
+            ax=ax,
+            alpha=0.1 if self.test_scores is not None else 1.0,
+            label="Train" if self.test_scores is not None else None,
+            **self.kwargs,
+        )
+        if self.test_scores is not None:
+            embedding = reducer.transform(self.test_scores[0])
+            sns.scatterplot(
+                x=embedding[:, 0],
+                y=embedding[:, 1],
+                hue=self.test_labels,
+                ax=ax,
+                label="Test",
+                **self.kwargs,
+            )
+        plt.tight_layout()
+        self.figure_ = fig
+        return self
```

### Comparing `cca_zoo-2.5.0/cca_zoo/visualisation/weights.py` & `cca_zoo-2.6.0/cca_zoo/visualisation/weights.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.5.0/pyproject.toml` & `cca_zoo-2.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 [tool.poetry]
 name = "cca-zoo"
-version = "2.5.0"
+version = "2.6.0"
 description = "Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework"
 authors = ["jameschapman <james.chapman.19@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jameschapman19/cca_zoo"
 keywords = ["cca"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0.0"
-numpy = "*"
-scipy = "*"
 scikit-learn = "^1.2.2"
-pandas = "*"
 tensorly = "*"
-joblib = "*"
 tqdm = "*"
 
 # Optional dependencies
 jax = {version = "*", optional = true}
 numpyro = {version = "*", optional = true}
 arviz = {version = "*", optional = true}
 funsor = {version = "*", optional = true}
```

### Comparing `cca_zoo-2.5.0/PKG-INFO` & `cca_zoo-2.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cca-zoo
-Version: 2.5.0
+Version: 2.6.0
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 License: MIT
 Keywords: cca
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 Requires-Python: >=3.8,<4.0.0
@@ -17,21 +17,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: deep
 Provides-Extra: probabilistic
 Provides-Extra: visualisation
 Requires-Dist: arviz ; extra == "probabilistic"
 Requires-Dist: funsor ; extra == "probabilistic"
 Requires-Dist: jax ; extra == "probabilistic"
-Requires-Dist: joblib
 Requires-Dist: lightning ; extra == "deep"
-Requires-Dist: numpy
 Requires-Dist: numpyro ; extra == "probabilistic"
-Requires-Dist: pandas
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: scipy
 Requires-Dist: tensorly
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; (sys_platform == "darwin") and (extra == "deep")
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; (sys_platform == "linux") and (extra == "deep")
 Requires-Dist: torch (>=2.0.1,<3.0.0) ; (sys_platform == "win32") and (extra == "deep")
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
@@ -91,14 +87,20 @@
 
 Note that `deep` requires `torch` and `lightning` which may be better installed separately following the [PyTorch installation guide](https://pytorch.org/get-started/locally/).
 
 `probabilistic` requires `numpyro` which may be better installed separately following the [NumPyro installation guide](https://num.pyro.ai/en/stable/getting_started.html#installation).
 
 `visualisation` requires `matplotlib` and `seaborn`
 
+## Plug into the Machine Learning Ecosystem
+
+CCA-Zoo is designed to be compatible with the machine learning ecosystem. It is built on top of `scikit-learn`, `tensorly`, `torch`, `pytorch-lightning`, and `numpyro`.
+
+<img src="docs/_static/CCA_Zoo_map.svg" alt="drawing" width="1000"/>
+
 ## 🏎️ Performance Highlights
 CCA-Zoo shines when it comes to high-dimensional data analysis. It significantly outperforms scikit-learn, particularly as dimensionality increases. For comprehensive benchmarks, see our [script](benchmark/cca_high_dimensions.py) and the graph below.
 
 ![Benchmark Plot CCA](benchmark/CCA_Speed_Benchmark.svg)
 ![Benchmark Plot PLS](benchmark/PLS_Speed_Benchmark.svg)
 
 ## 📚 Detailed Documentation
```

