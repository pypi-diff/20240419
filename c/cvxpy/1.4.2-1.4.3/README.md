# Comparing `tmp/cvxpy-1.4.2.tar.gz` & `tmp/cvxpy-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxpy-1.4.2.tar", last modified: Fri Jan 19 02:18:12 2024, max compression
+gzip compressed data, was "cvxpy-1.4.3.tar", last modified: Tue Apr 16 08:08:50 2024, max compression
```

## Comparing `cvxpy-1.4.2.tar` & `cvxpy-1.4.3.tar`

### file list

```diff
@@ -1,853 +1,853 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.020658 cvxpy-1.4.2/
--rw-r--r--   0 runner     (501) staff       (20)    11344 2024-01-19 02:11:42.000000 cvxpy-1.4.2/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      102 2024-01-19 02:11:42.000000 cvxpy-1.4.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     8760 2024-01-19 02:18:12.020329 cvxpy-1.4.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6950 2024-01-19 02:11:42.000000 cvxpy-1.4.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.515482 cvxpy-1.4.2/cvxpy/
--rw-r--r--   0 runner     (501) staff       (20)     3038 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.540914 cvxpy-1.4.2/cvxpy/atoms/
--rw-r--r--   0 runner     (501) staff       (20)     5385 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.553880 cvxpy-1.4.2/cvxpy/atoms/affine/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3967 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/add_expr.py
--rw-r--r--   0 runner     (501) staff       (20)     5719 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/affine_atom.py
--rw-r--r--   0 runner     (501) staff       (20)    15481 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/binary_operators.py
--rw-r--r--   0 runner     (501) staff       (20)     1137 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/bmat.py
--rw-r--r--   0 runner     (501) staff       (20)     2313 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/conj.py
--rw-r--r--   0 runner     (501) staff       (20)     6168 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     4371 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/cumsum.py
--rw-r--r--   0 runner     (501) staff       (20)     5357 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/diag.py
--rw-r--r--   0 runner     (501) staff       (20)     1644 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/diff.py
--rw-r--r--   0 runner     (501) staff       (20)     2977 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/hstack.py
--rw-r--r--   0 runner     (501) staff       (20)     1459 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/imag.py
--rw-r--r--   0 runner     (501) staff       (20)     6401 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/index.py
--rw-r--r--   0 runner     (501) staff       (20)     4379 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/kron.py
--rw-r--r--   0 runner     (501) staff       (20)     3310 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/partial_trace.py
--rw-r--r--   0 runner     (501) staff       (20)     3370 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/partial_transpose.py
--rw-r--r--   0 runner     (501) staff       (20)     3204 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/promote.py
--rw-r--r--   0 runner     (501) staff       (20)     1486 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/real.py
--rw-r--r--   0 runner     (501) staff       (20)     5340 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/reshape.py
--rw-r--r--   0 runner     (501) staff       (20)     3553 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/sum.py
--rw-r--r--   0 runner     (501) staff       (20)     2937 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/trace.py
--rw-r--r--   0 runner     (501) staff       (20)     2872 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/transpose.py
--rw-r--r--   0 runner     (501) staff       (20)     2752 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/unary_operators.py
--rw-r--r--   0 runner     (501) staff       (20)     4701 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/upper_tri.py
--rw-r--r--   0 runner     (501) staff       (20)     1108 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/vec.py
--rw-r--r--   0 runner     (501) staff       (20)     3033 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/vstack.py
--rw-r--r--   0 runner     (501) staff       (20)     4182 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/affine/wraps.py
--rw-r--r--   0 runner     (501) staff       (20)    16154 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/atom.py
--rw-r--r--   0 runner     (501) staff       (20)     4313 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/axis_atom.py
--rw-r--r--   0 runner     (501) staff       (20)     3132 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/condition_number.py
--rw-r--r--   0 runner     (501) staff       (20)     2943 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/cummax.py
--rw-r--r--   0 runner     (501) staff       (20)     2423 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/dist_ratio.py
--rw-r--r--   0 runner     (501) staff       (20)     4928 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/dotsort.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.565007 cvxpy-1.4.2/cvxpy/atoms/elementwise/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2457 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/abs.py
--rw-r--r--   0 runner     (501) staff       (20)     4790 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/ceil.py
--rw-r--r--   0 runner     (501) staff       (20)     2414 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/elementwise.py
--rw-r--r--   0 runner     (501) staff       (20)     2746 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/entr.py
--rw-r--r--   0 runner     (501) staff       (20)     2358 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/exp.py
--rw-r--r--   0 runner     (501) staff       (20)     3520 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/huber.py
--rw-r--r--   0 runner     (501) staff       (20)      703 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/inv_pos.py
--rw-r--r--   0 runner     (501) staff       (20)     3009 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/kl_div.py
--rw-r--r--   0 runner     (501) staff       (20)     2757 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/log.py
--rw-r--r--   0 runner     (501) staff       (20)     2046 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/log1p.py
--rw-r--r--   0 runner     (501) staff       (20)     2036 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/log_normcdf.py
--rw-r--r--   0 runner     (501) staff       (20)     1417 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/loggamma.py
--rw-r--r--   0 runner     (501) staff       (20)     2345 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/logistic.py
--rw-r--r--   0 runner     (501) staff       (20)     3519 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/maximum.py
--rw-r--r--   0 runner     (501) staff       (20)     3222 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/minimum.py
--rw-r--r--   0 runner     (501) staff       (20)      699 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/neg.py
--rw-r--r--   0 runner     (501) staff       (20)      696 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/pos.py
--rw-r--r--   0 runner     (501) staff       (20)    14794 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/power.py
--rw-r--r--   0 runner     (501) staff       (20)     2988 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/rel_entr.py
--rw-r--r--   0 runner     (501) staff       (20)      779 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/scalene.py
--rw-r--r--   0 runner     (501) staff       (20)      739 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/sqrt.py
--rw-r--r--   0 runner     (501) staff       (20)      691 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/square.py
--rw-r--r--   0 runner     (501) staff       (20)     2682 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/elementwise/xexp.py
--rw-r--r--   0 runner     (501) staff       (20)      243 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/errormsg.py
--rw-r--r--   0 runner     (501) staff       (20)     3300 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/eye_minus_inv.py
--rw-r--r--   0 runner     (501) staff       (20)     3518 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/gen_lambda_max.py
--rw-r--r--   0 runner     (501) staff       (20)    12147 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/geo_mean.py
--rw-r--r--   0 runner     (501) staff       (20)     4909 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/gmatmul.py
--rw-r--r--   0 runner     (501) staff       (20)     1292 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/harmonic_mean.py
--rw-r--r--   0 runner     (501) staff       (20)     1197 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/inv_prod.py
--rw-r--r--   0 runner     (501) staff       (20)     3291 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/lambda_max.py
--rw-r--r--   0 runner     (501) staff       (20)      811 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/lambda_min.py
--rw-r--r--   0 runner     (501) staff       (20)     2318 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/lambda_sum_largest.py
--rw-r--r--   0 runner     (501) staff       (20)      834 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/lambda_sum_smallest.py
--rw-r--r--   0 runner     (501) staff       (20)     2324 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/length.py
--rw-r--r--   0 runner     (501) staff       (20)     3645 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/log_det.py
--rw-r--r--   0 runner     (501) staff       (20)     2690 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/log_sum_exp.py
--rw-r--r--   0 runner     (501) staff       (20)     4538 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/matrix_frac.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/max.py
--rw-r--r--   0 runner     (501) staff       (20)     3632 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/min.py
--rw-r--r--   0 runner     (501) staff       (20)     1304 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/mixed_norm.py
--rw-r--r--   0 runner     (501) staff       (20)     3363 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/norm.py
--rw-r--r--   0 runner     (501) staff       (20)     3212 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/norm1.py
--rw-r--r--   0 runner     (501) staff       (20)     3376 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/norm_inf.py
--rw-r--r--   0 runner     (501) staff       (20)     2271 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/norm_nuc.py
--rw-r--r--   0 runner     (501) staff       (20)     2801 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/one_minus_pos.py
--rw-r--r--   0 runner     (501) staff       (20)     4730 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/perspective.py
--rw-r--r--   0 runner     (501) staff       (20)     2694 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/pf_eigenvalue.py
--rw-r--r--   0 runner     (501) staff       (20)     8451 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/pnorm.py
--rw-r--r--   0 runner     (501) staff       (20)     4180 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/prod.py
--rw-r--r--   0 runner     (501) staff       (20)      975 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/ptp.py
--rw-r--r--   0 runner     (501) staff       (20)     8139 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/quad_form.py
--rw-r--r--   0 runner     (501) staff       (20)     4351 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/quad_over_lin.py
--rw-r--r--   0 runner     (501) staff       (20)     2381 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/sigma_max.py
--rw-r--r--   0 runner     (501) staff       (20)     2121 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/sign.py
--rw-r--r--   0 runner     (501) staff       (20)     2179 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/stats.py
--rw-r--r--   0 runner     (501) staff       (20)     3117 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/sum_largest.py
--rw-r--r--   0 runner     (501) staff       (20)      802 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/sum_smallest.py
--rw-r--r--   0 runner     (501) staff       (20)      930 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/sum_squares.py
--rw-r--r--   0 runner     (501) staff       (20)     4048 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/suppfunc.py
--rw-r--r--   0 runner     (501) staff       (20)     2101 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/total_variation.py
--rw-r--r--   0 runner     (501) staff       (20)     3832 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/tr_inv.py
--rw-r--r--   0 runner     (501) staff       (20)     3821 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/atoms/von_neumann_entr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.570285 cvxpy-1.4.2/cvxpy/constraints/
--rw-r--r--   0 runner     (501) staff       (20)     1122 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2303 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/cones.py
--rw-r--r--   0 runner     (501) staff       (20)     7254 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/constraint.py
--rw-r--r--   0 runner     (501) staff       (20)    13846 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/exponential.py
--rw-r--r--   0 runner     (501) staff       (20)     4576 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/finite_set.py
--rw-r--r--   0 runner     (501) staff       (20)     7905 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/nonpos.py
--rw-r--r--   0 runner     (501) staff       (20)    11646 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/power.py
--rw-r--r--   0 runner     (501) staff       (20)     3242 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/psd.py
--rw-r--r--   0 runner     (501) staff       (20)     6030 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/second_order.py
--rw-r--r--   0 runner     (501) staff       (20)     3831 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     5264 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/constraints/zero.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.570771 cvxpy-1.4.2/cvxpy/cvxcore/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.489203 cvxpy-1.4.2/cvxpy/cvxcore/include/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.587142 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/
--rw-r--r--   0 runner     (501) staff       (20)      694 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/CMakeLists.txt
--rw-r--r--   0 runner     (501) staff       (20)     1161 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Cholesky
--rw-r--r--   0 runner     (501) staff       (20)     1900 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/CholmodSupport
--rw-r--r--   0 runner     (501) staff       (20)    12799 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Core
--rw-r--r--   0 runner     (501) staff       (20)      122 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Dense
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Eigen
--rw-r--r--   0 runner     (501) staff       (20)     1777 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Eigenvalues
--rw-r--r--   0 runner     (501) staff       (20)     1940 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Geometry
--rw-r--r--   0 runner     (501) staff       (20)      829 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Householder
--rw-r--r--   0 runner     (501) staff       (20)     2083 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers
--rw-r--r--   0 runner     (501) staff       (20)      894 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Jacobi
--rw-r--r--   0 runner     (501) staff       (20)     1389 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/KLUSupport
--rw-r--r--   0 runner     (501) staff       (20)     1268 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/LU
--rw-r--r--   0 runner     (501) staff       (20)      991 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/MetisSupport
--rw-r--r--   0 runner     (501) staff       (20)     2451 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/OrderingMethods
--rw-r--r--   0 runner     (501) staff       (20)     1751 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/PaStiXSupport
--rw-r--r--   0 runner     (501) staff       (20)     1116 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/PardisoSupport
--rw-r--r--   0 runner     (501) staff       (20)     1272 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/QR
--rw-r--r--   0 runner     (501) staff       (20)      900 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc
--rw-r--r--   0 runner     (501) staff       (20)     1162 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SPQRSupport
--rw-r--r--   0 runner     (501) staff       (20)     1584 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SVD
--rw-r--r--   0 runner     (501) staff       (20)      888 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Sparse
--rw-r--r--   0 runner     (501) staff       (20)     1235 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseCholesky
--rw-r--r--   0 runner     (501) staff       (20)     2240 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseCore
--rw-r--r--   0 runner     (501) staff       (20)     1814 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseLU
--rw-r--r--   0 runner     (501) staff       (20)     1195 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseQR
--rw-r--r--   0 runner     (501) staff       (20)      797 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdDeque
--rw-r--r--   0 runner     (501) staff       (20)      726 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdList
--rw-r--r--   0 runner     (501) staff       (20)      803 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdVector
--rw-r--r--   0 runner     (501) staff       (20)     2243 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SuperLUSupport
--rw-r--r--   0 runner     (501) staff       (20)     1382 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/UmfPackSupport
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.501766 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.588768 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/
--rw-r--r--   0 runner     (501) staff       (20)    24934 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h
--rw-r--r--   0 runner     (501) staff       (20)    18760 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h
--rw-r--r--   0 runner     (501) staff       (20)     3974 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.589347 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/
--rw-r--r--   0 runner     (501) staff       (20)    25441 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.627734 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/
--rw-r--r--   0 runner     (501) staff       (20)    19214 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArithmeticSequence.h
--rw-r--r--   0 runner     (501) staff       (20)    16782 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Array.h
--rw-r--r--   0 runner     (501) staff       (20)     8217 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7018 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h
--rw-r--r--   0 runner     (501) staff       (20)     2738 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h
--rw-r--r--   0 runner     (501) staff       (20)    41673 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h
--rwxr-xr-x   0 runner     (501) staff       (20)    12488 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h
--rw-r--r--   0 runner     (501) staff       (20)    14075 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    18648 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Block.h
--rw-r--r--   0 runner     (501) staff       (20)     4429 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h
--rw-r--r--   0 runner     (501) staff       (20)     5981 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h
--rw-r--r--   0 runner     (501) staff       (20)     6990 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h
--rw-r--r--   0 runner     (501) staff       (20)    63841 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h
--rw-r--r--   0 runner     (501) staff       (20)     4745 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h
--rw-r--r--   0 runner     (501) staff       (20)     7909 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)    36282 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     8256 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     3937 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     5551 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h
--rw-r--r--   0 runner     (501) staff       (20)    31529 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h
--rw-r--r--   0 runner     (501) staff       (20)    24484 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h
--rw-r--r--   0 runner     (501) staff       (20)    25360 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h
--rw-r--r--   0 runner     (501) staff       (20)     9870 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h
--rw-r--r--   0 runner     (501) staff       (20)    14670 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)      988 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h
--rw-r--r--   0 runner     (501) staff       (20)    11654 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h
--rw-r--r--   0 runner     (501) staff       (20)     5841 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h
--rw-r--r--   0 runner     (501) staff       (20)     4909 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h
--rw-r--r--   0 runner     (501) staff       (20)     5759 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h
--rw-r--r--   0 runner     (501) staff       (20)    21679 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h
--rw-r--r--   0 runner     (501) staff       (20)    38812 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    11543 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)     8238 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/IO.h
--rw-r--r--   0 runner     (501) staff       (20)     9620 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/IndexedView.h
--rw-r--r--   0 runner     (501) staff       (20)     3503 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h
--rw-r--r--   0 runner     (501) staff       (20)     7256 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Map.h
--rw-r--r--   0 runner     (501) staff       (20)    11281 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h
--rw-r--r--   0 runner     (501) staff       (20)    60784 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)     7156 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    24343 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h
--rw-r--r--   0 runner     (501) staff       (20)    23856 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h
--rw-r--r--   0 runner     (501) staff       (20)     2520 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h
--rw-r--r--   0 runner     (501) staff       (20)     3620 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h
--rw-r--r--   0 runner     (501) staff       (20)    12884 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h
--rw-r--r--   0 runner     (501) staff       (20)     9207 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PartialReduxEvaluator.h
--rw-r--r--   0 runner     (501) staff       (20)    20748 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    49193 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7336 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Product.h
--rw-r--r--   0 runner     (501) staff       (20)    53832 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h
--rw-r--r--   0 runner     (501) staff       (20)     7756 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Random.h
--rw-r--r--   0 runner     (501) staff       (20)    19195 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h
--rw-r--r--   0 runner     (501) staff       (20)    17821 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h
--rw-r--r--   0 runner     (501) staff       (20)     5656 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h
--rw-r--r--   0 runner     (501) staff       (20)    17033 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Reshaped.h
--rw-r--r--   0 runner     (501) staff       (20)     4284 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h
--rw-r--r--   0 runner     (501) staff       (20)     7522 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h
--rw-r--r--   0 runner     (501) staff       (20)     6143 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Select.h
--rw-r--r--   0 runner     (501) staff       (20)    14999 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h
--rw-r--r--   0 runner     (501) staff       (20)     1697 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     6837 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h
--rw-r--r--   0 runner     (501) staff       (20)     9368 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h
--rw-r--r--   0 runner     (501) staff       (20)     6170 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     8700 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h
--rw-r--r--   0 runner     (501) staff       (20)    21641 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/StlIterators.h
--rw-r--r--   0 runner     (501) staff       (20)     4212 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h
--rw-r--r--   0 runner     (501) staff       (20)     2765 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h
--rw-r--r--   0 runner     (501) staff       (20)    17606 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h
--rw-r--r--   0 runner     (501) staff       (20)    13567 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h
--rw-r--r--   0 runner     (501) staff       (20)    38277 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     3488 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h
--rw-r--r--   0 runner     (501) staff       (20)    35168 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h
--rw-r--r--   0 runner     (501) staff       (20)    11997 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.494203 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.629967 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/
--rw-r--r--   0 runner     (501) staff       (20)    15223 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     8102 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    64608 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     2564 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.632108 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/
--rw-r--r--   0 runner     (501) staff       (20)    17160 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    13344 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    87891 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     2134 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.635392 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/
--rw-r--r--   0 runner     (501) staff       (20)    16540 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     2323 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)   119355 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     9490 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
--rw-r--r--   0 runner     (501) staff       (20)    24820 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
--rwxr-xr-x   0 runner     (501) staff       (20)   102394 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.638801 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/
--rw-r--r--   0 runner     (501) staff       (20)    17317 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    23547 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h
--rw-r--r--   0 runner     (501) staff       (20)     2387 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    10744 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    35476 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
--rw-r--r--   0 runner     (501) staff       (20)     5509 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.642689 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/
--rw-r--r--   0 runner     (501) staff       (20)    26903 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/BFloat16.h
--rw-r--r--   0 runner     (501) staff       (20)     5251 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h
--rw-r--r--   0 runner     (501) staff       (20)    67696 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)     3770 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
--rw-r--r--   0 runner     (501) staff       (20)    35534 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Half.h
--rw-r--r--   0 runner     (501) staff       (20)     1746 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h
--rw-r--r--   0 runner     (501) staff       (20)     3746 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.644261 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/
--rw-r--r--   0 runner     (501) staff       (20)     2695 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    57047 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     2256 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.492441 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.644730 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/
--rw-r--r--   0 runner     (501) staff       (20)      691 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/math_constants.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.646417 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/
--rw-r--r--   0 runner     (501) staff       (20)    17541 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)    16159 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    33615 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.649523 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/
--rw-r--r--   0 runner     (501) staff       (20)    22503 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     6815 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner     (501) staff       (20)     3083 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)   189525 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    51286 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.651984 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/
--rw-r--r--   0 runner     (501) staff       (20)    14251 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     6765 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h
--rwxr-xr-x   0 runner     (501) staff       (20)    64465 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     3650 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.653700 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/
--rw-r--r--   0 runner     (501) staff       (20)     1194 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    21200 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)     1351 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.656483 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/
--rw-r--r--   0 runner     (501) staff       (20)     7428 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/InteropHeaders.h
--rw-r--r--   0 runner     (501) staff       (20)    12539 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/MathFunctions.h
--rw-r--r--   0 runner     (501) staff       (20)    27786 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/PacketMath.h
--rw-r--r--   0 runner     (501) staff       (20)    21856 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
--rw-r--r--   0 runner     (501) staff       (20)     2626 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/TypeCasting.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.658119 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/
--rw-r--r--   0 runner     (501) staff       (20)    16728 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h
--rw-r--r--   0 runner     (501) staff       (20)     8024 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
--rwxr-xr-x   0 runner     (501) staff       (20)    36894 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.661603 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/
--rw-r--r--   0 runner     (501) staff       (20)     6686 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)    20921 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)     8334 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)     4998 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)      607 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h
--rw-r--r--   0 runner     (501) staff       (20)    40146 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.673869 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/
--rw-r--r--   0 runner     (501) staff       (20)   108448 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
--rw-r--r--   0 runner     (501) staff       (20)    20104 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    15948 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
--rw-r--r--   0 runner     (501) staff       (20)     6936 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     5106 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    21724 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)     6368 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     5582 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h
--rw-r--r--   0 runner     (501) staff       (20)    21354 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    11570 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     9958 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)     5209 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     6164 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     4126 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h
--rw-r--r--   0 runner     (501) staff       (20)    20987 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    13867 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    14722 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h
--rw-r--r--   0 runner     (501) staff       (20)    10571 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)    14678 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     6707 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
--rw-r--r--   0 runner     (501) staff       (20)     5882 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.683284 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/
--rwxr-xr-x   0 runner     (501) staff       (20)    23156 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h
--rw-r--r--   0 runner     (501) staff       (20)    19876 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ConfigureVectorization.h
--rw-r--r--   0 runner     (501) staff       (20)    21931 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h
--rwxr-xr-x   0 runner     (501) staff       (20)     4892 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h
--rw-r--r--   0 runner     (501) staff       (20)    15555 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h
--rw-r--r--   0 runner     (501) staff       (20)     6696 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/IndexedViewHelper.h
--rw-r--r--   0 runner     (501) staff       (20)    10949 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/IntegralConstant.h
--rwxr-xr-x   0 runner     (501) staff       (20)     4268 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h
--rw-r--r--   0 runner     (501) staff       (20)    52909 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h
--rw-r--r--   0 runner     (501) staff       (20)    46661 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h
--rwxr-xr-x   0 runner     (501) staff       (20)    29336 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h
--rw-r--r--   0 runner     (501) staff       (20)       85 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/NonMPL2.h
--rw-r--r--   0 runner     (501) staff       (20)     1024 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h
--rw-r--r--   0 runner     (501) staff       (20)     1432 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReshapedHelper.h
--rw-r--r--   0 runner     (501) staff       (20)    10676 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h
--rw-r--r--   0 runner     (501) staff       (20)    12003 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/SymbolicIndex.h
--rw-r--r--   0 runner     (501) staff       (20)    35762 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.693311 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/
--rw-r--r--   0 runner     (501) staff       (20)    12559 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    17274 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h
--rw-r--r--   0 runner     (501) staff       (20)     4178 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    22970 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    17176 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)     9716 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)    14349 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
--rw-r--r--   0 runner     (501) staff       (20)     5575 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
--rw-r--r--   0 runner     (501) staff       (20)    23640 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h
--rw-r--r--   0 runner     (501) staff       (20)    21078 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h
--rw-r--r--   0 runner     (501) staff       (20)     3650 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    35182 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
--rw-r--r--   0 runner     (501) staff       (20)     4104 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    22764 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.702700 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/
--rw-r--r--   0 runner     (501) staff       (20)    18939 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h
--rw-r--r--   0 runner     (501) staff       (20)     8403 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h
--rw-r--r--   0 runner     (501) staff       (20)     3624 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h
--rw-r--r--   0 runner     (501) staff       (20)    20726 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h
--rw-r--r--   0 runner     (501) staff       (20)    11962 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h
--rw-r--r--   0 runner     (501) staff       (20)     8955 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h
--rw-r--r--   0 runner     (501) staff       (20)     9812 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h
--rw-r--r--   0 runner     (501) staff       (20)    34367 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h
--rw-r--r--   0 runner     (501) staff       (20)     6862 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h
--rw-r--r--   0 runner     (501) staff       (20)     8063 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h
--rw-r--r--   0 runner     (501) staff       (20)     6724 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h
--rw-r--r--   0 runner     (501) staff       (20)    61930 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h
--rw-r--r--   0 runner     (501) staff       (20)     7664 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h
--rw-r--r--   0 runner     (501) staff       (20)     6190 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.704319 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/
--rw-r--r--   0 runner     (501) staff       (20)     5945 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SIMD.h
--rw-r--r--   0 runner     (501) staff       (20)     5387 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.705761 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/
--rw-r--r--   0 runner     (501) staff       (20)     4784 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h
--rw-r--r--   0 runner     (501) staff       (20)     5365 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h
--rw-r--r--   0 runner     (501) staff       (20)    23611 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.756834 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/
--rw-r--r--   0 runner     (501) staff       (20)     6771 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
--rw-r--r--   0 runner     (501) staff       (20)     6850 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
--rw-r--r--   0 runner     (501) staff       (20)     8887 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
--rw-r--r--   0 runner     (501) staff       (20)    15036 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
--rw-r--r--   0 runner     (501) staff       (20)    14940 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
--rw-r--r--   0 runner     (501) staff       (20)    13379 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7349 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
--rw-r--r--   0 runner     (501) staff       (20)     4212 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.761130 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/
--rw-r--r--   0 runner     (501) staff       (20)    16383 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.761658 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/KLUSupport/
--rw-r--r--   0 runner     (501) staff       (20)    11555 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/KLUSupport/KLUSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.814118 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/
--rw-r--r--   0 runner     (501) staff       (20)     3439 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h
--rw-r--r--   0 runner     (501) staff       (20)    32383 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h
--rw-r--r--   0 runner     (501) staff       (20)    15727 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h
--rw-r--r--   0 runner     (501) staff       (20)    22069 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h
--rw-r--r--   0 runner     (501) staff       (20)     3555 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.815086 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/
--rw-r--r--   0 runner     (501) staff       (20)    13693 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/InverseSize4.h
--rw-r--r--   0 runner     (501) staff       (20)    13662 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.815552 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/
--rw-r--r--   0 runner     (501) staff       (20)     4588 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.817497 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/
--rw-r--r--   0 runner     (501) staff       (20)    16105 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h
--rw-r--r--   0 runner     (501) staff       (20)    61681 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
--rw-r--r--   0 runner     (501) staff       (20)     5248 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.817995 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/
--rw-r--r--   0 runner     (501) staff       (20)    22249 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.818767 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/
--rw-r--r--   0 runner     (501) staff       (20)    20092 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.822220 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/
--rw-r--r--   0 runner     (501) staff       (20)    25498 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)     4662 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    23429 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
--rw-r--r--   0 runner     (501) staff       (20)    26768 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)    14641 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h
--rw-r--r--   0 runner     (501) staff       (20)     2993 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.822712 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/
--rw-r--r--   0 runner     (501) staff       (20)    11826 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.825420 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/
--rw-r--r--   0 runner     (501) staff       (20)    54214 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h
--rw-r--r--   0 runner     (501) staff       (20)    32988 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h
--rw-r--r--   0 runner     (501) staff       (20)     5099 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
--rw-r--r--   0 runner     (501) staff       (20)    14743 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h
--rw-r--r--   0 runner     (501) staff       (20)    15957 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.826795 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/
--rw-r--r--   0 runner     (501) staff       (20)    24216 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
--rw-r--r--   0 runner     (501) staff       (20)     5830 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.843420 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/
--rw-r--r--   0 runner     (501) staff       (20)    10670 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h
--rw-r--r--   0 runner     (501) staff       (20)     8743 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h
--rw-r--r--   0 runner     (501) staff       (20)    13166 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     2191 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    11368 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h
--rw-r--r--   0 runner     (501) staff       (20)    24360 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h
--rw-r--r--   0 runner     (501) staff       (20)     6485 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h
--rw-r--r--   0 runner     (501) staff       (20)    13606 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h
--rw-r--r--   0 runner     (501) staff       (20)    25524 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)     4757 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
--rw-r--r--   0 runner     (501) staff       (20)    13256 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     5808 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     3080 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h
--rw-r--r--   0 runner     (501) staff       (20)     1107 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h
--rw-r--r--   0 runner     (501) staff       (20)    12589 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h
--rw-r--r--   0 runner     (501) staff       (20)    57475 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)    17451 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h
--rw-r--r--   0 runner     (501) staff       (20)     7329 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h
--rw-r--r--   0 runner     (501) staff       (20)     7593 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h
--rw-r--r--   0 runner     (501) staff       (20)     1699 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h
--rw-r--r--   0 runner     (501) staff       (20)    15600 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h
--rw-r--r--   0 runner     (501) staff       (20)    25889 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
--rw-r--r--   0 runner     (501) staff       (20)     4424 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h
--rw-r--r--   0 runner     (501) staff       (20)     8704 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
--rw-r--r--   0 runner     (501) staff       (20)     3175 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h
--rw-r--r--   0 runner     (501) staff       (20)     6437 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h
--rw-r--r--   0 runner     (501) staff       (20)     6827 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h
--rw-r--r--   0 runner     (501) staff       (20)    14832 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h
--rw-r--r--   0 runner     (501) staff       (20)     8127 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h
--rw-r--r--   0 runner     (501) staff       (20)     9657 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.852482 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/
--rw-r--r--   0 runner     (501) staff       (20)    33316 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h
--rw-r--r--   0 runner     (501) staff       (20)     4303 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h
--rw-r--r--   0 runner     (501) staff       (20)     7602 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h
--rw-r--r--   0 runner     (501) staff       (20)     4974 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h
--rw-r--r--   0 runner     (501) staff       (20)    12837 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
--rw-r--r--   0 runner     (501) staff       (20)     2049 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h
--rw-r--r--   0 runner     (501) staff       (20)     6712 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     6584 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
--rw-r--r--   0 runner     (501) staff       (20)     3681 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
--rw-r--r--   0 runner     (501) staff       (20)    10217 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
--rw-r--r--   0 runner     (501) staff       (20)     4181 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
--rw-r--r--   0 runner     (501) staff       (20)     5723 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     8485 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
--rw-r--r--   0 runner     (501) staff       (20)     9028 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
--rw-r--r--   0 runner     (501) staff       (20)     4979 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h
--rw-r--r--   0 runner     (501) staff       (20)     4545 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.852950 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/
--rw-r--r--   0 runner     (501) staff       (20)    29167 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.854986 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/
--rw-r--r--   0 runner     (501) staff       (20)     4730 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h
--rw-r--r--   0 runner     (501) staff       (20)     4155 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h
--rw-r--r--   0 runner     (501) staff       (20)     5338 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h
--rw-r--r--   0 runner     (501) staff       (20)     2809 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.855449 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/
--rw-r--r--   0 runner     (501) staff       (20)    34324 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.856001 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/
--rw-r--r--   0 runner     (501) staff       (20)    24456 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.861936 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/
--rw-r--r--   0 runner     (501) staff       (20)     2913 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/Image.h
--rw-r--r--   0 runner     (501) staff       (20)     2742 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h
--rw-r--r--   0 runner     (501) staff       (20)     1748 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h
--rw-r--r--   0 runner     (501) staff       (20)    30560 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/blas.h
--rw-r--r--   0 runner     (501) staff       (20)     7834 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h
--rwxr-xr-x   0 runner     (501) staff       (20)  1058369 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h
--rw-r--r--   0 runner     (501) staff       (20)      474 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke_mangling.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.866920 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/
--rw-r--r--   0 runner     (501) staff       (20)    14060 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)    21431 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)    59020 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h
--rw-r--r--   0 runner     (501) staff       (20)     4828 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     6089 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)    12283 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/IndexedViewMethods.h
--rw-r--r--   0 runner     (501) staff       (20)     6387 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     3350 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
--rw-r--r--   0 runner     (501) staff       (20)     6915 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ReshapedMethods.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.871742 cvxpy-1.4.2/cvxpy/cvxcore/python/
--rw-r--r--   0 runner     (501) staff       (20)      316 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    20241 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/canonInterface.py
--rw-r--r--   0 runner     (501) staff       (20)     2403 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore.i
--rw-r--r--   0 runner     (501) staff       (20)    28678 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore.py
--rw-r--r--   0 runner     (501) staff       (20)   881862 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore_wrap.cxx
--rw-r--r--   0 runner     (501) staff       (20)    54061 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/python/numpy.i
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.876619 cvxpy-1.4.2/cvxpy/cvxcore/src/
--rw-r--r--   0 runner     (501) staff       (20)       24 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/.keep
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/LinOp.hpp
--rw-r--r--   0 runner     (501) staff       (20)    39627 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/LinOpOperations.cpp
--rw-r--r--   0 runner     (501) staff       (20)      844 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/LinOpOperations.hpp
--rw-r--r--   0 runner     (501) staff       (20)     3365 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/ProblemData.hpp
--rw-r--r--   0 runner     (501) staff       (20)     5057 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/Utils.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1454 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/Utils.hpp
--rw-r--r--   0 runner     (501) staff       (20)     8098 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/cvxcore.cpp
--rw-r--r--   0 runner     (501) staff       (20)     1351 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/cvxcore/src/cvxcore.hpp
--rw-r--r--   0 runner     (501) staff       (20)     1299 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/error.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.879372 cvxpy-1.4.2/cvxpy/expressions/
--rw-r--r--   0 runner     (501) staff       (20)      590 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.881338 cvxpy-1.4.2/cvxpy/expressions/constants/
--rw-r--r--   0 runner     (501) staff       (20)      670 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/constants/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1729 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/constants/callback_param.py
--rw-r--r--   0 runner     (501) staff       (20)     8063 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/constants/constant.py
--rw-r--r--   0 runner     (501) staff       (20)     3737 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/constants/parameter.py
--rw-r--r--   0 runner     (501) staff       (20)     3421 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/cvxtypes.py
--rw-r--r--   0 runner     (501) staff       (20)    27398 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    16595 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/leaf.py
--rw-r--r--   0 runner     (501) staff       (20)     4202 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/expressions/variable.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.883309 cvxpy-1.4.2/cvxpy/interface/
--rw-r--r--   0 runner     (501) staff       (20)      611 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5171 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/base_matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)    10925 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/matrix_utilities.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.885276 cvxpy-1.4.2/cvxpy/interface/numpy_interface/
--rw-r--r--   0 runner     (501) staff       (20)      818 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/numpy_interface/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2058 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/numpy_interface/matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     2527 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/numpy_interface/ndarray_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     3446 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/numpy_interface/sparse_matrix_interface.py
--rw-r--r--   0 runner     (501) staff       (20)     1929 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/interface/scipy_wrapper.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.888430 cvxpy-1.4.2/cvxpy/lin_ops/
--rw-r--r--   0 runner     (501) staff       (20)      684 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    73514 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/canon_backend.py
--rw-r--r--   0 runner     (501) staff       (20)     1126 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/lin_constraints.py
--rw-r--r--   0 runner     (501) staff       (20)     3402 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/lin_op.py
--rw-r--r--   0 runner     (501) staff       (20)    18699 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/lin_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    12117 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/lin_ops/tree_mat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.891491 cvxpy-1.4.2/cvxpy/problems/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4958 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/iterative.py
--rw-r--r--   0 runner     (501) staff       (20)     7339 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/objective.py
--rw-r--r--   0 runner     (501) staff       (20)     1615 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/param_prob.py
--rw-r--r--   0 runner     (501) staff       (20)    63502 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/problem.py
--rw-r--r--   0 runner     (501) staff       (20)     2921 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/problems/xpress_problem.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/py.typed
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.897034 cvxpy-1.4.2/cvxpy/reductions/
--rw-r--r--   0 runner     (501) staff       (20)     1452 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4850 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/canonicalization.py
--rw-r--r--   0 runner     (501) staff       (20)     2667 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/chain.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.898111 cvxpy-1.4.2/cvxpy/reductions/complex2real/
--rw-r--r--   0 runner     (501) staff       (20)      566 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.904001 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     4508 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1058 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3462 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      912 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1780 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1460 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     7500 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      860 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/param_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      815 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1042 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1554 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1720 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     8221 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/complex2real/complex2real.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.906474 cvxpy-1.4.2/cvxpy/reductions/cone2cone/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cone2cone/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    17759 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cone2cone/affine2direct.py
--rw-r--r--   0 runner     (501) staff       (20)     7030 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cone2cone/approximations.py
--rw-r--r--   0 runner     (501) staff       (20)     4753 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cone2cone/exotic2common.py
--rw-r--r--   0 runner     (501) staff       (20)     6515 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cone2cone/soc2psd.py
--rw-r--r--   0 runner     (501) staff       (20)     5848 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/cvx_attr2constr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.907865 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/
--rw-r--r--   0 runner     (501) staff       (20)      564 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.923065 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     4711 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1091 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      965 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1067 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/geo_mean_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1486 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/huber_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      677 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/indicator_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      937 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/kl_div_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1194 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/lambda_max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1490 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/lambda_sum_largest_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      710 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log1p_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1049 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2282 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_det_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1685 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_sum_exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1113 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/logistic_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1220 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/matrix_frac_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1211 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/mul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1310 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/normNuc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3661 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/perspective_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2389 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1427 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1277 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1185 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      938 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/rel_entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1124 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/sigma_max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2134 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/suppfunc_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1683 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/tr_inv_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1962 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/von_neumann_entr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1149 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/xexp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)    16778 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py
--rw-r--r--   0 runner     (501) staff       (20)     5414 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dcp2cone/dcp2cone.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.924322 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.938113 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     5737 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      995 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/add_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      732 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/constant_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      101 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/div_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/exp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1434 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/eye_minus_inv_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      241 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/finite_set_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      152 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/geo_mean_canon.py
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/gmatmul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      101 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/log_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      126 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/mul_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/mulexpression_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      169 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/nonpos_constr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      253 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/norm1_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      255 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/norm_inf_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      173 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/one_minus_pos_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1015 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/parameter_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      684 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/pf_eigenvalue_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      697 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/pnorm_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      122 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      154 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/prod_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      326 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      290 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      704 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/sum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      288 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/trace_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      125 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/xexp_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      161 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/zero_constr_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     3284 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/dgp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)      273 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/util.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.939187 cvxpy-1.4.2/cvxpy/reductions/discrete2mixedint/
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/discrete2mixedint/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2750 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.941730 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/
--rw-r--r--   0 runner     (501) staff       (20)      562 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     9529 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)     3453 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/inverse.py
--rw-r--r--   0 runner     (501) staff       (20)     5154 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/sets.py
--rw-r--r--   0 runner     (501) staff       (20)     1154 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/tighten.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.942633 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/
--rw-r--r--   0 runner     (501) staff       (20)      566 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.948493 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     2000 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      748 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/abs_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1106 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/cummax_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1133 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/cumsum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1429 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/dotsort_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1333 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/max_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      765 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/maximum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      869 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/min_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      875 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/minimum_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1173 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/norm1_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1329 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/norm_inf_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      917 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/sum_largest_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1451 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py
--rw-r--r--   0 runner     (501) staff       (20)     2689 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/eval_params.py
--rw-r--r--   0 runner     (501) staff       (20)     2051 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/flip_objective.py
--rw-r--r--   0 runner     (501) staff       (20)     1944 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/inverse_data.py
--rw-r--r--   0 runner     (501) staff       (20)     2597 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/matrix_stuffing.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.950017 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/
--rw-r--r--   0 runner     (501) staff       (20)      564 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.952521 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/
--rw-r--r--   0 runner     (501) staff       (20)     2072 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1475 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/huber_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1431 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/power_canon.py
--rw-r--r--   0 runner     (501) staff       (20)      967 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/quad_form_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     1298 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/quad_over_lin_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     2379 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py
--rw-r--r--   0 runner     (501) staff       (20)    12079 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py
--rw-r--r--   0 runner     (501) staff       (20)     5050 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/reduction.py
--rw-r--r--   0 runner     (501) staff       (20)     3020 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solution.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.957603 cvxpy-1.4.2/cvxpy/reductions/solvers/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7382 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/bisection.py
--rw-r--r--   0 runner     (501) staff       (20)     3636 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/compr_matrix.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.968509 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/
--rw-r--r--   0 runner     (501) staff       (20)     1145 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7745 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    11094 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    14611 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/conic_solver.py
--rw-r--r--   0 runner     (501) staff       (20)    12853 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/copt_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    18657 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    13569 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6715 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     5058 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6658 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     8904 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glop_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     3939 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     4477 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    14366 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    32952 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     9595 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/nag_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     9445 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    15817 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scip_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    11028 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    13211 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scs_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     6623 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py
--rw-r--r--   0 runner     (501) staff       (20)    15320 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py
--rw-r--r--   0 runner     (501) staff       (20)     1085 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/constant_solver.py
--rw-r--r--   0 runner     (501) staff       (20)     5292 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/defines.py
--rw-r--r--   0 runner     (501) staff       (20)     4177 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/intermediate_chain.py
--rw-r--r--   0 runner     (501) staff       (20)     4372 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/kktsolver.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.968975 cvxpy-1.4.2/cvxpy/reductions/solvers/lp_solvers/
--rw-r--r--   0 runner     (501) staff       (20)      566 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/lp_solvers/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:11.973454 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5955 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     5766 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)    10060 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     4222 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     3773 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/piqp_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     5723 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     3557 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/qp_solver.py
--rw-r--r--   0 runner     (501) staff       (20)     9408 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py
--rw-r--r--   0 runner     (501) staff       (20)     2495 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/solver.py
--rw-r--r--   0 runner     (501) staff       (20)    18035 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/solving_chain.py
--rw-r--r--   0 runner     (501) staff       (20)     2830 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/solvers/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     6122 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/reductions/utilities.py
--rw-r--r--   0 runner     (501) staff       (20)     5232 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/settings.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.002046 cvxpy-1.4.2/cvxpy/tests/
--rw-r--r--   0 runner     (501) staff       (20)      563 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1497 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/base_test.py
--rw-r--r--   0 runner     (501) staff       (20)     1963 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/ram_limited.py
--rw-r--r--   0 runner     (501) staff       (20)    51611 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/solver_test_helpers.py
--rw-r--r--   0 runner     (501) staff       (20)    14047 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_KKT.py
--rw-r--r--   0 runner     (501) staff       (20)    73557 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)    10047 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_benchmarks.py
--rw-r--r--   0 runner     (501) staff       (20)    29369 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_complex.py
--rw-r--r--   0 runner     (501) staff       (20)    29845 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_cone2cone.py
--rw-r--r--   0 runner     (501) staff       (20)    84023 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_conic_solvers.py
--rw-r--r--   0 runner     (501) staff       (20)     1493 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_constant.py
--rw-r--r--   0 runner     (501) staff       (20)    19098 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_constant_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)    14649 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_constraints.py
--rw-r--r--   0 runner     (501) staff       (20)     7343 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_convolution.py
--rw-r--r--   0 runner     (501) staff       (20)     2983 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_copy.py
--rw-r--r--   0 runner     (501) staff       (20)     3491 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_curvature.py
--rw-r--r--   0 runner     (501) staff       (20)     3939 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_custom_solver.py
--rw-r--r--   0 runner     (501) staff       (20)    25483 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_derivative.py
--rw-r--r--   0 runner     (501) staff       (20)     7749 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_dgp.py
--rw-r--r--   0 runner     (501) staff       (20)    27264 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_dgp2dcp.py
--rw-r--r--   0 runner     (501) staff       (20)     7197 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_domain.py
--rw-r--r--   0 runner     (501) staff       (20)    32906 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_dpp.py
--rw-r--r--   0 runner     (501) staff       (20)    26488 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_dqcp.py
--rw-r--r--   0 runner     (501) staff       (20)     3900 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_errors.py
--rw-r--r--   0 runner     (501) staff       (20)    21418 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_examples.py
--rw-r--r--   0 runner     (501) staff       (20)    14401 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_expression_methods.py
--rw-r--r--   0 runner     (501) staff       (20)    53751 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_expressions.py
--rw-r--r--   0 runner     (501) staff       (20)    32554 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_grad.py
--rw-r--r--   0 runner     (501) staff       (20)     1570 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_gurobi_write.py
--rw-r--r--   0 runner     (501) staff       (20)     7545 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_interfaces.py
--rw-r--r--   0 runner     (501) staff       (20)     7671 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_kron_canon.py
--rw-r--r--   0 runner     (501) staff       (20)     4949 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_lin_ops.py
--rw-r--r--   0 runner     (501) staff       (20)     2637 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_linalg_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    16619 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_linear_cone.py
--rw-r--r--   0 runner     (501) staff       (20)     5135 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_matrices.py
--rw-r--r--   0 runner     (501) staff       (20)     4090 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_mip_vars.py
--rw-r--r--   0 runner     (501) staff       (20)     2993 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_monotonicity.py
--rw-r--r--   0 runner     (501) staff       (20)     6616 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_nonlinear_atoms.py
--rw-r--r--   0 runner     (501) staff       (20)     4985 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_objectives.py
--rw-r--r--   0 runner     (501) staff       (20)     4260 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_param_cone_prog.py
--rw-r--r--   0 runner     (501) staff       (20)     4223 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_param_quad_prog.py
--rw-r--r--   0 runner     (501) staff       (20)    13315 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_perspective.py
--rw-r--r--   0 runner     (501) staff       (20)     4337 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_power_tools.py
--rw-r--r--   0 runner     (501) staff       (20)    85390 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_problem.py
--rw-r--r--   0 runner     (501) staff       (20)    69327 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_python_backends.py
--rw-r--r--   0 runner     (501) staff       (20)    22394 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_qp_solvers.py
--rw-r--r--   0 runner     (501) staff       (20)     7929 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_quad_form.py
--rw-r--r--   0 runner     (501) staff       (20)     6631 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_quadratic.py
--rw-r--r--   0 runner     (501) staff       (20)     5931 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_scalarize.py
--rw-r--r--   0 runner     (501) staff       (20)     3247 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_semidefinite_vars.py
--rw-r--r--   0 runner     (501) staff       (20)     3992 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_shape.py
--rw-r--r--   0 runner     (501) staff       (20)     2694 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_sign.py
--rw-r--r--   0 runner     (501) staff       (20)     7775 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_suppfunc.py
--rw-r--r--   0 runner     (501) staff       (20)    14254 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_valinvec2mixedint.py
--rw-r--r--   0 runner     (501) staff       (20)     1901 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_versioning.py
--rw-r--r--   0 runner     (501) staff       (20)     9116 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/tests/test_von_neumann_entr.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.005013 cvxpy-1.4.2/cvxpy/transforms/
--rw-r--r--   0 runner     (501) staff       (20)      996 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3670 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/indicator.py
--rw-r--r--   0 runner     (501) staff       (20)     2088 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/linearize.py
--rw-r--r--   0 runner     (501) staff       (20)    10918 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/partial_optimize.py
--rw-r--r--   0 runner     (501) staff       (20)     5056 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/scalarize.py
--rw-r--r--   0 runner     (501) staff       (20)     6761 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/transforms/suppfunc.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.013266 cvxpy-1.4.2/cvxpy/utilities/
--rw-r--r--   0 runner     (501) staff       (20)      629 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5446 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/canonical.py
--rw-r--r--   0 runner     (501) staff       (20)    15044 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/coeff_extractor.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.013729 cvxpy-1.4.2/cvxpy/utilities/cpp/
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/cpp/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.014629 cvxpy-1.4.2/cvxpy/utilities/cpp/sparsecholesky/
--rw-r--r--   0 runner     (501) staff       (20)       36 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/cpp/sparsecholesky/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3778 2024-01-19 02:11:42.000000 cvxpy-1.4.2/cvxpy/utilities/cpp/sparsecholesky/main.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2968 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/cvxpy_upgrade.py
--rw-r--r--   0 runner     (501) staff       (20)     3264 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/debug_tools.py
--rw-r--r--   0 runner     (501) staff       (20)      245 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/deterministic.py
--rw-r--r--   0 runner     (501) staff       (20)     1424 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/grad.py
--rw-r--r--   0 runner     (501) staff       (20)     6226 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/key_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     8922 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/linalg.py
--rw-r--r--   0 runner     (501) staff       (20)     2437 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/performance_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2178 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/perspective_utils.py
--rw-r--r--   0 runner     (501) staff       (20)    19336 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/power_tools.py
--rw-r--r--   0 runner     (501) staff       (20)     1552 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/replace_quad_forms.py
--rw-r--r--   0 runner     (501) staff       (20)     1399 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/scopes.py
--rw-r--r--   0 runner     (501) staff       (20)     4983 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/shape.py
--rw-r--r--   0 runner     (501) staff       (20)     1968 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/sign.py
--rw-r--r--   0 runner     (501) staff       (20)     1825 2024-01-19 02:11:43.000000 cvxpy-1.4.2/cvxpy/utilities/versioning.py
--rw-r--r--   0 runner     (501) staff       (20)      213 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.016579 cvxpy-1.4.2/cvxpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     8760 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    35727 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-19 02:13:05.000000 cvxpy-1.4.2/cvxpy.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      430 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       43 2024-01-19 02:18:11.000000 cvxpy-1.4.2/cvxpy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1212 2024-01-19 02:11:43.000000 cvxpy-1.4.2/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-19 02:18:12.015998 cvxpy-1.4.2/setup/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-19 02:11:43.000000 cvxpy-1.4.2/setup/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1810 2024-01-19 02:11:43.000000 cvxpy-1.4.2/setup/extensions.py
--rw-r--r--   0 runner     (501) staff       (20)     4833 2024-01-19 02:11:43.000000 cvxpy-1.4.2/setup/versioning.py
--rw-r--r--   0 runner     (501) staff       (20)      398 2024-01-19 02:18:12.021410 cvxpy-1.4.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     3196 2024-01-19 02:11:43.000000 cvxpy-1.4.2/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.716191 cvxpy-1.4.3/
+-rw-r--r--   0 runner     (501) staff       (20)    11344 2024-04-16 08:04:14.000000 cvxpy-1.4.3/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      102 2024-04-16 08:04:14.000000 cvxpy-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     8760 2024-04-16 08:08:50.715794 cvxpy-1.4.3/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6950 2024-04-16 08:04:14.000000 cvxpy-1.4.3/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.224555 cvxpy-1.4.3/cvxpy/
+-rw-r--r--   0 runner     (501) staff       (20)     3001 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.251641 cvxpy-1.4.3/cvxpy/atoms/
+-rw-r--r--   0 runner     (501) staff       (20)     5385 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.264913 cvxpy-1.4.3/cvxpy/atoms/affine/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3967 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/add_expr.py
+-rw-r--r--   0 runner     (501) staff       (20)     5719 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/affine_atom.py
+-rw-r--r--   0 runner     (501) staff       (20)    15481 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/binary_operators.py
+-rw-r--r--   0 runner     (501) staff       (20)     1137 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/bmat.py
+-rw-r--r--   0 runner     (501) staff       (20)     2313 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/conj.py
+-rw-r--r--   0 runner     (501) staff       (20)     6168 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/conv.py
+-rw-r--r--   0 runner     (501) staff       (20)     4371 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/cumsum.py
+-rw-r--r--   0 runner     (501) staff       (20)     5357 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/diag.py
+-rw-r--r--   0 runner     (501) staff       (20)     1644 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/diff.py
+-rw-r--r--   0 runner     (501) staff       (20)     2977 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/hstack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1459 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/imag.py
+-rw-r--r--   0 runner     (501) staff       (20)     6401 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/index.py
+-rw-r--r--   0 runner     (501) staff       (20)     4379 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/kron.py
+-rw-r--r--   0 runner     (501) staff       (20)     3310 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/partial_trace.py
+-rw-r--r--   0 runner     (501) staff       (20)     3370 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/partial_transpose.py
+-rw-r--r--   0 runner     (501) staff       (20)     3204 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/promote.py
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/real.py
+-rw-r--r--   0 runner     (501) staff       (20)     5340 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/reshape.py
+-rw-r--r--   0 runner     (501) staff       (20)     3553 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/sum.py
+-rw-r--r--   0 runner     (501) staff       (20)     2937 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/trace.py
+-rw-r--r--   0 runner     (501) staff       (20)     2872 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/transpose.py
+-rw-r--r--   0 runner     (501) staff       (20)     2752 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/unary_operators.py
+-rw-r--r--   0 runner     (501) staff       (20)     4701 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/upper_tri.py
+-rw-r--r--   0 runner     (501) staff       (20)     1108 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/vec.py
+-rw-r--r--   0 runner     (501) staff       (20)     3033 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/vstack.py
+-rw-r--r--   0 runner     (501) staff       (20)     4182 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/affine/wraps.py
+-rw-r--r--   0 runner     (501) staff       (20)    16154 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/atom.py
+-rw-r--r--   0 runner     (501) staff       (20)     4313 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/axis_atom.py
+-rw-r--r--   0 runner     (501) staff       (20)     3132 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/condition_number.py
+-rw-r--r--   0 runner     (501) staff       (20)     2943 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/cummax.py
+-rw-r--r--   0 runner     (501) staff       (20)     2423 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/dist_ratio.py
+-rw-r--r--   0 runner     (501) staff       (20)     4928 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/dotsort.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.276686 cvxpy-1.4.3/cvxpy/atoms/elementwise/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2457 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/abs.py
+-rw-r--r--   0 runner     (501) staff       (20)     4790 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/ceil.py
+-rw-r--r--   0 runner     (501) staff       (20)     2414 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/elementwise.py
+-rw-r--r--   0 runner     (501) staff       (20)     2746 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/entr.py
+-rw-r--r--   0 runner     (501) staff       (20)     2358 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/exp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3520 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/huber.py
+-rw-r--r--   0 runner     (501) staff       (20)      703 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/inv_pos.py
+-rw-r--r--   0 runner     (501) staff       (20)     3009 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/kl_div.py
+-rw-r--r--   0 runner     (501) staff       (20)     2757 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/log.py
+-rw-r--r--   0 runner     (501) staff       (20)     2046 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/log1p.py
+-rw-r--r--   0 runner     (501) staff       (20)     2036 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/log_normcdf.py
+-rw-r--r--   0 runner     (501) staff       (20)     1417 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/loggamma.py
+-rw-r--r--   0 runner     (501) staff       (20)     2345 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/logistic.py
+-rw-r--r--   0 runner     (501) staff       (20)     3519 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/maximum.py
+-rw-r--r--   0 runner     (501) staff       (20)     3222 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/minimum.py
+-rw-r--r--   0 runner     (501) staff       (20)      699 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/neg.py
+-rw-r--r--   0 runner     (501) staff       (20)      696 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/pos.py
+-rw-r--r--   0 runner     (501) staff       (20)    14794 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     2988 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/rel_entr.py
+-rw-r--r--   0 runner     (501) staff       (20)      779 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/scalene.py
+-rw-r--r--   0 runner     (501) staff       (20)      739 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/sqrt.py
+-rw-r--r--   0 runner     (501) staff       (20)      691 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/square.py
+-rw-r--r--   0 runner     (501) staff       (20)     2682 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/elementwise/xexp.py
+-rw-r--r--   0 runner     (501) staff       (20)      243 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/errormsg.py
+-rw-r--r--   0 runner     (501) staff       (20)     3300 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/eye_minus_inv.py
+-rw-r--r--   0 runner     (501) staff       (20)     3518 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/gen_lambda_max.py
+-rw-r--r--   0 runner     (501) staff       (20)    12147 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/geo_mean.py
+-rw-r--r--   0 runner     (501) staff       (20)     4909 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/gmatmul.py
+-rw-r--r--   0 runner     (501) staff       (20)     1292 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/harmonic_mean.py
+-rw-r--r--   0 runner     (501) staff       (20)     1197 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/inv_prod.py
+-rw-r--r--   0 runner     (501) staff       (20)     3291 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/lambda_max.py
+-rw-r--r--   0 runner     (501) staff       (20)      811 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/lambda_min.py
+-rw-r--r--   0 runner     (501) staff       (20)     2318 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/lambda_sum_largest.py
+-rw-r--r--   0 runner     (501) staff       (20)      834 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/lambda_sum_smallest.py
+-rw-r--r--   0 runner     (501) staff       (20)     2324 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/length.py
+-rw-r--r--   0 runner     (501) staff       (20)     3645 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/log_det.py
+-rw-r--r--   0 runner     (501) staff       (20)     2690 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/log_sum_exp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4538 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/matrix_frac.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/max.py
+-rw-r--r--   0 runner     (501) staff       (20)     3632 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/min.py
+-rw-r--r--   0 runner     (501) staff       (20)     1304 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/mixed_norm.py
+-rw-r--r--   0 runner     (501) staff       (20)     3363 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/norm.py
+-rw-r--r--   0 runner     (501) staff       (20)     3212 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/norm1.py
+-rw-r--r--   0 runner     (501) staff       (20)     3376 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/norm_inf.py
+-rw-r--r--   0 runner     (501) staff       (20)     2271 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/norm_nuc.py
+-rw-r--r--   0 runner     (501) staff       (20)     2801 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/one_minus_pos.py
+-rw-r--r--   0 runner     (501) staff       (20)     4730 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/perspective.py
+-rw-r--r--   0 runner     (501) staff       (20)     2694 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/pf_eigenvalue.py
+-rw-r--r--   0 runner     (501) staff       (20)     8451 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/pnorm.py
+-rw-r--r--   0 runner     (501) staff       (20)     4180 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/prod.py
+-rw-r--r--   0 runner     (501) staff       (20)      975 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/ptp.py
+-rw-r--r--   0 runner     (501) staff       (20)     8139 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/quad_form.py
+-rw-r--r--   0 runner     (501) staff       (20)     4351 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/quad_over_lin.py
+-rw-r--r--   0 runner     (501) staff       (20)     2381 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/sigma_max.py
+-rw-r--r--   0 runner     (501) staff       (20)     2121 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     2179 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     3117 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/sum_largest.py
+-rw-r--r--   0 runner     (501) staff       (20)      802 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/sum_smallest.py
+-rw-r--r--   0 runner     (501) staff       (20)      930 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/sum_squares.py
+-rw-r--r--   0 runner     (501) staff       (20)     4048 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/suppfunc.py
+-rw-r--r--   0 runner     (501) staff       (20)     2101 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/total_variation.py
+-rw-r--r--   0 runner     (501) staff       (20)     3832 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/tr_inv.py
+-rw-r--r--   0 runner     (501) staff       (20)     3821 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/atoms/von_neumann_entr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.281964 cvxpy-1.4.3/cvxpy/constraints/
+-rw-r--r--   0 runner     (501) staff       (20)     1122 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2303 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/cones.py
+-rw-r--r--   0 runner     (501) staff       (20)     7254 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/constraint.py
+-rw-r--r--   0 runner     (501) staff       (20)    13846 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/exponential.py
+-rw-r--r--   0 runner     (501) staff       (20)     4576 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/finite_set.py
+-rw-r--r--   0 runner     (501) staff       (20)     7905 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/nonpos.py
+-rw-r--r--   0 runner     (501) staff       (20)    11646 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/power.py
+-rw-r--r--   0 runner     (501) staff       (20)     3242 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/psd.py
+-rw-r--r--   0 runner     (501) staff       (20)     6030 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/second_order.py
+-rw-r--r--   0 runner     (501) staff       (20)     3831 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     5264 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/constraints/zero.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.282427 cvxpy-1.4.3/cvxpy/cvxcore/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.198065 cvxpy-1.4.3/cvxpy/cvxcore/include/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.297698 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/
+-rw-r--r--   0 runner     (501) staff       (20)      694 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/CMakeLists.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1161 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Cholesky
+-rw-r--r--   0 runner     (501) staff       (20)     1900 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/CholmodSupport
+-rw-r--r--   0 runner     (501) staff       (20)    12799 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Core
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Dense
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Eigen
+-rw-r--r--   0 runner     (501) staff       (20)     1777 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Eigenvalues
+-rw-r--r--   0 runner     (501) staff       (20)     1940 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Geometry
+-rw-r--r--   0 runner     (501) staff       (20)      829 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Householder
+-rw-r--r--   0 runner     (501) staff       (20)     2083 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers
+-rw-r--r--   0 runner     (501) staff       (20)      894 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Jacobi
+-rw-r--r--   0 runner     (501) staff       (20)     1389 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/KLUSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1268 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/LU
+-rw-r--r--   0 runner     (501) staff       (20)      991 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/MetisSupport
+-rw-r--r--   0 runner     (501) staff       (20)     2451 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/OrderingMethods
+-rw-r--r--   0 runner     (501) staff       (20)     1751 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/PaStiXSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1116 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/PardisoSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1272 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/QR
+-rw-r--r--   0 runner     (501) staff       (20)      900 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc
+-rw-r--r--   0 runner     (501) staff       (20)     1162 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SPQRSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1584 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SVD
+-rw-r--r--   0 runner     (501) staff       (20)      888 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Sparse
+-rw-r--r--   0 runner     (501) staff       (20)     1235 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseCholesky
+-rw-r--r--   0 runner     (501) staff       (20)     2240 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseCore
+-rw-r--r--   0 runner     (501) staff       (20)     1814 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseLU
+-rw-r--r--   0 runner     (501) staff       (20)     1195 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseQR
+-rw-r--r--   0 runner     (501) staff       (20)      797 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdDeque
+-rw-r--r--   0 runner     (501) staff       (20)      726 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdList
+-rw-r--r--   0 runner     (501) staff       (20)      803 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdVector
+-rw-r--r--   0 runner     (501) staff       (20)     2243 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SuperLUSupport
+-rw-r--r--   0 runner     (501) staff       (20)     1382 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/UmfPackSupport
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.210806 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.299262 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24934 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h
+-rw-r--r--   0 runner     (501) staff       (20)    18760 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h
+-rw-r--r--   0 runner     (501) staff       (20)     3974 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.299848 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    25441 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.337909 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/
+-rw-r--r--   0 runner     (501) staff       (20)    19214 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArithmeticSequence.h
+-rw-r--r--   0 runner     (501) staff       (20)    16782 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Array.h
+-rw-r--r--   0 runner     (501) staff       (20)     8217 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7018 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h
+-rw-r--r--   0 runner     (501) staff       (20)     2738 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h
+-rw-r--r--   0 runner     (501) staff       (20)    41673 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    12488 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h
+-rw-r--r--   0 runner     (501) staff       (20)    14075 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    18648 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Block.h
+-rw-r--r--   0 runner     (501) staff       (20)     4429 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)     5981 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h
+-rw-r--r--   0 runner     (501) staff       (20)     6990 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h
+-rw-r--r--   0 runner     (501) staff       (20)    63841 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     4745 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h
+-rw-r--r--   0 runner     (501) staff       (20)     7909 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    36282 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     8256 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     3937 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     5551 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h
+-rw-r--r--   0 runner     (501) staff       (20)    31529 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    24484 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    25360 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)     9870 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h
+-rw-r--r--   0 runner     (501) staff       (20)    14670 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)      988 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    11654 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h
+-rw-r--r--   0 runner     (501) staff       (20)     5841 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     4909 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h
+-rw-r--r--   0 runner     (501) staff       (20)     5759 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    21679 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)    38812 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    11543 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     8238 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/IO.h
+-rw-r--r--   0 runner     (501) staff       (20)     9620 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/IndexedView.h
+-rw-r--r--   0 runner     (501) staff       (20)     3503 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     7256 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Map.h
+-rw-r--r--   0 runner     (501) staff       (20)    11281 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    60784 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     7156 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    24343 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    23856 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     2520 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     3620 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h
+-rw-r--r--   0 runner     (501) staff       (20)    12884 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h
+-rw-r--r--   0 runner     (501) staff       (20)     9207 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PartialReduxEvaluator.h
+-rw-r--r--   0 runner     (501) staff       (20)    20748 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    49193 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7336 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Product.h
+-rw-r--r--   0 runner     (501) staff       (20)    53832 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h
+-rw-r--r--   0 runner     (501) staff       (20)     7756 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Random.h
+-rw-r--r--   0 runner     (501) staff       (20)    19195 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h
+-rw-r--r--   0 runner     (501) staff       (20)    17821 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h
+-rw-r--r--   0 runner     (501) staff       (20)     5656 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h
+-rw-r--r--   0 runner     (501) staff       (20)    17033 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Reshaped.h
+-rw-r--r--   0 runner     (501) staff       (20)     4284 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h
+-rw-r--r--   0 runner     (501) staff       (20)     7522 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h
+-rw-r--r--   0 runner     (501) staff       (20)     6143 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Select.h
+-rw-r--r--   0 runner     (501) staff       (20)    14999 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     1697 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     6837 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h
+-rw-r--r--   0 runner     (501) staff       (20)     9368 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     6170 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     8700 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h
+-rw-r--r--   0 runner     (501) staff       (20)    21641 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/StlIterators.h
+-rw-r--r--   0 runner     (501) staff       (20)     4212 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h
+-rw-r--r--   0 runner     (501) staff       (20)     2765 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h
+-rw-r--r--   0 runner     (501) staff       (20)    17606 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h
+-rw-r--r--   0 runner     (501) staff       (20)    13567 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h
+-rw-r--r--   0 runner     (501) staff       (20)    38277 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     3488 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)    35168 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    11997 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.202986 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.340164 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/
+-rw-r--r--   0 runner     (501) staff       (20)    15223 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     8102 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    64608 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2564 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.342437 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/
+-rw-r--r--   0 runner     (501) staff       (20)    17160 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    13344 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    87891 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2134 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.345814 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/
+-rw-r--r--   0 runner     (501) staff       (20)    16540 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     2323 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)   119355 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     9490 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h
+-rw-r--r--   0 runner     (501) staff       (20)    24820 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h
+-rwxr-xr-x   0 runner     (501) staff       (20)   102394 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.349296 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/
+-rw-r--r--   0 runner     (501) staff       (20)    17317 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    23547 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h
+-rw-r--r--   0 runner     (501) staff       (20)     2387 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    10744 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    35476 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h
+-rw-r--r--   0 runner     (501) staff       (20)     5509 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.353295 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/
+-rw-r--r--   0 runner     (501) staff       (20)    26903 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/BFloat16.h
+-rw-r--r--   0 runner     (501) staff       (20)     5251 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    67696 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)     3770 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h
+-rw-r--r--   0 runner     (501) staff       (20)    35534 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Half.h
+-rw-r--r--   0 runner     (501) staff       (20)     1746 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h
+-rw-r--r--   0 runner     (501) staff       (20)     3746 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.354903 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/
+-rw-r--r--   0 runner     (501) staff       (20)     2695 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    57047 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     2256 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.201376 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.355453 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/
+-rw-r--r--   0 runner     (501) staff       (20)      691 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/math_constants.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.356954 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/
+-rw-r--r--   0 runner     (501) staff       (20)    17541 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)    16159 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    33615 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.360111 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/
+-rw-r--r--   0 runner     (501) staff       (20)    22503 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     6815 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     3083 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)   189525 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    51286 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.362387 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/
+-rw-r--r--   0 runner     (501) staff       (20)    14251 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     6765 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    64465 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.364007 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    21200 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.366727 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/
+-rw-r--r--   0 runner     (501) staff       (20)     7428 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/InteropHeaders.h
+-rw-r--r--   0 runner     (501) staff       (20)    12539 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/MathFunctions.h
+-rw-r--r--   0 runner     (501) staff       (20)    27786 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/PacketMath.h
+-rw-r--r--   0 runner     (501) staff       (20)    21856 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h
+-rw-r--r--   0 runner     (501) staff       (20)     2626 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/TypeCasting.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.368323 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/
+-rw-r--r--   0 runner     (501) staff       (20)    16728 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h
+-rw-r--r--   0 runner     (501) staff       (20)     8024 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    36894 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.371459 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/
+-rw-r--r--   0 runner     (501) staff       (20)     6686 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    20921 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     8334 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)     4998 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)      607 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h
+-rw-r--r--   0 runner     (501) staff       (20)    40146 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.382875 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/
+-rw-r--r--   0 runner     (501) staff       (20)   108448 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h
+-rw-r--r--   0 runner     (501) staff       (20)    20104 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    15948 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h
+-rw-r--r--   0 runner     (501) staff       (20)     6936 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5106 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    21724 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     6368 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5582 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h
+-rw-r--r--   0 runner     (501) staff       (20)    21354 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    11570 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     9958 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     5209 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     6164 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     4126 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h
+-rw-r--r--   0 runner     (501) staff       (20)    20987 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    13867 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14722 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h
+-rw-r--r--   0 runner     (501) staff       (20)    10571 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)    14678 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     6707 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h
+-rw-r--r--   0 runner     (501) staff       (20)     5882 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.392244 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/
+-rwxr-xr-x   0 runner     (501) staff       (20)    23156 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    19876 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ConfigureVectorization.h
+-rw-r--r--   0 runner     (501) staff       (20)    21931 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4892 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)    15555 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h
+-rw-r--r--   0 runner     (501) staff       (20)     6696 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/IndexedViewHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    10949 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/IntegralConstant.h
+-rwxr-xr-x   0 runner     (501) staff       (20)     4268 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h
+-rw-r--r--   0 runner     (501) staff       (20)    52909 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h
+-rw-r--r--   0 runner     (501) staff       (20)    46661 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h
+-rwxr-xr-x   0 runner     (501) staff       (20)    29336 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h
+-rw-r--r--   0 runner     (501) staff       (20)       85 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/NonMPL2.h
+-rw-r--r--   0 runner     (501) staff       (20)     1024 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h
+-rw-r--r--   0 runner     (501) staff       (20)     1432 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ReshapedHelper.h
+-rw-r--r--   0 runner     (501) staff       (20)    10676 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h
+-rw-r--r--   0 runner     (501) staff       (20)    12003 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/SymbolicIndex.h
+-rw-r--r--   0 runner     (501) staff       (20)    35762 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.400056 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/
+-rw-r--r--   0 runner     (501) staff       (20)    12559 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17274 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     4178 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22970 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    17176 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     9716 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)    14349 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)     5575 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h
+-rw-r--r--   0 runner     (501) staff       (20)    23640 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h
+-rw-r--r--   0 runner     (501) staff       (20)    21078 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h
+-rw-r--r--   0 runner     (501) staff       (20)     3650 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    35182 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h
+-rw-r--r--   0 runner     (501) staff       (20)     4104 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    22764 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.407606 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/
+-rw-r--r--   0 runner     (501) staff       (20)    18939 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h
+-rw-r--r--   0 runner     (501) staff       (20)     8403 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h
+-rw-r--r--   0 runner     (501) staff       (20)     3624 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h
+-rw-r--r--   0 runner     (501) staff       (20)    20726 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h
+-rw-r--r--   0 runner     (501) staff       (20)    11962 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h
+-rw-r--r--   0 runner     (501) staff       (20)     8955 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     9812 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h
+-rw-r--r--   0 runner     (501) staff       (20)    34367 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h
+-rw-r--r--   0 runner     (501) staff       (20)     6862 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h
+-rw-r--r--   0 runner     (501) staff       (20)     8063 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     6724 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h
+-rw-r--r--   0 runner     (501) staff       (20)    61930 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h
+-rw-r--r--   0 runner     (501) staff       (20)     7664 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h
+-rw-r--r--   0 runner     (501) staff       (20)     6190 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.408647 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/
+-rw-r--r--   0 runner     (501) staff       (20)     5945 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SIMD.h
+-rw-r--r--   0 runner     (501) staff       (20)     5387 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.410157 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/
+-rw-r--r--   0 runner     (501) staff       (20)     4784 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h
+-rw-r--r--   0 runner     (501) staff       (20)     5365 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h
+-rw-r--r--   0 runner     (501) staff       (20)    23611 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.414283 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/
+-rw-r--r--   0 runner     (501) staff       (20)     6771 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h
+-rw-r--r--   0 runner     (501) staff       (20)     6850 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h
+-rw-r--r--   0 runner     (501) staff       (20)     8887 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)    15036 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)    14940 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h
+-rw-r--r--   0 runner     (501) staff       (20)    13379 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7349 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h
+-rw-r--r--   0 runner     (501) staff       (20)     4212 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.414778 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Jacobi/
+-rw-r--r--   0 runner     (501) staff       (20)    16383 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.415267 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/KLUSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    11555 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/KLUSupport/KLUSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.418121 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/
+-rw-r--r--   0 runner     (501) staff       (20)     3439 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h
+-rw-r--r--   0 runner     (501) staff       (20)    32383 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)    15727 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)    22069 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     3555 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.419492 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/arch/
+-rw-r--r--   0 runner     (501) staff       (20)    13693 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/arch/InverseSize4.h
+-rw-r--r--   0 runner     (501) staff       (20)    13662 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.420014 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/MetisSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     4588 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.421774 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/
+-rw-r--r--   0 runner     (501) staff       (20)    16105 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h
+-rw-r--r--   0 runner     (501) staff       (20)    61681 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h
+-rw-r--r--   0 runner     (501) staff       (20)     5248 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.422247 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    22249 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.422786 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    20092 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.426341 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/
+-rw-r--r--   0 runner     (501) staff       (20)    25498 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     4662 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    23429 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h
+-rw-r--r--   0 runner     (501) staff       (20)    26768 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)    14641 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.426807 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    11826 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.438011 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/
+-rw-r--r--   0 runner     (501) staff       (20)    54214 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)    32988 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h
+-rw-r--r--   0 runner     (501) staff       (20)     5099 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h
+-rw-r--r--   0 runner     (501) staff       (20)    14743 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    15957 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.444796 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/
+-rw-r--r--   0 runner     (501) staff       (20)    24216 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h
+-rw-r--r--   0 runner     (501) staff       (20)     5830 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.463449 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/
+-rw-r--r--   0 runner     (501) staff       (20)    10670 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8743 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h
+-rw-r--r--   0 runner     (501) staff       (20)    13166 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     2191 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    11368 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h
+-rw-r--r--   0 runner     (501) staff       (20)    24360 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h
+-rw-r--r--   0 runner     (501) staff       (20)     6485 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h
+-rw-r--r--   0 runner     (501) staff       (20)    13606 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h
+-rw-r--r--   0 runner     (501) staff       (20)    25524 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)     4757 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h
+-rw-r--r--   0 runner     (501) staff       (20)    13256 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     5808 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     3080 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h
+-rw-r--r--   0 runner     (501) staff       (20)     1107 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h
+-rw-r--r--   0 runner     (501) staff       (20)    12589 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h
+-rw-r--r--   0 runner     (501) staff       (20)    57475 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)    17451 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     7329 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h
+-rw-r--r--   0 runner     (501) staff       (20)     7593 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h
+-rw-r--r--   0 runner     (501) staff       (20)     1699 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h
+-rw-r--r--   0 runner     (501) staff       (20)    15600 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h
+-rw-r--r--   0 runner     (501) staff       (20)    25889 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h
+-rw-r--r--   0 runner     (501) staff       (20)     4424 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h
+-rw-r--r--   0 runner     (501) staff       (20)     8704 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h
+-rw-r--r--   0 runner     (501) staff       (20)     3175 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h
+-rw-r--r--   0 runner     (501) staff       (20)     6437 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h
+-rw-r--r--   0 runner     (501) staff       (20)     6827 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h
+-rw-r--r--   0 runner     (501) staff       (20)    14832 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     8127 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h
+-rw-r--r--   0 runner     (501) staff       (20)     9657 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.471781 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/
+-rw-r--r--   0 runner     (501) staff       (20)    33316 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h
+-rw-r--r--   0 runner     (501) staff       (20)     4303 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h
+-rw-r--r--   0 runner     (501) staff       (20)     7602 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h
+-rw-r--r--   0 runner     (501) staff       (20)     4974 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h
+-rw-r--r--   0 runner     (501) staff       (20)    12837 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h
+-rw-r--r--   0 runner     (501) staff       (20)     2049 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h
+-rw-r--r--   0 runner     (501) staff       (20)     6712 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     6584 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     3681 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h
+-rw-r--r--   0 runner     (501) staff       (20)    10217 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     4181 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h
+-rw-r--r--   0 runner     (501) staff       (20)     5723 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     8485 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h
+-rw-r--r--   0 runner     (501) staff       (20)     9028 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h
+-rw-r--r--   0 runner     (501) staff       (20)     4979 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h
+-rw-r--r--   0 runner     (501) staff       (20)     4545 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.472231 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseQR/
+-rw-r--r--   0 runner     (501) staff       (20)    29167 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.474355 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/
+-rw-r--r--   0 runner     (501) staff       (20)     4730 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h
+-rw-r--r--   0 runner     (501) staff       (20)     4155 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h
+-rw-r--r--   0 runner     (501) staff       (20)     5338 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h
+-rw-r--r--   0 runner     (501) staff       (20)     2809 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.474839 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    34324 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.475441 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/
+-rw-r--r--   0 runner     (501) staff       (20)    24456 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.481556 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/
+-rw-r--r--   0 runner     (501) staff       (20)     2913 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/Image.h
+-rw-r--r--   0 runner     (501) staff       (20)     2742 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h
+-rw-r--r--   0 runner     (501) staff       (20)     1748 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h
+-rw-r--r--   0 runner     (501) staff       (20)    30560 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/blas.h
+-rw-r--r--   0 runner     (501) staff       (20)     7834 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h
+-rwxr-xr-x   0 runner     (501) staff       (20)  1058369 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h
+-rw-r--r--   0 runner     (501) staff       (20)      474 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/lapacke_mangling.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.486284 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/
+-rw-r--r--   0 runner     (501) staff       (20)    14060 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    21431 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    59020 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     4828 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     6089 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)    12283 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/IndexedViewMethods.h
+-rw-r--r--   0 runner     (501) staff       (20)     6387 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     3350 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h
+-rw-r--r--   0 runner     (501) staff       (20)     6915 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ReshapedMethods.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.491871 cvxpy-1.4.3/cvxpy/cvxcore/python/
+-rw-r--r--   0 runner     (501) staff       (20)      316 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    20241 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/canonInterface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2403 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore.i
+-rw-r--r--   0 runner     (501) staff       (20)    28678 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore.py
+-rw-r--r--   0 runner     (501) staff       (20)   881862 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore_wrap.cxx
+-rw-r--r--   0 runner     (501) staff       (20)    54061 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/python/numpy.i
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.497495 cvxpy-1.4.3/cvxpy/cvxcore/src/
+-rw-r--r--   0 runner     (501) staff       (20)       24 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/.keep
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/LinOp.hpp
+-rw-r--r--   0 runner     (501) staff       (20)    39627 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/LinOpOperations.cpp
+-rw-r--r--   0 runner     (501) staff       (20)      844 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/LinOpOperations.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     3365 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/ProblemData.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     5057 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/Utils.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1454 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/Utils.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     8098 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/cvxcore.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     1351 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/cvxcore/src/cvxcore.hpp
+-rw-r--r--   0 runner     (501) staff       (20)     1299 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/error.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.500537 cvxpy-1.4.3/cvxpy/expressions/
+-rw-r--r--   0 runner     (501) staff       (20)      590 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.502718 cvxpy-1.4.3/cvxpy/expressions/constants/
+-rw-r--r--   0 runner     (501) staff       (20)      670 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/constants/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1729 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/constants/callback_param.py
+-rw-r--r--   0 runner     (501) staff       (20)     8063 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/constants/constant.py
+-rw-r--r--   0 runner     (501) staff       (20)     3737 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/constants/parameter.py
+-rw-r--r--   0 runner     (501) staff       (20)     3421 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/cvxtypes.py
+-rw-r--r--   0 runner     (501) staff       (20)    27398 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    16595 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/leaf.py
+-rw-r--r--   0 runner     (501) staff       (20)     4202 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/expressions/variable.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.504169 cvxpy-1.4.3/cvxpy/interface/
+-rw-r--r--   0 runner     (501) staff       (20)      611 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5171 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/base_matrix_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)    10925 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/matrix_utilities.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.506220 cvxpy-1.4.3/cvxpy/interface/numpy_interface/
+-rw-r--r--   0 runner     (501) staff       (20)      818 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/numpy_interface/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2058 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/numpy_interface/matrix_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2527 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/numpy_interface/ndarray_interface.py
+-rw-r--r--   0 runner     (501) staff       (20)     3446 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/interface/numpy_interface/sparse_matrix_interface.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.509412 cvxpy-1.4.3/cvxpy/lin_ops/
+-rw-r--r--   0 runner     (501) staff       (20)      684 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    74815 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/canon_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)     1126 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/lin_constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)     3402 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/lin_op.py
+-rw-r--r--   0 runner     (501) staff       (20)    18699 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/lin_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    12117 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/lin_ops/tree_mat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.512902 cvxpy-1.4.3/cvxpy/problems/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4958 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/iterative.py
+-rw-r--r--   0 runner     (501) staff       (20)     7339 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/objective.py
+-rw-r--r--   0 runner     (501) staff       (20)     1615 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/param_prob.py
+-rw-r--r--   0 runner     (501) staff       (20)    63502 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/problem.py
+-rw-r--r--   0 runner     (501) staff       (20)     2921 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/problems/xpress_problem.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/py.typed
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.528406 cvxpy-1.4.3/cvxpy/reductions/
+-rw-r--r--   0 runner     (501) staff       (20)     1452 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4850 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/canonicalization.py
+-rw-r--r--   0 runner     (501) staff       (20)     2667 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/chain.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.536158 cvxpy-1.4.3/cvxpy/reductions/complex2real/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.582506 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4508 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1058 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3462 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      912 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1780 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1460 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     7500 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      860 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/param_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      815 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1042 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1554 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1720 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     8221 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/complex2real/complex2real.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.585201 cvxpy-1.4.3/cvxpy/reductions/cone2cone/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cone2cone/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    17759 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cone2cone/affine2direct.py
+-rw-r--r--   0 runner     (501) staff       (20)     7030 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cone2cone/approximations.py
+-rw-r--r--   0 runner     (501) staff       (20)     4753 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cone2cone/exotic2common.py
+-rw-r--r--   0 runner     (501) staff       (20)     6514 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cone2cone/soc2psd.py
+-rw-r--r--   0 runner     (501) staff       (20)     5848 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/cvx_attr2constr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.586721 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/
+-rw-r--r--   0 runner     (501) staff       (20)      564 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.602304 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     4711 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1091 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      965 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1067 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/geo_mean_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1486 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/huber_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      677 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/indicator_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      937 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/kl_div_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1194 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/lambda_max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1490 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/lambda_sum_largest_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      710 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log1p_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1049 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2282 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_det_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1685 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_sum_exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1113 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/logistic_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1220 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/matrix_frac_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1211 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/mul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1310 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/normNuc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3661 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/perspective_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2389 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1427 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1277 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1185 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      938 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/rel_entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1124 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/sigma_max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2134 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/suppfunc_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1683 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/tr_inv_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1962 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/von_neumann_entr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1149 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/xexp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)    16778 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py
+-rw-r--r--   0 runner     (501) staff       (20)     5414 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dcp2cone/dcp2cone.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.603705 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.618813 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     5737 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      995 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/add_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      732 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/constant_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      101 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/div_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/exp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1434 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/eye_minus_inv_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      241 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/finite_set_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      152 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/geo_mean_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/gmatmul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      101 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/log_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      126 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/mul_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/mulexpression_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      169 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/nonpos_constr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      253 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/norm1_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      255 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/norm_inf_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      173 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/one_minus_pos_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1015 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/parameter_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      684 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/pf_eigenvalue_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      697 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/pnorm_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      122 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      154 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/prod_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      326 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      290 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      704 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/sum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      288 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/trace_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      125 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/xexp_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      161 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/zero_constr_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     3284 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/dgp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)      273 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/util.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.619816 cvxpy-1.4.3/cvxpy/reductions/discrete2mixedint/
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/discrete2mixedint/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2750 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.622521 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/
+-rw-r--r--   0 runner     (501) staff       (20)      562 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     9529 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3453 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/inverse.py
+-rw-r--r--   0 runner     (501) staff       (20)     5154 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/sets.py
+-rw-r--r--   0 runner     (501) staff       (20)     1154 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/tighten.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.625496 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.632273 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     2000 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      748 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/abs_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1106 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/cummax_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1133 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/cumsum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1429 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/dotsort_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1333 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/max_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      765 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/maximum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      869 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/min_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      875 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/minimum_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1173 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/norm1_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1329 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/norm_inf_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      917 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/sum_largest_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1451 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py
+-rw-r--r--   0 runner     (501) staff       (20)     2689 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/eval_params.py
+-rw-r--r--   0 runner     (501) staff       (20)     2051 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/flip_objective.py
+-rw-r--r--   0 runner     (501) staff       (20)     1944 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/inverse_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     2597 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/matrix_stuffing.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.634045 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/
+-rw-r--r--   0 runner     (501) staff       (20)      564 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.637322 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/
+-rw-r--r--   0 runner     (501) staff       (20)     2072 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1475 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/huber_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1431 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/power_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)      967 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/quad_form_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     1298 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/quad_over_lin_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     2379 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py
+-rw-r--r--   0 runner     (501) staff       (20)    12079 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py
+-rw-r--r--   0 runner     (501) staff       (20)     5050 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/reduction.py
+-rw-r--r--   0 runner     (501) staff       (20)     3020 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solution.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.642839 cvxpy-1.4.3/cvxpy/reductions/solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7382 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/bisection.py
+-rw-r--r--   0 runner     (501) staff       (20)     3636 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/compr_matrix.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.655411 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)     1145 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7745 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    11094 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    14611 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/conic_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    12853 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/copt_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    18657 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    13569 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6715 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5058 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6658 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     8904 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glop_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     3939 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     4477 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    14570 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    32952 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9595 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/nag_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     9445 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    15817 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scip_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    11028 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    13211 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scs_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     6624 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)    15320 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py
+-rw-r--r--   0 runner     (501) staff       (20)     1085 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/constant_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)     5292 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/defines.py
+-rw-r--r--   0 runner     (501) staff       (20)     4177 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/intermediate_chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     4372 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/kktsolver.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.656011 cvxpy-1.4.3/cvxpy/reductions/solvers/lp_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      566 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/lp_solvers/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.661458 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5955 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5766 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)    10300 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     4222 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     3773 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/piqp_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     5723 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     3557 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/qp_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)     9408 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py
+-rw-r--r--   0 runner     (501) staff       (20)     2495 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    18035 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/solving_chain.py
+-rw-r--r--   0 runner     (501) staff       (20)     2830 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/solvers/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     6122 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/reductions/utilities.py
+-rw-r--r--   0 runner     (501) staff       (20)     5232 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/settings.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.695114 cvxpy-1.4.3/cvxpy/tests/
+-rw-r--r--   0 runner     (501) staff       (20)      563 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1497 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/base_test.py
+-rw-r--r--   0 runner     (501) staff       (20)     1963 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/ram_limited.py
+-rw-r--r--   0 runner     (501) staff       (20)    51613 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/solver_test_helpers.py
+-rw-r--r--   0 runner     (501) staff       (20)    14047 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_KKT.py
+-rw-r--r--   0 runner     (501) staff       (20)    73557 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)    10047 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_benchmarks.py
+-rw-r--r--   0 runner     (501) staff       (20)     6308 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_coeff_extractor.py
+-rw-r--r--   0 runner     (501) staff       (20)    29369 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_complex.py
+-rw-r--r--   0 runner     (501) staff       (20)    29845 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_cone2cone.py
+-rw-r--r--   0 runner     (501) staff       (20)    84033 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_conic_solvers.py
+-rw-r--r--   0 runner     (501) staff       (20)     1493 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_constant.py
+-rw-r--r--   0 runner     (501) staff       (20)    19098 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_constant_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)    14649 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_constraints.py
+-rw-r--r--   0 runner     (501) staff       (20)     7343 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_convolution.py
+-rw-r--r--   0 runner     (501) staff       (20)     2983 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_copy.py
+-rw-r--r--   0 runner     (501) staff       (20)     3491 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_curvature.py
+-rw-r--r--   0 runner     (501) staff       (20)     3939 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_custom_solver.py
+-rw-r--r--   0 runner     (501) staff       (20)    25483 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_derivative.py
+-rw-r--r--   0 runner     (501) staff       (20)     7749 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_dgp.py
+-rw-r--r--   0 runner     (501) staff       (20)    27264 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_dgp2dcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     7197 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_domain.py
+-rw-r--r--   0 runner     (501) staff       (20)    32906 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_dpp.py
+-rw-r--r--   0 runner     (501) staff       (20)    26488 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_dqcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     3900 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_errors.py
+-rw-r--r--   0 runner     (501) staff       (20)    21418 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_examples.py
+-rw-r--r--   0 runner     (501) staff       (20)    14401 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_expression_methods.py
+-rw-r--r--   0 runner     (501) staff       (20)    53751 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_expressions.py
+-rw-r--r--   0 runner     (501) staff       (20)    32554 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_grad.py
+-rw-r--r--   0 runner     (501) staff       (20)     1570 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_gurobi_write.py
+-rw-r--r--   0 runner     (501) staff       (20)     7545 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_interfaces.py
+-rw-r--r--   0 runner     (501) staff       (20)     7671 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_kron_canon.py
+-rw-r--r--   0 runner     (501) staff       (20)     4949 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_lin_ops.py
+-rw-r--r--   0 runner     (501) staff       (20)     2637 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_linalg_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    16619 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_linear_cone.py
+-rw-r--r--   0 runner     (501) staff       (20)     5135 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_matrices.py
+-rw-r--r--   0 runner     (501) staff       (20)     4090 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_mip_vars.py
+-rw-r--r--   0 runner     (501) staff       (20)     2993 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_monotonicity.py
+-rw-r--r--   0 runner     (501) staff       (20)     6616 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_nonlinear_atoms.py
+-rw-r--r--   0 runner     (501) staff       (20)     4985 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_objectives.py
+-rw-r--r--   0 runner     (501) staff       (20)     4260 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_param_cone_prog.py
+-rw-r--r--   0 runner     (501) staff       (20)     4223 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_param_quad_prog.py
+-rw-r--r--   0 runner     (501) staff       (20)    13315 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_perspective.py
+-rw-r--r--   0 runner     (501) staff       (20)     4337 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_power_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)    85390 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_problem.py
+-rw-r--r--   0 runner     (501) staff       (20)    69130 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_python_backends.py
+-rw-r--r--   0 runner     (501) staff       (20)    22549 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_qp_solvers.py
+-rw-r--r--   0 runner     (501) staff       (20)     7929 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_quad_form.py
+-rw-r--r--   0 runner     (501) staff       (20)     6631 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_quadratic.py
+-rw-r--r--   0 runner     (501) staff       (20)     5931 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_scalarize.py
+-rw-r--r--   0 runner     (501) staff       (20)     3247 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_semidefinite_vars.py
+-rw-r--r--   0 runner     (501) staff       (20)     3992 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_shape.py
+-rw-r--r--   0 runner     (501) staff       (20)     2694 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     7775 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_suppfunc.py
+-rw-r--r--   0 runner     (501) staff       (20)    14254 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_valinvec2mixedint.py
+-rw-r--r--   0 runner     (501) staff       (20)     1901 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_versioning.py
+-rw-r--r--   0 runner     (501) staff       (20)     9116 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/tests/test_von_neumann_entr.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.698284 cvxpy-1.4.3/cvxpy/transforms/
+-rw-r--r--   0 runner     (501) staff       (20)      996 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3670 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/indicator.py
+-rw-r--r--   0 runner     (501) staff       (20)     2088 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/linearize.py
+-rw-r--r--   0 runner     (501) staff       (20)    10918 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/partial_optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)     5056 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/scalarize.py
+-rw-r--r--   0 runner     (501) staff       (20)     6761 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/transforms/suppfunc.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.707844 cvxpy-1.4.3/cvxpy/utilities/
+-rw-r--r--   0 runner     (501) staff       (20)      629 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5446 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/canonical.py
+-rw-r--r--   0 runner     (501) staff       (20)    13612 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/coeff_extractor.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.708860 cvxpy-1.4.3/cvxpy/utilities/cpp/
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/cpp/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.709864 cvxpy-1.4.3/cvxpy/utilities/cpp/sparsecholesky/
+-rw-r--r--   0 runner     (501) staff       (20)       36 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/cpp/sparsecholesky/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3778 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/cpp/sparsecholesky/main.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2968 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/cvxpy_upgrade.py
+-rw-r--r--   0 runner     (501) staff       (20)     3264 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/debug_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)      245 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/deterministic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1424 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/grad.py
+-rw-r--r--   0 runner     (501) staff       (20)     6226 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/key_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     8922 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/linalg.py
+-rw-r--r--   0 runner     (501) staff       (20)     2437 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/performance_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2178 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/perspective_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)    19336 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/power_tools.py
+-rw-r--r--   0 runner     (501) staff       (20)     1552 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/replace_quad_forms.py
+-rw-r--r--   0 runner     (501) staff       (20)     1399 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/scopes.py
+-rw-r--r--   0 runner     (501) staff       (20)     4983 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/shape.py
+-rw-r--r--   0 runner     (501) staff       (20)     1968 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/sign.py
+-rw-r--r--   0 runner     (501) staff       (20)     1825 2024-04-16 08:04:14.000000 cvxpy-1.4.3/cvxpy/utilities/versioning.py
+-rw-r--r--   0 runner     (501) staff       (20)      213 2024-04-16 08:08:49.000000 cvxpy-1.4.3/cvxpy/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.711809 cvxpy-1.4.3/cvxpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     8760 2024-04-16 08:08:49.000000 cvxpy-1.4.3/cvxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    35730 2024-04-16 08:08:50.000000 cvxpy-1.4.3/cvxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-16 08:08:49.000000 cvxpy-1.4.3/cvxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-04-16 08:05:25.000000 cvxpy-1.4.3/cvxpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      430 2024-04-16 08:08:49.000000 cvxpy-1.4.3/cvxpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       43 2024-04-16 08:08:49.000000 cvxpy-1.4.3/cvxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1318 2024-04-16 08:04:14.000000 cvxpy-1.4.3/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-16 08:08:50.711212 cvxpy-1.4.3/setup/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-04-16 08:04:14.000000 cvxpy-1.4.3/setup/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1810 2024-04-16 08:04:14.000000 cvxpy-1.4.3/setup/extensions.py
+-rw-r--r--   0 runner     (501) staff       (20)     4833 2024-04-16 08:04:14.000000 cvxpy-1.4.3/setup/versioning.py
+-rw-r--r--   0 runner     (501) staff       (20)      398 2024-04-16 08:08:50.717196 cvxpy-1.4.3/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     3196 2024-04-16 08:04:14.000000 cvxpy-1.4.3/setup.py
```

### Comparing `cvxpy-1.4.2/LICENSE` & `cvxpy-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/PKG-INFO` & `cvxpy-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpy
-Version: 1.4.2
+Version: 1.4.3
 Summary: A domain-specific language for modeling convex optimization problems in Python.
 Home-page: https://github.com/cvxpy/cvxpy
 Author: Steven Diamond, Eric Chu, Stephen Boyd
 Author-email: stevend2@stanford.edu, akshayka@cs.stanford.edu, echu508@stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cvxpy-1.4.2/README.md` & `cvxpy-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/__init__.py` & `cvxpy-1.4.3/cvxpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 from cvxpy.version import (
     version as __version__,
 )  # cvxpy/version.py is auto-generated
