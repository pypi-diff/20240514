# Comparing `tmp/tejd_build_tools-1.7.0.dev2-py3-none-any.whl.zip` & `tmp/tejd_build_tools-1.7.0.dev3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 692630 bytes, number of entries: 200
--rw-r--r--  2.0 unx       10 b- defN 24-May-14 19:32 tejd_build_tools/VERSION
--rw-r--r--  2.0 unx       26 b- defN 24-May-14 19:32 tejd_build_tools/__init__.py
--rw-r--r--  2.0 unx     1045 b- defN 24-May-14 19:32 tejd_build_tools/te_version.py
+Zip file size: 651925 bytes, number of entries: 188
+-rw-r--r--  2.0 unx       10 b- defN 24-May-14 19:53 tejd_build_tools/VERSION
+-rw-r--r--  2.0 unx       26 b- defN 24-May-14 19:53 tejd_build_tools/__init__.py
+-rw-r--r--  2.0 unx     1045 b- defN 24-May-14 19:53 tejd_build_tools/te_version.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 19:03 tejd_build_tools/build_tools/__init__.py
 -rw-r--r--  2.0 unx     6242 b- defN 24-May-14 19:32 tejd_build_tools/build_tools/build_ext.py
 -rw-r--r--  2.0 unx     4459 b- defN 24-May-14 19:04 tejd_build_tools/build_tools/utils.py
+-rw-r--r--  2.0 unx     2462 b- defN 24-May-14 19:53 tejd_build_tools/common/util/system.cpp
 -rw-r--r--  2.0 unx     2663 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/.clang-format
 -rw-r--r--  2.0 unx       51 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/.git
 -rw-r--r--  2.0 unx     1965 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/CMakeLists.txt
 -rw-r--r--  2.0 unx     2776 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/CONTRIBUTING.md
 -rw-r--r--  2.0 unx     1148 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/LICENSE.txt
 -rw-r--r--  2.0 unx     8430 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/README.FE.0.x.md
 -rw-r--r--  2.0 unx    12897 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/README.FE.1.0.md
@@ -161,27 +162,14 @@
 -rw-r--r--  2.0 unx     6208 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_instancenorm.py
 -rw-r--r--  2.0 unx     6283 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_layernorm.py
 -rw-r--r--  2.0 unx     8261 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_matmul_bias_relu.py
 -rw-r--r--  2.0 unx    40019 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_mhas.py
 -rw-r--r--  2.0 unx     6363 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_rmsnorm.py
 -rw-r--r--  2.0 unx      445 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_utils.py
 -rw-r--r--  2.0 unx     3282 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/python_fe/test_wgrads.py
--rw-r--r--  2.0 unx     1001 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/conftest.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     3280 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_apply_rope.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     6736 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_batchnorm.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     7277 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_bias.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     3083 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_genstats.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     1939 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_reduction.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     3978 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_instancenorm.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     4093 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_layernorm.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     5472 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_matmul_bias_relu.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx    27856 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_mhas.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     5156 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_rmsnorm.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx      912 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_utils.cpython-310-pytest-8.0.2.pyc
--rw-r--r--  2.0 unx     2793 b- defN 24-May-14 17:32 tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_wgrads.cpython-310-pytest-8.0.2.pyc
 -rw-r--r--  2.0 unx     1410 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/unit_tests/CMakeLists.txt
 -rw-r--r--  2.0 unx    15870 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/unit_tests/serialize.cpp
 -rw-r--r--  2.0 unx     2787 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/unit_tests/validate.cpp
 -rw-r--r--  2.0 unx     1568 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/test/unit_tests/version.cpp
 -rw-r--r--  2.0 unx     4596 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/activation.h
 -rw-r--r--  2.0 unx     1250 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/cast.h
 -rw-r--r--  2.0 unx     1160 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/cast_transpose_noop.h
@@ -190,13 +178,13 @@
 -rw-r--r--  2.0 unx     5094 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/gemm.h
 -rw-r--r--  2.0 unx     8990 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/layer_norm.h
 -rw-r--r--  2.0 unx     5381 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/recipe.h
 -rw-r--r--  2.0 unx     7518 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/rmsnorm.h
 -rw-r--r--  2.0 unx     6281 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/softmax.h
 -rw-r--r--  2.0 unx     9573 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/transformer_engine.h
 -rw-r--r--  2.0 unx    11118 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/transpose.h
