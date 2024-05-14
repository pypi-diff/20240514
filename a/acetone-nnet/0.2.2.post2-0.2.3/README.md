# Comparing `tmp/acetone_nnet-0.2.2.post2.tar.gz` & `tmp/acetone_nnet-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.2.post2.tar", last modified: Mon May 13 07:06:56 2024, max compression
+gzip compressed data, was "acetone_nnet-0.2.3.tar", last modified: Tue May 14 08:11:16 2024, max compression
```

## Comparing `acetone_nnet-0.2.2.post2.tar` & `acetone_nnet-0.2.3.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.278494 acetone_nnet-0.2.2.post2/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.2.post2/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.2.post2/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.2.post2/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7888 2024-05-13 07:06:56.278494 acetone_nnet-0.2.2.post2/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6497 2024-04-19 14:35:17.000000 acetone_nnet-0.2.2.post2/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2067 2024-05-13 07:06:44.000000 acetone_nnet-0.2.2.post2/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-13 07:06:56.278494 acetone_nnet-0.2.2.post2/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.253494 acetone_nnet-0.2.2.post2/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.257494 acetone_nnet-0.2.2.post2/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.259494 acetone_nnet-0.2.2.post2/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.260494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-26 12:50:09.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4742 2024-05-06 12:16:27.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.262494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3217 2024-05-06 13:03:06.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.263494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.264494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8205 2024-05-13 07:02:54.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.265494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.266494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.267494 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10588 2024-05-06 08:24:39.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6667 2024-05-06 08:24:16.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6085 2024-05-13 06:58:55.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5128 2024-05-06 08:24:06.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.267494 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.267494 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    19049 2024-04-26 09:35:35.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.268494 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    15073 2024-04-25 13:20:44.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.268494 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5954 2024-05-06 13:02:03.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.268494 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    30096 2024-05-13 07:05:00.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4361 2024-04-25 09:51:05.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2976 2024-04-24 07:19:46.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.269494 acetone_nnet-0.2.2.post2/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.270494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.272494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.274494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.275494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.275494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.276494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.276494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.277494 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1244 2024-05-06 08:26:40.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-13 07:06:56.277494 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7888 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-13 07:06:56.000000 acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.3/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.3/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6679 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5294 2024-05-14 06:41:04.000000 acetone_nnet-0.2.3/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2065 2024-05-14 08:10:46.000000 acetone_nnet-0.2.3/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-05-14 08:11:16.626575 acetone_nnet-0.2.3/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.586562 acetone_nnet-0.2.3/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.696564 acetone_nnet-0.2.3/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1801 2024-05-13 12:52:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.715564 acetone_nnet-0.2.3/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.3/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.751564 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-05-13 12:08:36.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4742 2024-05-06 12:16:27.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:15.926566 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3217 2024-05-06 13:03:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.064568 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.089568 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-05-13 09:26:47.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8205 2024-05-13 07:02:54.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.144569 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3207 2024-05-13 13:41:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3632 2024-05-13 13:41:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3669 2024-05-13 13:41:04.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3929 2024-05-13 13:41:00.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.163570 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.209570 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10588 2024-05-06 08:24:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6667 2024-05-06 08:24:16.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6085 2024-05-13 06:58:55.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5128 2024-05-06 08:24:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25546 2024-05-14 07:43:39.000000 acetone_nnet-0.2.3/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.210570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.210570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18466 2024-05-14 07:01:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.226570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14538 2024-05-14 06:56:48.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.233570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3871 2024-05-13 14:43:41.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5370 2024-05-14 07:02:59.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.234570 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    30296 2024-05-14 07:20:12.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4461 2024-05-13 14:13:26.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2907 2024-05-13 13:34:22.000000 acetone_nnet-0.2.3/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.250571 acetone_nnet-0.2.3/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.372572 acetone_nnet-0.2.3/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.488573 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.525574 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-05-13 08:47:00.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-05-13 08:46:52.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-05-13 08:46:45.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-05-13 08:47:06.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.566574 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-05-13 08:47:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-05-13 08:47:14.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-05-13 13:12:23.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-05-13 08:47:28.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.568575 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.597575 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1768 2024-05-03 11:58:23.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6868 2024-05-06 08:26:35.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1689 2024-05-02 13:54:50.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-05-13 09:26:54.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.610575 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.621575 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1244 2024-05-06 08:26:40.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.3/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-05-14 08:11:16.625575 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6679 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6926 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-05-14 08:11:15.000000 acetone_nnet-0.2.3/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2.2.post2/AUTHORS.md` & `acetone_nnet-0.2.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/COPYING` & `acetone_nnet-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/LICENSE` & `acetone_nnet-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/README.md` & `acetone_nnet-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: acetone-nnet
+Version: 0.2.3
+Summary: Predictable programming framework for ML applications in safety-critical systems.
+Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
+Project-URL: Repository, https://github.com/onera/acetone/
+Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: C
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Embedded Systems
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: <3.12,>=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: COPYING
+License-File: AUTHORS.md
+Requires-Dist: numpy==1.23.5
+Requires-Dist: numpyencoder==0.3.0
+Requires-Dist: onnx==1.14.0
+Requires-Dist: tensorflow==2.12.0
+Requires-Dist: pystache==0.6.5
+
 # ACETONE
 Predictable programming framework for ML applications in safety-critical systems.
 
 This repo contains the code of the framework presented in the ECRTS'22 paper  ["ACETONE: Predictable programming framework for ML applications in safety-critical systems"](https://drops.dagstuhl.de/entities/document/10.4230/LIPIcs.ECRTS.2022.3).
 
 This framework generate a C code corresponding to a neural network given as input.
 