-import cvxpy.interface.scipy_wrapper
 from cvxpy.atoms import *
 from cvxpy.constraints import (
     Constraint as Constraint,
     Cone as Cone,
     PSD as PSD,
     SOC as SOC,
     NonPos as NonPos,
```

### Comparing `cvxpy-1.4.2/cvxpy/atoms/__init__.py` & `cvxpy-1.4.3/cvxpy/atoms/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/__init__.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/add_expr.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/add_expr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/affine_atom.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/affine_atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/binary_operators.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/binary_operators.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/bmat.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/bmat.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/conj.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/conj.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/conv.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/conv.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/cumsum.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/cumsum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/diag.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/diag.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/diff.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/diff.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/hstack.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/hstack.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/imag.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/imag.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/index.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/index.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/kron.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/kron.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/partial_trace.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/partial_trace.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/partial_transpose.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/partial_transpose.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/promote.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/promote.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/real.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/real.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/reshape.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/reshape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/sum.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/sum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/trace.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/trace.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/transpose.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/transpose.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/unary_operators.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/unary_operators.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/upper_tri.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/upper_tri.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/vec.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/vec.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/vstack.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/vstack.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/affine/wraps.py` & `cvxpy-1.4.3/cvxpy/atoms/affine/wraps.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/atom.py` & `cvxpy-1.4.3/cvxpy/atoms/atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/axis_atom.py` & `cvxpy-1.4.3/cvxpy/atoms/axis_atom.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/condition_number.py` & `cvxpy-1.4.3/cvxpy/atoms/condition_number.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/cummax.py` & `cvxpy-1.4.3/cvxpy/atoms/cummax.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/dist_ratio.py` & `cvxpy-1.4.3/cvxpy/atoms/dist_ratio.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/dotsort.py` & `cvxpy-1.4.3/cvxpy/atoms/dotsort.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/__init__.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/abs.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/abs.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/ceil.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/ceil.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/elementwise.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/elementwise.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/entr.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/exp.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/exp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/huber.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/huber.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/inv_pos.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/inv_pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/kl_div.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/kl_div.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/log.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/log.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/log1p.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/log1p.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/log_normcdf.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/log_normcdf.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/loggamma.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/loggamma.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/logistic.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/logistic.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/maximum.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/maximum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/minimum.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/minimum.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/neg.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/neg.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/pos.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/power.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/power.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/rel_entr.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/rel_entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/scalene.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/scalene.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/sqrt.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/sqrt.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/square.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/square.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/elementwise/xexp.py` & `cvxpy-1.4.3/cvxpy/atoms/elementwise/xexp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/eye_minus_inv.py` & `cvxpy-1.4.3/cvxpy/atoms/eye_minus_inv.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/gen_lambda_max.py` & `cvxpy-1.4.3/cvxpy/atoms/gen_lambda_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/geo_mean.py` & `cvxpy-1.4.3/cvxpy/atoms/geo_mean.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/gmatmul.py` & `cvxpy-1.4.3/cvxpy/atoms/gmatmul.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/harmonic_mean.py` & `cvxpy-1.4.3/cvxpy/atoms/harmonic_mean.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/inv_prod.py` & `cvxpy-1.4.3/cvxpy/atoms/inv_prod.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/lambda_max.py` & `cvxpy-1.4.3/cvxpy/atoms/lambda_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/lambda_min.py` & `cvxpy-1.4.3/cvxpy/atoms/lambda_min.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/lambda_sum_largest.py` & `cvxpy-1.4.3/cvxpy/atoms/lambda_sum_largest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/lambda_sum_smallest.py` & `cvxpy-1.4.3/cvxpy/atoms/lambda_sum_smallest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/length.py` & `cvxpy-1.4.3/cvxpy/atoms/length.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/log_det.py` & `cvxpy-1.4.3/cvxpy/atoms/log_det.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/log_sum_exp.py` & `cvxpy-1.4.3/cvxpy/atoms/log_sum_exp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/matrix_frac.py` & `cvxpy-1.4.3/cvxpy/atoms/matrix_frac.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/max.py` & `cvxpy-1.4.3/cvxpy/atoms/max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/min.py` & `cvxpy-1.4.3/cvxpy/atoms/min.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/mixed_norm.py` & `cvxpy-1.4.3/cvxpy/atoms/mixed_norm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/norm.py` & `cvxpy-1.4.3/cvxpy/atoms/norm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/norm1.py` & `cvxpy-1.4.3/cvxpy/atoms/norm1.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/norm_inf.py` & `cvxpy-1.4.3/cvxpy/atoms/norm_inf.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/norm_nuc.py` & `cvxpy-1.4.3/cvxpy/atoms/norm_nuc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/one_minus_pos.py` & `cvxpy-1.4.3/cvxpy/atoms/one_minus_pos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/perspective.py` & `cvxpy-1.4.3/cvxpy/atoms/perspective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/pf_eigenvalue.py` & `cvxpy-1.4.3/cvxpy/atoms/pf_eigenvalue.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/pnorm.py` & `cvxpy-1.4.3/cvxpy/atoms/pnorm.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/prod.py` & `cvxpy-1.4.3/cvxpy/atoms/prod.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/ptp.py` & `cvxpy-1.4.3/cvxpy/atoms/ptp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/quad_form.py` & `cvxpy-1.4.3/cvxpy/atoms/quad_form.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/quad_over_lin.py` & `cvxpy-1.4.3/cvxpy/atoms/quad_over_lin.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/sigma_max.py` & `cvxpy-1.4.3/cvxpy/atoms/sigma_max.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/sign.py` & `cvxpy-1.4.3/cvxpy/atoms/sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/stats.py` & `cvxpy-1.4.3/cvxpy/atoms/stats.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/sum_largest.py` & `cvxpy-1.4.3/cvxpy/atoms/sum_largest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/sum_smallest.py` & `cvxpy-1.4.3/cvxpy/atoms/sum_smallest.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/sum_squares.py` & `cvxpy-1.4.3/cvxpy/atoms/sum_squares.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/suppfunc.py` & `cvxpy-1.4.3/cvxpy/atoms/suppfunc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/total_variation.py` & `cvxpy-1.4.3/cvxpy/atoms/total_variation.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/tr_inv.py` & `cvxpy-1.4.3/cvxpy/atoms/tr_inv.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/atoms/von_neumann_entr.py` & `cvxpy-1.4.3/cvxpy/atoms/von_neumann_entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/__init__.py` & `cvxpy-1.4.3/cvxpy/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/cones.py` & `cvxpy-1.4.3/cvxpy/constraints/cones.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/constraint.py` & `cvxpy-1.4.3/cvxpy/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/exponential.py` & `cvxpy-1.4.3/cvxpy/constraints/exponential.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/finite_set.py` & `cvxpy-1.4.3/cvxpy/constraints/finite_set.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/nonpos.py` & `cvxpy-1.4.3/cvxpy/constraints/nonpos.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/power.py` & `cvxpy-1.4.3/cvxpy/constraints/power.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/psd.py` & `cvxpy-1.4.3/cvxpy/constraints/psd.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/second_order.py` & `cvxpy-1.4.3/cvxpy/constraints/second_order.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/utilities.py` & `cvxpy-1.4.3/cvxpy/constraints/utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/constraints/zero.py` & `cvxpy-1.4.3/cvxpy/constraints/zero.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/CMakeLists.txt` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Cholesky` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Cholesky`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/CholmodSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/CholmodSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Core` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Core`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Eigenvalues` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Eigenvalues`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Geometry` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Geometry`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Householder` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Householder`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/IterativeLinearSolvers`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Jacobi` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Jacobi`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/KLUSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/KLUSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/LU` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/LU`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/MetisSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/MetisSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/OrderingMethods` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/OrderingMethods`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/PaStiXSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/PaStiXSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/PardisoSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/PardisoSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/QR` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/QR`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/QtAlignedMalloc`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SPQRSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SPQRSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SVD` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SVD`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/Sparse` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/Sparse`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseCholesky` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseCholesky`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseCore` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseCore`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseLU` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseLU`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SparseQR` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SparseQR`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdDeque` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdDeque`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdList` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdList`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/StdVector` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/StdVector`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/SuperLUSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/SuperLUSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/UmfPackSupport` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/UmfPackSupport`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LDLT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Cholesky/LLT_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/CholmodSupport/CholmodSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArithmeticSequence.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArithmeticSequence.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Array.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Array.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArrayBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ArrayWrapper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Assign.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/AssignEvaluator.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Assign_MKL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/BandMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Block.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Block.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/BooleanRedux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CommaInitializer.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ConditionEstimator.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CoreEvaluators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CoreIterators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseNullaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseTernaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/CwiseUnaryView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseCoeffsBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DenseStorage.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Diagonal.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/DiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Dot.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/EigenBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ForceAlignedAccess.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Fuzzy.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GeneralProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GenericPacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/GlobalFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/IO.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/IO.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/IndexedView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/IndexedView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Inverse.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Map.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Map.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MapBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MathFunctionsImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Matrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/MatrixBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NestByValue.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NoAlias.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/NumTraits.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PartialReduxEvaluator.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PartialReduxEvaluator.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PermutationMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/PlainObjectBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Product.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Product.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ProductEvaluators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Random.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Random.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Redux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Ref.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Replicate.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Reshaped.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Reshaped.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/ReturnByValue.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Reverse.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Select.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Select.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SelfCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Solve.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SolveTriangular.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/SolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/StableNorm.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/StlIterators.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/StlIterators.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Stride.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Swap.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Transpose.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Transpositions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/TriangularMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/VectorBlock.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/VectorwiseOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/Visitor.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AVX512/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductCommon.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/MatrixProductMMA.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/AltiVec/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/Half.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/PacketMathHalf.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/CUDA/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/BFloat16.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/BFloat16.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/ConjHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/GenericPacketMathFunctionsFwd.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Half.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Half.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/Settings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/Default/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/GPU/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/math_constants.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/HIP/hcc/math_constants.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/MSA/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/NEON/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SSE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SVE/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/InteropHeaders.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/InteropHeaders.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/SyclMemoryModel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/TypeCasting.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/SYCL/TypeCasting.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/Complex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/MathFunctions.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/arch/ZVector/PacketMath.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/AssignmentFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/BinaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/NullaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/StlFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/TernaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/functors/UnaryFunctors.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralBlockPanelKernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrixTriangular_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/GeneralMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/Parallelizer.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/SelfadjointRank2Update.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularMatrixVector_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverMatrix_BLAS.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/products/TriangularSolverVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/BlasUtil.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ConfigureVectorization.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ConfigureVectorization.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Constants.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/DisableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ForwardDeclarations.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/IndexedViewHelper.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/IndexedViewHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/IntegralConstant.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/IntegralConstant.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/MKL_support.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Macros.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Memory.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/Meta.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ReenableStupidWarnings.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/ReshapedHelper.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/ReshapedHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/StaticAssert.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/SymbolicIndex.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/SymbolicIndex.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Core/util/XprHelper.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/ComplexSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/EigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/GeneralizedSelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/HessenbergDecomposition.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/MatrixBaseEigenvalues.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealQZ.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/RealSchur_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/SelfAdjointEigenSolver_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Eigenvalues/Tridiagonalization.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/AlignedBox.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/AngleAxis.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/EulerAngles.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Homogeneous.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Hyperplane.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/OrthoMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/ParametrizedLine.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Quaternion.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Rotation2D.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/RotationBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Scaling.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Transform.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Translation.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/Umeyama.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SIMD.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SIMD.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Geometry/arch/Geometry_SSE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/BlockHouseholder.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/Householder.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Householder/HouseholderSequence.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BasicPreconditioners.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/BiCGSTAB.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/ConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteCholesky.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IncompleteLUT.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/IterativeSolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/LeastSquareConjugateGradient.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/IterativeLinearSolvers/SolveWithGuess.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/Jacobi/Jacobi.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/KLUSupport/KLUSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/KLUSupport/KLUSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/Determinant.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/FullPivLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/InverseImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/PartialPivLU_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/InverseSize4.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/arch/InverseSize4.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/LU/arch/Inverse_SSE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/MetisSupport/MetisSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Amd.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Eigen_Colamd.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/OrderingMethods/Ordering.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PaStiXSupport/PaStiXSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/PardisoSupport/PardisoSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/ColPivHouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/CompleteOrthogonalDecomposition.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/FullPivHouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/QR/HouseholderQR_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SPQRSupport/SuiteSparseQRSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/BDCSVD.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/JacobiSVD_LAPACKE.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/SVDBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SVD/UpperBidiagonalization.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCholesky/SimplicialCholesky_impl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/AmbiVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/CompressedStorage.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/ConservativeSparseSparseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/MappedSparseMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseAssign.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseBlock.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseColEtree.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCompressedBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseBinaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseCwiseUnaryOp.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDenseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDiagonalProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseDot.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseFuzzy.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMap.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseMatrixBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparsePermutation.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseProduct.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRedux.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseRef.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSelfAdjointView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSolverBase.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseSparseProductWithPruning.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTranspose.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseTriangularView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseUtil.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/SparseView.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseCore/TriangularSolver.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLUImpl.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Memory.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Structs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_SupernodalMatrix.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_Utils.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_column_dfs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_copy_to_ucol.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_gemm_kernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_heap_relax_snode.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_kernel_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_bmod.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_panel_dfs.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pivotL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_pruneL.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseLU/SparseLU_relax_snode.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SparseQR/SparseQR.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdDeque.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdList.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/StdVector.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/StlSupport/details.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/SuperLUSupport/SuperLUSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/UmfPackSupport/UmfPackSupport.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/Image.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/Image.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/Kernel.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/RealSvd2x2.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/blas.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/blas.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/lapack.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/misc/lapacke.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ArrayCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/BlockMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/CommonCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/IndexedViewMethods.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/IndexedViewMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseBinaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/MatrixCwiseUnaryOps.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/include/Eigen/src/plugins/ReshapedMethods.h` & `cvxpy-1.4.3/cvxpy/cvxcore/include/Eigen/src/plugins/ReshapedMethods.h`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/python/canonInterface.py` & `cvxpy-1.4.3/cvxpy/cvxcore/python/canonInterface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore.i` & `cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore.i`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore.py` & `cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/python/cvxcore_wrap.cxx` & `cvxpy-1.4.3/cvxpy/cvxcore/python/cvxcore_wrap.cxx`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/python/numpy.i` & `cvxpy-1.4.3/cvxpy/cvxcore/python/numpy.i`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/LinOp.hpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/LinOp.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/LinOpOperations.cpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/LinOpOperations.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/LinOpOperations.hpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/LinOpOperations.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/ProblemData.hpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/ProblemData.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/Utils.cpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/Utils.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/Utils.hpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/Utils.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/cvxcore.cpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/cvxcore.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/cvxcore/src/cvxcore.hpp` & `cvxpy-1.4.3/cvxpy/cvxcore/src/cvxcore.hpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/error.py` & `cvxpy-1.4.3/cvxpy/error.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/__init__.py` & `cvxpy-1.4.3/cvxpy/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/constants/__init__.py` & `cvxpy-1.4.3/cvxpy/expressions/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/constants/callback_param.py` & `cvxpy-1.4.3/cvxpy/expressions/constants/callback_param.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/constants/constant.py` & `cvxpy-1.4.3/cvxpy/expressions/constants/constant.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/constants/parameter.py` & `cvxpy-1.4.3/cvxpy/expressions/constants/parameter.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/cvxtypes.py` & `cvxpy-1.4.3/cvxpy/expressions/cvxtypes.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/expression.py` & `cvxpy-1.4.3/cvxpy/expressions/expression.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/leaf.py` & `cvxpy-1.4.3/cvxpy/expressions/leaf.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/expressions/variable.py` & `cvxpy-1.4.3/cvxpy/expressions/variable.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/__init__.py` & `cvxpy-1.4.3/cvxpy/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/base_matrix_interface.py` & `cvxpy-1.4.3/cvxpy/interface/base_matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/matrix_utilities.py` & `cvxpy-1.4.3/cvxpy/interface/matrix_utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/numpy_interface/__init__.py` & `cvxpy-1.4.3/cvxpy/interface/numpy_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/numpy_interface/matrix_interface.py` & `cvxpy-1.4.3/cvxpy/interface/numpy_interface/matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/numpy_interface/ndarray_interface.py` & `cvxpy-1.4.3/cvxpy/interface/numpy_interface/ndarray_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/interface/numpy_interface/sparse_matrix_interface.py` & `cvxpy-1.4.3/cvxpy/interface/numpy_interface/sparse_matrix_interface.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/__init__.py` & `cvxpy-1.4.3/cvxpy/lin_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/canon_backend.py` & `cvxpy-1.4.3/cvxpy/lin_ops/canon_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     Sparse representation of a 3D Tensor. Semantically similar to COO format, with one extra
     dimension. Here, 'row' is axis 0, 'col' axis 1, and 'parameter_offset' axis 2.
     """
     data: np.ndarray
     row: np.ndarray
     col: np.ndarray
     parameter_offset: np.ndarray
+    shape: tuple[int, int]  # (rows, cols)
+
+    def __post_init__(self):
+        assert self.data.shape == self.row.shape == self.col.shape == self.parameter_offset.shape
 
     @classmethod
     def combine(cls, tensors: list[TensorRepresentation]) -> TensorRepresentation:
         """
         Concatenates the row, col, parameter_offset, and data fields of a list of
         TensorRepresentations.
         """
@@ -62,29 +66,61 @@
         # Appending to numpy arrays vs. appending to lists and casting to array at the end was
         # faster for relevant dimensions in our testing.
         for t in tensors:
             data = np.append(data, t.data)
             row = np.append(row, t.row)
             col = np.append(col, t.col)
             parameter_offset = np.append(parameter_offset, t.parameter_offset)
-        return cls(data, row, col, parameter_offset)
+        assert all(t.shape == tensors[0].shape for t in tensors)
+        return cls(data, row, col, parameter_offset, tensors[0].shape)
 
     def __eq__(self, other: TensorRepresentation) -> bool:
         return isinstance(other, TensorRepresentation) and \
             np.all(self.data == other.data) and \
             np.all(self.row == other.row) and \
             np.all(self.col == other.col) and \
-            np.all(self.parameter_offset == other.parameter_offset)
+            np.all(self.parameter_offset == other.parameter_offset) and \
+            self.shape == other.shape
+    
+    def __add__(self, other: TensorRepresentation) -> TensorRepresentation:
+        if self.shape != other.shape:
+            raise ValueError("Shapes must match for addition.")
+        return TensorRepresentation(
+            np.concatenate([self.data, other.data]),
+            np.concatenate([self.row, other.row]),
+            np.concatenate([self.col, other.col]),
+            np.concatenate([self.parameter_offset, other.parameter_offset]),
+            self.shape
+        )
+
+    @classmethod
+    def empty_with_shape(cls, shape: tuple[int, int]) -> TensorRepresentation:
+        return cls(
+            np.array([], dtype=float),
+            np.array([], dtype=int),
+            np.array([], dtype=int),
+            np.array([], dtype=int),
+            shape,
+        )
+
+    def flatten_tensor(self, num_param_slices: int) -> sp.csc_matrix:
+        """
+        Flatten into 2D scipy csc-matrix in column-major order and transpose.
+        """
+        rows = (self.col.astype(np.int64) * np.int64(self.shape[0]) + self.row.astype(np.int64))
+        cols = self.parameter_offset.astype(np.int64)
+        shape = (np.int64(np.prod(self.shape)), num_param_slices)
+        return sp.csc_matrix((self.data, (rows, cols)), shape=shape)
 
-    def get_param_slice(self, param_offset: int, shape: tuple[int, int]) -> sp.csc_matrix:
+    def get_param_slice(self, param_offset: int) -> sp.csc_matrix:
         """
         Returns a single slice of the tensor for a given parameter offset.
         """
         mask = self.parameter_offset == param_offset
-        return sp.csc_matrix((self.data[mask], (self.row[mask], self.col[mask])), shape)
+        return sp.csc_matrix((self.data[mask], (self.row[mask], self.col[mask])), self.shape)
 
 
 class CanonBackend(ABC):
     def __init__(self, id_to_col: dict[int, int], param_to_size: dict[int, int],
                  param_to_col: dict[int, int], param_size_plus_one: int, var_length: int):
         """
         CanonBackend handles the compilation from LinOp trees to a final sparse tensor through its
@@ -156,25 +192,26 @@
     - A new constant of size n has shape (1, n, 1)
     """
 
     def build_matrix(self, lin_ops: list[LinOp]) -> sp.csc_matrix:
         self.id_to_col[-1] = self.var_length
 
         constraint_res = []
+        total_rows = sum(np.prod(lin_op.shape) for lin_op in lin_ops)
         row_offset = 0
         for lin_op in lin_ops:
             lin_op_rows = np.prod(lin_op.shape)
             empty_view = self.get_empty_view()
             lin_op_tensor = self.process_constraint(lin_op, empty_view)
-            constraint_res.append((lin_op_tensor.get_tensor_representation(row_offset)))
+            constraint_res.append(lin_op_tensor.get_tensor_representation(row_offset, total_rows))
             row_offset += lin_op_rows
         tensor_res = self.concatenate_tensors(constraint_res)
 
         self.id_to_col.pop(-1)
-        return self.reshape_tensors(tensor_res, row_offset)
+        return tensor_res.flatten_tensor(self.param_size_plus_one)
 
     def process_constraint(self, lin_op: LinOp, empty_view: TensorView) -> TensorView:
         """
         Depth-first parsing of a linOp node.
 
         Parameters
         ----------
@@ -266,23 +303,14 @@
     def concatenate_tensors(tensors: list[TensorRepresentation]) -> TensorRepresentation:
         """
         Takes list of tensors which have already been offset along axis 0 (rows) and
         combines them into a single tensor.
         """
         return TensorRepresentation.combine(tensors)
 
-    def reshape_tensors(self, tensor: TensorRepresentation, total_rows: int) -> sp.csc_matrix:
-        """
-        Reshape into 2D scipy csc-matrix in column-major order and transpose.
-        """
-        rows = (tensor.col.astype(np.int64) * np.int64(total_rows) + tensor.row.astype(np.int64))
-        cols = tensor.parameter_offset.astype(np.int64)
-        shape = (np.int64(total_rows) * np.int64(self.var_length + 1), self.param_size_plus_one)
-        return sp.csc_matrix((tensor.data, (rows, cols)), shape=shape)
-
     @abstractmethod
     def get_empty_view(self) -> TensorView:
         """
         Returns an empty view of the corresponding TensorView subclass, coupling the CanonBackend
         subclass with the TensorView subclass.
         """
         pass  # noqa
@@ -1560,15 +1588,15 @@
     def rows(self) -> int:
         """
         Number of rows of the TensorView.
         """
         pass  # noqa
 
     @abstractmethod
-    def get_tensor_representation(self, row_offset: int) -> TensorRepresentation:
+    def get_tensor_representation(self, row_offset: int, total_rows: int) -> TensorRepresentation:
         """
         Returns [A b].
         """
         pass  # noqa
 
     @abstractmethod
     def select_rows(self, rows: np.ndarray) -> None:
@@ -1681,37 +1709,39 @@
         This is the second dimension of the 3d tensor.
         """
         if self.tensor is not None:
             return next(iter(next(iter(self.tensor.values())).values())).shape[1]
         else:
             raise ValueError
 
-    def get_tensor_representation(self, row_offset: int) -> TensorRepresentation:
+    def get_tensor_representation(self, row_offset: int, total_rows: int) -> TensorRepresentation:
         """
         Returns a TensorRepresentation of [A b] tensor.
         This function iterates through all the tensor data and constructs the
         respective representation in COO format. To obtain the data, the tensor must be
         flattened as it is not in a sparse format. The row and column indices are obtained
         with numpy tiling/repeating along with their respective offsets.
 
         Note: CVXPY currently only supports usage of sparse matrices after the canonicalization.
         Therefore, we must return tensor representations in a (data, (row,col)) format.
         This could be changed once dense matrices are accepted.
         """
         assert self.tensor is not None
+        shape = (total_rows, self.var_length + 1)
         tensor_representations = []
         for variable_id, variable_tensor in self.tensor.items():
             for parameter_id, parameter_tensor in variable_tensor.items():
                 param_size, rows, cols = parameter_tensor.shape
                 tensor_representations.append(TensorRepresentation(
                     parameter_tensor.flatten(order='F'),
                     np.repeat(np.tile(np.arange(rows), cols), param_size) + row_offset,
                     np.repeat(np.repeat(np.arange(cols), rows), param_size)
                     + self.id_to_col[variable_id],
                     np.tile(np.arange(param_size), rows * cols) + self.param_to_col[parameter_id],
+                    shape=shape
                 ))
         return TensorRepresentation.combine(tensor_representations)
 
     def select_rows(self, rows: np.ndarray) -> None:
         """
         Select 'rows' from tensor.
         The rows of the 3d tensor are in axis=1, this function selects a subset
@@ -1778,35 +1808,37 @@
         if self.tensor is not None:
             for param_dict in self.tensor.values():
                 for param_id, param_mat in param_dict.items():
                     return param_mat.shape[0] // self.param_to_size[param_id]
         else:
             raise ValueError('Tensor cannot be None')
 
-    def get_tensor_representation(self, row_offset: int) -> TensorRepresentation:
+    def get_tensor_representation(self, row_offset: int, total_rows: int) -> TensorRepresentation:
         """
         Returns a TensorRepresentation of [A b] tensor.
         This function iterates through all the tensor data and constructs their
         respective representation in COO format. The row data is adjusted according
         to the position of each element within a parameter slice. The parameter_offset
         finds which slice the original row indices belong to before applying the column
         offset.
         """
         assert self.tensor is not None
+        shape = (total_rows, self.var_length + 1)
         tensor_representations = []
         for variable_id, variable_tensor in self.tensor.items():
             for parameter_id, parameter_matrix in variable_tensor.items():
                 p = self.param_to_size[parameter_id]
                 m = parameter_matrix.shape[0] // p
                 coo_repr = parameter_matrix.tocoo(copy=False)
                 tensor_representations.append(TensorRepresentation(
                     coo_repr.data,
                     (coo_repr.row % m) + row_offset,
                     coo_repr.col + self.id_to_col[variable_id],
                     coo_repr.row // m + np.ones(coo_repr.nnz) * self.param_to_col[parameter_id],
+                    shape=shape
                 ))
         return TensorRepresentation.combine(tensor_representations)
 
     def select_rows(self, rows: np.ndarray) -> None:
         """
         Select 'rows' from tensor. If there are multiple parameters 'p',
         we must select the same 'rows' from each parameter slice. This is done by
```

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/lin_constraints.py` & `cvxpy-1.4.3/cvxpy/lin_ops/lin_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/lin_op.py` & `cvxpy-1.4.3/cvxpy/lin_ops/lin_op.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/lin_utils.py` & `cvxpy-1.4.3/cvxpy/lin_ops/lin_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/lin_ops/tree_mat.py` & `cvxpy-1.4.3/cvxpy/lin_ops/tree_mat.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/__init__.py` & `cvxpy-1.4.3/cvxpy/problems/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/iterative.py` & `cvxpy-1.4.3/cvxpy/problems/iterative.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/objective.py` & `cvxpy-1.4.3/cvxpy/problems/objective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/param_prob.py` & `cvxpy-1.4.3/cvxpy/problems/param_prob.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/problem.py` & `cvxpy-1.4.3/cvxpy/problems/problem.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/problems/xpress_problem.py` & `cvxpy-1.4.3/cvxpy/problems/xpress_problem.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/canonicalization.py` & `cvxpy-1.4.3/cvxpy/reductions/canonicalization.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/chain.py` & `cvxpy-1.4.3/cvxpy/reductions/chain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/abs_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/aff_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/constant_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/equality_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/inequality_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/matrix_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/param_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/param_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/pnorm_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/psd_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/soc_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/canonicalizers/variable_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/complex2real/complex2real.py` & `cvxpy-1.4.3/cvxpy/reductions/complex2real/complex2real.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/cone2cone/affine2direct.py` & `cvxpy-1.4.3/cvxpy/reductions/cone2cone/affine2direct.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/cone2cone/approximations.py` & `cvxpy-1.4.3/cvxpy/reductions/cone2cone/approximations.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/cone2cone/exotic2common.py` & `cvxpy-1.4.3/cvxpy/reductions/cone2cone/exotic2common.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/cone2cone/soc2psd.py` & `cvxpy-1.4.3/cvxpy/reductions/cone2cone/soc2psd.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 
         psd_constraints = []
 
         soc_constraint_ids = []
         soc_id_from_psd = {}
 
         for constraint in soc_constraints:
-            """
-            The SOC constraint :math:`\\lVert X \\rVert_2 \leq t` is modeled by `t` and `X`.
+            r"""
+            The SOC constraint :math:`\lVert X \rVert_2 \leq t` is modeled by `t` and `X`.
             We extract these `t` and `X` from the SOC constraint object.
             """
             t, X = constraint.args
             soc_constraint_ids.append(constraint.id)
 
             """
             A PSD constraint object will constrain the matrix M specified in its constructor to
```

### Comparing `cvxpy-1.4.2/cvxpy/reductions/cvx_attr2constr.py` & `cvxpy-1.4.3/cvxpy/reductions/cvx_attr2constr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/entr_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/entr_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/exp_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/exp_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/geo_mean_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/geo_mean_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/huber_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/huber_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/indicator_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/indicator_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/kl_div_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/kl_div_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/lambda_max_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/lambda_max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/lambda_sum_largest_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/lambda_sum_largest_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log1p_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log1p_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_det_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_det_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/log_sum_exp_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/log_sum_exp_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/logistic_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/logistic_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/matrix_frac_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/matrix_frac_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/mul_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/mul_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/normNuc_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/normNuc_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/perspective_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/perspective_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/pnorm_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/pnorm_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/power_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/power_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/quad_form_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/quad_form_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/quad_over_lin_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/quad_over_lin_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/rel_entr_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/rel_entr_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/sigma_max_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/sigma_max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/suppfunc_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/suppfunc_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/tr_inv_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/tr_inv_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/von_neumann_entr_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/von_neumann_entr_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/canonicalizers/xexp_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/canonicalizers/xexp_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/cone_matrix_stuffing.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dcp2cone/dcp2cone.py` & `cvxpy-1.4.3/cvxpy/reductions/dcp2cone/dcp2cone.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/add_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/add_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/constant_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/constant_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/eye_minus_inv_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/eye_minus_inv_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/mulexpression_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/mulexpression_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/parameter_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/parameter_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/pf_eigenvalue_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/pf_eigenvalue_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/pnorm_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/pnorm_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/canonicalizers/sum_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/canonicalizers/sum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dgp2dcp/dgp2dcp.py` & `cvxpy-1.4.3/cvxpy/reductions/dgp2dcp/dgp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py` & `cvxpy-1.4.3/cvxpy/reductions/discrete2mixedint/valinvec2mixedint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py` & `cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/dqcp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/inverse.py` & `cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/inverse.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/sets.py` & `cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/sets.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/dqcp2dcp/tighten.py` & `cvxpy-1.4.3/cvxpy/reductions/dqcp2dcp/tighten.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/abs_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/abs_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/cummax_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/cummax_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/cumsum_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/cumsum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/dotsort_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/dotsort_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/max_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/max_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/maximum_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/maximum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/min_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/min_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/minimum_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/minimum_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/norm1_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/norm1_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/norm_inf_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/norm_inf_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/canonicalizers/sum_largest_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/canonicalizers/sum_largest_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py` & `cvxpy-1.4.3/cvxpy/reductions/eliminate_pwl/eliminate_pwl.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/eval_params.py` & `cvxpy-1.4.3/cvxpy/reductions/eval_params.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/flip_objective.py` & `cvxpy-1.4.3/cvxpy/reductions/flip_objective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/inverse_data.py` & `cvxpy-1.4.3/cvxpy/reductions/inverse_data.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/matrix_stuffing.py` & `cvxpy-1.4.3/cvxpy/reductions/matrix_stuffing.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/huber_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/huber_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/power_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/power_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/quad_form_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/quad_form_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/canonicalizers/quad_over_lin_canon.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/canonicalizers/quad_over_lin_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/qp2symbolic_qp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py` & `cvxpy-1.4.3/cvxpy/reductions/qp2quad_form/qp_matrix_stuffing.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/reduction.py` & `cvxpy-1.4.3/cvxpy/reductions/reduction.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solution.py` & `cvxpy-1.4.3/cvxpy/reductions/solution.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/bisection.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/bisection.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/compr_matrix.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/compr_matrix.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cbc_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/clarabel_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/conic_solver.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/conic_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/copt_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/copt_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cplex_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/cvxopt_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/diffcp_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/ecos_bb_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/ecos_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glop_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glop_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glpk_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/glpk_mi_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/gurobi_conif.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,23 +42,25 @@
 
     # Map of Gurobi status to CVXPY status.
     STATUS_MAP = {2: s.OPTIMAL,
                   3: s.INFEASIBLE,
                   4: s.INFEASIBLE_OR_UNBOUNDED,  # Triggers reoptimize.
                   5: s.UNBOUNDED,
                   6: s.SOLVER_ERROR,
-                  7: s.SOLVER_ERROR,
-                  8: s.SOLVER_ERROR,
-                  # TODO could be anything.
-                  # means time expired.
-                  9: s.USER_LIMIT,
-                  10: s.SOLVER_ERROR,
-                  11: s.SOLVER_ERROR,
-                  12: s.SOLVER_ERROR,
-                  13: s.SOLVER_ERROR}
+                  7: s.USER_LIMIT, # ITERATION_LIMIT
+                  8: s.USER_LIMIT, # NODE_LIMIT
+                  9: s.USER_LIMIT,  # TIME_LIMIT
+                  10: s.USER_LIMIT, # SOLUTION_LIMIT
+                  11: s.USER_LIMIT, # INTERRUPTED
+                  12: s.SOLVER_ERROR, # NUMERIC
+                  13: s.USER_LIMIT, # SUBOPTIMAL
+                  14: s.USER_LIMIT, # INPROGRESS
+                  15: s.USER_LIMIT, # USER_OBJ_LIMIT
+                  16: s.USER_LIMIT, # WORK_LIMIT
+                  17: s.USER_LIMIT} # MEM_LIMIT
 
     def name(self):
         """The name of the solver.
         """
         return s.GUROBI
 
     def import_solver(self) -> None:
```

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/mosek_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/nag_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/nag_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/pdlp_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scip_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scip_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scipy_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/scs_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/scs_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/sdpa_conif.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             eq_dual.update(leq_dual)
             dual_vars = eq_dual
             return Solution(status, opt_val, primal_vars, dual_vars, {})
         else:
             return failure_solution(status)
 
     def solve_via_data(self, data, warm_start: bool, verbose: bool, solver_opts, solver_cache=None):
-        """
+        r"""
         CVXPY represents cone programs as
             (P) min_x { c^T x : A x + b \in K } + d
 
         SDPA Python takes a conic program in CLP format:
             (P) min_x { c^T x : A x - b \in J, x \in K }
 
         CVXPY (P) -> CLP (P), by
```

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/conic_solvers/xpress_conif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/constant_solver.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/constant_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/defines.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/defines.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/intermediate_chain.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/intermediate_chain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/kktsolver.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/kktsolver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/lp_solvers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/lp_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/__init__.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/copt_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/cplex_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/gurobi_qpif.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,25 +29,28 @@
 
     # Keyword arguments for the CVXPY interface.
     INTERFACE_ARGS = ["save_file", "reoptimize"]
 
     # Map of Gurobi status to CVXPY status.
     STATUS_MAP = {2: s.OPTIMAL,
                   3: s.INFEASIBLE,
+                  4: s.INFEASIBLE_OR_UNBOUNDED,  # Triggers reoptimize.
                   5: s.UNBOUNDED,
-                  4: s.INFEASIBLE_OR_UNBOUNDED,
-                  6: s.INFEASIBLE,
-                  7: s.SOLVER_ERROR,
-                  8: s.SOLVER_ERROR,
-                  9: s.USER_LIMIT,  # Maximum time expired
-                  # TODO could be anything.
-                  10: s.SOLVER_ERROR,
-                  11: s.SOLVER_ERROR,
-                  12: s.SOLVER_ERROR,
-                  13: s.OPTIMAL_INACCURATE}
+                  6: s.SOLVER_ERROR,
+                  7: s.USER_LIMIT, # ITERATION_LIMIT
+                  8: s.USER_LIMIT, # NODE_LIMIT
+                  9: s.USER_LIMIT,  # TIME_LIMIT
+                  10: s.USER_LIMIT, # SOLUTION_LIMIT
+                  11: s.USER_LIMIT, # INTERRUPTED
+                  12: s.SOLVER_ERROR, # NUMERIC
+                  13: s.USER_LIMIT, # SUBOPTIMAL
+                  14: s.USER_LIMIT, # INPROGRESS
+                  15: s.USER_LIMIT, # USER_OBJ_LIMIT
+                  16: s.USER_LIMIT, # WORK_LIMIT
+                  17: s.USER_LIMIT} # MEM_LIMIT
 
     def name(self):
         return s.GUROBI
 
     def import_solver(self) -> None:
         import gurobipy
         gurobipy