--rw-r--r--  2.0 unx    10142 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/LICENSE
--rw-r--r--  2.0 unx      151 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-May-14 19:32 tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    25106 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/RECORD
-200 files, 3843894 bytes uncompressed, 649988 bytes compressed:  83.1%
+-rw-r--r--  2.0 unx    10142 b- defN 24-May-14 19:53 tejd_build_tools-1.7.0.dev3.dist-info/LICENSE
+-rw-r--r--  2.0 unx      151 b- defN 24-May-14 19:53 tejd_build_tools-1.7.0.dev3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 19:53 tejd_build_tools-1.7.0.dev3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-14 19:53 tejd_build_tools-1.7.0.dev3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    23135 b- defN 24-May-14 19:53 tejd_build_tools-1.7.0.dev3.dist-info/RECORD
+188 files, 3770809 bytes uncompressed, 612769 bytes compressed:  83.8%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: tejd_build_tools/build_tools/build_ext.py
 Comment: 
 
 Filename: tejd_build_tools/build_tools/utils.py
 Comment: 
 
+Filename: tejd_build_tools/common/util/system.cpp
+Comment: 
+
 Filename: tejd_build_tools/cudnn-frontend/.clang-format
 Comment: 
 
 Filename: tejd_build_tools/cudnn-frontend/.git
 Comment: 
 
 Filename: tejd_build_tools/cudnn-frontend/CMakeLists.txt
@@ -492,53 +495,14 @@
 
 Filename: tejd_build_tools/cudnn-frontend/test/python_fe/test_utils.py
 Comment: 
 
 Filename: tejd_build_tools/cudnn-frontend/test/python_fe/test_wgrads.py
 Comment: 
 
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/conftest.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_apply_rope.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_batchnorm.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_bias.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_genstats.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_reduction.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_instancenorm.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_layernorm.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_matmul_bias_relu.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_mhas.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_rmsnorm.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_utils.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
-Filename: tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_wgrads.cpython-310-pytest-8.0.2.pyc
-Comment: 
-
 Filename: tejd_build_tools/cudnn-frontend/test/unit_tests/CMakeLists.txt
 Comment: 
 
 Filename: tejd_build_tools/cudnn-frontend/test/unit_tests/serialize.cpp
 Comment: 
 
 Filename: tejd_build_tools/cudnn-frontend/test/unit_tests/validate.cpp
@@ -579,23 +543,23 @@
 
 Filename: tejd_build_tools/include/transformer_engine/transformer_engine.h
 Comment: 
 
 Filename: tejd_build_tools/include/transformer_engine/transpose.h
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev2.dist-info/LICENSE
+Filename: tejd_build_tools-1.7.0.dev3.dist-info/LICENSE
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev2.dist-info/METADATA
+Filename: tejd_build_tools-1.7.0.dev3.dist-info/METADATA
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev2.dist-info/WHEEL
+Filename: tejd_build_tools-1.7.0.dev3.dist-info/WHEEL
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt
+Filename: tejd_build_tools-1.7.0.dev3.dist-info/top_level.txt
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev2.dist-info/RECORD
+Filename: tejd_build_tools-1.7.0.dev3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tejd_build_tools/VERSION

```diff
@@ -1 +1 @@
-1.7.0.dev2
+1.7.0.dev3
```

## tejd_build_tools/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.7.0.dev2'
+__version__ = '1.7.0.dev3'
```

## Comparing `tejd_build_tools-1.7.0.dev2.dist-info/LICENSE` & `tejd_build_tools-1.7.0.dev3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tejd_build_tools-1.7.0.dev2.dist-info/RECORD` & `tejd_build_tools-1.7.0.dev3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-tejd_build_tools/VERSION,sha256=IhqjB9t7pS5aJsCafLq1yKKU-tJalyT43c-oeCQDkec,10
-tejd_build_tools/__init__.py,sha256=tXhz3ylShfo5u4A7IOKPVpPHyDp8yQfD0Jjikck4QCU,26
+tejd_build_tools/VERSION,sha256=iXvP3I-HGvq4QVwDMNrK39rfY8LGGu9eoti6ZZDJQ9s,10
+tejd_build_tools/__init__.py,sha256=2v8hg3BN7mHlTcIdIEESdf-dcejjeuKn1A1Sxv2X9TM,26
 tejd_build_tools/te_version.py,sha256=wzQBnaq0vLKeRsPEpIIqw1AosLYQhjuCR-zsU5cqYL4,1045
 tejd_build_tools/build_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tejd_build_tools/build_tools/build_ext.py,sha256=jbqCUBE66jtZ4pnjmFDu6p2_wdI5G0O4tqr1201ufAs,6242
 tejd_build_tools/build_tools/utils.py,sha256=tdGYs-NvV0_kiq9nDhAgyDCrcmJNBdFAm76bkc8aX40,4459
