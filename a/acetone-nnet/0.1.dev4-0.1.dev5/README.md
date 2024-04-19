# Comparing `tmp/acetone_nnet-0.1.dev4.tar.gz` & `tmp/acetone_nnet-0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.1.dev4.tar", last modified: Wed Apr 17 12:06:44 2024, max compression
+gzip compressed data, was "acetone_nnet-0.1.dev5.tar", last modified: Fri Apr 19 14:28:02 2024, max compression
```

## Comparing `acetone_nnet-0.1.dev4.tar` & `acetone_nnet-0.1.dev5.tar`

### file list

```diff
@@ -1,145 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.386792 acetone_nnet-0.1.dev4/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.1.dev4/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev4/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev4/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-17 12:06:44.386792 acetone_nnet-0.1.dev4/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6470 2024-04-16 12:29:53.000000 acetone_nnet-0.1.dev4/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2044 2024-04-17 12:05:41.000000 acetone_nnet-0.1.dev4/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-17 12:06:44.386792 acetone_nnet-0.1.dev4/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.235790 acetone_nnet-0.1.dev4/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.246790 acetone_nnet-0.1.dev4/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-12 11:36:39.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.248790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1872 2024-04-17 09:10:33.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4087 2024-04-12 11:42:37.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.250790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3168 2024-04-17 09:50:55.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.251790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1461 2024-04-12 11:51:36.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4324 2024-04-15 11:48:34.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1466 2024-04-12 11:51:50.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1477 2024-04-12 11:52:28.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1476 2024-04-12 11:52:33.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.252790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.253790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.254790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.255790 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    24499 2024-04-17 09:12:32.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.255790 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.255790 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7516 2024-04-17 09:10:02.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.255790 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    17216 2024-04-17 09:51:26.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.256790 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.256790 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25232 2024-04-12 14:49:23.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4014 2024-04-12 09:54:11.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2453 2024-04-12 09:55:41.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.256790 acetone_nnet-0.1.dev4/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.284790 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.314791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.332791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.338791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.341791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.362791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2122 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.371791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.381791 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      912 2024-04-17 09:11:31.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      930 2024-04-17 09:12:00.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-17 12:06:44.385792 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6830 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      129 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-17 12:06:44.000000 acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.377583 acetone_nnet-0.1.dev5/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.1.dev5/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev5/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.1.dev5/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-19 14:28:02.377583 acetone_nnet-0.1.dev5/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6470 2024-04-16 12:29:53.000000 acetone_nnet-0.1.dev5/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2061 2024-04-19 14:27:36.000000 acetone_nnet-0.1.dev5/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-19 14:28:02.377583 acetone_nnet-0.1.dev5/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.124580 acetone_nnet-0.1.dev5/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.151580 acetone_nnet-0.1.dev5/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.152580 acetone_nnet-0.1.dev5/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3263 2024-04-19 14:26:35.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.153580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-18 12:29:33.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.155580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3168 2024-04-17 09:50:55.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.156580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1672 2024-04-18 13:27:34.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1677 2024-04-18 13:28:07.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1688 2024-04-18 13:28:11.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1687 2024-04-18 13:28:13.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.158580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.158580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.159580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.160580 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.160580 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.160580 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18238 2024-04-19 13:55:52.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.160580 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14173 2024-04-19 12:59:15.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.161580 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.161580 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    27450 2024-04-18 12:36:48.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4103 2024-04-18 14:54:31.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3220 2024-04-19 13:56:29.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.161580 acetone_nnet-0.1.dev5/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.211581 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.277582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.303582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.309582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.312582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.334582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.342582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.356582 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:28:02.376583 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7852 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-19 14:28:02.000000 acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.1.dev4/AUTHORS.md` & `acetone_nnet-0.1.dev5/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/COPYING` & `acetone_nnet-0.1.dev5/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/LICENSE` & `acetone_nnet-0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/PKG-INFO` & `acetone_nnet-0.1.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1.dev4
+Version: 0.1.dev5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.1.dev4/README.md` & `acetone_nnet-0.1.dev5/README.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/pyproject.toml` & `acetone_nnet-0.1.dev5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.1.dev4"
+version = "0.1.dev5"
 requires-python = ">=3.10"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
@@ -53,13 +53,13 @@
     "templates/layers/*.tpl",
     "templates/layers/Resize/*.tpl",
     "templates/layers/Pad/*.tpl",
     "templates/layers/Gemm/*.tpl",
     "templates/layers/Conv/*.tpl"]
 
 [project.scripts]
