# Comparing `tmp/tejd_build_tools-1.7.0.dev1-py3-none-any.whl.zip` & `tmp/tejd_build_tools-1.7.0.dev2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 692639 bytes, number of entries: 200
--rw-r--r--  2.0 unx       10 b- defN 24-May-14 19:24 tejd_build_tools/VERSION
--rw-r--r--  2.0 unx       26 b- defN 24-May-14 19:24 tejd_build_tools/__init__.py
--rw-r--r--  2.0 unx     1045 b- defN 24-May-14 19:24 tejd_build_tools/te_version.py
+Zip file size: 692630 bytes, number of entries: 200
+-rw-r--r--  2.0 unx       10 b- defN 24-May-14 19:32 tejd_build_tools/VERSION
+-rw-r--r--  2.0 unx       26 b- defN 24-May-14 19:32 tejd_build_tools/__init__.py
+-rw-r--r--  2.0 unx     1045 b- defN 24-May-14 19:32 tejd_build_tools/te_version.py
 -rw-r--r--  2.0 unx        0 b- defN 24-May-14 19:03 tejd_build_tools/build_tools/__init__.py
--rw-r--r--  2.0 unx     6272 b- defN 24-May-14 19:03 tejd_build_tools/build_tools/build_ext.py
+-rw-r--r--  2.0 unx     6242 b- defN 24-May-14 19:32 tejd_build_tools/build_tools/build_ext.py
 -rw-r--r--  2.0 unx     4459 b- defN 24-May-14 19:04 tejd_build_tools/build_tools/utils.py
 -rw-r--r--  2.0 unx     2663 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/.clang-format
 -rw-r--r--  2.0 unx       51 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/.git
 -rw-r--r--  2.0 unx     1965 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/CMakeLists.txt
 -rw-r--r--  2.0 unx     2776 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/CONTRIBUTING.md
 -rw-r--r--  2.0 unx     1148 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/LICENSE.txt
 -rw-r--r--  2.0 unx     8430 b- defN 24-May-14 17:08 tejd_build_tools/cudnn-frontend/README.FE.0.x.md
@@ -190,13 +190,13 @@
 -rw-r--r--  2.0 unx     5094 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/gemm.h
 -rw-r--r--  2.0 unx     8990 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/layer_norm.h
 -rw-r--r--  2.0 unx     5381 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/recipe.h
 -rw-r--r--  2.0 unx     7518 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/rmsnorm.h
 -rw-r--r--  2.0 unx     6281 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/softmax.h
 -rw-r--r--  2.0 unx     9573 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/transformer_engine.h
 -rw-r--r--  2.0 unx    11118 b- defN 24-May-14 16:53 tejd_build_tools/include/transformer_engine/transpose.h
--rw-r--r--  2.0 unx    10142 b- defN 24-May-14 19:24 tejd_build_tools-1.7.0.dev1.dist-info/LICENSE
--rw-r--r--  2.0 unx      151 b- defN 24-May-14 19:24 tejd_build_tools-1.7.0.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-14 19:24 tejd_build_tools-1.7.0.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 24-May-14 19:24 tejd_build_tools-1.7.0.dev1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    25106 b- defN 24-May-14 19:24 tejd_build_tools-1.7.0.dev1.dist-info/RECORD
-200 files, 3843924 bytes uncompressed, 649997 bytes compressed:  83.1%
+-rw-r--r--  2.0 unx    10142 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      151 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 24-May-14 19:32 tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    25106 b- defN 24-May-14 19:33 tejd_build_tools-1.7.0.dev2.dist-info/RECORD
+200 files, 3843894 bytes uncompressed, 649988 bytes compressed:  83.1%
```

## zipnote {}

```diff
@@ -579,23 +579,23 @@
 
 Filename: tejd_build_tools/include/transformer_engine/transformer_engine.h
 Comment: 
 
 Filename: tejd_build_tools/include/transformer_engine/transpose.h
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev1.dist-info/LICENSE
+Filename: tejd_build_tools-1.7.0.dev2.dist-info/LICENSE
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev1.dist-info/METADATA
+Filename: tejd_build_tools-1.7.0.dev2.dist-info/METADATA
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev1.dist-info/WHEEL
+Filename: tejd_build_tools-1.7.0.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev1.dist-info/top_level.txt
+Filename: tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: tejd_build_tools-1.7.0.dev1.dist-info/RECORD
+Filename: tejd_build_tools-1.7.0.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tejd_build_tools/VERSION

```diff
@@ -1 +1 @@
-1.7.0.dev1
+1.7.0.dev2
```

## tejd_build_tools/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.7.0.dev1'
+__version__ = '1.7.0.dev2'
```

## tejd_build_tools/build_tools/build_ext.py

```diff
@@ -12,15 +12,15 @@
 
 from pathlib import Path
 from subprocess import CalledProcessError
 from typing import List, Optional
 
 import setuptools
 