+tejd_build_tools/common/util/system.cpp,sha256=1LhWYtR59vDc61KJ9LFwqDbz1CPSyGoOX3YYUfsVI7c,2462
 tejd_build_tools/cudnn-frontend/.clang-format,sha256=gQFk79UqPdKJksQIFkWmOuMMJ1j6yQBzNa2lOiWiPb0,2663
 tejd_build_tools/cudnn-frontend/.git,sha256=a9pmDWgoNWr6xXkENhe3yCiiOR3UZ5HHCV2sm34pR0g,51
 tejd_build_tools/cudnn-frontend/CMakeLists.txt,sha256=ucmwfqDv8lCYIZq9gd0Bed1fH8KDucHDnASySA5TcLM,1965
 tejd_build_tools/cudnn-frontend/CONTRIBUTING.md,sha256=F9DxdHSaYHQLJDOFjN7-lXhd8om-ZNmdRxCuEjESQmM,2776
 tejd_build_tools/cudnn-frontend/LICENSE.txt,sha256=P8S0c6LAh2ioBmv35KWKEYUGDzrWdPLKniARvKSt8s4,1148
 tejd_build_tools/cudnn-frontend/README.FE.0.x.md,sha256=WvJb-P21y0dqatBty_GBgurJdsPT6AI5vNXk4ZYCJyk,8430
 tejd_build_tools/cudnn-frontend/README.FE.1.0.md,sha256=vEehZg8c3vp-tGxP6DZAANj607rQlY-r5zBRyfFWgTc,12897
@@ -160,27 +161,14 @@
 tejd_build_tools/cudnn-frontend/test/python_fe/test_instancenorm.py,sha256=4zRRHeg34fBGZkIITBbLNEwHb8wst5HR-oWOMsdGBP4,6208
 tejd_build_tools/cudnn-frontend/test/python_fe/test_layernorm.py,sha256=iotn2Xwho6hqgQojWFQddp7JM9vR6iCx181WmY09j5Q,6283
 tejd_build_tools/cudnn-frontend/test/python_fe/test_matmul_bias_relu.py,sha256=8x4ksHD9S-C2-slhFSspoXCscuZNfvpvRC_XxY3s864,8261
 tejd_build_tools/cudnn-frontend/test/python_fe/test_mhas.py,sha256=4YC24tDXx7fWHEn_3yd4APRVofZLniwOAob1Sq-tH8Y,40019
 tejd_build_tools/cudnn-frontend/test/python_fe/test_rmsnorm.py,sha256=o27SPD8pVrh2G82SqbZYNFYXm6EjFwfpgwlogiWpgrM,6363
 tejd_build_tools/cudnn-frontend/test/python_fe/test_utils.py,sha256=FgrvavR-mqgRuJuW7yqa1R2A5EK1OpWP_Xb8di3Viqc,445
 tejd_build_tools/cudnn-frontend/test/python_fe/test_wgrads.py,sha256=b5hDIvZ_hUX-cA0C9ofY8T-_qUwpAPOFR8kojznqQZc,3282
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/conftest.cpython-310-pytest-8.0.2.pyc,sha256=H1-GGbQ56ScmJY4peAlIUR0fxPxGaJmqFPg7_H_76vc,1001
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_apply_rope.cpython-310-pytest-8.0.2.pyc,sha256=WEdP8V-e16TbGMjIDQpkC5DYvVfJRl_AqneZvNfcLOc,3280
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_batchnorm.cpython-310-pytest-8.0.2.pyc,sha256=Jn0dd_GYWj7F4WwsLjb8tyVWPV1ZTzhVmWtHqUG_hB4,6736
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_bias.cpython-310-pytest-8.0.2.pyc,sha256=BiY23xmmY9R_HzGXHMsd8KuolniRNQUDwNtlvM29cx4,7277
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_genstats.cpython-310-pytest-8.0.2.pyc,sha256=9VFIPYgBV8tPyRL_vcZ2HMHsMWL_dAp79e16psCfM3E,3083
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_conv_reduction.cpython-310-pytest-8.0.2.pyc,sha256=MI0rAJeqiT2uk3Thg-7XP0JAxNul6IR36HfUKVhJILo,1939
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_instancenorm.cpython-310-pytest-8.0.2.pyc,sha256=DofYvTXsxXfAhvFNn16iEYKUDTB8aKpnbEtrCEKSLR8,3978
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_layernorm.cpython-310-pytest-8.0.2.pyc,sha256=LOXcLb_h8dYOpZNEDjyXdCqS7kDr1Nm5_X1vsPEzvQE,4093
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_matmul_bias_relu.cpython-310-pytest-8.0.2.pyc,sha256=UOSe9oU7lZ_RlXHX5UR1c3EhMZ-PsaZ9Mg7GHVgk5mg,5472
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_mhas.cpython-310-pytest-8.0.2.pyc,sha256=flq0XzLYofCXg1agL5yjkzP_tRoPmJFZGAhPTLZ7-ko,27856
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_rmsnorm.cpython-310-pytest-8.0.2.pyc,sha256=zUjvn3SDmAK_qCOMBjuxT9XVVLXsDKnlssxI7s9KuyU,5156
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_utils.cpython-310-pytest-8.0.2.pyc,sha256=HoRKnhyr44tfVSyEIiqQK_ZTKAyO3eCYVulb3ADojbw,912
-tejd_build_tools/cudnn-frontend/test/python_fe/__pycache__/test_wgrads.cpython-310-pytest-8.0.2.pyc,sha256=BMoaHwi0OD9a9Ci3akfsj4SUdzKnsVMD195Am4sFLv8,2793
 tejd_build_tools/cudnn-frontend/test/unit_tests/CMakeLists.txt,sha256=suYhmpxQTTNG0xdv-jniGhWrmU7L66-mKaXPzzEvEVg,1410
 tejd_build_tools/cudnn-frontend/test/unit_tests/serialize.cpp,sha256=hiOakNkma0oiNsEszbLCMeGyi14bg4KACIMqQnDBpOE,15870
 tejd_build_tools/cudnn-frontend/test/unit_tests/validate.cpp,sha256=p_oorRz1KFET2K9zUB8Aol_1Zgtpk7X5UbNxOFMvo5o,2787
 tejd_build_tools/cudnn-frontend/test/unit_tests/version.cpp,sha256=894m1Y_oWb_xVHMHirW2225SVbG6Iql3QqSTzCAOAXo,1568
 tejd_build_tools/include/transformer_engine/activation.h,sha256=JWhwHxrsEr0yhRYfL4c4_Wit8lam_KTPCJMm4f89tZ0,4596
 tejd_build_tools/include/transformer_engine/cast.h,sha256=Wmh4GFWRVWdcUwZoy_188oz_rSgg59rJPBPN0bSn3BE,1250
 tejd_build_tools/include/transformer_engine/cast_transpose_noop.h,sha256=Ygy-dXZbZCmIF54rvgInIRC4QkduvTY-DgBU3nR5s_g,1160
