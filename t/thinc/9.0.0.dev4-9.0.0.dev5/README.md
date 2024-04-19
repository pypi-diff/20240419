# Comparing `tmp/thinc-9.0.0.dev4.tar.gz` & `tmp/thinc-9.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinc-9.0.0.dev4.tar", last modified: Tue Jan 16 12:08:16 2024, max compression
+gzip compressed data, was "thinc-9.0.0.dev5.tar", last modified: Mon Apr  8 14:01:16 2024, max compression
```

## Comparing `thinc-9.0.0.dev4.tar` & `thinc-9.0.0.dev5.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/
--rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-01-16 12:08:16.191423 thinc-9.0.0.dev4/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.163423 thinc-9.0.0.dev4/thinc/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)      213 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/about.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5915 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/api.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.167423 thinc-9.0.0.dev4/thinc/backends/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/__init__.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)     5320 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_cupy_allocators.py
--rw-r--r--   0 vsts      (1001) docker     (127)    18822 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_custom_kernels.cu
--rw-r--r--   0 vsts      (1001) docker     (127)    25370 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_custom_kernels.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_murmur3.cu
--rw-r--r--   0 vsts      (1001) docker     (127)     2740 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/_param_server.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2026 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cblas.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)     2076 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cblas.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)    14601 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cpu_kernels.hh
--rw-r--r--   0 vsts      (1001) docker     (127)    12947 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/cupy_ops.py
--rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/mps_ops.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/numpy_ops.pxd
--rw-r--r--   0 vsts      (1001) docker     (127)    38254 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/numpy_ops.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)    58702 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/backends/ops.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3092 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/initializers.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.175423 thinc-9.0.0.dev4/thinc/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)     4396 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2245 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/add.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1587 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/array_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/bidirectional.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1740 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/cauchysimilarity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3444 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/chain.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/clipped_linear.py
--rw-r--r--   0 vsts      (1001) docker     (127)      648 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/clone.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5188 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/concatenate.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2113 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/dish.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2955 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/dropout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2690 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/embed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1640 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/expand_window.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2120 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/gelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2147 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hard_swish.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2194 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hard_swish_mobilenet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3615 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/hashembed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2534 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1720 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/linear.py
--rw-r--r--   0 vsts      (1001) docker     (127)      877 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2array.py
--rw-r--r--   0 vsts      (1001) docker     (127)      622 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2padded.py
--rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/list2ragged.py
--rw-r--r--   0 vsts      (1001) docker     (127)      609 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/logistic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6451 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/lstm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/map_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2594 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/maxout.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2269 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/mish.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1768 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/multisoftmax.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4281 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/mxnetwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      511 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/noop.py
--rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/padded2list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/parametricattention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2972 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/parametricattention_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/premap_ids.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)    12439 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/pytorchwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      773 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/ragged2list.py
--rw-r--r--   0 vsts      (1001) docker     (127)      815 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_first.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_last.py
--rw-r--r--   0 vsts      (1001) docker     (127)      720 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_max.py
--rw-r--r--   0 vsts      (1001) docker     (127)      712 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_mean.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/reduce_sum.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2057 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/relu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/remap_ids.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2092 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/residual.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2755 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/resizable.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/siamese.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1945 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sigmoid.py
--rw-r--r--   0 vsts      (1001) docker     (127)      652 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sigmoid_activation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3237 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/softmax.py
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/softmax_activation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8175 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/sparselinear.pyx
--rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/strings2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2128 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/swish.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6549 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/tensorflowwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3276 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2018 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/tuplify.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_array.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_array2d.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_cpu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1674 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_flatten_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_getitem.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2893 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_nvtx_range.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4856 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_padded.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4446 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_ragged.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1791 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_reshape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/layers/with_signpost_interval.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16308 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/loss.py
--rw-r--r--   0 vsts      (1001) docker     (127)    34919 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/model.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11467 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/mypy.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14580 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/py.typed
--rw-r--r--   0 vsts      (1001) docker     (127)    11342 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/schedules.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.175423 thinc-9.0.0.dev4/thinc/shims/
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4315 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/mxnet.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9340 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/pytorch.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6060 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2482 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/shim.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10604 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/tensorflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2457 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/shims/torchscript.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.179423 thinc-9.0.0.dev4/thinc/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.179423 thinc-9.0.0.dev4/thinc/tests/backends/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/test_mem.py
--rw-r--r--   0 vsts      (1001) docker     (127)    52692 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/backends/test_ops.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2209 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)       92 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/enable_mxnet.py
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/enable_tensorflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2448 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_basic_tagger.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_combinators.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5441 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_feed_forward.py
--rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_hash_embed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9974 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_layers_api.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7342 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_linear.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5650 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_lstm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1650 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mappers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3669 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mnist.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_mxnet_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_parametric_attention_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6951 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_pytorch_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3695 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_reduce.py
--rw-r--r--   0 vsts      (1001) docker     (127)      874 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_resizable.py
--rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_shim.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2869 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_softmax.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_sparse_linear.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13111 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_tensorflow_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_torchscriptwrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_transforms.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2252 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_uniqued.py
--rw-r--r--   0 vsts      (1001) docker     (127)      802 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_debug.py
--rw-r--r--   0 vsts      (1001) docker     (127)      871 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_flatten.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10169 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/layers/test_with_transforms.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/model/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19918 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/test_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1386 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/model/test_validation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/configs/
--rw-r--r--   0 vsts      (1001) docker     (127)      195 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/configs/mypy-default.ini
--rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/configs/mypy-plugin.ini
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/modules/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_no_plugin.py
--rw-r--r--   0 vsts      (1001) docker     (127)      831 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_plugin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.183423 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     2416 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      576 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-no-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      494 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-plugin.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/mypy/test_mypy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/regression/issue519/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/program.py
--rw-r--r--   0 vsts      (1001) docker     (127)      817 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/issue519/test_issue519.py
--rw-r--r--   0 vsts      (1001) docker     (127)      328 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/test_issue208.py
--rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/regression/test_issue564.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc/tests/shims/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/shims/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/shims/test_pytorch_grad_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3587 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/strategies.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5833 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_examples.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1800 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_import__all__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1896 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_indexing.py
--rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_initializers.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12083 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_loss.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4997 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_optimizers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3471 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_schedules.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6788 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1559 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5647 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/test_util.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47816 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/types.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21106 2024-01-16 12:07:52.000000 thinc-9.0.0.dev4/thinc/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-01-16 12:08:16.187423 thinc-9.0.0.dev4/thinc.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     5528 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-01-16 12:08:16.000000 thinc-9.0.0.dev4/thinc.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.120429 thinc-9.0.0.dev5/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      222 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-04-08 14:01:16.120429 thinc-9.0.0.dev5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      350 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-04-08 14:01:16.120429 thinc-9.0.0.dev5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     3045 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.096428 thinc-9.0.0.dev5/thinc/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)      213 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/about.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5915 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/api.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.096428 thinc-9.0.0.dev5/thinc/backends/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/__init__.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     5320 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2216 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/_cupy_allocators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    18822 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/_custom_kernels.cu
+-rw-r--r--   0 vsts      (1001) docker     (127)    25370 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/_custom_kernels.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5210 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/_murmur3.cu
+-rw-r--r--   0 vsts      (1001) docker     (127)     2740 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/_param_server.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2026 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/cblas.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)     2076 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/cblas.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    14601 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/cpu_kernels.hh
+-rw-r--r--   0 vsts      (1001) docker     (127)    12950 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/cupy_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      607 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/mps_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1989 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/numpy_ops.pxd
+-rw-r--r--   0 vsts      (1001) docker     (127)    38254 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/numpy_ops.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    58702 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/backends/ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3158 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1281 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/initializers.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.108429 thinc-9.0.0.dev5/thinc/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4396 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2245 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1587 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/array_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2191 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/bidirectional.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1740 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/cauchysimilarity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3444 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/chain.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4447 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/clipped_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      648 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5188 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/concatenate.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2113 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/dish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2955 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/dropout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2690 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1640 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/expand_window.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2120 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/gelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2147 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/hard_swish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2194 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/hard_swish_mobilenet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3615 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/hashembed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2534 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1720 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      877 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/list2array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      622 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/list2padded.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      863 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/list2ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      609 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/logistic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6451 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1027 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/map_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2594 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/maxout.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2269 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/mish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1768 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/multisoftmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4281 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/mxnetwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      511 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      702 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/padded2list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/parametricattention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2972 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/parametricattention_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2315 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/premap_ids.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)    12439 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/pytorchwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      773 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/ragged2list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      815 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/reduce_first.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/reduce_last.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      720 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/reduce_max.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      712 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/reduce_mean.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/reduce_sum.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2057 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/relu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/remap_ids.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2092 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/residual.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2755 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1614 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/siamese.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1945 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/sigmoid.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      652 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/sigmoid_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3237 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/softmax_activation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8175 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/sparselinear.pyx
+-rw-r--r--   0 vsts      (1001) docker     (127)      953 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/strings2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2128 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/swish.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6549 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/tensorflowwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3276 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2018 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/tuplify.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2061 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3578 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_array.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_array2d.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1427 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_cpu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1674 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1953 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_flatten_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1167 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_getitem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2893 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1292 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_nvtx_range.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4856 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_padded.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4446 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_ragged.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1791 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_reshape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1511 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/layers/with_signpost_interval.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16308 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/loss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34919 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11467 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/mypy.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14580 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (127)    11342 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/schedules.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.108429 thinc-9.0.0.dev5/thinc/shims/
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4315 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/mxnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9340 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/pytorch.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6060 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2482 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/shim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10604 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/tensorflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2461 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/shims/torchscript.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.108429 thinc-9.0.0.dev5/thinc/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.112429 thinc-9.0.0.dev5/thinc/tests/backends/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/backends/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      359 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/backends/test_mem.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    52692 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/backends/test_ops.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2209 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       92 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/enable_mxnet.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/enable_tensorflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.112429 thinc-9.0.0.dev5/thinc/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2430 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_basic_tagger.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7828 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_combinators.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5441 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_feed_forward.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      533 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_hash_embed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9974 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_layers_api.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7342 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5650 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_lstm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1650 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_mappers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3669 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_mnist.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6292 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_mxnet_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      285 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_parametric_attention_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6951 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_pytorch_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3695 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_reduce.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      874 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_resizable.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      945 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2869 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_softmax.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_sparse_linear.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13111 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_tensorflow_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      806 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_torchscriptwrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_transforms.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2252 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_uniqued.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      802 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_with_debug.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      871 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_with_flatten.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10169 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/layers/test_with_transforms.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.112429 thinc-9.0.0.dev5/thinc/tests/model/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19918 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/model/test_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1386 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/model/test_validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.112429 thinc-9.0.0.dev5/thinc/tests/mypy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/mypy/configs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      195 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/configs/mypy-default.ini
+-rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/configs/mypy-plugin.ini
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/mypy/modules/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/modules/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      167 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/modules/fail_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      565 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/modules/fail_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/modules/success_no_plugin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      831 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/modules/success_plugin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/mypy/outputs/
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/outputs/fail-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     2416 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/outputs/fail-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      576 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/outputs/success-no-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      494 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/outputs/success-plugin.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     3072 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/mypy/test_mypy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/regression/issue519/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/issue519/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/issue519/program.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      817 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/issue519/test_issue519.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      328 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/test_issue208.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      520 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/regression/test_issue564.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc/tests/shims/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/shims/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/shims/test_pytorch_grad_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3587 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/strategies.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5833 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1749 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1800 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_import__all__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1896 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_indexing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      988 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_initializers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12083 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_loss.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4997 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_optimizers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3471 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6788 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1559 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5647 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/test_util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3600 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47816 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21106 2024-04-08 14:00:59.000000 thinc-9.0.0.dev5/thinc/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-08 14:01:16.116429 thinc-9.0.0.dev5/thinc.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    15268 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     5528 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       66 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)     1192 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-08 14:01:16.000000 thinc-9.0.0.dev5/thinc.egg-info/top_level.txt
```

### Comparing `thinc-9.0.0.dev4/LICENSE` & `thinc-9.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/PKG-INFO` & `thinc-9.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev4
+Version: 9.0.0.dev5
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev4 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev5 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
```

### Comparing `thinc-9.0.0.dev4/README.md` & `thinc-9.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/setup.cfg` & `thinc-9.0.0.dev5/setup.cfg`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/setup.py` & `thinc-9.0.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/api.py` & `thinc-9.0.0.dev5/thinc/api.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/__init__.py` & `thinc-9.0.0.dev5/thinc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/_cupy_allocators.py` & `thinc-9.0.0.dev5/thinc/backends/_cupy_allocators.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/_custom_kernels.cu` & `thinc-9.0.0.dev5/thinc/backends/_custom_kernels.cu`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/_custom_kernels.py` & `thinc-9.0.0.dev5/thinc/backends/_custom_kernels.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/_murmur3.cu` & `thinc-9.0.0.dev5/thinc/backends/_murmur3.cu`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/_param_server.py` & `thinc-9.0.0.dev5/thinc/backends/_param_server.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/cblas.pxd` & `thinc-9.0.0.dev5/thinc/backends/cblas.pxd`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/cblas.pyx` & `thinc-9.0.0.dev5/thinc/backends/cblas.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/cpu_kernels.hh` & `thinc-9.0.0.dev5/thinc/backends/cpu_kernels.hh`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/cupy_ops.py` & `thinc-9.0.0.dev5/thinc/backends/cupy_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy
 
 from .. import registry
-from ..compat import cupy, cupyx
+from ..compat import cublas, cupy, cupyx
 from ..types import DeviceTypes
 from ..util import (
     is_cupy_array,
     is_mxnet_gpu_array,
     is_tensorflow_gpu_array,
     is_torch_cuda_array,
     mxnet2xp,
@@ -253,15 +253,15 @@
 
     def clip_gradient(self, gradient, threshold):
         # We do not use CuPy's linalg.norm, since it uses scalar reductions
         # using one CUDA block. This is a lot slower than the cuBLAS
         # implementation.
         def frobenius_norm(X):
             X_vec = X.reshape(-1)
-            return cupy.cublas.nrm2(X_vec)
+            return cublas.nrm2(X_vec)
 
         grad_norm = cupy.maximum(frobenius_norm(gradient), 1e-12)
         gradient *= cupy.minimum(threshold, grad_norm) / grad_norm
         return gradient
 
     def seq2col(self, seq, nW, *, lengths=None):
         """Given an (M, N) sequence of vectors, return an (M, N*(nW*2+1)) sequence.
```