```

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/osqp_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/piqp_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/piqp_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/proxqp_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/qp_solver.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/qp_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/qp_solvers/xpress_qpif.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/solver.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/solving_chain.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/solving_chain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/solvers/utilities.py` & `cvxpy-1.4.3/cvxpy/reductions/solvers/utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/reductions/utilities.py` & `cvxpy-1.4.3/cvxpy/reductions/utilities.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/settings.py` & `cvxpy-1.4.3/cvxpy/settings.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/__init__.py` & `cvxpy-1.4.3/cvxpy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/base_test.py` & `cvxpy-1.4.3/cvxpy/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/ram_limited.py` & `cvxpy-1.4.3/cvxpy/tests/ram_limited.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/solver_test_helpers.py` & `cvxpy-1.4.3/cvxpy/tests/solver_test_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             msg = """\n
             CVXPY problems with `diag` variables are not supported for
             stationarity checks as of now
             """
             self.tester.fail(msg)
         bad_norms = []
 
-        """The convention that we follow for construting the Lagrangian is: 1) Move all
+        r"""The convention that we follow for construting the Lagrangian is: 1) Move all
         explicitly passed constraints to the problem (via Problem.constraints) into the
         Lagrangian --- dLdX == 0 for any such variables 2) Constraints that have
         implicitly been imposed on variables at the time of declaration via specific
         flags (e.g.: PSD/symmetric etc.), in such a case we check, `dLdX\in K^{*}`, where
         `K` is the convex cone corresponding to the implicit constraint on `X`
         """
         for (opt_var, v) in g.items():
@@ -187,15 +187,15 @@
                         'Hollow' matrices i.e. matrices with diagonal entries zero"""
                     g_bad_mat = np.reshape(g[opt_var].toarray(), opt_var.shape)
                     diag_entries = np.diag(opt_var.value)
                     dual_cone_violation = np.linalg.norm(diag_entries) / np.sqrt(opt_var.size)
                     if diag_entries > 10**(-places):
                         bad_norms.append((dual_cone_violation, opt_var))
                 elif opt_var.is_symmetric():
-                    """The dual cone to the set of symmetric matrices is the
+                    r"""The dual cone to the set of symmetric matrices is the
                     set of skew-symmetric matrices, so we check if dLdX \in
                     set(skew-symmetric-matrices)
                     g[opt_var] is the problematic gradient in question"""
                     g_bad_mat = np.reshape(g[opt_var].toarray(), opt_var.shape)
                     mat = g_bad_mat + g_bad_mat.T
                     dual_cone_violation = np.linalg.norm(mat) / np.sqrt(opt_var.size)
                     if dual_cone_violation > 10**(-places):
```

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_KKT.py` & `cvxpy-1.4.3/cvxpy/tests/test_KKT.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_atoms.py` & `cvxpy-1.4.3/cvxpy/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_benchmarks.py` & `cvxpy-1.4.3/cvxpy/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_complex.py` & `cvxpy-1.4.3/cvxpy/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_cone2cone.py` & `cvxpy-1.4.3/cvxpy/tests/test_cone2cone.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_conic_solvers.py` & `cvxpy-1.4.3/cvxpy/tests/test_conic_solvers.py`

 * *Files 0% similar despite different names*

```diff
@@ -2258,15 +2258,15 @@
     def test_copt_sdp_1min(self) -> None:
         StandardTestSDPs.test_sdp_1min(solver='COPT')
 
     def test_copt_sdp_1max(self) -> None:
         StandardTestSDPs.test_sdp_1max(solver='COPT')
 
     def test_copt_sdp_2(self) -> None:
-        StandardTestSDPs.test_sdp_2(solver='COPT')
+        StandardTestSDPs.test_sdp_2(solver='COPT', places=2)
 
     def test_copt_params(self) -> None:
         n = 10
         m = 4
         np.random.seed(0)
         A = np.random.randn(m, n)
         x = np.random.randn(n)
```

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_constant.py` & `cvxpy-1.4.3/cvxpy/tests/test_constant.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_constant_atoms.py` & `cvxpy-1.4.3/cvxpy/tests/test_constant_atoms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_constraints.py` & `cvxpy-1.4.3/cvxpy/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_convolution.py` & `cvxpy-1.4.3/cvxpy/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_copy.py` & `cvxpy-1.4.3/cvxpy/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_curvature.py` & `cvxpy-1.4.3/cvxpy/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_custom_solver.py` & `cvxpy-1.4.3/cvxpy/tests/test_custom_solver.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_derivative.py` & `cvxpy-1.4.3/cvxpy/tests/test_derivative.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_dgp.py` & `cvxpy-1.4.3/cvxpy/tests/test_dgp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_dgp2dcp.py` & `cvxpy-1.4.3/cvxpy/tests/test_dgp2dcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_domain.py` & `cvxpy-1.4.3/cvxpy/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_dpp.py` & `cvxpy-1.4.3/cvxpy/tests/test_dpp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_dqcp.py` & `cvxpy-1.4.3/cvxpy/tests/test_dqcp.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_errors.py` & `cvxpy-1.4.3/cvxpy/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_examples.py` & `cvxpy-1.4.3/cvxpy/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_expression_methods.py` & `cvxpy-1.4.3/cvxpy/tests/test_expression_methods.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_expressions.py` & `cvxpy-1.4.3/cvxpy/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_grad.py` & `cvxpy-1.4.3/cvxpy/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_gurobi_write.py` & `cvxpy-1.4.3/cvxpy/tests/test_gurobi_write.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_interfaces.py` & `cvxpy-1.4.3/cvxpy/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_kron_canon.py` & `cvxpy-1.4.3/cvxpy/tests/test_kron_canon.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_lin_ops.py` & `cvxpy-1.4.3/cvxpy/tests/test_lin_ops.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_linalg_utils.py` & `cvxpy-1.4.3/cvxpy/tests/test_linalg_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_linear_cone.py` & `cvxpy-1.4.3/cvxpy/tests/test_linear_cone.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_matrices.py` & `cvxpy-1.4.3/cvxpy/tests/test_matrices.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_mip_vars.py` & `cvxpy-1.4.3/cvxpy/tests/test_mip_vars.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_monotonicity.py` & `cvxpy-1.4.3/cvxpy/tests/test_monotonicity.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_nonlinear_atoms.py` & `cvxpy-1.4.3/cvxpy/tests/test_nonlinear_atoms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_objectives.py` & `cvxpy-1.4.3/cvxpy/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_param_cone_prog.py` & `cvxpy-1.4.3/cvxpy/tests/test_param_cone_prog.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_param_quad_prog.py` & `cvxpy-1.4.3/cvxpy/tests/test_param_quad_prog.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_perspective.py` & `cvxpy-1.4.3/cvxpy/tests/test_perspective.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_power_tools.py` & `cvxpy-1.4.3/cvxpy/tests/test_power_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_problem.py` & `cvxpy-1.4.3/cvxpy/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_python_backends.py` & `cvxpy-1.4.3/cvxpy/tests/test_python_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,43 +19,50 @@
 
 @dataclass
 class linOpHelper:
     """
     Helper class that allows to access properties of linOps without
     needing to create a full linOps instance
     """
+
     shape: None | tuple[int, ...] = None
     type: None | str = None
     data: None | int | np.ndarray | list[slice] = None
     args: None | list[linOpHelper] = None
 
 
 def test_tensor_representation():
-    A = TensorRepresentation(np.array([10]), np.array([0]), np.array([1]), np.array([0]))
-    B = TensorRepresentation(np.array([20]), np.array([1]), np.array([1]), np.array([1]))
+    A = TensorRepresentation(
+        np.array([10]), np.array([0]), np.array([1]), np.array([0]), shape=(2, 2)
+    )
+    B = TensorRepresentation(
+        np.array([20]), np.array([1]), np.array([1]), np.array([1]), shape=(2, 2)
+    )
     combined = TensorRepresentation.combine([A, B])
     assert np.all(combined.data == np.array([10, 20]))
     assert np.all(combined.row == np.array([0, 1]))
     assert np.all(combined.col == np.array([1, 1]))
     assert np.all(combined.parameter_offset == np.array([0, 1]))
+    assert combined.shape == (2, 2)
+    flattened = combined.flatten_tensor(2)
+    assert np.all(flattened.toarray() == np.array([[0, 0], [0, 0], [10, 0], [0, 20]]))
 
 
 class TestBackendInstance:
-
     def test_get_backend(self):
         args = ({1: 0, 2: 2}, {-1: 1, 3: 1}, {3: 0, -1: 1}, 2, 4)
 
         backend = CanonBackend.get_backend(s.SCIPY_CANON_BACKEND, *args)
         assert isinstance(backend, SciPyCanonBackend)
 
         backend = CanonBackend.get_backend(s.NUMPY_CANON_BACKEND, *args)
         assert isinstance(backend, NumPyCanonBackend)
 
         with pytest.raises(KeyError):
-            CanonBackend.get_backend('notabackend')
+            CanonBackend.get_backend("notabackend")
 
 
 backends = [s.SCIPY_CANON_BACKEND, s.NUMPY_CANON_BACKEND]
 
 
 class TestBackends:
     @staticmethod
@@ -64,72 +71,72 @@
         # Not used explicitly in most test cases.
         # Some tests specify other values as needed within the test case.
         kwargs = {
             "id_to_col": {1: 0, 2: 2},
             "param_to_size": {-1: 1, 3: 1},
             "param_to_col": {3: 0, -1: 1},
             "param_size_plus_one": 2,
-            "var_length": 4
+            "var_length": 4,
         }
 
         backend = CanonBackend.get_backend(request.param, **kwargs)
         assert isinstance(backend, PythonCanonBackend)
         return backend
 
     def test_mapping(self, backend):
-        func = backend.get_func('sum')
+        func = backend.get_func("sum")
         assert isinstance(func, Callable)
         with pytest.raises(KeyError):
-            backend.get_func('notafunc')
+            backend.get_func("notafunc")
 
     def test_neg(self, backend):
         """
-         define x = Variable((2,2)) with
-         [[x11, x12],
-          [x21, x22]]
+        define x = Variable((2,2)) with
+        [[x11, x12],
+         [x21, x22]]
 
-         x is represented as eye(4) in the A matrix (in column-major order), i.e.,
+        x is represented as eye(4) in the A matrix (in column-major order), i.e.,
 
-          x11 x21 x12 x22
-         [[1   0   0   0],
-          [0   1   0   0],
-          [0   0   1   0],
-          [0   0   0   1]]
+         x11 x21 x12 x22
+        [[1   0   0   0],
+         [0   1   0   0],
+         [0   0   1   0],
+         [0   0   0   1]]
+
+        neg(x) means we now have
+         [[-x11, -x21],
+          [-x12, -x22]],
 
-         neg(x) means we now have
-          [[-x11, -x21],
-           [-x12, -x22]],
-
-          i.e.,
-
-          x11 x21 x12 x22
-         [[-1  0   0   0],
-          [0  -1   0   0],
-          [0   0  -1   0],
-          [0   0   0  -1]]
-         """
+         i.e.,
+
+         x11 x21 x12 x22
+        [[-1  0   0   0],
+         [0  -1   0   0],
+         [0   0  -1   0],
+         [0   0   0  -1]]
+        """
         empty_view = backend.get_empty_view()
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, empty_view)
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         neg_lin_op = linOpHelper()
         out_view = backend.neg(neg_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 4)).toarray()
         assert np.all(A == -np.eye(4))
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_transpose(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -152,38 +159,33 @@
          [0   0   1   0],
          [0   1   0   0],
          [0   0   0   1]]
 
         -> It reduces to reordering the rows of A.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         transpose_lin_op = linOpHelper((2, 2))
         out_view = backend.transpose(transpose_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0],
-             [0, 0, 1, 0],
-             [0, 1, 0, 0],
-             [0, 0, 0, 1]]
-        )
+        expected = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_upper_tri(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -201,35 +203,33 @@
 
          x11 x21 x12 x22
         [[0   0   0   1]]
 
         -> It reduces to selecting a subset of the rows of A.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         upper_tri_lin_op = linOpHelper(args=[linOpHelper((2, 2))])
         out_view = backend.upper_tri(upper_tri_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(1, 4)).toarray()
-        expected = np.array(
-            [[0, 0, 1, 0]]
-        )
+        expected = np.array([[0, 0, 1, 0]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_index(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -251,47 +251,42 @@
          Passing a single slice only returns the corresponding row of A.
          Note: Passing a single slice does not happen when slicing e.g. x[0], which is expanded to
          the 2d case.
 
          -> It reduces to selecting a subset of the rows of A.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         index_2d_lin_op = linOpHelper(data=[slice(0, 2, 1), slice(0, 1, 1)], args=[variable_lin_op])
         out_view = backend.index(index_2d_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 2)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(2, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0],
-             [0, 1, 0, 0]]
-        )
+        expected = np.array([[1, 0, 0, 0], [0, 1, 0, 0]])
         assert np.all(A == expected)
 
         index_1d_lin_op = linOpHelper(data=[slice(0, 1, 1)], args=[variable_lin_op])
         out_view = backend.index(index_1d_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(1, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0]]
-        )
+        expected = np.array([[1, 0, 0, 0]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_diag_mat(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -310,36 +305,33 @@
          x11 x21 x12 x22
         [[1   0   0   0],
          [0   0   0   1]]
 
         -> It reduces to selecting a subset of the rows of A.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         diag_mat_lin_op = linOpHelper(shape=(2, 2), data=0)
         out_view = backend.diag_mat(diag_mat_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 2)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(2, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0],
-             [0, 0, 0, 1]]
-        )
+        expected = np.array([[1, 0, 0, 0], [0, 0, 0, 1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_diag_mat_with_offset(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -357,36 +349,34 @@
 
          x11 x21 x12 x22
         [[0   0   1   0]]
 
         -> It reduces to selecting a subset of the rows of A.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         k = 1
         diag_mat_lin_op = linOpHelper(shape=(1, 1), data=k)
         out_view = backend.diag_mat(diag_mat_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(1, 4)).toarray()
-        expected = np.array(
-            [[0, 0, 1, 0]]
-        )
+        expected = np.array([[0, 0, 1, 0]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_diag_vec(self, backend):
         """
         define x = Variable((2,)) with
         [x1, x2]
 
         x is represented as eye(2) in the A matrix, i.e.,
@@ -403,38 +393,33 @@
          x1  x2
         [[1  0],
          [0  0],
          [0  0],
          [0  1]]
         """
 
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 2)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(2, 2)).toarray()
         assert np.all(view_A == np.eye(2))
 
         diag_vec_lin_op = linOpHelper(shape=(2, 2), data=0)
         out_view = backend.diag_vec(diag_vec_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 2)).toarray()
-        expected = np.array(
-            [[1, 0],
-             [0, 0],
-             [0, 0],
-             [0, 1]]
-        )
+        expected = np.array([[1, 0], [0, 0], [0, 0], [0, 1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_diag_vec_with_offset(self, backend):
         """
         define x = Variable((2,)) with
         [x1, x2]
 
         x is represented as eye(2) in the A matrix, i.e.,
@@ -460,44 +445,36 @@
         [0  0],
         [0  0],
         [0  0],
         [0  1],
         [0  0]]
         """
 
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 2)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(2, 2)).toarray()
         assert np.all(view_A == np.eye(2))
 
         k = 1
         diag_vec_lin_op = linOpHelper(shape=(3, 3), data=k)
         out_view = backend.diag_vec(diag_vec_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 9)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(9, 2)).toarray()
         expected = np.array(
-            [[0, 0],
-             [0, 0],
-             [0, 0],
-             [1, 0],
-             [0, 0],
-             [0, 0],
-             [0, 0],
-             [0, 1],
-             [0, 0]]
+            [[0, 0], [0, 0], [0, 0], [1, 0], [0, 0], [0, 0], [0, 0], [0, 1], [0, 0]]
         )
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 9) == view.get_tensor_representation(0, 9)
 
     def test_sum_entries(self, backend):
         """
         define x = Variable((2,)) with
         [x1, x2]
 
         x is represented as eye(2) in the A matrix, i.e.,
@@ -510,35 +487,33 @@
 
         Thus, when using the same columns as before, we now have
 
          x1  x2
         [[1  1]]
         """
 
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 2)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(2, 2)).toarray()
         assert np.all(view_A == np.eye(2))
 
         sum_entries_lin_op = linOpHelper()
         out_view = backend.sum_entries(sum_entries_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(1, 2)).toarray()
-        expected = np.array(
-            [[1, 1]]
-        )
+        expected = np.array([[1, 1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_promote(self, backend):
         """
         define x = Variable((1,)) with
         [x1,]
 
         x is represented as eye(1) in the A matrix, i.e.,
@@ -552,57 +527,53 @@
 
          x1
         [[1],
          [1],
          [1]]
         """
 
-        variable_lin_op = linOpHelper((1,), type='variable', data=1)
+        variable_lin_op = linOpHelper((1,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 1)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(1, 1)).toarray()
         assert np.all(view_A == np.eye(1))
 
         promote_lin_op = linOpHelper((3,))
         out_view = backend.promote(promote_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(3, 1)).toarray()
-        expected = np.array(
-            [[1],
-             [1],
-             [1]]
-        )
+        expected = np.array([[1], [1], [1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_hstack(self, backend):
         """
         define x,y = Variable((1,)), Variable((1,))
 
         hstack([x, y]) means the expression should be represented in the A matrix as if it
         was a Variable of shape (2,), i.e.,
 
           x  y
         [[1  0],
          [0  1]]
         """
 
-        lin_op_x = linOpHelper((1,), type='variable', data=1)
-        lin_op_y = linOpHelper((1,), type='variable', data=2)
+        lin_op_x = linOpHelper((1,), type="variable", data=1)
+        lin_op_y = linOpHelper((1,), type="variable", data=2)
 
         hstack_lin_op = linOpHelper(args=[lin_op_x, lin_op_y])
         backend.id_to_col = {1: 0, 2: 1}
         out_view = backend.hstack(hstack_lin_op, backend.get_empty_view())
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 2)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(2, 2)).toarray()
         expected = np.eye(2)
         assert np.all(A == expected)
 
     def test_vstack(self, backend):
@@ -622,30 +593,25 @@
          x1   x2  y1  y2
         [[1   0   0   0],
          [0   0   1   0],
          [0   1   0   0],
          [0   0   0   1]]
         """
 
-        lin_op_x = linOpHelper((1, 2), type='variable', data=1)
-        lin_op_y = linOpHelper((1, 2), type='variable', data=2)
+        lin_op_x = linOpHelper((1, 2), type="variable", data=1)
+        lin_op_y = linOpHelper((1, 2), type="variable", data=2)
 
         vstack_lin_op = linOpHelper(args=[lin_op_x, lin_op_y])
         backend.id_to_col = {1: 0, 2: 2}
         out_view = backend.vstack(vstack_lin_op, backend.get_empty_view())
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0],
-             [0, 0, 1, 0],
-             [0, 1, 0, 0],
-             [0, 0, 0, 1]]
-        )
+        expected = np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]])
         assert np.all(A == expected)
 
     def test_mul(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
@@ -662,40 +628,35 @@
          x11 x21 x12 x22
         [[1   2   0   0],
          [3   4   0   0],
          [0   0   1   2],
          [0   0   3   4]]
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        lhs = linOpHelper((2, 2), type='dense_const', data=np.array([[1, 2], [3, 4]]))
+        lhs = linOpHelper((2, 2), type="dense_const", data=np.array([[1, 2], [3, 4]]))
 
         mul_lin_op = linOpHelper(data=lhs, args=[variable_lin_op])
         out_view = backend.mul(mul_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 4)).toarray()
-        expected = np.array(
-            [[1, 2, 0, 0],
-             [3, 4, 0, 0],
-             [0, 0, 1, 2],
-             [0, 0, 3, 4]]
-        )
+        expected = np.array([[1, 2, 0, 0], [3, 4, 0, 0], [0, 0, 1, 2], [0, 0, 3, 4]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_rmul(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -709,38 +670,35 @@
 
         i.e., when represented in the A matrix:
          x11 x21 x12 x22
         [[1   0   2   0],
          [0   1   0   2]]
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        rhs = linOpHelper((2,), type='dense_const', data=np.array([1, 2]))
+        rhs = linOpHelper((2,), type="dense_const", data=np.array([1, 2]))
 
         rmul_lin_op = linOpHelper(data=rhs, args=[variable_lin_op])
         out_view = backend.rmul(rmul_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 2)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(2, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 2, 0],
-             [0, 1, 0, 2]]
-        )
+        expected = np.array([[1, 0, 2, 0], [0, 1, 0, 2]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 2) == view.get_tensor_representation(0, 2)
 
     def test_mul_elementwise(self, backend):
         """
         define x = Variable((2,)) with
         [x1, x2]
 
         x is represented as eye(2) in the A matrix, i.e.,
@@ -753,38 +711,35 @@
          E.g. for a = (2,3), we obtain
 
          x1  x2
         [[2  0],
          [0  3]]
         """
 
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 2)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(2, 2)).toarray()
         assert np.all(view_A == np.eye(2))
 
-        lhs = linOpHelper((2,), type='dense_const', data=np.array([2, 3]))
+        lhs = linOpHelper((2,), type="dense_const", data=np.array([2, 3]))
 
         mul_elementwise_lin_op = linOpHelper(data=lhs)
         out_view = backend.mul_elem(mul_elementwise_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 2)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(2, 2)).toarray()
-        expected = np.array(
-            [[2, 0],
-             [0, 3]]
-        )
+        expected = np.array([[2, 0], [0, 3]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 2) == view.get_tensor_representation(0, 2)
 
     def test_div(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -796,40 +751,35 @@
          x11 x21 x12 x22
         [[1   0   0   0],
          [0   1/3 0   0],
          [0   0   1/2 0],
          [0   0   0   1/4]]
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        lhs = linOpHelper((2, 2), type='dense_const', data=np.array([[1, 2], [3, 4]]))
+        lhs = linOpHelper((2, 2), type="dense_const", data=np.array([[1, 2], [3, 4]]))
 
         div_lin_op = linOpHelper(data=lhs)
         out_view = backend.div(div_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 4)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(4, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 0],
-             [0, 1 / 3, 0, 0],
-             [0, 0, 1 / 2, 0],
-             [0, 0, 0, 1 / 4]]
-        )
+        expected = np.array([[1, 0, 0, 0], [0, 1 / 3, 0, 0], [0, 0, 1 / 2, 0], [0, 0, 0, 1 / 4]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_trace(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -843,35 +793,33 @@
 
         trace(x) means we sum the diagonal entries of x, i.e.
 
          x11 x21 x12 x22
         [[1   0   0   1]]
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
         trace_lin_op = linOpHelper(args=[variable_lin_op])
         out_view = backend.trace(trace_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 1)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(1, 4)).toarray()
-        expected = np.array(
-            [[1, 0, 0, 1]]
-        )
+        expected = np.array([[1, 0, 0, 1]])
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == view.get_tensor_representation(0, 1)
 
     def test_conv(self, backend):
         """
         define x = Variable((3,)) with
         [x1, x2, x3]
 
         having f = [1,2,3], conv(f, x) means we repeat the column vector of f for each column in
@@ -880,41 +828,37 @@
         [[1  0  0],
          [2  1  0],
          [3  2  1],
          [0  3  2],
          [0  0  3]]
         """
 
-        variable_lin_op = linOpHelper((3,), type='variable', data=1)
+        variable_lin_op = linOpHelper((3,), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 3)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(3, 3)).toarray()
         assert np.all(view_A == np.eye(3))
 
-        f = linOpHelper((3,), type='dense_const', data=np.array([1, 2, 3]))
+        f = linOpHelper((3,), type="dense_const", data=np.array([1, 2, 3]))
         conv_lin_op = linOpHelper(data=f, shape=(5, 1), args=[variable_lin_op])
 
         out_view = backend.conv(conv_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 5)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(5, 3)).toarray()
         expected = np.array(
-            [[1., 0., 0.],
-             [2., 1., 0.],
-             [3., 2., 1.],
-             [0., 3., 2.],
-             [0., 0., 3.]]
+            [[1.0, 0.0, 0.0], [2.0, 1.0, 0.0], [3.0, 2.0, 1.0], [0.0, 3.0, 2.0], [0.0, 0.0, 3.0]]
         )
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 5) == view.get_tensor_representation(0, 5)
 
     def test_kron_r(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -922,15 +866,15 @@
         a = [[1],
              [2]],
 
         kron(a, x) means we have
         [[x11, x12],
          [x21, x22],
          [2x11, 2x12],
-         [2x21, 2x22]]        
+         [2x21, 2x22]]
 
         i.e. as represented in the A matrix (again in column-major order)
 
          x11 x21 x12 x22
         [[1   0   0   0],
          [0   1   0   0],
          [2   0   0   0],
@@ -949,44 +893,46 @@
          [0   0   1   0],
          [0   0   2   0],
          [0   0   0   1],
          [0   0   0   2]]
         So we must swap the row indices of the resulting matrix.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        a = linOpHelper((2, 1), type='dense_const', data=np.array([[1], [2]]))
+        a = linOpHelper((2, 1), type="dense_const", data=np.array([[1], [2]]))
         kron_r_lin_op = linOpHelper(data=a, args=[variable_lin_op])
 
         out_view = backend.kron_r(kron_r_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 8)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(8, 4)).toarray()
         expected = np.array(
-            [[1., 0., 0., 0.],
-             [0., 1., 0., 0.],
-             [2., 0., 0., 0.],
-             [0., 2., 0., 0.],
-             [0., 0., 1., 0.],
-             [0., 0., 0., 1.],
-             [0., 0., 2., 0.],
-             [0., 0., 0., 2.]]
+            [
+                [1.0, 0.0, 0.0, 0.0],
+                [0.0, 1.0, 0.0, 0.0],
+                [2.0, 0.0, 0.0, 0.0],
+                [0.0, 2.0, 0.0, 0.0],
+                [0.0, 0.0, 1.0, 0.0],
+                [0.0, 0.0, 0.0, 1.0],
+                [0.0, 0.0, 2.0, 0.0],
+                [0.0, 0.0, 0.0, 2.0],
+            ]
         )
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 8) == view.get_tensor_representation(0, 8)
 
     def test_kron_l(self, backend):
         """
         define x = Variable((2,2)) with
         [[x11, x12],
          [x21, x22]]
 
@@ -1018,71 +964,73 @@
          [0   0   1   0],
          [0   0   2   0],
          [0   0   0   1],
          [0   0   0   2]]
         So we must swap the row indices of the resulting matrix.
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         view = backend.process_constraint(variable_lin_op, backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        a = linOpHelper((1, 2), type='dense_const', data=np.array([[1, 2]]))
+        a = linOpHelper((1, 2), type="dense_const", data=np.array([[1, 2]]))
         kron_l_lin_op = linOpHelper(data=a, args=[variable_lin_op])
 
         out_view = backend.kron_l(kron_l_lin_op, view)
-        A = out_view.get_tensor_representation(0)
+        A = out_view.get_tensor_representation(0, 8)
 
         # cast to numpy
         A = sp.coo_matrix((A.data, (A.row, A.col)), shape=(8, 4)).toarray()
         expected = np.array(
-            [[1., 0., 0., 0.],
-             [0., 1., 0., 0.],
-             [2., 0., 0., 0.],
-             [0., 2., 0., 0.],
-             [0., 0., 1., 0.],
-             [0., 0., 0., 1.],
-             [0., 0., 2., 0.],
-             [0., 0., 0., 2.]]
+            [
+                [1.0, 0.0, 0.0, 0.0],
+                [0.0, 1.0, 0.0, 0.0],
+                [2.0, 0.0, 0.0, 0.0],
+                [0.0, 2.0, 0.0, 0.0],
+                [0.0, 0.0, 1.0, 0.0],
+                [0.0, 0.0, 0.0, 1.0],
+                [0.0, 0.0, 2.0, 0.0],
+                [0.0, 0.0, 0.0, 2.0],
+            ]
         )
         assert np.all(A == expected)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 8) == view.get_tensor_representation(0, 8)
 
     def test_get_kron_row_indices(self, backend):
         """
         kron(l,r)
-        with 
+        with
         l = [[x1, x3],  r = [[a],
              [x2, x4]]       [b]]
 
         yields
         [[ax1, ax3],
          [bx1, bx3],
          [ax2, ax4],
          [bx2, bx4]]
-        
-        Which is what we get when we compute kron(l,r) directly, 
+
+        Which is what we get when we compute kron(l,r) directly,
         as l is represented as eye(4) and r is reshaped into a column vector.
-        
+
         So we have:
-        kron(l,r) = 
+        kron(l,r) =
         [[a, 0, 0, 0],
          [b, 0, 0, 0],
          [0, a, 0, 0],
          [0, b, 0, 0],
          [0, 0, a, 0],
          [0, 0, b, 0],
          [0, 0, 0, a],
-         [0, 0, 0, b]].            
+         [0, 0, 0, b]].
 
         Thus, this function should return arange(8).
         """
         indices = backend._get_kron_row_indices((2, 2), (2, 1))
         assert np.all(indices == np.arange(8))
 
         """
@@ -1135,24 +1083,23 @@
         b = {"b": [2]}
         assert view.combine_potentially_none(a, None) == a
         assert view.combine_potentially_none(None, a) == a
         assert view.combine_potentially_none(a, b) == view.add_dicts(a, b)
 
 
 class TestParametrizedBackends:
-
     @staticmethod
     @pytest.fixture(params=backends)
     def param_backend(request):
         kwargs = {
             "id_to_col": {1: 0},
             "param_to_size": {-1: 1, 2: 2},
             "param_to_col": {2: 0, -1: 2},
             "param_size_plus_one": 3,
-            "var_length": 2
+            "var_length": 2,
         }
 
         backend = CanonBackend.get_backend(request.param, **kwargs)
         assert isinstance(backend, PythonCanonBackend)
         return backend
 
     def test_parametrized_diag_vec(self, param_backend):
@@ -1178,45 +1125,37 @@
 
          [[0  0],
           [0  0],
           [0  0],
           [0  1]]]
         """
 
-        param_lin_op = linOpHelper((2,), type='param', data=2)
+        param_lin_op = linOpHelper((2,), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 3}
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
         diag_vec_lin_op = linOpHelper(shape=(2, 2), data=0)
         out_view = param_backend.diag_vec(diag_vec_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 4)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (4, 2)).toarray()
-        expected_idx_zero = np.array(
-            [[1., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.]]
-        )
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
+        expected_idx_zero = np.array([[1.0, 0.0], [0.0, 0.0], [0.0, 0.0], [0.0, 0.0]])
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (4, 2)).toarray()
-        expected_idx_one = np.array(
-            [[0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 1.]]
-        )
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
+        expected_idx_one = np.array([[0.0, 0.0], [0.0, 0.0], [0.0, 0.0], [0.0, 1.0]])
         assert np.all(slice_idx_one == expected_idx_one)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == param_var_view.get_tensor_representation(
+            0, 4
+        )
 
     def test_parametrized_diag_vec_with_offset(self, param_backend):
         """
         Starting with a parametrized expression
         x1  x2
         [[[1  0],
           [0  0]],
@@ -1242,56 +1181,62 @@
          [0  0],         [0  0],
          [0  0],         [0  0],
          [0  0],         [0  0],
          [0  0],         [0  1],
          [0  0]]         [0  0]]
         """
 
-        param_lin_op = linOpHelper((2,), type='param', data=2)
+        param_lin_op = linOpHelper((2,), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 3}
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
         k = 1
         diag_vec_lin_op = linOpHelper(shape=(3, 3), data=k)
         out_view = param_backend.diag_vec(diag_vec_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 9)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (9, 2)).toarray()
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
         expected_idx_zero = np.array(
-            [[0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [1., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.]]
+            [
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [1.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+            ]
         )
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (9, 2)).toarray()
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
         expected_idx_one = np.array(
-            [[0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 0.],
-             [0., 1.],
-             [0., 0.]]
+            [
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 0.0],
+                [0.0, 1.0],
+                [0.0, 0.0],
+            ]
         )
         assert np.all(slice_idx_one == expected_idx_one)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 9) == param_var_view.get_tensor_representation(
+            0, 9
+        )
 
     def test_parametrized_sum_entries(self, param_backend):
         """
         starting with a parametrized expression
         x1  x2
         [[[1  0],
          [0  0]],
@@ -1304,39 +1249,37 @@
         Thus, when using the same columns as before, we now have
 
          x1  x2
         [[[1  0]],
 
          [[0  1]]]
         """
-        param_lin_op = linOpHelper((2,), type='param', data=2)
+        param_lin_op = linOpHelper((2,), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 3}
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
         sum_entries_lin_op = linOpHelper()
         out_view = param_backend.sum_entries(sum_entries_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 1)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (1, 2)).toarray()
-        expected_idx_zero = np.array(
-            [[1., 0.]]
-        )
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
+        expected_idx_zero = np.array([[1.0, 0.0]])
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (1, 2)).toarray()
-        expected_idx_one = np.array(
-            [[0., 1.]]
-        )
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
+        expected_idx_one = np.array([[0.0, 1.0]])
         assert np.all(slice_idx_one == expected_idx_one)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == param_var_view.get_tensor_representation(
+            0, 1
+        )
 
     def test_parametrized_mul(self, param_backend):
         """
         Continuing from the non-parametrized example when the lhs is a parameter,
         instead of multiplying with known values, the matrix is split up into four slices,
         each representing an element of the parameter, i.e. instead of
          x11 x21 x12 x22
@@ -1367,79 +1310,67 @@
 
             [[0   0   0   0],
              [0   1   0   0],
              [0   0   0   0],
              [0   0   0   1]]
         ]
         """
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         param_backend.param_to_size = {-1: 1, 2: 4}
         param_backend.param_to_col = {2: 0, -1: 4}
         param_backend.param_size_plus_one = 5
         param_backend.var_length = 4
         view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        lhs_parameter = linOpHelper((2, 2), type='param', data=2)
+        lhs_parameter = linOpHelper((2, 2), type="param", data=2)
 
         mul_lin_op = linOpHelper(data=lhs_parameter, args=[variable_lin_op])
         out_view = param_backend.mul(mul_lin_op, view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 4)
 
         # indices are: variable 1, parameter 2, 0 index of the list
-        slice_idx_zero = out_repr.get_param_slice(0, (4, 4)).toarray()
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
         expected_idx_zero = np.array(
-            [[1., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 1., 0.],
-             [0., 0., 0., 0.]]
+            [[1.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 1.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_zero == expected_idx_zero)
 
         # indices are: variable 1, parameter 2, 1 index of the list
-        slice_idx_one = out_repr.get_param_slice(1, (4, 4)).toarray()
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
         expected_idx_one = np.array(
-            [[0., 0., 0., 0.],
-             [1., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 1., 0.]]
+            [[0.0, 0.0, 0.0, 0.0], [1.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 1.0, 0.0]]
         )
         assert np.all(slice_idx_one == expected_idx_one)
 
         # indices are: variable 1, parameter 2, 2 index of the list
-        slice_idx_two = out_repr.get_param_slice(2, (4, 4)).toarray()
+        slice_idx_two = out_repr.get_param_slice(2).toarray()[:, :-1]
         expected_idx_two = np.array(
-            [[0., 1., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 1.],
-             [0., 0., 0., 0.]]
+            [[0.0, 1.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 1.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_two == expected_idx_two)
 
         # indices are: variable 1, parameter 2, 3 index of the list
-        slice_idx_three = out_repr.get_param_slice(3, (4, 4)).toarray()
+        slice_idx_three = out_repr.get_param_slice(3).toarray()[:, :-1]
         expected_idx_three = np.array(
-            [[0., 0., 0., 0.],
-             [0., 1., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 1.]]
+            [[0.0, 0.0, 0.0, 0.0], [0.0, 1.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 1.0]]
         )
         assert np.all(slice_idx_three == expected_idx_three)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == view.get_tensor_representation(0, 4)
 
     def test_parametrized_rhs_mul(self, param_backend):
         """
         Continuing from the non-parametrized example when the expression
-        that is multiplied by is parametrized. For a variable that 
+        that is multiplied by is parametrized. For a variable that
         was multiplied elementwise by a parameter, instead of
          x11 x21 x12 x22
         [[1   2   0   0],
          [3   4   0   0],
          [0   0   1   2],
          [0   0   3   4]]
 
@@ -1465,66 +1396,57 @@
 
             [[0   0   0   0],
              [0   0   0   0],
              [0   0   0   2],
              [0   0   0   4]]
         ]
         """
-        param_lin_op = linOpHelper((2, 2), type='param', data=2)
+        param_lin_op = linOpHelper((2, 2), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 4}
         param_backend.param_to_size = {-1: 1, 2: 4}
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        param_backend.var_length = 4
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
-        lhs = linOpHelper((2, 2), type='dense_const', data=np.array([[1, 2], [3, 4]]))
+        lhs = linOpHelper((2, 2), type="dense_const", data=np.array([[1, 2], [3, 4]]))
 
         mul_lin_op = linOpHelper(data=lhs, args=[variable_lin_op])
         out_view = param_backend.mul(mul_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 4)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (4, 4)).toarray()
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
         expected_idx_zero = np.array(
-            [[1., 0., 0., 0.],
-             [3., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.]]
+            [[1.0, 0.0, 0.0, 0.0], [3.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (4, 4)).toarray()
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
         expected_idx_one = np.array(
-            [[0., 2., 0., 0.],
-             [0., 4., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.]]
+            [[0.0, 2.0, 0.0, 0.0], [0.0, 4.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_one == expected_idx_one)
 
-        slice_idx_two = out_repr.get_param_slice(2, (4, 4)).toarray()
+        slice_idx_two = out_repr.get_param_slice(2).toarray()[:, :-1]
         expected_idx_two = np.array(
-            [[0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 1., 0.],
-             [0., 0., 3., 0.]]
+            [[0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 1.0, 0.0], [0.0, 0.0, 3.0, 0.0]]
         )
         assert np.all(slice_idx_two == expected_idx_two)
 
-        slice_idx_three = out_repr.get_param_slice(3, (4, 4)).toarray()
+        slice_idx_three = out_repr.get_param_slice(3).toarray()[:, :-1]
         expected_idx_three = np.array(
-            [[0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 2.],
-             [0., 0., 0., 4.]]
+            [[0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 2.0], [0.0, 0.0, 0.0, 4.0]]
         )
         assert np.all(slice_idx_three == expected_idx_three)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == param_var_view.get_tensor_representation(
+            0, 4
+        )
 
     def test_parametrized_rmul(self, param_backend):
         """
         Continuing from the non-parametrized example when the rhs is a parameter,
         instead of multiplying with known values, the matrix is split up into two slices,
         each representing an element of the parameter, i.e. instead of
          x11 x21 x12 x22
@@ -1540,52 +1462,46 @@
           [0   1   0   0]]
 
          [[0   0   1   0],
           [0   0   0   1]]
         ]
         """
 
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         param_backend.var_length = 4
         view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 4)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(4, 4)).toarray()
         assert np.all(view_A == np.eye(4))
 
-        rhs_parameter = linOpHelper((2,), type='param', data=2)
+        rhs_parameter = linOpHelper((2,), type="param", data=2)
 
         rmul_lin_op = linOpHelper(data=rhs_parameter, args=[variable_lin_op])
         out_view = param_backend.rmul(rmul_lin_op, view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 2)
 
         # indices are: variable 1, parameter 2, 0 index of the list
-        slice_idx_zero = out_repr.get_param_slice(0, (2, 4)).toarray()
-        expected_idx_zero = np.array(
-            [[1, 0, 0, 0],
-             [0, 1, 0, 0]]
-        )
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
+        expected_idx_zero = np.array([[1, 0, 0, 0], [0, 1, 0, 0]])
         assert np.all(slice_idx_zero == expected_idx_zero)
 
         # indices are: variable 1, parameter 2, 1 index of the list
-        slice_idx_one = out_repr.get_param_slice(1, (2, 4)).toarray()
-        expected_idx_one = np.array(
-            [[0, 0, 1, 0],
-             [0, 0, 0, 1]]
-        )
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
+        expected_idx_one = np.array([[0, 0, 1, 0], [0, 0, 0, 1]])
         assert np.all(slice_idx_one == expected_idx_one)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 2) == view.get_tensor_representation(0, 2)
 
     def test_parametrized_rhs_rmul(self, param_backend):
         """
         Continuing from the non-parametrized example when the expression
-        that is multiplied by is parametrized. For a variable that 
+        that is multiplied by is parametrized. For a variable that
         was multiplied elementwise by a parameter, instead of
 
          x11 x21 x12 x22
         [[1   0   3   0],
          [0   1   0   3],
          [2   0   4   0],
          [0   2   0   4]]
@@ -1612,67 +1528,57 @@
 
          [[0   0   0   0],
           [0   0   0   3],
           [0   0   0   0],
           [0   0   0   4]]
         ]
         """
-        param_lin_op = linOpHelper((2, 2), type='param', data=2)
+        param_lin_op = linOpHelper((2, 2), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 4}
         param_backend.param_to_size = {-1: 1, 2: 4}
         param_backend.var_length = 4
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
-        rhs = linOpHelper((2, 2), type='dense_const', data=np.array([[1, 2], [3, 4]]))
+        rhs = linOpHelper((2, 2), type="dense_const", data=np.array([[1, 2], [3, 4]]))
 
         rmul_lin_op = linOpHelper(data=rhs, args=[variable_lin_op])
         out_view = param_backend.rmul(rmul_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 4)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (4, 4)).toarray()
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
         expected_idx_zero = np.array(
-            [[1., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [2., 0., 0., 0.],
-             [0., 0., 0., 0.]]
+            [[1.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [2.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (4, 4)).toarray()
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
         expected_idx_one = np.array(
-            [[0., 0., 0., 0.],
-             [0., 1., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 2., 0., 0.]]
+            [[0.0, 0.0, 0.0, 0.0], [0.0, 1.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 2.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_one == expected_idx_one)
 
-        slice_idx_two = out_repr.get_param_slice(2, (4, 4)).toarray()
+        slice_idx_two = out_repr.get_param_slice(2).toarray()[:, :-1]
         expected_idx_two = np.array(
-            [[0., 0., 3., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 4., 0.],
-             [0., 0., 0., 0.]]
+            [[0.0, 0.0, 3.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 4.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_two == expected_idx_two)
 
-        slice_idx_three = out_repr.get_param_slice(3, (4, 4)).toarray()
+        slice_idx_three = out_repr.get_param_slice(3).toarray()[:, :-1]
         expected_idx_three = np.array(
-            [[0., 0., 0., 0.],
-             [0., 0., 0., 3.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 4.]]
+            [[0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 3.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 4.0]]
         )
         assert np.all(slice_idx_three == expected_idx_three)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == param_var_view.get_tensor_representation(
+            0, 4
+        )
 
     def test_mul_elementwise_parametrized(self, param_backend):
         """
         Continuing the non-parametrized example when 'a' is a parameter, instead of multiplying
         with known values, the matrix is split up into two slices, each representing an element
         of the parameter, i.e. instead of
          x1  x2
@@ -1687,51 +1593,45 @@
           [0  0]],
 
          [[0  0],
           [0  1]]
         ]
         """
 
-        variable_lin_op = linOpHelper((2,), type='variable', data=1)
+        variable_lin_op = linOpHelper((2,), type="variable", data=1)
         view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
 
         # cast to numpy
-        view_A = view.get_tensor_representation(0)
+        view_A = view.get_tensor_representation(0, 2)
         view_A = sp.coo_matrix((view_A.data, (view_A.row, view_A.col)), shape=(2, 2)).toarray()
         assert np.all(view_A == np.eye(2))
 
-        lhs_parameter = linOpHelper((2,), type='param', data=2)
+        lhs_parameter = linOpHelper((2,), type="param", data=2)
 
         mul_elementwise_lin_op = linOpHelper(data=lhs_parameter)
         out_view = param_backend.mul_elem(mul_elementwise_lin_op, view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 2)
 
         # indices are: variable 1, parameter 2, 0 index of the list
-        slice_idx_zero = out_repr.get_param_slice(0, (2, 2)).toarray()
-        expected_idx_zero = np.array(
-            [[1, 0],
-             [0, 0]]
-        )
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
+        expected_idx_zero = np.array([[1, 0], [0, 0]])
         assert np.all(slice_idx_zero == expected_idx_zero)
 
         # indices are: variable 1, parameter 2, 1 index of the list
-        slice_idx_one = out_repr.get_param_slice(1, (2, 2)).toarray()
-        expected_idx_one = np.array(
-            [[0, 0],
-             [0, 1]]
-        )
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
+        expected_idx_one = np.array([[0, 0], [0, 1]])
         assert np.all(slice_idx_one == expected_idx_one)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 2) == view.get_tensor_representation(0, 2)
 
     def test_parametrized_div(self, param_backend):
         """
         Continuing from the non-parametrized example when the expression
-        that is divided by is parametrized. For a variable that 
+        that is divided by is parametrized. For a variable that
         was multiplied elementwise by a parameter, instead of
          x11 x21 x12 x22
         [[1   0   0   0],
          [0   1/3 0   0],
          [0   0   1/2 0],
          [0   0   0   1/4]]
 
@@ -1757,65 +1657,71 @@
 
             [[0   0   0   0],
              [0   0   0   0],
              [0   0   0   0],
              [0   0   0   1/4]]
         ]
         """
-        param_lin_op = linOpHelper((2, 2), type='param', data=2)
+        param_lin_op = linOpHelper((2, 2), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 4}
         param_backend.param_to_size = {-1: 1, 2: 4}
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        param_backend.var_length = 4
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
-        lhs = linOpHelper((2, 2), type='dense_const', data=np.array([[1, 2], [3, 4]]))
+        lhs = linOpHelper((2, 2), type="dense_const", data=np.array([[1, 2], [3, 4]]))
 
         div_lin_op = linOpHelper(data=lhs)
         out_view = param_backend.div(div_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 4)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (4, 4)).toarray()
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
         expected_idx_zero = np.array(
-            [[1., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.]]
+            [[1.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0]]
         )
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (4, 4)).toarray()
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
         expected_idx_one = np.array(
-            [[0., 0., 0., 0.],
-             [0., 1/3, 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.]]
+            [
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 1 / 3, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+            ]
         )
         assert np.all(slice_idx_one == expected_idx_one)
 
-        slice_idx_two = out_repr.get_param_slice(2, (4, 4)).toarray()
+        slice_idx_two = out_repr.get_param_slice(2).toarray()[:, :-1]
         expected_idx_two = np.array(
-            [[0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 1/2, 0.],
-             [0., 0., 0., 0.]]
+            [
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 1 / 2, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+            ]
         )
         assert np.all(slice_idx_two == expected_idx_two)
 
-        slice_idx_three = out_repr.get_param_slice(3, (4, 4)).toarray()
+        slice_idx_three = out_repr.get_param_slice(3).toarray()[:, :-1]
         expected_idx_three = np.array(
-            [[0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 0.],
-             [0., 0., 0., 1/4]]
+            [
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 0.0],
+                [0.0, 0.0, 0.0, 1 / 4],
+            ]
         )
         assert np.all(slice_idx_three == expected_idx_three)
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 4) == param_var_view.get_tensor_representation(
+            0, 4
+        )
 
     def test_parametrized_trace(self, param_backend):
         """
         Continuing from the non-parametrized example, instead of a pure variable
         input, we take a variable that has been multiplied elementwise by a parameter.
 
         The trace of this expression is then given by
@@ -1827,64 +1733,59 @@
             [[0   0   0   0]],
 
             [[0   0   0   0]],
 
             [[0   0   0   1]]
         ]
         """
-        param_lin_op = linOpHelper((2, 2), type='param', data=2)
+        param_lin_op = linOpHelper((2, 2), type="param", data=2)
         param_backend.param_to_col = {2: 0, -1: 4}
         param_backend.param_to_size = {-1: 1, 2: 4}
-        variable_lin_op = linOpHelper((2, 2), type='variable', data=1)
+        param_backend.var_length = 4
+        variable_lin_op = linOpHelper((2, 2), type="variable", data=1)
         var_view = param_backend.process_constraint(variable_lin_op, param_backend.get_empty_view())
         mul_elem_lin_op = linOpHelper(data=param_lin_op)
         param_var_view = param_backend.mul_elem(mul_elem_lin_op, var_view)
 
         trace_lin_op = linOpHelper(args=[variable_lin_op])
         out_view = param_backend.trace(trace_lin_op, param_var_view)
-        out_repr = out_view.get_tensor_representation(0)
+        out_repr = out_view.get_tensor_representation(0, 1)
 
-        slice_idx_zero = out_repr.get_param_slice(0, (1, 4)).toarray()
-        expected_idx_zero = np.array(
-            [[1., 0., 0., 0.]]
-        )
+        slice_idx_zero = out_repr.get_param_slice(0).toarray()[:, :-1]
+        expected_idx_zero = np.array([[1.0, 0.0, 0.0, 0.0]])
         assert np.all(slice_idx_zero == expected_idx_zero)
 
-        slice_idx_one = out_repr.get_param_slice(1, (1, 4)).toarray()
-        expected_idx_one = np.array(
-            [[0., 0., 0., 0.]]
-        )
+        slice_idx_one = out_repr.get_param_slice(1).toarray()[:, :-1]
+        expected_idx_one = np.array([[0.0, 0.0, 0.0, 0.0]])
         assert np.all(slice_idx_one == expected_idx_one)
 
-        slice_idx_two = out_repr.get_param_slice(2, (1, 4)).toarray()
-        expected_idx_two = np.array(
-            [[0., 0., 0., 0.]]
-        )
+        slice_idx_two = out_repr.get_param_slice(2).toarray()[:, :-1]
+        expected_idx_two = np.array([[0.0, 0.0, 0.0, 0.0]])
         assert np.all(slice_idx_two == expected_idx_two)
 
-        slice_idx_three = out_repr.get_param_slice(3, (1, 4)).toarray()
-        expected_idx_three = np.array(
-            [[0., 0., 0., 1.]]
-        )
+        slice_idx_three = out_repr.get_param_slice(3).toarray()[:, :-1]
+        expected_idx_three = np.array([[0.0, 0.0, 0.0, 1.0]])
         assert np.all(slice_idx_three == expected_idx_three)
 
         # Note: view is edited in-place:
-        assert out_view.get_tensor_representation(0) == param_var_view.get_tensor_representation(0)
+        assert out_view.get_tensor_representation(0, 1) == param_var_view.get_tensor_representation(
+            0, 1
+        )
 
 
 class TestNumPyBackend:
     @staticmethod
     @pytest.fixture()
     def numpy_backend():
         kwargs = {
             "id_to_col": {1: 0},
             "param_to_size": {-1: 1, 2: 2},
             "param_to_col": {2: 0, -1: 2},
             "param_size_plus_one": 3,
-            "var_length": 2
+            "var_length": 2,
         }
         backend = CanonBackend.get_backend(s.NUMPY_CANON_BACKEND, **kwargs)
         assert isinstance(backend, NumPyCanonBackend)
         return backend
 
     def test_get_variable_tensor(self, numpy_backend):
         outer = numpy_backend.get_variable_tensor((2,), 1)
@@ -1892,15 +1793,15 @@
         inner = outer[1]
         assert inner.keys() == {-1}, "Should only be in parameter slice -1, i.e. non parametrized."
         tensor = inner[-1]
         assert isinstance(tensor, np.ndarray), "Should be a numpy array"
         assert tensor.shape == (1, 2, 2), "Should be a 1x2x2 tensor"
         assert np.all(tensor[0] == np.eye(2)), "Should be eye(2)"
 
-    @pytest.mark.parametrize('data', [np.array([[1, 2], [3, 4]]), sp.eye(2) * 4])
+    @pytest.mark.parametrize("data", [np.array([[1, 2], [3, 4]]), sp.eye(2) * 4])
     def test_get_data_tensor(self, numpy_backend, data):
         outer = numpy_backend.get_data_tensor(data)
         assert outer.keys() == {-1}, "Should only be constant variable ID."
         inner = outer[-1]
         assert inner.keys() == {-1}, "Should only be in parameter slice -1, i.e. non parametrized."
         tensor = inner[-1]
         assert isinstance(tensor, np.ndarray), "Should be a numpy array"
@@ -1915,42 +1816,43 @@
         outer = numpy_backend.get_param_tensor(shape, 3)
         assert outer.keys() == {-1}, "Should only be constant variable ID."
         inner = outer[-1]
         assert inner.keys() == {3}, "Should only be the parameter slice of parameter with id 3."
         tensor = inner[3]
         assert isinstance(tensor, np.ndarray), "Should be a numpy array"
         assert tensor.shape == (4, 4, 1), "Should be a 4x4x1 tensor"
-        assert np.all(tensor[:, :, 0] == np.eye(size)), 'Should be eye(4) along axes 1 and 2'
+        assert np.all(tensor[:, :, 0] == np.eye(size)), "Should be eye(4) along axes 1 and 2"
 
     def test_tensor_view_add_dicts(self, numpy_backend):
         view = numpy_backend.get_empty_view()
 
         one = np.array([1])
         two = np.array([2])
         three = np.array([3])
 
         assert view.add_dicts({}, {}) == {}
         assert view.add_dicts({"a": one}, {"a": two}) == {"a": three}
         assert view.add_dicts({"a": one}, {"b": two}) == {"a": one, "b": two}
-        assert view.add_dicts({"a": {"c": one}}, {"a": {"c": one}}) == {'a': {'c': two}}
-        with pytest.raises(ValueError,
-                           match="Values must either be dicts or <class 'numpy.ndarray'>"):
+        assert view.add_dicts({"a": {"c": one}}, {"a": {"c": one}}) == {"a": {"c": two}}
+        with pytest.raises(
+            ValueError, match="Values must either be dicts or <class 'numpy.ndarray'>"
+        ):
             view.add_dicts({"a": 1}, {"a": 2})
 
 
 class TestSciPyBackend:
     @staticmethod
     @pytest.fixture()
     def scipy_backend():
         kwargs = {
             "id_to_col": {1: 0},
             "param_to_size": {-1: 1, 2: 2},
             "param_to_col": {2: 0, -1: 2},
             "param_size_plus_one": 3,
-            "var_length": 2
+            "var_length": 2,
         }
         backend = CanonBackend.get_backend(s.SCIPY_CANON_BACKEND, **kwargs)
         assert isinstance(backend, SciPyCanonBackend)
         return backend
 
     def test_get_variable_tensor(self, scipy_backend):
         outer = scipy_backend.get_variable_tensor((2,), 1)
@@ -1958,15 +1860,15 @@
         inner = outer[1]
         assert inner.keys() == {-1}, "Should only be in parameter slice -1, i.e. non parametrized."
         tensor = inner[-1]
         assert isinstance(tensor, sp.spmatrix), "Should be a scipy sparse matrix"
         assert tensor.shape == (2, 2), "Should be a 1*2x2 tensor"
         assert np.all(tensor == np.eye(2)), "Should be eye(2)"
 
-    @pytest.mark.parametrize('data', [np.array([[1, 2], [3, 4]]), sp.eye(2) * 4])
+    @pytest.mark.parametrize("data", [np.array([[1, 2], [3, 4]]), sp.eye(2) * 4])
     def test_get_data_tensor(self, scipy_backend, data):
         outer = scipy_backend.get_data_tensor(data)
         assert outer.keys() == {-1}, "Should only be constant variable ID."
         inner = outer[-1]
         assert inner.keys() == {-1}, "Should only be in parameter slice -1, i.e. non parametrized."
         tensor = inner[-1]
         assert isinstance(tensor, sp.spmatrix), "Should be a scipy sparse matrix"
@@ -1981,48 +1883,49 @@
         outer = scipy_backend.get_param_tensor(shape, 3)
         assert outer.keys() == {-1}, "Should only be constant variable ID."
         inner = outer[-1]
         assert inner.keys() == {3}, "Should only be the parameter slice of parameter with id 3."
         tensor = inner[3]
         assert isinstance(tensor, sp.spmatrix), "Should be a scipy sparse matrix"
         assert tensor.shape == (16, 1), "Should be a 4*4x1 tensor"
-        assert (tensor.reshape((size, size)) != sp.eye(size, format='csr')).nnz == 0, \
-            'Should be eye(4) when reshaping'
+        assert (
+            tensor.reshape((size, size)) != sp.eye(size, format="csr")
+        ).nnz == 0, "Should be eye(4) when reshaping"
 
     def test_tensor_view_add_dicts(self, scipy_backend):
         view = scipy_backend.get_empty_view()
 
         one = sp.eye(1)
         two = sp.eye(1) * 2
         three = sp.eye(1) * 3
 
         assert view.add_dicts({}, {}) == {}
         assert view.add_dicts({"a": one}, {"a": two}) == {"a": three}
         assert view.add_dicts({"a": one}, {"b": two}) == {"a": one, "b": two}
-        assert view.add_dicts({"a": {"c": one}}, {"a": {"c": one}}) == {'a': {'c': two}}
-        with pytest.raises(ValueError,
-                           match="Values must either be dicts or "
-                                 "<class 'scipy.sparse."):
+        assert view.add_dicts({"a": {"c": one}}, {"a": {"c": one}}) == {"a": {"c": two}}
+        with pytest.raises(
+            ValueError, match="Values must either be dicts or " "<class 'scipy.sparse."
+        ):
             view.add_dicts({"a": 1}, {"a": 2})
 
     @staticmethod
-    @pytest.mark.parametrize('shape', [(1, 1), (2, 2), (3, 3), (4, 4)])
+    @pytest.mark.parametrize("shape", [(1, 1), (2, 2), (3, 3), (4, 4)])
     def test_stacked_kron_r(shape, scipy_backend):
         p = 2
         reps = 3
         param_id = 2
         matrices = [sp.random(*shape, random_state=i, density=0.5) for i in range(p)]
         stacked = sp.vstack(matrices)
         repeated = scipy_backend._stacked_kron_r({param_id: stacked}, reps)
         repeated = repeated[param_id]
         expected = sp.vstack([sp.kron(sp.eye(reps), m) for m in matrices])
         assert (expected != repeated).nnz == 0
 
     @staticmethod
-    @pytest.mark.parametrize('shape', [(1, 1), (2, 2), (3, 3), (4, 4)])
+    @pytest.mark.parametrize("shape", [(1, 1), (2, 2), (3, 3), (4, 4)])
     def test_stacked_kron_l(shape, scipy_backend):
         p = 2
         reps = 3
         param_id = 2
         matrices = [sp.random(*shape, random_state=i, density=0.5) for i in range(p)]
         stacked = sp.vstack(matrices)
         repeated = scipy_backend._stacked_kron_l({param_id: stacked}, reps)
@@ -2030,21 +1933,21 @@
         expected = sp.vstack([sp.kron(m, sp.eye(reps)) for m in matrices])
         assert (expected != repeated).nnz == 0
 
     @staticmethod
     def test_reshape_single_constant_tensor(scipy_backend):
         a = sp.csc_matrix(np.tile(np.arange(6), 3).reshape((-1, 1)))
         reshaped = scipy_backend._reshape_single_constant_tensor(a, (3, 2))
-        expected = np.arange(6).reshape((3, 2), order='F')
+        expected = np.arange(6).reshape((3, 2), order="F")
         expected = sp.csc_matrix(np.tile(expected, (3, 1)))
         assert (reshaped != expected).nnz == 0
 
     @staticmethod
-    @pytest.mark.parametrize('shape', [(1, 1), (2, 2), (3, 2), (2, 3)])
+    @pytest.mark.parametrize("shape", [(1, 1), (2, 2), (3, 2), (2, 3)])
     def test_transpose_stacked(shape, scipy_backend):
         p = 2
         param_id = 2
         matrices = [sp.random(*shape, random_state=i, density=0.5) for i in range(p)]
         stacked = sp.vstack(matrices)
         transposed = scipy_backend._transpose_stacked(stacked, param_id)
         expected = sp.vstack([m.T for m in matrices])
-        assert (expected != transposed).nnz == 0
+        assert (expected != transposed).nnz == 0
```

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_qp_solvers.py` & `cvxpy-1.4.3/cvxpy/tests/test_qp_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,33 +347,35 @@
         p = Problem(Minimize(objective), [x[2] >= 3])
         self.solve_QP(p, solver)
         self.assertAlmostEqual(3, x.value[2], places=4)
         self.assertAlmostEqual(5, objective.value, places=4)
 
     def huber(self, solver) -> None:
         # Generate problem data