@@ -189,12 +177,12 @@
 tejd_build_tools/include/transformer_engine/gemm.h,sha256=vKSx2r7TLdESDJpm0kLh-R6CCHqRPjcAseHILbdrZ6c,5094
 tejd_build_tools/include/transformer_engine/layer_norm.h,sha256=WlNPs755_SsmI9weEqngZGVjOEj7Cs5P7BiLQLYyY1A,8990
 tejd_build_tools/include/transformer_engine/recipe.h,sha256=tGBMzSwJBd8VUrvVdK7YJBPc26GsmnWT3SChrR9EdAc,5381
 tejd_build_tools/include/transformer_engine/rmsnorm.h,sha256=NcjI4zBnADzC3tw_ZwM5SCLIRsUf8hksfpbvPAhsX4I,7518
 tejd_build_tools/include/transformer_engine/softmax.h,sha256=MSBcmUmWOTD9Nt-T7cEl6pxVmSyS7zskXpW8nCOlTxo,6281
 tejd_build_tools/include/transformer_engine/transformer_engine.h,sha256=u89GUQnqAg1C_KzFtcDS0f-uKA_vuaepZcVW8B7rICE,9573
 tejd_build_tools/include/transformer_engine/transpose.h,sha256=vzGwzqHj1WaKyX5GFA6IAPwycVb3CCotG1FUksnMDoU,11118
-tejd_build_tools-1.7.0.dev2.dist-info/LICENSE,sha256=vqG0Jm8UmfpLuxbW51d-a1tT0e8BCDWp1GCHYCLMhyI,10142
-tejd_build_tools-1.7.0.dev2.dist-info/METADATA,sha256=Uz1iLFbBeEB7sK4yAj56eSCIvnjUM5cCZwJ5CWuwtVU,151
-tejd_build_tools-1.7.0.dev2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt,sha256=KPLvv8ekYraJSt7QjK0ByGJElFL3k4YpDq7p0K0H6y0,17
-tejd_build_tools-1.7.0.dev2.dist-info/RECORD,,
+tejd_build_tools-1.7.0.dev3.dist-info/LICENSE,sha256=vqG0Jm8UmfpLuxbW51d-a1tT0e8BCDWp1GCHYCLMhyI,10142
+tejd_build_tools-1.7.0.dev3.dist-info/METADATA,sha256=etkGB6K52o8xJbEMUnRMlSUeghrAuKr3eA-dRXo2KFM,151
+tejd_build_tools-1.7.0.dev3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+tejd_build_tools-1.7.0.dev3.dist-info/top_level.txt,sha256=KPLvv8ekYraJSt7QjK0ByGJElFL3k4YpDq7p0K0H6y0,17
+tejd_build_tools-1.7.0.dev3.dist-info/RECORD,,
```