### Comparing `thinc-9.0.0.dev4/thinc/backends/mps_ops.py` & `thinc-9.0.0.dev5/thinc/backends/mps_ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/numpy_ops.pxd` & `thinc-9.0.0.dev5/thinc/backends/numpy_ops.pxd`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/numpy_ops.pyx` & `thinc-9.0.0.dev5/thinc/backends/numpy_ops.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/backends/ops.py` & `thinc-9.0.0.dev5/thinc/backends/ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/compat.py` & `thinc-9.0.0.dev5/thinc/compat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import warnings
 
 from packaging.version import Version
 
 try:  # pragma: no cover
     import cupy
+    import cupy.cublas
     import cupyx
 
     has_cupy = True
+    cublas = cupy.cublas
     cupy_version = Version(cupy.__version__)
     try:
         cupy.cuda.runtime.getDeviceCount()
         has_cupy_gpu = True
     except cupy.cuda.runtime.CUDARuntimeError:
         has_cupy_gpu = False
 
     if cupy_version.major >= 10:
         # fromDlpack was deprecated in v10.0.0.
         cupy_from_dlpack = cupy.from_dlpack
     else:
         cupy_from_dlpack = cupy.fromDlpack
 except (ImportError, AttributeError):
+    cublas = None
     cupy = None
     cupyx = None
     cupy_version = Version("0.0.0")
     has_cupy = False
     cupy_from_dlpack = None
     has_cupy_gpu = False
