# Comparing `tmp/mtbp3-0.2.4-py3-none-any.whl.zip` & `tmp/mtbp3-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 255975 bytes, number of entries: 54
+Zip file size: 256003 bytes, number of entries: 54
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/.DS_Store
 -rw-r--r--  2.0 unx      351 b- defN 80-Jan-01 00:00 mtbp3/__init__.py
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/data/.DS_Store
 -rw-r--r--  2.0 unx    19789 b- defN 80-Jan-01 00:00 mtbp3/data/supp_ectd/fda_ctoc_v2.3.3.txt
 -rw-r--r--  2.0 unx  1016108 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/FMQ/FMQ_Consolidated_List.csv
 -rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/!!readme_26_1_English.txt
 -rw-r--r--  2.0 unx     2221 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt.asc
@@ -39,18 +39,18 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile11
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile12
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile20
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile3
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 mtbp3/health/__init__.py
 -rw-r--r--  2.0 unx     9095 b- defN 80-Jan-01 00:00 mtbp3/health/clinical.py
--rw-r--r--  2.0 unx     2113 b- defN 80-Jan-01 00:00 mtbp3/health/ectd.py
+-rw-r--r--  2.0 unx     2176 b- defN 80-Jan-01 00:00 mtbp3/health/ectd.py
 -rw-r--r--  2.0 unx    34117 b- defN 80-Jan-01 00:00 mtbp3/health/emt.py
 -rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 mtbp3/util/__init__.py
 -rw-r--r--  2.0 unx    13604 b- defN 80-Jan-01 00:00 mtbp3/util/cdt.py
 -rw-r--r--  2.0 unx    17343 b- defN 80-Jan-01 00:00 mtbp3/util/cdtg.py
 -rw-r--r--  2.0 unx    11887 b- defN 80-Jan-01 00:00 mtbp3/util/lsr.py
--rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx     5143 b- defN 16-Jan-01 00:00 mtbp3-0.2.4.dist-info/RECORD
-54 files, 1409369 bytes uncompressed, 247469 bytes compressed:  82.4%
+-rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 mtbp3-0.2.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.5.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5143 b- defN 16-Jan-01 00:00 mtbp3-0.2.5.dist-info/RECORD
+54 files, 1409432 bytes uncompressed, 247497 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: mtbp3/util/cdtg.py
 Comment: 
 
 Filename: mtbp3/util/lsr.py
 Comment: 
 
-Filename: mtbp3-0.2.4.dist-info/LICENSE
+Filename: mtbp3-0.2.5.dist-info/LICENSE
 Comment: 
 
-Filename: mtbp3-0.2.4.dist-info/METADATA
+Filename: mtbp3-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: mtbp3-0.2.4.dist-info/WHEEL
+Filename: mtbp3-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: mtbp3-0.2.4.dist-info/RECORD
+Filename: mtbp3-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mtbp3/health/ectd.py

```diff
@@ -12,25 +12,27 @@
 #
 #  You should have received a copy of the GNU General Public license
 #  along with this program. If not, see <https://www.gnu.org/license/>
 
 import pandas as pd
 import os
 from mtbp3.util.cdt import ListTree
+import mtbp3
     
 class ctoc_by_fda:
     def __init__(self, version="2.3.3"):
         assert isinstance(version, str) and all(char.isdigit() or char == '.' for char in version), "Version must be a string with integers and dots"
         self.version = version
+        self.folder_name = mtbp3.get_data(f'supp_ectd/fda_ctoc_v{version}.txt')
         self.ctoc = self.__load_list()
 
     def __load_list(self):
-        file_path = f'data/supp_ectd/fda_ctoc_v{self.version}.txt'
         #file_path = f'./mtbp3/data/supp_ectd/fda_ctoc_v{self.version}.txt'
-        if os.path.exists(file_path):
+        file_path = self.folder_name
+        if os.path.isfile(file_path):
             with open(file_path, 'r') as file:
                 lines = file.readlines()
             lines = [line.strip() for line in lines if line.strip()]
             return lines
         else:
             print(f"Version {self.version} not found.")
             return []
```

## Comparing `mtbp3-0.2.4.dist-info/LICENSE` & `mtbp3-0.2.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtbp3-0.2.4.dist-info/METADATA` & `mtbp3-0.2.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtbp3
-Version: 0.2.4
+Version: 0.2.5
 Summary: my tool box
 License: GNU General Public License v3.0
 Author: Y. Hsu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `mtbp3-0.2.4.dist-info/RECORD` & `mtbp3-0.2.5.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 mtbp3/data/test_lsr/testfolder1/testfile10,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder1/testfile11,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder1/testfile12,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder2/testfile20,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder2/testfile3,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/health/__init__.py,sha256=BqJVi0OMHyBp0zcg0IYDcPK1c9q8Fdil-Kcb2AHwNGY,19
 mtbp3/health/clinical.py,sha256=EiDRv70YPkc7sWtAs20a2X6c23uE3SWE9vucZQI1wYs,9095
-mtbp3/health/ectd.py,sha256=r-cifGeHTXbxwgFdkZX7nGfjR2fvEyXjifTAoovguic,2113
+mtbp3/health/ectd.py,sha256=5PLTtdD1LR8RnXQ-p4PAazSWO2p8W6y_c9Ej2JhP_IE,2176
 mtbp3/health/emt.py,sha256=FwQUI70DL-O1Y_pGKjDiLziNcgWAYxlYXG6L-Egn0sk,34117
 mtbp3/util/__init__.py,sha256=dbXCXornfglTSgUXCslcrqXyt1lMaUjf5TCn0RdHApc,58
 mtbp3/util/cdt.py,sha256=XhIKL5vt11fIbMMj5qVBi1_GHsdJNvFLAYszOd0V6zc,13604
 mtbp3/util/cdtg.py,sha256=GC71CPeUhQIpsezfGlZsqASLm-kTQCBM7hl0hbda3Eo,17343
 mtbp3/util/lsr.py,sha256=zwoEKj2slqYa17joB1Zit55G9QEd52MVuW3teV4bUJk,11887
-mtbp3-0.2.4.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
-mtbp3-0.2.4.dist-info/METADATA,sha256=2sBcpiWFc1kvgJjn9hKv3kM-2uDUxq8A96IR-Pys4Ho,2672
-mtbp3-0.2.4.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-mtbp3-0.2.4.dist-info/RECORD,,
+mtbp3-0.2.5.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
+mtbp3-0.2.5.dist-info/METADATA,sha256=j1OxVD5m5lrdznLl32Ws8Y0ZVp0pON-3AIpR2egAsrc,2672
+mtbp3-0.2.5.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+mtbp3-0.2.5.dist-info/RECORD,,
```