-from transformer_engine.build_tools.utils import (
+from .utils import (
     cmake_bin,
     debug_build_enabled,
     found_ninja,
 )
 
 
 class CMakeExtension(setuptools.Extension):
```

## Comparing `tejd_build_tools-1.7.0.dev1.dist-info/LICENSE` & `tejd_build_tools-1.7.0.dev2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tejd_build_tools-1.7.0.dev1.dist-info/RECORD` & `tejd_build_tools-1.7.0.dev2.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-tejd_build_tools/VERSION,sha256=roPipIp-5IiIOAhyNgCs_NpOHEbbf0OTH6a0sId0_-Y,10
-tejd_build_tools/__init__.py,sha256=_MNdIJxZKmXOrs85NzaKvaYijhtVLn3VPkBmFGdFedw,26
+tejd_build_tools/VERSION,sha256=IhqjB9t7pS5aJsCafLq1yKKU-tJalyT43c-oeCQDkec,10
+tejd_build_tools/__init__.py,sha256=tXhz3ylShfo5u4A7IOKPVpPHyDp8yQfD0Jjikck4QCU,26
 tejd_build_tools/te_version.py,sha256=wzQBnaq0vLKeRsPEpIIqw1AosLYQhjuCR-zsU5cqYL4,1045
 tejd_build_tools/build_tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-tejd_build_tools/build_tools/build_ext.py,sha256=-z-5hSlUqGF53ADIJcTs13FzY_ajf0_AyQhaDAnxbgw,6272
+tejd_build_tools/build_tools/build_ext.py,sha256=jbqCUBE66jtZ4pnjmFDu6p2_wdI5G0O4tqr1201ufAs,6242
 tejd_build_tools/build_tools/utils.py,sha256=tdGYs-NvV0_kiq9nDhAgyDCrcmJNBdFAm76bkc8aX40,4459
 tejd_build_tools/cudnn-frontend/.clang-format,sha256=gQFk79UqPdKJksQIFkWmOuMMJ1j6yQBzNa2lOiWiPb0,2663
 tejd_build_tools/cudnn-frontend/.git,sha256=a9pmDWgoNWr6xXkENhe3yCiiOR3UZ5HHCV2sm34pR0g,51
 tejd_build_tools/cudnn-frontend/CMakeLists.txt,sha256=ucmwfqDv8lCYIZq9gd0Bed1fH8KDucHDnASySA5TcLM,1965
 tejd_build_tools/cudnn-frontend/CONTRIBUTING.md,sha256=F9DxdHSaYHQLJDOFjN7-lXhd8om-ZNmdRxCuEjESQmM,2776
 tejd_build_tools/cudnn-frontend/LICENSE.txt,sha256=P8S0c6LAh2ioBmv35KWKEYUGDzrWdPLKniARvKSt8s4,1148
 tejd_build_tools/cudnn-frontend/README.FE.0.x.md,sha256=WvJb-P21y0dqatBty_GBgurJdsPT6AI5vNXk4ZYCJyk,8430
@@ -189,12 +189,12 @@
 tejd_build_tools/include/transformer_engine/gemm.h,sha256=vKSx2r7TLdESDJpm0kLh-R6CCHqRPjcAseHILbdrZ6c,5094
 tejd_build_tools/include/transformer_engine/layer_norm.h,sha256=WlNPs755_SsmI9weEqngZGVjOEj7Cs5P7BiLQLYyY1A,8990
 tejd_build_tools/include/transformer_engine/recipe.h,sha256=tGBMzSwJBd8VUrvVdK7YJBPc26GsmnWT3SChrR9EdAc,5381
 tejd_build_tools/include/transformer_engine/rmsnorm.h,sha256=NcjI4zBnADzC3tw_ZwM5SCLIRsUf8hksfpbvPAhsX4I,7518
 tejd_build_tools/include/transformer_engine/softmax.h,sha256=MSBcmUmWOTD9Nt-T7cEl6pxVmSyS7zskXpW8nCOlTxo,6281
 tejd_build_tools/include/transformer_engine/transformer_engine.h,sha256=u89GUQnqAg1C_KzFtcDS0f-uKA_vuaepZcVW8B7rICE,9573
 tejd_build_tools/include/transformer_engine/transpose.h,sha256=vzGwzqHj1WaKyX5GFA6IAPwycVb3CCotG1FUksnMDoU,11118
-tejd_build_tools-1.7.0.dev1.dist-info/LICENSE,sha256=vqG0Jm8UmfpLuxbW51d-a1tT0e8BCDWp1GCHYCLMhyI,10142
-tejd_build_tools-1.7.0.dev1.dist-info/METADATA,sha256=RA75HPMgIxuLU9bqiV4-_UQw5-3RcvoNE9jby79cvRk,151
-tejd_build_tools-1.7.0.dev1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-tejd_build_tools-1.7.0.dev1.dist-info/top_level.txt,sha256=KPLvv8ekYraJSt7QjK0ByGJElFL3k4YpDq7p0K0H6y0,17
-tejd_build_tools-1.7.0.dev1.dist-info/RECORD,,
+tejd_build_tools-1.7.0.dev2.dist-info/LICENSE,sha256=vqG0Jm8UmfpLuxbW51d-a1tT0e8BCDWp1GCHYCLMhyI,10142
+tejd_build_tools-1.7.0.dev2.dist-info/METADATA,sha256=Uz1iLFbBeEB7sK4yAj56eSCIvnjUM5cCZwJ5CWuwtVU,151
+tejd_build_tools-1.7.0.dev2.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+tejd_build_tools-1.7.0.dev2.dist-info/top_level.txt,sha256=KPLvv8ekYraJSt7QjK0ByGJElFL3k4YpDq7p0K0H6y0,17
+tejd_build_tools-1.7.0.dev2.dist-info/RECORD,,
```