```

### Comparing `thinc-9.0.0.dev4/thinc/config.py` & `thinc-9.0.0.dev5/thinc/config.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/initializers.py` & `thinc-9.0.0.dev5/thinc/initializers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/__init__.py` & `thinc-9.0.0.dev5/thinc/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/add.py` & `thinc-9.0.0.dev5/thinc/layers/add.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/array_getitem.py` & `thinc-9.0.0.dev5/thinc/layers/array_getitem.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/bidirectional.py` & `thinc-9.0.0.dev5/thinc/layers/bidirectional.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/cauchysimilarity.py` & `thinc-9.0.0.dev5/thinc/layers/cauchysimilarity.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/chain.py` & `thinc-9.0.0.dev5/thinc/layers/chain.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/clipped_linear.py` & `thinc-9.0.0.dev5/thinc/layers/clipped_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/clone.py` & `thinc-9.0.0.dev5/thinc/layers/clone.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/concatenate.py` & `thinc-9.0.0.dev5/thinc/layers/concatenate.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/dish.py` & `thinc-9.0.0.dev5/thinc/layers/dish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/dropout.py` & `thinc-9.0.0.dev5/thinc/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/embed.py` & `thinc-9.0.0.dev5/thinc/layers/embed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/expand_window.py` & `thinc-9.0.0.dev5/thinc/layers/expand_window.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/gelu.py` & `thinc-9.0.0.dev5/thinc/layers/gelu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/hard_swish.py` & `thinc-9.0.0.dev5/thinc/layers/hard_swish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/hard_swish_mobilenet.py` & `thinc-9.0.0.dev5/thinc/layers/hard_swish_mobilenet.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/hashembed.py` & `thinc-9.0.0.dev5/thinc/layers/hashembed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/layernorm.py` & `thinc-9.0.0.dev5/thinc/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/linear.py` & `thinc-9.0.0.dev5/thinc/layers/linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/list2array.py` & `thinc-9.0.0.dev5/thinc/layers/list2array.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/list2padded.py` & `thinc-9.0.0.dev5/thinc/layers/list2padded.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/list2ragged.py` & `thinc-9.0.0.dev5/thinc/layers/list2ragged.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/logistic.py` & `thinc-9.0.0.dev5/thinc/layers/logistic.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/lstm.py` & `thinc-9.0.0.dev5/thinc/layers/lstm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/map_list.py` & `thinc-9.0.0.dev5/thinc/layers/map_list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/maxout.py` & `thinc-9.0.0.dev5/thinc/layers/maxout.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/mish.py` & `thinc-9.0.0.dev5/thinc/layers/mish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/multisoftmax.py` & `thinc-9.0.0.dev5/thinc/layers/multisoftmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/mxnetwrapper.py` & `thinc-9.0.0.dev5/thinc/layers/mxnetwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/padded2list.py` & `thinc-9.0.0.dev5/thinc/layers/padded2list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/parametricattention.py` & `thinc-9.0.0.dev5/thinc/layers/parametricattention.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/parametricattention_v2.py` & `thinc-9.0.0.dev5/thinc/layers/parametricattention_v2.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/premap_ids.pyx` & `thinc-9.0.0.dev5/thinc/layers/premap_ids.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/pytorchwrapper.py` & `thinc-9.0.0.dev5/thinc/layers/pytorchwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/ragged2list.py` & `thinc-9.0.0.dev5/thinc/layers/ragged2list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/reduce_first.py` & `thinc-9.0.0.dev5/thinc/layers/reduce_first.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/reduce_last.py` & `thinc-9.0.0.dev5/thinc/layers/reduce_last.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/reduce_max.py` & `thinc-9.0.0.dev5/thinc/layers/reduce_max.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/reduce_mean.py` & `thinc-9.0.0.dev5/thinc/layers/reduce_mean.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/reduce_sum.py` & `thinc-9.0.0.dev5/thinc/layers/reduce_sum.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/relu.py` & `thinc-9.0.0.dev5/thinc/layers/relu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/remap_ids.py` & `thinc-9.0.0.dev5/thinc/layers/remap_ids.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/residual.py` & `thinc-9.0.0.dev5/thinc/layers/residual.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/resizable.py` & `thinc-9.0.0.dev5/thinc/layers/resizable.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/siamese.py` & `thinc-9.0.0.dev5/thinc/layers/siamese.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/sigmoid.py` & `thinc-9.0.0.dev5/thinc/layers/sigmoid.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/sigmoid_activation.py` & `thinc-9.0.0.dev5/thinc/layers/sigmoid_activation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/softmax.py` & `thinc-9.0.0.dev5/thinc/layers/softmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/softmax_activation.py` & `thinc-9.0.0.dev5/thinc/layers/softmax_activation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/sparselinear.pyx` & `thinc-9.0.0.dev5/thinc/layers/sparselinear.pyx`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/strings2arrays.py` & `thinc-9.0.0.dev5/thinc/layers/strings2arrays.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/swish.py` & `thinc-9.0.0.dev5/thinc/layers/swish.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/tensorflowwrapper.py` & `thinc-9.0.0.dev5/thinc/layers/tensorflowwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/torchscriptwrapper.py` & `thinc-9.0.0.dev5/thinc/layers/torchscriptwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/tuplify.py` & `thinc-9.0.0.dev5/thinc/layers/tuplify.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/uniqued.py` & `thinc-9.0.0.dev5/thinc/layers/uniqued.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_array.py` & `thinc-9.0.0.dev5/thinc/layers/with_array.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_array2d.py` & `thinc-9.0.0.dev5/thinc/layers/with_array2d.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_cpu.py` & `thinc-9.0.0.dev5/thinc/layers/with_cpu.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_debug.py` & `thinc-9.0.0.dev5/thinc/layers/with_debug.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_flatten.py` & `thinc-9.0.0.dev5/thinc/layers/with_flatten.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_flatten_v2.py` & `thinc-9.0.0.dev5/thinc/layers/with_flatten_v2.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_getitem.py` & `thinc-9.0.0.dev5/thinc/layers/with_getitem.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_list.py` & `thinc-9.0.0.dev5/thinc/layers/with_list.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_nvtx_range.py` & `thinc-9.0.0.dev5/thinc/layers/with_nvtx_range.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_padded.py` & `thinc-9.0.0.dev5/thinc/layers/with_padded.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_ragged.py` & `thinc-9.0.0.dev5/thinc/layers/with_ragged.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_reshape.py` & `thinc-9.0.0.dev5/thinc/layers/with_reshape.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/layers/with_signpost_interval.py` & `thinc-9.0.0.dev5/thinc/layers/with_signpost_interval.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/loss.py` & `thinc-9.0.0.dev5/thinc/loss.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/model.py` & `thinc-9.0.0.dev5/thinc/model.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/mypy.py` & `thinc-9.0.0.dev5/thinc/mypy.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/optimizers.py` & `thinc-9.0.0.dev5/thinc/optimizers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/schedules.py` & `thinc-9.0.0.dev5/thinc/schedules.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/mxnet.py` & `thinc-9.0.0.dev5/thinc/shims/mxnet.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/pytorch.py` & `thinc-9.0.0.dev5/thinc/shims/pytorch.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/pytorch_grad_scaler.py` & `thinc-9.0.0.dev5/thinc/shims/pytorch_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/shim.py` & `thinc-9.0.0.dev5/thinc/shims/shim.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/tensorflow.py` & `thinc-9.0.0.dev5/thinc/shims/tensorflow.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/shims/torchscript.py` & `thinc-9.0.0.dev5/thinc/shims/torchscript.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         The PyTorch device to run the model on. When this argument is
         set to "None", the default device for the currently active Thinc
         ops is used.
     """
 
     def __init__(
         self,
-        model: Optional["torch.ScriptModule"],
+        model: Optional["torch.jit.ScriptModule"],
         config=None,
         optimizer: Any = None,
         mixed_precision: bool = False,
         grad_scaler: Optional[PyTorchGradScaler] = None,
         device: Optional["torch.device"] = None,
     ):
         if model is not None and not isinstance(model, torch.jit.ScriptModule):
```