@@ -130,55 +157,14 @@
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 acetone_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
-As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
-
-* The neural network is Sequential and Feedforward
-
-* The neural-network is describeb in one of the following formats:
-  * JSON (specifique decription made for the framework. Confer to the file [JSON_from_keras_model.py](./src/format_importer/H5_importer/JSON_from_keras_model.py))
-  * NNET 
-  * ONNX
-  * H5 (by transforming into a JSON file)
-
-* Its layers are amongst the following (both Keras and Onnx layers):
-  * Dense
-  * Convolutional (Conv2D) (3 option for the algorithm)
-  * Pooling (AveragePooling2D, MaxPooling2D)
-  * Flatten
-  * Normalization (Normalization layers of Keras)
-  * Dropout (Dropout layers of Keras)
-  * Reshape
-  * Permute
-  * MatMul
-  * Gemm
-  * Gather
-  * Dot
-  * Concatenate
-  * Clip
-  * Add (where one of the inputs is an ONNX initializer)
-  * Resize (Cubic interpolation, Linear interpolation, Nearest)
-  * Pad (Wrap padding, Edge padding, Reflect padding, Constant padding)
-  * Broadcast (Add, Average, Divide, Maximum, Minimum, Multiply, Subtract)
-  * Unsqueeze (ONNX layer)
-  * LRN (ONNX layer)
-  * Shape (ONNX layer)
-  * BatchNormalization (ONNX layer)
-
-* Its activation layers are amongst the following:
-  * Linear
-  * Tanh
-  * ReLu
-  * Sigmoid
-  * Softmax
-  * Exp
-  * Log
+Please refer to the [`implemented.md`](./implemented.md) file to see the current capabilities of the framework.
 
 ## License
 
 The project is under the GNU Lesser General Public License as published by the Free Software Foundation ; either version 3 of  the License or (at your option) any later version.
 
-See LICENSE for details.
+See LICENSE for details.
```

### Comparing `acetone_nnet-0.2.2.post2/pyproject.toml` & `acetone_nnet-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2.2-2"
+version = "0.2.3"
 requires-python = ">=3.10, <3.12"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     CodeGenerator, Layer,
     Add_Bias, Concatenate, Dense, Dot, Flatten, Gather, Gemm, InputLayer, MatMul, Softmax, BatchNormalization,
     Add, Average, Broadcast, Divide, Maximum, Minimum, Multiply, Subtract,
     Conv2D, Conv2D_6loops, Conv2D_gemm, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pad, Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Pooling2D, MaxPooling2D, AveragePooling2D,
     Resize, ResizeCubic, ResizeLinear, ResizeNearest,