-acetone_generate = "acetone_nnet.cli_acetone:cli_acetone"
-acetone_compare = "acetone_nnet.cli_compare:cli_compare"
+acetone_generate = "acetone_nnet.bin.bin_acetone:acetone_generate"
+acetone_compare = "acetone_nnet.bin.bin_acetone:acetone_compare"
 
 [project.urls]
 Repository = "https://github.com/onera/acetone/"
 "Bug Tracker" = "https://github.com/onera/acetone/issues"
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest
 )
 
 from .activation_functions import (
-    ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
+    ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
 
 from .neural_network import CodeGenerator
 
 from .Layer import Layer
 
 __all__ = (
     "CodeGenerator",
-    "ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip",
+    "ActivationFunctions", "Linear", "Sigmoid", "ReLu", "TanH", "Exponential", "Logarithm", "Clip", "LeakyReLu",
     "Layer",
     layers.__all__
 )
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,31 @@
 
     def write_activation_str(self, local_var):
 
         s = local_var +' > 0 ? '+ local_var +' : 0' # output = condition ? value_if_true : value_if_false
         
         return s
 
+class LeakyReLu(ActivationFunctions):
+    
+    def __init__(self,alpha):
+        super().__init__()
+        self.name = 'leakyrelu'
+        self.comment = ' and apply rectifier'
+        self.alpha = alpha
+    
+    def compute(self, z):
+        return np.maximum(self.alpha*z,z)
+
+    def write_activation_str(self, local_var):
+
+        s = local_var +' > 0 ? '+ local_var +' : '+str(self.alpha)+'*'+local_var # output = condition ? value_if_true : value_if_false
+        
+        return s
+
 class TanH(ActivationFunctions):
     def __init__(self):
         super().__init__()
         self.name = 'hyperb_tan'
         self.comment = ' and apply hyperbolic tangent function'
         
     
@@ -137,9 +154,8 @@
         self.min = min
     
     def compute(self, z):
         return np.clip(z,self.min,self.max)
     
     def write_activation_str(self,local_var):
         s = local_var +' > '+str(self.max)+' ? '+ str(self.max) +' : (' + local_var + ' < ' + str(self.min) + ' ? ' + str(self.min) + ' : ' + local_var + ')'
-        return s
-    
+        return s
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,27 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 
-#Addition of several tensor
-class Add(Broadcast):
+#Multiplication of several tensors
+class Multiply(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Add'
-        self.specific_operator = ' + '
+        self.name = 'Multiply'
+        self.specific_operator = '*'
     
     def forward_path_layer(self, inputs):
-        output = inputs[0]
-        for input in inputs[1:]:
-            output += input
-        return self.activation_function.compute(output)
+        if(self.constant is None):
+            constant = 1
+        else: 
+            constant = self.constant
+        if(len(inputs.shape) == 4):
+            output = inputs[0]
+            for input in inputs[1:]:
+                output *= input
+        else:
+            output = inputs
+        return self.activation_function.compute(constant*output)
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,40 +18,42 @@
  ******************************************************************************
 """
 
 from ...Layer import Layer
 
 from abc import abstractmethod
 import pystache
+import numpy as np
 
 #The class of the Layers which compute operation with broadcast numpy style
 #attribut: none
 #input: a list of tensor
 #output: the resultant tensor
 class Broadcast(Layer):
-    def __init__(self, idx, size, input_shapes, output_shape,activation_function):
+    def __init__(self, idx, size, input_shapes, output_shape,activation_function, constant = None):
         super().__init__()
         self.idx = idx
         self.size = size
         self.name = ''
         self.input_shapes = input_shapes
         
         self.output_height = output_shape[2]
         self.output_width = output_shape[3]
         self.output_channels = output_shape[1]
         self.specific_operator = ''
         self.activation_function = activation_function
+        self.constant = constant
+        if(constant is not None):
+            self.constant_size = self.count_elements_array(self.constant)
 
     #Go through all the indices and do the operation
     def generate_inference_code_layer(self):
 
         mustach_hash = {}
 
-        mustach_hash = {}
-
         mustach_hash['name'] = self.name
         mustach_hash['idx'] = "{:02d}".format(self.idx)
         mustach_hash['comment'] = self.activation_function.comment
         mustach_hash['road'] = self.path
         mustach_hash['size'] = self.size
 
         mustach_hash['activation_function'] = self.activation_function.write_activation_str('tensor_temp[k]')
@@ -88,14 +90,23 @@
             previous_dict['input_width'] = self.input_shapes[k][3]
             previous_dict['input_height'] = self.input_shapes[k][2]
             previous_dict['input_channels'] = self.input_shapes[k][1]
             if(k != len(self.previous_layer) -1):
                 previous_dict['operator'] = self.specific_operator
             mustach_hash['broadcast'].append(previous_dict)
         
+        if(self.constant is not None):
+            constant_dict = {}
+            constant_dict['cst_width'] = self.input_shapes[-1][3]
+            constant_dict['cst_height'] = self.input_shapes[-1][2]
+            constant_dict['cst_channels'] = self.input_shapes[-1][1]
+            constant_dict['operator'] = self.specific_operator
+            mustach_hash['constant'] = [constant_dict]
+
+        
         with open(self.template_path+'layers/template_Broadcast.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
 
     @abstractmethod
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,11 +25,18 @@
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.name = 'Divide'
         self.specific_operator = '/'
     
     def forward_path_layer(self, inputs):
-        output = inputs[0]
-        for input in inputs[1:]:
-            output /= input
-        return self.activation_function.compute(output)
+        if(self.constant is None):
+            constant = 1
+        else: 
+            constant = self.constant
+        if(len(inputs.shape) == 4):
+            output = inputs[0]
+            for input in inputs[1:]:
+                output *= input
+        else:
+            output = inputs
+        return self.activation_function.compute(output/constant)
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,20 +16,27 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 
-#Multiplication of several tensors
-class Multiply(Broadcast):
+#Subtraction of several tensors
+class Subtract(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Multiply'
-        self.specific_operator = '*'
+        self.name = 'Subtract'
+        self.specific_operator = ' - '
     
     def forward_path_layer(self, inputs):
-        output = inputs[0]
-        for input in inputs[1:]:
-            output *= input
-        return self.activation_function.compute(output)
+        if(self.constant is None):
+            constant = 0
+        else: 
+            constant = self.constant
+        if(len(inputs.shape) == 4):
+            output = inputs[0]
+            for input in inputs[1:]:
+                output *= input
+        else:
+            output = inputs
+        return self.activation_function.compute(output-constant)
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,22 +14,46 @@
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
-from .Broadcast import Broadcast
+from ..Layer import Layer
+import numpy as np
+import pystache
 
-#Subtraction of several tensors
-class Subtract(Broadcast):
-    
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.name = 'Subtract'
-        self.specific_operator = ' - '
+class Softmax(Layer):
+
+    def __init__(self, idx, size):
+        
+        super().__init__()
+        self.idx = idx
+        self.size = size
+        self.name = 'Softmax'
+
+    def generate_inference_code_layer(self):
+        output_str = self.previous_layer[0].output_str
+
+        mustach_hash = {}
+
+        mustach_hash['name'] = self.name
+        mustach_hash['idx'] = "{:02d}".format(self.idx)
+        mustach_hash['size'] = self.size
+        mustach_hash['road'] = self.path
+        mustach_hash['output_str'] = output_str
+
+        if (self.fused_layer):
+            mustach_hash['fused_layer'] = self.fused_layer.write_activation_str('output_'+str(self.path)+'[j]', self.idx, 'j')
+
+        with open(self.template_path+'layers/template_Softmax.c.tpl','r') as template_file:
+            template = template_file.read()
+        template_file.close()
+
+        return pystache.render(template, mustach_hash)
     
-    def forward_path_layer(self, inputs):
-        output = inputs[0]
-        for input in inputs[1:]:
-            output -= input
-        return self.activation_function.compute(output)
+    def forward_path_layer(self, input):
+        
+        exp = np.exp(input, dtype=np.float)
+        output = exp/np.sum(exp)
+
+        return output
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,15 +416,15 @@
 
         for cst in written:
             mustach_hash['cst'].append({'name':cst, 'size':written[cst]})
             
         if (any(isinstance(layer, Concatenate) 
                 or any(isinstance(layer, Conv2D)) 
                 or any(isinstance(layer, Dense))
-                or any(isinstance(layer, Broadcast)) 
+                or any(issubclass(layer, Broadcast)) 
                 or any(isinstance(layer, Gather)) 
                 or any(isinstance(layer, Pad))) for layer in self.layers):
             mustach_hash['tensor_temp'] = True
             mustach_hash['temp_size'] = max(self.l_size_max,self.patches_size_max)
  
         mustach_hash['layers'] = []
         for layer in self.layers:
@@ -444,14 +444,19 @@
             if type(layer) is Conv2D_indirect_gemm:
                 layer_hash['patches_size'] = layer.patches_size
                 to_print = True
             
             if type(layer) is BatchNormalization:
                 layer_hash['channels'] = layer.output_channels
                 to_print = True
+            
+            if issubclass(type(layer), Broadcast):
+                if(layer.constant is not None):
+                    layer_hash['constant_size'] = layer.constant_size
+                    to_print = True
 
             if (to_print):
                 mustach_hash['layers'].append(layer_hash)
         
         if(self.normalize):
             mustach_hash['normalization_cst'] = self.Normalizer.write_normalization_cst_in_header_file()
         
@@ -484,15 +489,15 @@
         
         for cst in written:
             mustach_hash['cst'].append({'name':cst, 'size':written[cst]})
         
         if (any(isinstance(layer, Concatenate) 
                 or any(isinstance(layer, Conv2D)) 
                 or any(isinstance(layer, Dense))
-                or any(isinstance(layer, Broadcast)) 
+                or any(issubclass(layer, Broadcast)) 
                 or any(isinstance(layer, Gather)) 
                 or any(isinstance(layer, Pad))) for layer in self.layers):
             mustach_hash['tensor_temp'] = True
             mustach_hash['temp_size'] = max(self.l_size_max,self.patches_size_max)
              
         if any(isinstance(layer, Conv2D_indirect_gemm) for layer in self.layers):
             mustach_hash['zero'] = True
@@ -521,14 +526,20 @@
             if type(layer) is BatchNormalization:
                 layer_hash['channels'] = layer.output_channels
                 layer_hash['mean'] = self.flatten_array_orderc(layer.mean)
                 layer_hash['var'] = self.flatten_array_orderc(layer.var)
                 layer_hash['scale'] = self.flatten_array_orderc(layer.scale)
                 to_print = True
             
+            if issubclass(type(layer), Broadcast):
+                if(layer.constant is not None):
+                    layer_hash['constant'] = self.flatten_array_orderc(layer.constant)
+                    layer_hash['constant_size'] = layer.constant_size
+                    to_print = True
+            
             if (to_print):
                 mustach_hash['layers'].append(layer_hash)
         
         with open(self.template_path+'template_global_var_file.c.tpl', 'r') as template_file:
             template = template_file.read()
         template_file.close()
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     model_dict =  json.loads(model_json)
 
     input_layer_size = 1
     for i in range(1, len(keras_model.input.shape)): #start in idx 1 cause idx 0 represents batch size, so it's None in inference phase
         input_layer_size = input_layer_size * keras_model.input.shape[i]
 
     model_dict['config']['data_format'] = 'channels_first'
-    if (hasattr(model_dict['config']['layers'][j]['config'],'data_format')
-        and (model_dict['config']['layers'][j]['config']['data_format'] == 'channels_last') for j in range(len(model_dict['config']['layers']))):
+    if (hasattr(layer['config'],'data_format')
+        and (layer['config']['data_format'] == 'channels_last') for layer in model_dict['config']['layers']):
         model_dict['config']['data_format'] = 'channels_last'
 
     if keras_model.layers[0].__class__.__name__ == 'InputLayer':
         start = 0
 
     else:
         start = 1
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,29 +27,29 @@
 from ...code_generator import (
     AveragePooling2D, MaxPooling2D,
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Constant_Pad,
     Add, Multiply, Subtract, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
     Concatenate, InputLayer, Dense, Softmax,  Dot, Flatten, BatchNormalization,
-    Linear, ReLu, Sigmoid, TanH
+    Linear, ReLu, Sigmoid, TanH, LeakyReLu
 )
 
 def create_actv_function_obj(activation_str):
 
         if activation_str == 'sigmoid':
             return Sigmoid()
         elif activation_str == 'relu':
             return ReLu()
         elif activation_str == 'tanh':
             return TanH()
         elif activation_str == 'linear':
             return Linear()
-        elif activation_str == 'softmax':
-            return Softmax()
+        elif activation_str == 'leaky_relu':
+            return LeakyReLu(0.2)
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
 
     elif 'std_gemm' in algorithm:
@@ -67,265 +67,227 @@
         return ResizeLinear(**kwargs)
     
     else:
         return ResizeNearest(**kwargs)
 
 def load_json(file_to_parse, conv_algorithm):
         
-        file = open(file_to_parse, 'r')
-        model = json.load(file)
-        data_format = model['config']['data_format'] 
+    file = open(file_to_parse, 'r')
+    model = json.load(file)
+    data_format = model['config']['data_format'] 
 
-        data_type = model['config']['layers'][0]['config']['dtype']
+    data_type = model['config']['layers'][0]['config']['dtype']
 
-        if data_type == 'float64':
-            data_type = 'double'
-            data_type_py = np.float64
+    if data_type == 'float64':
+        data_type = 'double'
+        data_type_py = np.float64
 
-        elif data_type == 'float32':
-            data_type = 'float'
-            data_type_py = np.float32
+    elif data_type == 'float32':
+        data_type = 'float'
+        data_type_py = np.float32
 
-        elif data_type == 'int':
-            data_type = 'long int'
-            data_type_py = np.int32
+    elif data_type == 'int':
+        data_type = 'long int'
+        data_type_py = np.int32
 
-        layers = []
+    layers = []
 
-        l_temp = InputLayer(0, model['config']['layers'][0]['config']['size'], model['config']['layers'][0]['config']['input_shape'], data_format)
+    l_temp = InputLayer(0, model['config']['layers'][0]['config']['size'], model['config']['layers'][0]['config']['input_shape'], data_format)
 
-        layers.append(l_temp)
+    layers.append(l_temp)
 
-        nb_softmax_layers = 0
+    nb_softmax_layers = 0
 
-        for idx, layer in list(islice(enumerate(model['config']['layers']), 1, None)):
-            add_softmax_layer = False
-            
-            idx += nb_softmax_layers
+    for idx, layer in list(islice(enumerate(model['config']['layers']), 1, None)):
+        add_softmax_layer = False
+        
+        idx += nb_softmax_layers
 
-            if 'activation' in layer['config']:
-                if layer['config']['activation'] == 'softmax':
-                    layer['config']['activation'] = 'linear'
-                    add_softmax_layer = True
-        
-            if layer['class_name'] == 'Dense':
-                weights = np.array(data_type_py(layer['weights']))
-                current_layer = Dense(idx=idx,
-                                      size=layer['config']['units'],
-                                      weights=np.array(data_type_py(layer['weights'])),
-                                      biases=data_type_py(layer['biases']),
-                                      activation_function=create_actv_function_obj(layer['config']['activation']))
-            
-            elif layer['class_name'] == 'Conv2D':
-                weights = np.array(data_type_py(layer['weights']))
-                current_layer = create_conv2d_obj(algorithm = conv_algorithm,
-                                                  conv_algorithm = conv_algorithm,
-                                                  idx = idx,
-                                                  size = layer['config']['size'],
-                                                  padding = layer['config']['padding'],
-                                                  strides = layer['config']['strides'][0],
-                                                  kernel_h = layer['config']['kernel_size'][0],
-                                                  kernel_w = layer['config']['kernel_size'][1],
-                                                  dilation_rate = layer['config']['dilation_rate'][0],
-                                                  nb_filters = layer['config']['filters'],
-                                                  input_shape = layer['config']['input_shape'],
-                                                  output_shape = layer['config']['output_shape'],
-                                                  weights = weights, 
-                                                  biases = data_type_py(layer['biases']),
-                                                  activation_function = create_actv_function_obj(layer['config']['activation']))
-            
-            elif layer['class_name'] == 'AveragePooling2D':
-                current_layer = AveragePooling2D(idx = idx,
-                                                 size = layer['config']['size'],
-                                                 padding = layer['config']['padding'],
-                                                 strides = layer['config']['strides'][0],
-                                                 pool_size = layer['config']['pool_size'][0],
-                                                 input_shape = layer['config']['input_shape'],
-                                                 output_shape = layer['config']['output_shape'],
-                                                 activation_function = Linear())
-            
-            elif layer['class_name'] == 'MaxPooling2D':
-                current_layer = MaxPooling2D(idx = idx,
-                                             size = layer['config']['size'],
-                                             padding = layer['config']['padding'],
-                                             strides = layer['config']['strides'][0],
-                                             pool_size = layer['config']['pool_size'][0],
-                                             input_shape = layer['config']['input_shape'],
-                                             output_shape = layer['config']['output_shape'],
-                                             activation_function = Linear())
-            
-            elif layer['class_name'] == 'Flatten':
-                current_layer = Flatten(idx = idx,
+        if 'activation' in layer['config']:
+            if layer['config']['activation'] == 'softmax':
+                layer['config']['activation'] = 'linear'
+                add_softmax_layer = True
+    
+        if layer['class_name'] == 'Dense':
+            current_layer = Dense(idx=idx,
+                                    size=layer['config']['units'],
+                                    weights=np.array(data_type_py(layer['weights'])),
+                                    biases=data_type_py(layer['biases']),
+                                    activation_function=create_actv_function_obj(layer['config']['activation']))
+        
+        elif layer['class_name'] == 'Conv2D':
+            current_layer = create_conv2d_obj(algorithm = conv_algorithm,
+                                                conv_algorithm = conv_algorithm,
+                                                idx = idx,
                                                 size = layer['config']['size'],
+                                                padding = layer['config']['padding'],
+                                                strides = layer['config']['strides'][0],
+                                                kernel_h = layer['config']['kernel_size'][0],
+                                                kernel_w = layer['config']['kernel_size'][1],
+                                                dilation_rate = layer['config']['dilation_rate'][0],
+                                                nb_filters = layer['config']['filters'],
                                                 input_shape = layer['config']['input_shape'],
-                                                data_format = data_format)
-            
-            elif layer['class_name'] == 'Add':
-                current_layer = Add(idx = layer['config']['idx'],
-                                    size = layer['config']['size'],
-                                    input_shapes = layer['config']['input_shape'],
-                                    output_shape = layer['config']['output_shape'],
-                                    activation_function = Linear())
-
-            elif layer['class_name'] == 'Multiply':
-                current_layer = Multiply(idx = layer['config']['idx'],
-                                         size = layer['config']['size'], 
-                                         input_shapes = layer['config']['input_shape'], 
-                                         output_shape = layer['config']['output_shape'],
-                                         activation_function= Linear())
-            
-            elif layer['class_name'] == 'Subtract':
-                current_layer = Subtract(idx = layer['config']['idx'], 
-                                         size = layer['config']['size'], 
-                                         input_shapes = layer['config']['input_shape'], 
-                                         output_shape = layer['config']['output_shape'],
-                                         activation_function= Linear())
-            
-            elif layer['class_name'] == 'Concatenate':
-                axis = layer['config']['axis']
-                if(data_format == 'channels_last'):
-                    if(axis == 3):
-                        axis = 1
-                    else:
-                        axis = axis + 1
-                current_layer = Concatenate(idx = layer['config']['idx'], 
+                                                output_shape = layer['config']['output_shape'],
+                                                weights = np.array(data_type_py(layer['weights'])), 
+                                                biases = data_type_py(layer['biases']),
+                                                activation_function = create_actv_function_obj(layer['config']['activation']))
+        
+        elif layer['class_name'] == 'AveragePooling2D':
+            current_layer = AveragePooling2D(idx = idx,
+                                                size = layer['config']['size'],
+                                                padding = layer['config']['padding'],
+                                                strides = layer['config']['strides'][0],
+                                                pool_size = layer['config']['pool_size'][0],
+                                                input_shape = layer['config']['input_shape'],
+                                                output_shape = layer['config']['output_shape'],
+                                                activation_function = Linear())
+        
+        elif layer['class_name'] == 'MaxPooling2D':
+            current_layer = MaxPooling2D(idx = idx,
                                             size = layer['config']['size'],
-                                            axis = axis, 
-                                            input_shapes = layer['config']['input_shape'], 
+                                            padding = layer['config']['padding'],
+                                            strides = layer['config']['strides'][0],
+                                            pool_size = layer['config']['pool_size'][0],
+                                            input_shape = layer['config']['input_shape'],
                                             output_shape = layer['config']['output_shape'],
-                                            activation_function=Linear())
-            
-            elif layer['class_name'] == 'Maximum':
-                current_layer = Maximum(idx = layer['config']['idx'], 
-                                         size = layer['config']['size'], 
-                                         input_shapes = layer['config']['input_shape'], 
-                                         output_shape = layer['config']['output_shape'],
-                                         activation_function= Linear())
-                
-            elif layer['class_name'] == 'Minimum':
-                current_layer = Minimum(idx = layer['config']['idx'], 
-                                         size = layer['config']['size'], 
-                                         input_shapes = layer['config']['input_shape'], 
-                                         output_shape = layer['config']['output_shape'],
-                                         activation_function= Linear())
-            
-            elif layer['class_name'] == 'Average':
-                current_layer = Average(idx = layer['config']['idx'], 
-                                         size = layer['config']['size'], 
-                                         input_shapes = layer['config']['input_shape'], 
-                                         output_shape = layer['config']['output_shape'],
-                                         activation_function= Linear())
-            
-            elif layer['class_name'] == 'Dot':
-                current_layer = Dot(idx = layer['config']['idx'],
-                                    size = layer['config']['size'],
-                                    axis= layer['config']['axes'],
-                                    input_shapes = layer['config']['input_shape'], 
-                                    output_shape = layer['config']['output_shape'],
-                                    activation_function = Linear())
-            
-            elif layer['class_name'] == 'UpSampling2D': # Need to make sure that the 'size' attribut of the Layer is renamed
-                target_size = layer['config']['scale']
-                if(type(target_size) == int):
-                    target_size = [target_size,target_size]
-                target_size = [1,1]+target_size
-                current_layer = create_resize_obj(mode = layer['config']['interpolation'],
-                                                  idx = layer['config']['idx'],
-                                                  size = layer['config']['size'],
-                                                  input_shape = layer['config']['input_shape'],
-                                                  axes = [],
-                                                  coordinate_transformation_mode = 'half_pixel',
-                                                  exclude_outside = 0,
-                                                  keep_aspect_ratio_policy = 'stretch',
-                                                  boolean_resize = True,
-                                                  target_size = target_size,
-                                                  roi = [],
-                                                  extrapolation_value = 0,
-                                                  nearest_mode = 'round_prefer_floor',
-                                                  cubic_coeff_a = -0.75,
-                                                  activation_function= Linear())
-            
-            elif layer['class_name'] == 'ZeroPadding1D':
-                pads = layer['config']['padding']
-                if(type(pads) == int):
-                    pads = [pads for i in range(8)]
+                                            activation_function = Linear())
+        
+        elif layer['class_name'] == 'Flatten':
+            current_layer = Flatten(idx = idx,
+                                            size = layer['config']['size'],
+                                            input_shape = layer['config']['input_shape'],
+                                            data_format = data_format)
+        
+        elif layer['class_name'] == 'Add':
+            current_layer = Add(idx = layer['config']['idx'],
+                                size = layer['config']['size'],
+                                input_shapes = layer['config']['input_shape'],
+                                output_shape = layer['config']['output_shape'],
+                                activation_function = Linear())
+
+        elif layer['class_name'] == 'Multiply':
+            current_layer = Multiply(idx = layer['config']['idx'],
+                                        size = layer['config']['size'], 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function= Linear())
+        
+        elif layer['class_name'] == 'Subtract':
+            current_layer = Subtract(idx = layer['config']['idx'], 
+                                        size = layer['config']['size'], 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function= Linear())
+        
+        elif layer['class_name'] == 'Concatenate':
+            axis = layer['config']['axis']
+            if(data_format == 'channels_last'):
+                if(axis == 3):
+                    axis = 1
                 else:
-                    pads = [0,0,pads[0],0,0,0,pads[1],0]
-
-                current_layer = Constant_Pad(idx = layer['config']['idx'],
-                                             size = layer['config']['size'],
-                                             pads = pads,
-                                             constant_value = 0,
-                                             axes = [],
-                                             input_shape = layer['config']['input_shape'],
-                                             activation_function = Linear())
-
-            elif layer['class_name'] == 'ZeroPadding2D':
-                pads = layer['config']['padding']
-                if(type(pads) == int):
-                    pads = [pads for i in range(8)]
+                    axis = axis + 1
+            current_layer = Concatenate(idx = layer['config']['idx'], 
+                                        size = layer['config']['size'],
+                                        axis = axis, 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function=Linear())
+        
+        elif layer['class_name'] == 'Maximum':
+            current_layer = Maximum(idx = layer['config']['idx'], 
+                                        size = layer['config']['size'], 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function= Linear())
+            
+        elif layer['class_name'] == 'Minimum':
+            current_layer = Minimum(idx = layer['config']['idx'], 
+                                        size = layer['config']['size'], 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function= Linear())
+        
+        elif layer['class_name'] == 'Average':
+            current_layer = Average(idx = layer['config']['idx'], 
+                                        size = layer['config']['size'], 
+                                        input_shapes = layer['config']['input_shape'], 
+                                        output_shape = layer['config']['output_shape'],
+                                        activation_function= Linear())
+        
+        elif layer['class_name'] == 'Dot':
+            current_layer = Dot(idx = layer['config']['idx'],
+                                size = layer['config']['size'],
+                                axis= layer['config']['axes'],
+                                input_shapes = layer['config']['input_shape'], 
+                                output_shape = layer['config']['output_shape'],
+                                activation_function = Linear())
+
+        elif layer['class_name'] == 'ZeroPadding2D':
+            pads = layer['config']['padding']
+            if(type(pads) == int):
+                pads = [pads for i in range(8)]
+            else:
+                if(type(pads[0]) == int):
+                    pad_top, pad_bottom = pads[0], pads[0]
+                    pad_left, pad_right = pads[1], pads[1]
                 else:
-                    if(type(pads[0]) == int):
-                        pad_top, pad_bottom = pads[0], pads[0]
-                        pad_left, pad_right = pads[1], pads[1]
-                    else:
-                        pad_top, pad_bottom = pads[0][0], pads[0][1]
-                        pad_left, pad_right = pads[1][0], pads[1][1]
-                    pads = [0,0,pad_top,pad_left,0,0,pad_bottom,pad_right]
-
-                current_layer = Constant_Pad(idx = layer['config']['idx'],
-                                             size = layer['config']['size'],
-                                             pads = pads,
-                                             constant_value = 0,
-                                             axes = [],
-                                             input_shape = layer['config']['input_shape'],
-                                             activation_function = Linear())
-            
-            elif layer['class_name'] == 'BatchNormalization':
-                current_layer = BatchNormalization(idx = layer['config']['idx'],
-                                                   size = layer['config']['size'],
-                                                   input_shape = layer['config']['input_shape'],
-                                                   epsilon = layer['config']['epsilon'],
-                                                   scale = np.array(data_type_py(layer['gamma'])),
-                                                   biases = np.array(data_type_py(layer['beta'])),
-                                                   mean = np.array(data_type_py(layer['moving_mean'])),
-                                                   var = np.array(data_type_py(layer['moving_var'])),
-                                                   activation_function = Linear())
-            
-            
-            elif  'Normalization' in layer['class_name']:
-                continue
+                    pad_top, pad_bottom = pads[0][0], pads[0][1]
+                    pad_left, pad_right = pads[1][0], pads[1][1]
+                pads = [0,0,pad_top,pad_left,0,0,pad_bottom,pad_right]
 
-            elif  'Dropout' in layer['class_name']:
-                continue
+            current_layer = Constant_Pad(idx = layer['config']['idx'],
+                                            size = layer['config']['size'],
+                                            pads = pads,
+                                            constant_value = 0,
+                                            axes = [],
+                                            input_shape = layer['config']['input_shape'],
+                                            activation_function = Linear())
+        
+        elif layer['class_name'] == 'BatchNormalization':
+            current_layer = BatchNormalization(idx = layer['config']['idx'],
+                                                size = layer['config']['size'],
+                                                input_shape = layer['config']['input_shape'],
+                                                epsilon = layer['config']['epsilon'],
+                                                scale = np.array(data_type_py(layer['gamma'])),
+                                                biases = np.array(data_type_py(layer['beta'])),
+                                                mean = np.array(data_type_py(layer['moving_mean'])),
+                                                var = np.array(data_type_py(layer['moving_var'])),
+                                                activation_function = Linear())
+        
+        
+        elif  'Normalization' in layer['class_name']:
+            continue
 
-            elif  layer['class_name'] == 'Reshape':
-                continue
+        elif  'Dropout' in layer['class_name']:
+            continue
 
-            elif  layer['class_name'] == 'Permute':
-                continue
+        elif  layer['class_name'] == 'Reshape':
+            continue
 
-            else:
-                raise TypeError("Error: layer"+layer['class_name']+" not supported\n")
-            
-            for i in layer['config']['prev_layer_idx']:
-                current_layer.previous_layer.append(layers[i])
-                layers[i].next_layer.append(current_layer)
+        elif  layer['class_name'] == 'Permute':
+            continue
 
+        else:
+            raise TypeError("Error: layer"+layer['class_name']+" not supported\n")
+        
+        for i in layer['config']['prev_layer_idx']:
+            current_layer.previous_layer.append(layers[i])
+            layers[i].next_layer.append(current_layer)
+
+        l_temp = current_layer
+        layers.append(current_layer)
+
+        # Separeted method to generate softmax
+        if add_softmax_layer:
+            nb_softmax_layers += 1
+            current_layer = Softmax(idx+1, l_temp.size)
+            l_temp.next_layer.append(current_layer)
+            current_layer.previous_layer.append(l_temp)
             l_temp = current_layer
             layers.append(current_layer)
 
-            # Separeted method to generate softmax
-            if add_softmax_layer:
-                nb_softmax_layers += 1
-                current_layer = Softmax(idx+1, l_temp.size)
-                l_temp.next_layer.append(current_layer)
-                current_layer.previous_layer.append(l_temp)
-                l_temp = current_layer
-                layers.append(current_layer)
-
-        layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
-        layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
-        print("Finished model initialization.")
-        file.close()
-        return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
+    layers, listRoad, maxRoad, dict_cst = graph_interpretor.tri_topo(layers)
+    layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
+    print("Finished model initialization.")
+    file.close()
+    return layers, data_type, data_type_py, data_format, maxRoad, dict_cst
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 6% similar despite different names*

```diff
@@ -421,87 +421,149 @@
                             pool_size = input_shape[2],
                             input_shape = input_shape,
                             output_shape = output_shape,
                             activation_function = Linear())
 
 ### Broadcats layers ###
 
-#create a layer Add
-def create_Add(node,idx,dict_input,dict_output,model):
+#create a layer Add_Biass 
+##### UNUSED #####
+def create_Add_Biass(node,idx,dict_input,dict_output,model):
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_output[node.output[0]] = idx
     right_tensor = look_for_initializer(node.input[0],model)
     left_tensor = look_for_initializer(node.input[1],model)
-    if(not right_tensor and not left_tensor):
-        input_shapes =[]
-        for input in node.input:
+    if(right_tensor):
+        biases = onnx.numpy_helper.to_array(right_tensor)
+        dict_input[idx] = [node.input[1]]
+    elif(left_tensor):
+        biases = onnx.numpy_helper.to_array(left_tensor)
+        dict_input[idx] = [node.input[0]]
+    return Add_Bias(idx = idx,
+                        size = size,
+                        biases = biases,
+                        activation_function = Linear())
+
+#create a layer Add
+def create_Add(node,idx,dict_input,dict_output,model):
+    output_shape = get_shape(node.output[0],model)
+    size = find_size(output_shape)
+    dict_output[node.output[0]] = idx
+    dict_input[idx] = []
+    constant = np.zeros(get_shape(node.input[0], model))
+    input_shapes =[]
+    for input in node.input:
+        cst = look_for_initializer(input,model)
+        if(cst):
+            constant = constant + onnx.numpy_helper.to_array(cst)
+        else:
+            dict_input[idx].append(input)
             input_shapes.append(get_shape(input,model))
-        dict_input[idx] = node.input
-        return Add(idx=idx,
-                    size=size,
-                    input_shapes=input_shapes,
-                    output_shape=output_shape,
-                    activation_function= Linear())
+    if(constant.any()):
+        if (len(constant.shape)<4):
+            for i in range(0,4-len(constant.shape)):
+                constant = np.expand_dims(constant,axis=0)
+        input_shapes.append(constant.shape)
     else:
-        if(right_tensor):
-            biases = onnx.numpy_helper.to_array(right_tensor)
-            dict_input[idx] = [node.input[1]]
-        elif(left_tensor):
-            biases = onnx.numpy_helper.to_array(left_tensor)
-            dict_input[idx] = [node.input[0]]
-        return Add_Bias(idx = idx,
-                            size = size,
-                            biases = biases,
-                            activation_function = Linear())
+        constant = None
+    return Add(idx = idx,
+                size = size,
+                input_shapes = input_shapes,
+                output_shape = output_shape,
+                activation_function = Linear(),
+                constant = constant)
     
 #create a layer Div
 def create_Div(node,idx,dict_input,dict_output,model):
     input_shapes =[]
+    constant = 1
+    dict_input[idx] = []
     for input in node.input:
-        input_shapes.append(get_shape(input,model))
+        factor = look_for_initializer(input,model)
+        if(factor):
+            constant = constant / onnx.numpy_helper.to_array(factor)
+        else:
+            dict_input[idx].append(input)
+            input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
-    dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
+    if((constant == np.ones(constant.shape)).all()):
+        constant = None
+    else:
+        if (len(constant.shape)<4):
+            for i in range(0,4-len(constant.shape)):
+                constant = np.expand_dims(constant,axis=0)
+        input_shapes.append(constant.shape)
     return Divide(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
-                    activation_function= Linear())
+                    activation_function= Linear(),
+                    constant=constant)
+
 
 #create a layer Mul
 def create_Mul(node,idx,dict_input,dict_output,model):
     input_shapes =[]
+    constant = 1
+    dict_input[idx] = []
     for input in node.input:
-        input_shapes.append(get_shape(input,model))
+        factor = look_for_initializer(input,model)
+        if(factor):
+            constant = constant * onnx.numpy_helper.to_array(factor)
+        else:
+            dict_input[idx].append(input)
+            input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
-    dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
+    if((constant == np.ones(constant.shape)).all()):
+        constant = None
+    else:
+        if (len(constant.shape)<4):
+            for i in range(0,4-len(constant.shape)):
+                constant = np.expand_dims(constant,axis=0)
+        input_shapes.append(constant.shape)
     return Multiply(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
-                    activation_function= Linear())
+                    activation_function= Linear(),
+                    constant=constant)
 
 #create a layer Sub
 def create_Sub(node,idx,dict_input,dict_output,model):
     input_shapes =[]
+    constant = 0
+    dict_input[idx] = []
     for input in node.input:
-        input_shapes.append(get_shape(input,model))
+        factor = look_for_initializer(input,model)
+        if(factor):
+            constant = constant - onnx.numpy_helper.to_array(factor)
+        else:
+            dict_input[idx].append(input)
+            input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
-    dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
+    if((constant == np.ones(constant.shape)).all()):
+        constant = None
+    else:
+        if (len(constant.shape)<4):
+            for i in range(0,4-len(constant.shape)):
+                constant = np.expand_dims(constant,axis=0)
+        input_shapes.append(constant.shape)
     return Subtract(idx=idx,
                     size=size,
                     input_shapes=input_shapes,
                     output_shape=output_shape,
-                    activation_function= Linear())
+                    activation_function= Linear(),
+                    constant=constant)
     
 #create a layer Max
 def create_Max(node,idx,dict_input,dict_output,model):
     input_shapes =[]
     for input in node.input:
         input_shapes.append(get_shape(input,model))
     output_shape = get_shape(node.output[0],model)
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,20 @@
  ******************************************************************************
 """
 import onnx
 from ..ONNX_importer.create_layer import *
 from ...graph.graph_interpretor import tri_topo
 
 def load_onnx(file_to_parse, conv_algorithm):
-    #Loading the model and adding value_info if it's not already in it 
-    model = onnx.load(file_to_parse)
+    #Loading the model and adding value_info if it's not already in it
+    if(type(file_to_parse) == str): 
+        model = onnx.load(file_to_parse)
+    else:
+        model = file_to_parse
+        
     if (not model.graph.value_info):
         model = onnx.shape_inference.infer_shapes(model)
     
     #The list of layers
     layers = []
     #Dictionnary of the outputs of each layers: {output_name:layer_idx_from_which_the_output_come_from}
     dict_output = {}
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/format_importer/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,47 +15,63 @@
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 import keras
+from keras.engine.functional import Functional
+from keras.engine.sequential import Sequential
+import onnx
+
 from .JSON_importer.parser_JSON import load_json
 from .ONNX_importer.parser_ONNX import load_onnx
 from .NNET_importer.parser_NNET import load_nnet
 from .H5_importer.JSON_from_keras_model import JSON_from_keras_model
+from .H5_importer.parser_h5 import load_keras
 
 def get_path(file, new_type):
     new_path = ""
     list_path = file.split("/")
     file_name = list_path[-1].split(".")[0]
 
     for dir in list_path[:-1]:
         new_path += dir+"/"
     
     new_path += file_name + "." + new_type
     return new_path
 
 def parser(file_to_parse, conv_algorithm, normalize=False):
 
-    if("json" in  file_to_parse[-4:]):
-        return load_json(file_to_parse, conv_algorithm)
+    if(type(file_to_parse) == str):
+        if("json" in  file_to_parse[-4:]):
+            return load_json(file_to_parse, conv_algorithm)
+        
+        elif("onnx" in file_to_parse[-4:]):
+            return load_onnx(file_to_parse, conv_algorithm)
+        
+        elif("h5" in file_to_parse[-4:]):
+            model = keras.models.load_model(file_to_parse)
+
+            print("Creating the .json file...")
+            new_path = get_path(file_to_parse,"json")
+            JSON_from_keras_model(model, new_path)
+            print("File created\n")
+
+            return load_json(new_path, conv_algorithm)
+        
+        elif("nnet" in file_to_parse[-4:]):
+            return load_nnet(file_to_parse,normalize)
+        
+        else:
+            print("\nError: model description ."+file_to_parse[-4:]+" not supported")
+            raise TypeError("Error: model description ."+file_to_parse[-4:]+" not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
     
-    elif("onnx" in file_to_parse[-4:]):
+    elif(type(file_to_parse) == onnx.ModelProto):
         return load_onnx(file_to_parse, conv_algorithm)
     
-    elif("h5" in file_to_parse[-4:]):
-        model = keras.models.load_model(file_to_parse)
-
-        print("Creating the .json file...")
-        new_path = get_path(file_to_parse,"json")
-        JSON_from_keras_model(model, new_path)
-        print("File created\n")
+    elif(type(file_to_parse) == Functional or type(file_to_parse) == Sequential):
+        return load_keras(file_to_parse, conv_algorithm)
 
-        return load_json(new_path, conv_algorithm)
-    
-    elif("nnet" in file_to_parse[-4:]):
-        return load_nnet(file_to_parse,normalize)
-    
     else:
-        print("\nError: model description ."+file_to_parse[-4:]+" not supported")
-        raise TypeError("Error: model description ."+file_to_parse[-4:]+" not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
+        print("\nError: model description .",type(file_to_parse),"not supported")
+        raise TypeError("Error: model description .",type(file_to_parse),"not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = fmin(tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)],{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]);
                 {{/broadcast}}
                 {{/min}}
                 {{#Average}}
                 tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = ({{#broadcast}}{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]{{operator}}{{/broadcast}})/{{prev_size}};
                 {{/Average}}
                 {{#other}}
-                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] ={{#broadcast}}{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]{{operator}}{{/broadcast}};
+                tensor_temp[j + {{output_width}}*(i + {{output_height}}*f)] = {{#broadcast}}{{output_str}}[(j%{{input_width}}) + {{input_width}}*((i%{{input_height}}) + {{input_height}}*(f % {{input_channels}}))]{{operator}}{{/broadcast}}{{#constant}}{{operator}}constant_{{name}}_{{idx}}[(j%{{cst_width}}) + {{cst_width}}*((i%{{cst_height}}) + {{cst_height}}*(f % {{cst_channels}}))]{{/constant}};
                 {{/other}}
             }
         }
     }
     
     for (k = 0; k < {{size}}; ++k)
     {
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files 19% similar despite different names*

```diff
@@ -34,8 +34,12 @@
     {{/patches_size}}
     {{#channels}}
 {{data_type}} mean_{{name}}_{{idx}}[{{channels}}] = {{mean}};
 {{data_type}} var_{{name}}_{{idx}}[{{channels}}] = {{var}};
 {{data_type}} scale_{{name}}_{{idx}}[{{channels}}] = {{scale}};
 
     {{/channels}}
+    {{#constant_size}}
+{{data_type}} constant_{{name}}_{{idx}}[{{constant_size}}] = {{constant}};
+
+    {{/constant_size}}
 {{/layers}}
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,20 @@
     {{#nb_biases}}
 extern {{data_type}} biases_{{name}}_{{idx}}[{{nb_biases}}];
     {{/nb_biases}}
     {{#patches_size}}
 extern {{data_type}} *ppatches_{{name}}_{{idx}}[{{patches_size}}];
     {{/patches_size}}
     {{#channels}}
-{{data_type}} mean_{{name}}_{{idx}}[{{channels}}];
-{{data_type}} var_{{name}}_{{idx}}[{{channels}}];
-{{data_type}} scale_{{name}}_{{idx}}[{{channels}}];
+extern {{data_type}} mean_{{name}}_{{idx}}[{{channels}}];
+extern {{data_type}} var_{{name}}_{{idx}}[{{channels}}];
+extern {{data_type}} scale_{{name}}_{{idx}}[{{channels}}];
     {{/channels}}
+    {{#constant_size}}
+extern {{data_type}} constant_{{name}}_{{idx}}[{{constant_size}}];
+    {{/constant_size}}
     
 {{/layers}}
 int inference({{data_type}} *prediction, {{data_type}} *nn_input);
 
 {{{normalization_cst}}}
 #endif
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.1.dev5/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.1.dev4
+Version: 0.1.dev5
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
```

### Comparing `acetone_nnet-0.1.dev4/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.1.dev5/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/acetone_nnet/cli_compare.py
 src/acetone_nnet.egg-info/PKG-INFO
 src/acetone_nnet.egg-info/SOURCES.txt
 src/acetone_nnet.egg-info/dependency_links.txt
 src/acetone_nnet.egg-info/entry_points.txt
 src/acetone_nnet.egg-info/requires.txt
 src/acetone_nnet.egg-info/top_level.txt
+src/acetone_nnet/bin/bin_acetone.py
 src/acetone_nnet/code_generator/Layer.py
 src/acetone_nnet/code_generator/__init__.py
 src/acetone_nnet/code_generator/activation_functions.py
 src/acetone_nnet/code_generator/neural_network.py
 src/acetone_nnet/code_generator/layers/AddBias.py
 src/acetone_nnet/code_generator/layers/BatchNormalization.py
 src/acetone_nnet/code_generator/layers/Concatenate.py
@@ -56,14 +57,15 @@
 src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
 src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
 src/acetone_nnet/format_importer/parser.py
 src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+src/acetone_nnet/format_importer/H5_importer/parser_h5.py
 src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
 src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
 src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
 src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
 src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
 src/acetone_nnet/graph/graph_interpretor.py
 src/acetone_nnet/templates/__init__.py
```