### Comparing `thinc-9.0.0.dev4/thinc/tests/backends/test_ops.py` & `thinc-9.0.0.dev5/thinc/tests/backends/test_ops.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/conftest.py` & `thinc-9.0.0.dev5/thinc/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_basic_tagger.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_basic_tagger.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     zipped = list(zip(Xs, Ys))
     random.shuffle(zipped)
     for i in range(0, len(zipped), batch_size):
         batch_X, batch_Y = zip(*zipped[i : i + batch_size])
         yield list(batch_X), list(batch_Y)
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     ("depth", "width", "vector_width", "nb_epoch"), [(2, 32, 16, 5)]
 )
 def test_small_end_to_end(depth, width, vector_width, nb_epoch, create_model, ancora):
     (train_X, train_Y), (dev_X, dev_Y) = ancora
     batch_size = 8
     model = create_model(depth, width, vector_width).initialize()
```

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_combinators.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_combinators.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_feed_forward.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_feed_forward.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_hash_embed.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_hash_embed.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_layers_api.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_layers_api.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_linear.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_lstm.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_lstm.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_mappers.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_mappers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_mnist.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_mnist.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_mxnet_wrapper.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_mxnet_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_pytorch_wrapper.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_pytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_reduce.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_reduce.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_resizable.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_resizable.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_shim.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_shim.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_softmax.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_softmax.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_sparse_linear.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_sparse_linear.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_tensorflow_wrapper.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_tensorflow_wrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_torchscriptwrapper.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_torchscriptwrapper.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_transforms.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_transforms.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_uniqued.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_uniqued.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_with_debug.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_with_debug.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_with_flatten.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_with_flatten.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/layers/test_with_transforms.py` & `thinc-9.0.0.dev5/thinc/tests/layers/test_with_transforms.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/model/test_model.py` & `thinc-9.0.0.dev5/thinc/tests/model/test_model.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/model/test_validation.py` & `thinc-9.0.0.dev5/thinc/tests/model/test_validation.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/mypy/modules/fail_plugin.py` & `thinc-9.0.0.dev5/thinc/tests/mypy/modules/fail_plugin.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/mypy/modules/success_plugin.py` & `thinc-9.0.0.dev5/thinc/tests/mypy/modules/success_plugin.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/mypy/outputs/fail-plugin.txt` & `thinc-9.0.0.dev5/thinc/tests/mypy/outputs/fail-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/mypy/outputs/success-no-plugin.txt` & `thinc-9.0.0.dev5/thinc/tests/mypy/outputs/success-no-plugin.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/mypy/test_mypy.py` & `thinc-9.0.0.dev5/thinc/tests/mypy/test_mypy.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/regression/issue519/test_issue519.py` & `thinc-9.0.0.dev5/thinc/tests/regression/issue519/test_issue519.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/regression/test_issue564.py` & `thinc-9.0.0.dev5/thinc/tests/regression/test_issue564.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/shims/test_pytorch_grad_scaler.py` & `thinc-9.0.0.dev5/thinc/tests/shims/test_pytorch_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/strategies.py` & `thinc-9.0.0.dev5/thinc/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_config.py` & `thinc-9.0.0.dev5/thinc/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_examples.py` & `thinc-9.0.0.dev5/thinc/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_import__all__.py` & `thinc-9.0.0.dev5/thinc/tests/test_import__all__.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_indexing.py` & `thinc-9.0.0.dev5/thinc/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_initializers.py` & `thinc-9.0.0.dev5/thinc/tests/test_initializers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_loss.py` & `thinc-9.0.0.dev5/thinc/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_optimizers.py` & `thinc-9.0.0.dev5/thinc/tests/test_optimizers.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_schedules.py` & `thinc-9.0.0.dev5/thinc/tests/test_schedules.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_serialize.py` & `thinc-9.0.0.dev5/thinc/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_types.py` & `thinc-9.0.0.dev5/thinc/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/test_util.py` & `thinc-9.0.0.dev5/thinc/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/tests/util.py` & `thinc-9.0.0.dev5/thinc/tests/util.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/types.py` & `thinc-9.0.0.dev5/thinc/types.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc/util.py` & `thinc-9.0.0.dev5/thinc/util.py`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc.egg-info/PKG-INFO` & `thinc-9.0.0.dev5/thinc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thinc
-Version: 9.0.0.dev4
+Version: 9.0.0.dev5
 Summary: A refreshing functional take on deep learning, compatible with your favorite libraries
 Home-page: https://github.com/explosion/thinc
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev4 Summary: A refreshing
+Metadata-Version: 2.1 Name: thinc Version: 9.0.0.dev5 Summary: A refreshing
 functional take on deep learning, compatible with your favorite libraries Home-
 page: https://github.com/explosion/thinc Author: Explosion Author-email:
 contact@explosion.ai License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: POSIX :: Linux Classifier: Operating System :: MacOS :: MacOS X Classifier:
```

### Comparing `thinc-9.0.0.dev4/thinc.egg-info/SOURCES.txt` & `thinc-9.0.0.dev5/thinc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `thinc-9.0.0.dev4/thinc.egg-info/requires.txt` & `thinc-9.0.0.dev5/thinc.egg-info/requires.txt`

 * *Files identical despite different names*