-    ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip
+    ActivationFunctions, Linear, Sigmoid, ReLu, TanH, Exponential, Logarithm, Clip, LeakyReLu
 )
 
 from .cli_acetone import cli_acetone
 from .cli_compare import cli_compare
 
 __all__ = (
     "cli_acetone", "cli_compare",
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.2.3/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.2.3/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.2.3/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/Layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,20 +68,20 @@
                 else:
                     pad_along_height = max(filter_height - (in_height % strides), 0)
                 if (in_width % strides == 0):
                     pad_along_width = max(filter_width - strides, 0)
                 else:
                     pad_along_width = max(filter_width - (in_width % strides), 0)
                 
-                if((padding == 'SAME_LOWER') or (padding == 'same')):
+                if((padding == 'SAME_UPPER') or (padding == 'same')):
                     pad_top = pad_along_height // 2
                     pad_bottom = pad_along_height - pad_top
                     pad_left = pad_along_width // 2
                     pad_right = pad_along_width - pad_left
-                elif(padding == 'SAME_UPPER'):
+                elif(padding == 'SAME_LOWER'):
                     pad_bottom = pad_along_height // 2
                     pad_top = pad_along_height - pad_bottom
                     pad_right = pad_along_width // 2
                     pad_left = pad_along_width - pad_right        
         else:
             pad_right, pad_left, pad_bottom, pad_top = padding[3], padding[1], padding[2], padding[0]
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 import pystache
 
 #The Constant mode of the Pad layers
 #Use a constant to fill paddings
 class Constant_Pad(Pad):
     
-    def __init__(self, idx, size, pads, constant_value, axes,input_shape,activation_function):
-        super().__init__(idx, size, pads, constant_value, axes,input_shape,activation_function)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.mode = 'constant'
     
     def generate_inference_code_layer(self):
 
         output_str = self.previous_layer[0].output_str
 
         mustach_hash = {}
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,38 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
+
 from .Pad import Pad
 
 import pystache
 
-#The Edge mode of the Pad layers
-#Pads with the edge values of array.
-class Edge_pad(Pad):
+#The Reflect mode of the Pad layers
+#Pads with the reflection of the vector mirrored on the first and last values of the vector along each axis.
+class Reflect_pad(Pad):
+    
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'reflect'
     
-    def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
-        super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
-        self.mode = 'edge'
-
-
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
-        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
-        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
-        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
-
-        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
+        mustach_hash['channels_max'] = self.input_shape[1] - 1
+        mustach_hash['height_max'] = self.input_shape[2] - 1
+        mustach_hash['width_max'] = self.input_shape[3] - 1
+        
+        with open(self.template_path+'layers/Pad/template_Reflect_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,38 +13,37 @@
  * without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
  * See the GNU Lesser General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
-
 from .Pad import Pad
 
 import pystache
 
-#The Reflect mode of the Pad layers
-#Pads with the reflection of the vector mirrored on the first and last values of the vector along each axis.
-class Reflect_pad(Pad):
-    
-    def __init__(self, idx, size, pads, constant_value, axes, input_shape,activation_function):
-        super().__init__(idx, size, pads, constant_value, axes, input_shape,activation_function)
-        self.mode = 'reflect'
+#The Edge mode of the Pad layers
+#Pads with the edge values of array.
+class Edge_pad(Pad):
     
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.mode = 'edge'
+
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
         mustach_hash['pads_left'] = self.pads[3]
-        mustach_hash['channels_max'] = self.input_shape[1] - 1
-        mustach_hash['height_max'] = self.input_shape[2] - 1
-        mustach_hash['width_max'] = self.input_shape[3] - 1
-        
-        with open(self.template_path+'layers/Pad/template_Reflect_Pad.c.tpl','r') as template_file:
+        mustach_hash['channels_and_pad_front'] = self.input_shape[1] + self.pads[1]
+        mustach_hash['height_and_pad_top'] = self.input_shape[2] + self.pads[2]
+        mustach_hash['width_and_pad_left'] = self.input_shape[3] + self.pads[3]
+
+        with open(self.template_path+'layers/Pad/template_Edge_Pad.c.tpl','r') as template_file:
             template = template_file.read()
         template_file.close()
 
         return pystache.render(template, mustach_hash)
     
 
     def generate_inference_code_layer(self):
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 import pystache
 
 #The Wrap mode of the Pad layers
 #Pads with the wrap of the vector along the axis. 
 #The first values are used to pad the end and the end values are used to pad the beginning.
 class Wrap_pad(Pad):
     
-    def __init__(self, idx, size, mode, pads, constant_value, axes, input_shape):
-        super().__init__(idx, size, mode, pads, constant_value, axes, input_shape)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
         self.mode = 'wrap'
     
     def write_padding(self):
         mustach_hash = {}
 
         mustach_hash['pads_front'] = self.pads[1]
         mustach_hash['pads_top'] = self.pads[2]
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.2.3/src/acetone_nnet/code_generator/neural_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ResizeLinear, ResizeCubic, ResizeNearest, 
     Conv2D, Conv2D_6loops, Conv2D_indirect_gemm, Conv2D_std_gemm,
     Pooling2D, MaxPooling2D, AveragePooling2D
 )
 
 class CodeGenerator(ABC):
 
-    def __init__(self, file, test_dataset_file = None, function_name = 'inference', nb_tests = None, conv_algorithm = 'conv_gemm_optim', normalize = False,**kwargs):
+    def __init__(self, file, test_dataset_file = None, function_name = 'inference', nb_tests = None, conv_algorithm = 'conv_gemm_optim', normalize = False, debug_mode = False, debug_target = [],**kwargs):
 
         self.file = file
         self.test_dataset_file = test_dataset_file
         self.function_name = function_name
         self.nb_tests = nb_tests
         self.conv_algorithm = conv_algorithm
         self.normalize = normalize
@@ -63,20 +63,22 @@
         if test_dataset_file:
             ds = self.load_test_dataset()
             self.test_dataset = ds
         else:
             print("creating random dataset")
             ds = self.create_test_dataset()
             self.test_dataset = ds
-            
+        
+        self.debug_mode = debug_mode
+        self.debug_target = debug_target
 
         self.files_to_gen = ['inference.c', 'inference.h', 'global_vars.c', 'main.c', 'Makefile', 'test_dataset.h', 'test_dataset.c']
         
     def create_test_dataset(self):
-        test_dataset = np.float32(np.random.default_rng(seed=10).random((int(self.nb_tests),1,int(self.layers[0].size))))
+        test_dataset = self.data_type_py(np.random.default_rng(seed=10).random((int(self.nb_tests),1,int(self.layers[0].size))))
         return test_dataset 
      
     def load_test_dataset(self):
         
         test_dataset = []
         try:
             with open(self.test_dataset_file, 'r') as f:
@@ -99,14 +101,17 @@
         
         return test_dataset
 
     def compute_inference(self, c_files_directory):
         with open(os.path.join(c_files_directory, 'output_python.txt'), 'w+') as fi:
             for nn_input in self.test_dataset:
 
+                if self.debug_mode:
+                    debug_output = []
+
                 if((self.data_format == 'channels_last') and (len(self.layers[0].input_shape) == 4)): 
                     shape = (self.layers[0].input_shape[2],self.layers[0].input_shape[3],self.layers[0].input_shape[1])
                     nn_input = np.transpose(np.reshape(nn_input, shape), (2,0,1))
 
                 if (self.normalize): nn_input = self.Normalizer.pre_processing(nn_input)
                 previous_layer_result = [nn_input for i in range(self.maxpath)]  # for the very first layer, it is the neural network input
                 
@@ -150,14 +155,18 @@
                     
                     if (len(layer.next_layer) > 1): #if the layer has more than one child, it needs to be stored
                         to_store[layer.idx] = previous_layer_result[layer.path]
                         
                     for prev in layer.previous_layer:
                         if ((prev.sorted == len(prev.next_layer)) and (prev in to_store)):#if all the children of the parent layer are "taken care of", we "forget" the parent's value ( *2 because of the creation of the dict in graph.to_save)
                             to_store.pop(prev.idx)
+                    
+                    if self.debug_mode:
+                        if layer.idx in self.debug_target or self.debug_target == []:
+                            debug_output.append(previous_layer_result[layer.path].flatten())
                             
                 nn_output = previous_layer_result[layer.path]
                 # print(nn_output) # write to file instead
                 
                 # Write results in text files to compare prediction.
                 if((self.data_format == 'channels_last') and hasattr(layer, 'output_channels')): nn_output = np.transpose(nn_output, (1,2,0))
                 nn_output = np.reshape(nn_output, -1)
@@ -170,15 +179,18 @@
                     # print(decimal.Decimal(nn_output[j]), end=' ', file=fi, flush=True)
                 print(" ",file=fi)
         
         fi.close()
 
         print("File output_python.txt generated.")
 
-        return nn_output
+        if self.debug_mode:
+            return nn_output, debug_output
+        else:
+            return nn_output
 
     def flatten_array_orderc(self, array):
     
         flattened_aray = array.flatten(order='C')
         s = '\n        {'
         for i in range(flattened_aray.size):
             s += str(flattened_aray[i])+', '
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,22 +273,14 @@
             current_layer = Concatenate(idx = idx,
                                         size = get_layer_size(layer_keras),
                                         axis = axis,
                                         input_shapes = get_input_dimensions(layer_keras.input_shape, data_format),
                                         output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
                                         activation_function = Linear())
         
-        elif layer_keras.__class__.__name__ == 'Dot':
-            current_layer = Dot(idx = idx,
-                                size = get_layer_size(layer_keras),
-                                axis = layer_keras.axes,
-                                input_shapes = get_input_dimensions(layer_keras.input_shape, data_format),
-                                output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
-                                activation_function = Linear())
-        
         elif layer_keras.__class__.__name__ == 'ZeroPadding2D':
             pads = layer_keras.padding
             if type(pads) == int:
                 pad_top, pad_bottom = pads, pads
                 pad_left, pad_right = pads, pads
             elif type(pads[0]) == int:
                 pad_top, pad_bottom = pads[0], pads[0]
@@ -337,18 +329,15 @@
                                                    activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'Reshape':
             continue
 
         elif layer_keras.__class__.__name__ == 'Dropout':
             continue
-
-        elif layer_keras.__class__.__name__ == 'Permute':
-            continue
-
+        
         else:
             raise TypeError("Error: layer "+layer_keras.__class__.__name__+" not supported\n")
 
         if type(model) == keras.Sequential:
             if idx - 1 >= 0:
                 current_layer.previous_layer.append(layers[idx-1])
                 layers[idx-1].next_layer.append(current_layer)
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,22 +208,14 @@
         
         elif layer['class_name'] == 'Average':
             current_layer = Average(idx = layer['config']['idx'], 
                                         size = layer['config']['size'], 
                                         input_shapes = layer['config']['input_shape'], 
                                         output_shape = layer['config']['output_shape'],
                                         activation_function= Linear())
-        
-        elif layer['class_name'] == 'Dot':
-            current_layer = Dot(idx = layer['config']['idx'],
-                                size = layer['config']['size'],
-                                axis= layer['config']['axes'],
-                                input_shapes = layer['config']['input_shape'], 
-                                output_shape = layer['config']['output_shape'],
-                                activation_function = Linear())
 
         elif layer['class_name'] == 'ZeroPadding2D':
             pads = layer['config']['padding']
             if(type(pads) == int):
                 pads = [pads for i in range(8)]
             else:
                 if(type(pads[0]) == int):
@@ -280,17 +272,14 @@
 
         elif  'Dropout' in layer['class_name']:
             continue
 
         elif  layer['class_name'] == 'Reshape':
             continue
 
-        elif  layer['class_name'] == 'Permute':
-            continue
-
         else:
             raise TypeError("Error: layer"+layer['class_name']+" not supported\n")
         
         for i in layer['config']['prev_layer_idx']:
             current_layer.previous_layer.append(layers[i])
             layers[i].next_layer.append(current_layer)
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,14 @@
         template_file.close()
 
         return  pystache.render(template, mustach_hash)
 
     def pre_processing(self, nn_input):
         inputs = nn_input.flatten()
         for i in range(self.input_size):
-            inputs[i] = (max(self.mins[i],min(self.maxes[i],nn_input[i])) - self.means[i]) / self.ranges[i]
+            inputs[i] = (max(self.mins[i],min(self.maxes[i],inputs[i])) - self.means[i]) / self.ranges[i]
         return np.reshape(inputs, nn_input.shape)
 
     def post_processing(self, nn_output):
         for i in range(len(nn_output)):
             nn_output[i] = nn_output[i]*self.ranges[-1] + self.means[-1]
         return nn_output
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,39 +28,33 @@
 from ...code_generator.activation_functions import Linear, ReLu
 
 keras.backend.set_floatx('float32')
 
 
 def load_nnet(file_to_parse, normalize):
     """
-    Reads nnet networks from ACAS project and to pull it in .h5 format
-    Inspired from : # https://github.com/NeuralNetworkVerification/Marabou/blob/master/maraboupy/MarabouNetworkNNet.py  read function
-    Args:
-        model_file_net (.nnet): file describing the neural network
-    Returns: 
-        model (.h5): Keras model
+    Inspired from : # https://github.com/NeuralNetworkVerification/Marabou/blob/master/maraboupy/MarabouNetworkNNet.py
     """
 
     #Recall : Example of nnet file head:
     #7,5,5,50,  numLayers, inputSize, outputSize, maxLayersize
     #5,50,50,50,50,50,50,5,    Layersizes
     #0
     #Inputs Values Min
     #Inputs Values Max
     #Moyennes de normalisation
     #ranges de normalisation 
     #weights
     #biaises
 
     layers = []
-    listRoad = [0,1]
     maxRoad = 1
     dict_cst = {}
-    data_type = 'float'
-    data_type_py = 'float32'
+    data_type = float
+    data_type_py = np.float32
 
     with open(file_to_parse) as f:
      
         line = f.readline()
 
         while line[0:2] == "//": # ignore header lines with credits
             line = f.readline() 
@@ -91,22 +85,14 @@
         biases = []
 
         for layernum in range(numLayers):
             previousLayerSize = layerSizes[layernum]
             currentLayerSize = layerSizes[layernum + 1]
             weights.append([])
             biases.append([])
-            
-            # weights
-            # for i in range(previousLayerSize):
-            #     line = f.readline()
-            #     aux = [float(x) for x in line.strip().split(",")[:-1]]
-            #     weights[layernum].append([])
-            #     for j in range(currentLayerSize):
-            #         weights[layernum][i].append(aux[j])
 
             # weights for non conventional nnet
             for i in range(currentLayerSize):
                 line = f.readline()
                 aux = [float(x) for x in line.strip().split(",")[:-1]]
                 weights[layernum].append([])
                 for j in range(previousLayerSize):
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,16 +396,18 @@
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = node.input
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = [1]
-    if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
+    if (('auto_pad' not in attributs) or ( attributs['auto_pad'].decode() == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
+    else:
+        attributs['auto_pad'] = attributs['auto_pad'].decode()
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
     return MaxPooling2D(idx = idx,
                         size = size,
                         padding =attributs['auto_pad'],
                         strides = attributs['strides'][0],
                         pool_size = attributs['kernel_shape'][0],
@@ -419,16 +421,18 @@
     output_shape = get_shape(node.output[0],model)
     size = find_size(output_shape)
     dict_input[idx] = [node.input[0]]
     dict_output[node.output[0]] = idx
     attributs = extract_attribut(node)
     if ('dilations' not in attributs):
         attributs['dilations'] = [1]
-    if (('auto_pad' not in attributs) or ( attributs['auto_pad'] == 'NOTSET')):
+    if (('auto_pad' not in attributs) or ( attributs['auto_pad'].decode() == 'NOTSET')):
         attributs['auto_pad'] = attributs['pads']
+    else:
+        attributs['auto_pad'] = attributs['auto_pad'].decode()
     if ('strides' not in attributs):
         attributs['strides'] = [1,1]
     return AveragePooling2D(idx=idx,
                             size=size, 
                             padding=attributs['auto_pad'],
                             strides=attributs['strides'][0], 
                             pool_size=attributs['kernel_shape'][0], 
@@ -670,15 +674,16 @@
 
 ###### Dict of all the functions ######
 unused_layers = {"Dropout":bypass,
                   "Constant":create_initializer,
                   "Unsqueeze":bypass,
                   "Reshape":bypass,
                   "LRN":bypass,
-                  "Shape":bypass}
+                  "Shape":bypass,
+                  "Flatten":bypass}
 
 ###### Function to fuse to ONNX layers ######
 
 #Fuse the activation layer ReLu with the prior layer
 def fuse_ReLu(node,dict_output,model,layers):
     layers[dict_output[node.input[0]]].activation_function = ReLu()
     bypass(node,dict_output,model)
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,23 @@
             parent.next_layer.append(layer)
             
     
     data_type_py = onnx.helper.tensor_dtype_to_np_dtype(model.graph.input[0].type.tensor_type.elem_type)
     
     if data_type_py == 'float64':
         data_type = 'double'
+        data_type_py = np.float64
 
     elif data_type_py == 'float32':
         data_type = 'float'
+        data_type_py = np.float32
 
     elif data_type_py == 'int':
         data_type = 'long int'
+        data_type_py = np.int32
     
     #Sorting the graph and adding the road to the layers
     layers, listRoad, maxRoad, dict_cst = tri_topo(layers)
     layers = list(map(lambda x:x.find_output_str(dict_cst), layers))
     data_format = 'channels_first'
     
     print("Finished model initialization.")
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.2.3/src/acetone_nnet/format_importer/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from keras.engine.functional import Functional
 from keras.engine.sequential import Sequential
 import onnx
 
 from .JSON_importer.parser_JSON import load_json
 from .ONNX_importer.parser_ONNX import load_onnx
 from .NNET_importer.parser_NNET import load_nnet
-from .H5_importer.JSON_from_keras_model import JSON_from_keras_model
 from .H5_importer.parser_h5 import load_keras
 
 def get_path(file, new_type):
     new_path = ""
     list_path = file.split("/")
     file_name = list_path[-1].split(".")[0]
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.2.3/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
     // gemm_nn
-    for (i = 0; i < {{m}}; i++)
+    for (i = 0; i < {{m}}; ++i)
     {
         for (p = 0; p < {{k}}; ++p)
         {
             register float weight = {{A}}[i*{{ldA}}+p];
             for(j = 0; j < {{n}}; ++j)
             {
                 tensor_temp[i*{{ldC}} + j] += weight * {{#direct}}*{{/direct}}({{B}}[p*{{ldB}} + j]);
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
     // gemm_nt
-    for (i = 0; i < {{m}}; i++)
+    for (i = 0; i < {{m}}; ++i)
     {
         for (j = 0; j < {{n}}; ++j)
         {
             register float output =0;
             for (p = 0; p < {{k}}; ++p)
             {
                 output += {{A}}[i*{{ldA}}+p]* {{#direct}}*{{/direct}}({{B}}[j*{{ldB}}+p]);
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
     // gemm_tn
-    for (i = 0; i < {{m}}; i++)
+    for (i = 0; i < {{m}}; ++i)
     {
         for (p = 0; p < {{k}}; ++p)
         {
             float register weight = {{A}}[p*{{ldA}}+i];
             for (j = 0; j < {{n}}; ++j)
             {
                 tensor_temp[i*{{ldC}}+j] += weight * {{#direct}}*{{/direct}}({{B}}[p*{{ldB}}+j]);
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-    // gemm_tt
-    for (i = 0; i < {{m}}; i++)
+    // gemm_nt
+    for (i = 0; i < {{m}}; ++i)
     {
         for (j = 0; j < {{n}}; ++j)
         {
-            float register sum = 0;
+            register float output =0;
             for (p = 0; p < {{k}}; ++p)
             {
-                sum += {{A}}[p*{{ldA}} +i]* {{#direct}}*{{/direct}}({{B}}[j*{{ldB}}+p]);
+                output += {{#alpha}}{{.}}{{/alpha}} * {{A}}[p*{{m}}+i] * ({{B}}[j*{{k}}+p]);
             }
-            sum += biases_{{name}}_{{idx}}[i];
+            output += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
-            tensor_temp[i*{{ldC}}+j] = {{{activation_function}}};
+            tensor_temp[j*{{m}}+i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
-            sum = {{{activation_function}}};
+            output = {{{activation_function}}};
             {{/linear}}
-            tensor_temp[i*{{ldC}}+j] = {{{fused_layer}}};
-        {{/fused_layer}}            
+            tensor_temp[j*{{m}}+i] = {{{fused_layer}}};
+        {{/fused_layer}}
         }
     }
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
         // gemm_nn
-    for (i = 0; i < {{m}}; i++)
+    for (i = 0; i < {{m}}; ++i)
     {
         for (p = 0; p < {{k}}; ++p)
         {
             register float weight = {{#alpha}}{{.}} * {{/alpha}}{{A}}[i*{{k}}+p];
             for(j = 0; j < {{n}}; ++j)
             {
                 tensor_temp[j*{{m}} + i] += weight * ({{B}}[j*{{k}} + p]);
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-    // gemm_nt
-    for (i = 0; i < {{m}}; i++)
+    // gemm_tt
+    for (i = 0; i < {{m}}; ++i)
     {
         for (j = 0; j < {{n}}; ++j)
         {
-            register float output =0;
+            float register sum = 0;
             for (p = 0; p < {{k}}; ++p)
             {
-                output += {{#alpha}}{{.}}{{/alpha}} * {{A}}[p*{{m}}+i] * ({{B}}[j*{{k}}+p]);
+                sum += {{#alpha}}{{.}}{{/alpha}} * {{A}}[p*{{m}} +i]* {{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
             }
-            output += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
+            sum += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
-            tensor_temp[j*{{m}}+i] = {{{activation_function}}};
+            tensor_temp[j*{{n}}+i] = {{{activation_function}}};
         {{/fused_layer}}
         {{#fused_layer}}
             {{^linear}}
-            output = {{{activation_function}}};
+            sum = {{{activation_function}}};
             {{/linear}}
-            tensor_temp[j*{{m}}+i] = {{{fused_layer}}};
-        {{/fused_layer}}
+            tensor_temp[j*{{n}}+i] = {{{fused_layer}}};
+        {{/fused_layer}}            
         }
     }
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
     // gemm_tn
     for (i = 0; i < {{m}}; i++)
     {
         for(j = 0; j < {{n}}; ++j)
         {
             float register output = 0;
-            for (p = 0; p < {{k}}; ++j)
+            for (p = 0; p < {{k}}; ++p)
             {
                 output += {{#alpha}}{{.}}{{/alpha}} * {{A}}[i*{{k}}+p] * {{#direct}}*{{/direct}}({{B}}[p*{{n}}+j]);
             }   
             output += {{#beta}}{{.}}{{/beta}} * biases_{{name}}_{{idx}}[i];
         {{^fused_layer}}
             tensor_temp[j*{{m}} + i] = {{{activation_function}}};
         {{/fused_layer}}
```

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.2.3/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2.2.post2/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.2.3/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -56,16 +56,16 @@
 src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
 src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
 src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
 src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
 src/acetone_nnet/format_importer/parser.py
-src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
 src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+src/acetone_nnet/format_importer/JSON_importer/JSON_from_keras_model.py
 src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
 src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
 src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
 src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
 src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
 src/acetone_nnet/graph/graph_interpretor.py
 src/acetone_nnet/templates/__init__.py
```