-        np.random.seed(2)
         n = 3
         m = 5
-        A = sp.random(m, n, density=0.8, format='csc')
+        data = [0.89, 0.39, 0.96, 0.34, 0.68, 0.18, 0.63 ,0.42, 0.51, 0.66, 0.43, 0.77]
+        indices = [0, 1, 2, 3, 4, 2, 3, 0, 1, 2, 3, 4]
+        indptr = [0, 5, 7, 12]
+        A = sp.csc_matrix((data, indices, indptr), shape=(m,n))
         x_true = np.random.randn(n) / np.sqrt(n)
         ind95 = (np.random.rand(m) < 0.95).astype(float)
         b = A.dot(x_true) + np.multiply(0.5*np.random.randn(m), ind95) \
             + np.multiply(10.*np.random.rand(m), 1. - ind95)
 
         # Solve the Huber regression problem
         x = Variable(n)
         objective = sum(huber(A @ x - b))
 
         # Solve problem with QP
         p = Problem(Minimize(objective))
         self.solve_QP(p, solver)
-        self.assertAlmostEqual(1.327429461061672, objective.value, places=3)
+        self.assertAlmostEqual(1.452797819667, objective.value, places=3)
         self.assertItemsAlmostEqual(x.value,
-                                    [-1.03751745, 0.86657204, -0.9649172],
+                                    [1.20524645, -0.85271489, -0.50838494],
                                     places=3)
 
     def equivalent_forms_1(self, solver) -> None:
         m = 100
         n = 80
         r = 70
         np.random.seed(1)
```

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_quad_form.py` & `cvxpy-1.4.3/cvxpy/tests/test_quad_form.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_quadratic.py` & `cvxpy-1.4.3/cvxpy/tests/test_quadratic.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_scalarize.py` & `cvxpy-1.4.3/cvxpy/tests/test_scalarize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_semidefinite_vars.py` & `cvxpy-1.4.3/cvxpy/tests/test_semidefinite_vars.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_shape.py` & `cvxpy-1.4.3/cvxpy/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_sign.py` & `cvxpy-1.4.3/cvxpy/tests/test_sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_suppfunc.py` & `cvxpy-1.4.3/cvxpy/tests/test_suppfunc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_valinvec2mixedint.py` & `cvxpy-1.4.3/cvxpy/tests/test_valinvec2mixedint.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_versioning.py` & `cvxpy-1.4.3/cvxpy/tests/test_versioning.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/tests/test_von_neumann_entr.py` & `cvxpy-1.4.3/cvxpy/tests/test_von_neumann_entr.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/__init__.py` & `cvxpy-1.4.3/cvxpy/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/indicator.py` & `cvxpy-1.4.3/cvxpy/transforms/indicator.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/linearize.py` & `cvxpy-1.4.3/cvxpy/transforms/linearize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/partial_optimize.py` & `cvxpy-1.4.3/cvxpy/transforms/partial_optimize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/scalarize.py` & `cvxpy-1.4.3/cvxpy/transforms/scalarize.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/transforms/suppfunc.py` & `cvxpy-1.4.3/cvxpy/transforms/suppfunc.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/__init__.py` & `cvxpy-1.4.3/cvxpy/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/canonical.py` & `cvxpy-1.4.3/cvxpy/utilities/canonical.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/coeff_extractor.py` & `cvxpy-1.4.3/cvxpy/utilities/coeff_extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """
-
-Copyright 2016 Jaehyun Park, 2017 Robin Verschueren, 2017 Akshay Agrawal
+Copyright, the CVXPY authors
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -14,67 +13,41 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from __future__ import annotations, division
 
 import operator
-from dataclasses import dataclass
+from typing import List
 
 import numpy as np
 import scipy.sparse as sp
 
 from cvxpy.cvxcore.python import canonInterface
+from cvxpy.lin_ops.canon_backend import TensorRepresentation
 from cvxpy.lin_ops.lin_op import NO_OP, LinOp
 from cvxpy.reductions.inverse_data import InverseData
 from cvxpy.utilities.replace_quad_forms import (
     replace_quad_forms,
     restore_quad_forms,
 )
 
 
-@dataclass
-class COOData:
-    """
-    Data for constructing a COO matrix.
-    """
-    data: np.ndarray
-    row: np.ndarray
-    col: np.ndarray
-    shape: tuple[int, int]
-    param_idxs: np.ndarray
-
-
 # TODO find best format for sparse matrices: csr, csc, dok, lil, ...
 class CoeffExtractor:
 
     def __init__(self, inverse_data, canon_backend: str | None) -> None:
         self.id_map = inverse_data.var_offsets
         self.x_length = inverse_data.x_length
         self.var_shapes = inverse_data.var_shapes
         self.param_shapes = inverse_data.param_shapes
         self.param_to_size = inverse_data.param_to_size
         self.param_id_map = inverse_data.param_id_map
         self.canon_backend = canon_backend
 
-    def get_coeffs(self, expr):
-        if expr.is_constant():
-            return self.constant(expr)
-        elif expr.is_affine():
-            return self.affine(expr)
-        elif expr.is_quadratic():
-            return self.quad_form(expr)
-        else:
-            raise Exception("Unknown expression type %s." % type(expr))
-
-    def constant(self, expr):
-        size = expr.size
-        return sp.csr_matrix((size, self.N)), np.reshape(expr.value, (size,),
-                                                         order='F')
-
     def affine(self, expr):
         """Extract problem data tensor from an expression that is reducible to
         A*x + b.
 
         Applying the tensor to a flattened parameter vector and reshaping
         will recover A and b (see the helpers in canonInterface).
 
@@ -130,15 +103,15 @@
 
         # Iterates over every entry of the parameters vector,
         # and obtains the Pi and qi for that entry i.
         # These are then combined into matrices [P1.flatten(), P2.flatten(), ...]
         # and [q1, q2, ...]
         constant = param_coeffs[-1, :]
         # TODO keep sparse.
-        c = param_coeffs[:-1, :].A
+        c = param_coeffs[:-1, :].toarray()
         num_params = param_coeffs.shape[1]
 
         # coeffs stores the P and q for each quad_form,
         # as well as for true variable nodes in the objective.
         coeffs = {}
         # The goal of this loop is to appropriately multiply
         # the matrix P of each quadratic term by the coefficients
@@ -146,78 +119,92 @@
         # to form a single matrix P.
         for var in affine_expr.variables():
             # quad_forms maps the ids of the SymbolicQuadForm atoms
             # in the objective to (modified parent node of quad form,
             #                      argument index of quad form,
             #                      quad form atom)
             if var.id in quad_forms:
+                # This was a dummy variable
                 var_id = var.id
                 orig_id = quad_forms[var_id][2].args[0].id
                 var_offset = affine_id_map[var_id][0]
                 var_size = affine_id_map[var_id][1]
                 c_part = c[var_offset:var_offset+var_size, :]
-                if quad_forms[var_id][2].P.value is not None:
-                    # Convert to sparse matrix.
-                    P = quad_forms[var_id][2].P.value
-                    if sp.issparse(P) and not isinstance(P, sp.coo_matrix):
-                        P = P.tocoo()
-                    else:
-                        P = sp.coo_matrix(P)
-                else:
-                    P = sp.eye(var_size, format='coo')
-                # We multiply the columns of P, by c_part
-                # by operating directly on the data.
-                if var_size > 1:
-                    # TODO remove zeros from data.
-                    data = P.data[:, None] * c_part[P.col]
-                    param_idxs = np.arange(c_part.shape[1])
+
+                # Convert to sparse matrix.
+                P = quad_forms[var_id][2].P
+                assert (
+                    P.value is not None
+                ), "P matrix must be instantiated before calling extract_quadratic_coeffs."
+                if sp.issparse(P) and not isinstance(P, sp.coo_matrix):
+                    P = P.value.tocoo()
                 else:
-                    # Eliminate zeros from data by tracking
-                    # which indices of the global parameter vector are used.
+                    P = sp.coo_matrix(P.value)
+
+                # We multiply P by the parameter coefficients.
+                if var_size == 1:
+                    # Single quad form in the expression, i.e., we multiply
+                    # the full P matrix by the non-zero entries of c_part.
+
                     nonzero_idxs = c_part[0] != 0
-                    data = P.data[:, None] * c_part[0:, nonzero_idxs]
-                    param_idxs = np.arange(c_part.shape[1])[nonzero_idxs]
-                P_tup = COOData(data, P.row, P.col, P.shape, param_idxs)
-                # Conceptually similar to
-                # P = P[:, :, None] * c_part[None, :, :]
+                    data = P.data[:, None] * c_part[:, nonzero_idxs]
+                    param_idxs = np.arange(num_params)[nonzero_idxs]
+                    P_tup = TensorRepresentation(
+                        data.flatten(order="F"),
+                        np.tile(P.row, len(param_idxs)),
+                        np.tile(P.col, len(param_idxs)),
+                        np.repeat(param_idxs, len(P.data)),
+                        P.shape
+                    )
+                else:
+                    # Multiple quad forms in the one expression, i.e., c_part
+                    # is now a matrix where each row corresponds to a different
+                    # variable.
+                    assert (P.col == P.row).all(), \
+                        "Only diagonal P matrices are supported for multiple quad forms."
+                    
+                    scaled_c_part = P @ c_part
+                    paramx_idx_row, param_idx_col = np.nonzero(scaled_c_part)
+                    c_vals = c_part[paramx_idx_row, param_idx_col]
+                    P_tup = TensorRepresentation(
+                        c_vals,
+                        paramx_idx_row,
+                        paramx_idx_row,
+                        param_idx_col,
+                        P.shape
+                    )
+
                 if orig_id in coeffs:
                     if 'P' in coeffs[orig_id]:
-                        # Concatenation becomes addition when constructing
-                        # COO matrix because repeated indices are summed.
-                        # Conceptually equivalent to
-                        # coeffs[orig_id]['P'] += P_tup
-                        acc_P = coeffs[orig_id]['P']
-                        acc_data = np.concatenate([acc_P.data, data], axis=0)
-                        acc_row = np.concatenate([acc_P.row, P.row], axis=0)
-                        acc_col = np.concatenate([acc_P.col, P.col], axis=0)
-                        P_tup = COOData(acc_data, acc_row, acc_col, P.shape, param_idxs)
-                        coeffs[orig_id]['P'] = P_tup
+                        coeffs[orig_id]['P'] =  coeffs[orig_id]['P'] + P_tup
                     else:
                         coeffs[orig_id]['P'] = P_tup
                 else:
+                    # No q for dummy variables.
                     coeffs[orig_id] = dict()
                     coeffs[orig_id]['P'] = P_tup
                     shape = (P.shape[0], c.shape[1])
-                    # Fast path for no parameters.
                     if num_params == 1:
+                        # Fast path for no parameters, keep q dense.
                         coeffs[orig_id]['q'] = np.zeros(shape)
                     else:
                         coeffs[orig_id]['q'] = sp.coo_matrix(([], ([], [])), shape=shape) 
             else:
+                # This was a true variable, so it can only have a q term.
                 var_offset = affine_id_map[var.id][0]
                 var_size = np.prod(affine_var_shapes[var.id], dtype=int)
                 if var.id in coeffs:
-                    # Fast path for no parameters.
+                    # Fast path for no parameters, q is dense and so is c.
                     if num_params == 1:
                         coeffs[var.id]['q'] += c[var_offset:var_offset+var_size, :]
                     else:
                         coeffs[var.id]['q'] += param_coeffs[var_offset:var_offset+var_size, :]
-                else:
+                else:   
                     coeffs[var.id] = dict()
-                    # Fast path for no parameters.
+                    # Fast path for no parameters, q is dense and so is c.
                     if num_params == 1:
                         coeffs[var.id]['q'] = c[var_offset:var_offset+var_size, :]
                     else:
                         coeffs[var.id]['q'] = param_coeffs[var_offset:var_offset+var_size, :]
         return coeffs, constant
 
     def quad_form(self, expr):
@@ -243,108 +230,95 @@
 
         # Extract quadratic matrices and vectors
         num_params = constant.shape[1]
         P_list = []
         q_list = []
         P_height = 0
         P_entries = 0
-        for var_id, offset in offsets:
+        for var_id, _ in offsets:
             shape = self.var_shapes[var_id]
             size = np.prod(shape, dtype=int)
             if var_id in coeffs and 'P' in coeffs[var_id]:
                 P = coeffs[var_id]['P']
                 P_entries += P.data.size
             else:
-                P = COOData([], [], [], (size, size), np.arange(num_params))
+                P = TensorRepresentation.empty_with_shape((size, size))
             if var_id in coeffs and 'q' in coeffs[var_id]:
                 q = coeffs[var_id]['q']
             else:
                 # Fast path for no parameters.
                 if num_params == 1:
                     q = np.zeros((size, num_params))
                 else:
                     q = sp.coo_matrix(([], ([], [])), (size, num_params))
 
             P_list.append(P)
             q_list.append(q)
             P_height += size
 
         if P_height != self.x_length:
-            raise RuntimeError("Resulting quadratic form does not have "
+            raise ValueError("Resulting quadratic form does not have "
                                "appropriate dimensions")
 
         # Stitch together Ps and qs and constant.
-        P = self.merge_P_list(P_list, P_entries, P_height, num_params)
+        P = self.merge_P_list(P_list, P_height, num_params)
         q = self.merge_q_list(q_list, constant, num_params)
         return P, q
 
     def merge_P_list(
             self, 
-            P_list: list, 
-            P_entries: int, 
+            P_list: List[TensorRepresentation],
             P_height: int, 
             num_params: int,
-        ) -> sp.coo_matrix:
+        ) -> sp.csc_matrix:
         """Conceptually we build a block diagonal matrix
            out of all the Ps, then flatten the first two dimensions.
            eg P1
                 P2
            We do this by extending each P with zero blocks above and below.
 
         Args:
-            P_list: list of P submatrices as COOData objects.
+            P_list: list of P submatrices as TensorRepresentation objects.
             P_entries: number of entries in the merged P matrix.
             P_height: number of rows in the merged P matrix.
             num_params: number of parameters in the problem.
         
         Returns:
-            A COO sparse representation of the merged P matrix.
+            A CSC sparse representation of the merged P matrix.
         """
-        gap_above = np.int64(0)
-        acc_height = np.int64(0)
-        rows = np.zeros(P_entries, dtype=np.int64)
-        cols = np.zeros(P_entries, dtype=np.int64)
-        vals = np.zeros(P_entries)
-        entry_offset = 0
-        for P in P_list:
-            """Conceptually, the code is equivalent to
-            ```
-            above = np.zeros((gap_above, P.shape[1], num_params))
-            below = np.zeros((gap_below, P.shape[1], num_params))
-            padded_P = np.concatenate([above, P, below], axis=0)
-            padded_P = np.reshape(padded_P, (P_height*P.shape[1], num_params),
-                                  order='F')
-            padded_P_list.append(padded_P)
-            ```
-            but done by constructing a COO matrix.
-            """
-            if len(P.data) > 0:
-                vals[entry_offset:entry_offset + P.data.size] = P.data.flatten(
-                    order='F'
-                )
-                P_cols_ext = P.col.astype(np.int64) * np.int64(P_height)
-                base_rows = gap_above + acc_height + P.row + P_cols_ext
-                full_rows = np.tile(base_rows, len(P.param_idxs))
-                rows[entry_offset:entry_offset + P.data.size] = full_rows
-                full_cols = np.repeat(P.param_idxs, P.col.size)
-                cols[entry_offset:entry_offset + P.data.size] = full_cols
-                entry_offset += P.data.size
-            gap_above += P.shape[0]
-            acc_height += P_height * np.int64(P.shape[1])
-
-        return sp.coo_matrix((vals, (rows, cols)), shape=(acc_height, num_params))
 
-    def merge_q_list(self, q_list: list, constant: sp.csc_matrix, num_params: int) -> sp.csr_matrix:
+        offset = 0
+        for P in P_list:
+            m, n = P.shape
+            assert m == n
+    
+            # Translate local to global indices within the block diagonal matrix.
+            P.row += offset
+            P.col += offset
+            P.shape = (P_height, P_height)
+    
+            offset += m
+
+        combined = TensorRepresentation.combine(P_list)
+
+        return combined.flatten_tensor(num_params)
+
+    def merge_q_list(
+        self,
+        q_list: List[sp.spmatrix | np.ndarray],
+        constant: sp.csc_matrix,
+        num_params: int,
+    ) -> sp.csr_matrix:
         """Stack q with constant offset as last row.
 
         Args:
-            q_list: list of q submatrices as COOData objects.
+            q_list: list of q submatrices as SciPy sparse matrices or NumPy arrays.
             constant: The constant offset as a CSC sparse matrix.
             num_params: number of parameters in the problem.
-        
+
         Returns:
             A CSR sparse representation of the merged q matrix.
         """
         # Fast path for no parameters.
         if num_params == 1:
             q = np.vstack(q_list)
             q = np.vstack([q, constant.A])
```

### Comparing `cvxpy-1.4.2/cvxpy/utilities/cpp/sparsecholesky/main.cpp` & `cvxpy-1.4.3/cvxpy/utilities/cpp/sparsecholesky/main.cpp`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/cvxpy_upgrade.py` & `cvxpy-1.4.3/cvxpy/utilities/cvxpy_upgrade.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/debug_tools.py` & `cvxpy-1.4.3/cvxpy/utilities/debug_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/grad.py` & `cvxpy-1.4.3/cvxpy/utilities/grad.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/key_utils.py` & `cvxpy-1.4.3/cvxpy/utilities/key_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/linalg.py` & `cvxpy-1.4.3/cvxpy/utilities/linalg.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/performance_utils.py` & `cvxpy-1.4.3/cvxpy/utilities/performance_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/perspective_utils.py` & `cvxpy-1.4.3/cvxpy/utilities/perspective_utils.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/power_tools.py` & `cvxpy-1.4.3/cvxpy/utilities/power_tools.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/replace_quad_forms.py` & `cvxpy-1.4.3/cvxpy/utilities/replace_quad_forms.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/scopes.py` & `cvxpy-1.4.3/cvxpy/utilities/scopes.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/shape.py` & `cvxpy-1.4.3/cvxpy/utilities/shape.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/sign.py` & `cvxpy-1.4.3/cvxpy/utilities/sign.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy/utilities/versioning.py` & `cvxpy-1.4.3/cvxpy/utilities/versioning.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/cvxpy.egg-info/PKG-INFO` & `cvxpy-1.4.3/cvxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxpy
-Version: 1.4.2
+Version: 1.4.3
 Summary: A domain-specific language for modeling convex optimization problems in Python.
 Home-page: https://github.com/cvxpy/cvxpy
 Author: Steven Diamond, Eric Chu, Stephen Boyd
 Author-email: stevend2@stanford.edu, akshayka@cs.stanford.edu, echu508@stanford.edu, boyd@stanford.edu
 License: Apache License, Version 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cvxpy-1.4.2/cvxpy.egg-info/SOURCES.txt` & `cvxpy-1.4.3/cvxpy.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,14 @@
 cvxpy/expressions/constants/__init__.py
 cvxpy/expressions/constants/callback_param.py
 cvxpy/expressions/constants/constant.py
 cvxpy/expressions/constants/parameter.py
 cvxpy/interface/__init__.py
 cvxpy/interface/base_matrix_interface.py
 cvxpy/interface/matrix_utilities.py
-cvxpy/interface/scipy_wrapper.py
 cvxpy/interface/numpy_interface/__init__.py
 cvxpy/interface/numpy_interface/matrix_interface.py
 cvxpy/interface/numpy_interface/ndarray_interface.py
 cvxpy/interface/numpy_interface/sparse_matrix_interface.py
 cvxpy/lin_ops/__init__.py
 cvxpy/lin_ops/canon_backend.py
 cvxpy/lin_ops/lin_constraints.py
@@ -679,14 +678,15 @@
 cvxpy/tests/__init__.py
 cvxpy/tests/base_test.py
 cvxpy/tests/ram_limited.py
 cvxpy/tests/solver_test_helpers.py
 cvxpy/tests/test_KKT.py
 cvxpy/tests/test_atoms.py
 cvxpy/tests/test_benchmarks.py
+cvxpy/tests/test_coeff_extractor.py
 cvxpy/tests/test_complex.py
 cvxpy/tests/test_cone2cone.py
 cvxpy/tests/test_conic_solvers.py
 cvxpy/tests/test_constant.py
 cvxpy/tests/test_constant_atoms.py
 cvxpy/tests/test_constraints.py
 cvxpy/tests/test_convolution.py
```

### Comparing `cvxpy-1.4.2/pyproject.toml` & `cvxpy-1.4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 [tool.ruff]
-select = ["E", "F", "I", "NPY201"]
+select = [
+    "E",
+    "F",
+    "I",
+    "NPY201",
+    "W605",  # Check for invalid escape sequences in docstrings (errors in py >= 3.11)
+]
 line-length = 100
 exclude = [
     "build",
     "examples",
     "doc",
     "cvxpy/cvxcore/*",
     "*__init__.py"
```

### Comparing `cvxpy-1.4.2/setup/extensions.py` & `cvxpy-1.4.3/setup/extensions.py`

 * *Files identical despite different names*

### Comparing `cvxpy-1.4.2/setup/versioning.py` & `cvxpy-1.4.3/setup/versioning.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 #   snippets. We have mostly left those comments in-place, but we sometimes preface
 #   them with the following remark:
 #      "The comment below is from the SciPy code which we repurposed for cvxpy."
 #
 
 MAJOR = 1
 MINOR = 4
-MICRO = 2
+MICRO = 3
 IS_RELEASED = True
 IS_RELEASE_BRANCH = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 
 # Return the git revision as a string
 def git_version():
```

### Comparing `cvxpy-1.4.2/setup.py` & `cvxpy-1.4.3/setup.py`

 * *Files identical despite different names*

