# Comparing `tmp/arm_adi-3.21.1-cp39-cp39-manylinux1_x86_64.whl.zip` & `tmp/arm_adi-3.21.1rc0-cp39-cp39-manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 460776 bytes, number of entries: 19
+Zip file size: 460806 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      683 b- defN 24-Mar-11 17:14 adi_py/__init__.py
 -rw-r--r--  2.0 unx     2703 b- defN 24-Mar-11 17:14 adi_py/constants.py
 -rw-r--r--  2.0 unx     1193 b- defN 24-Mar-11 17:14 adi_py/exception.py
 -rw-r--r--  2.0 unx     2437 b- defN 24-Mar-11 17:14 adi_py/logger.py
 -rw-r--r--  2.0 unx    72785 b- defN 24-Apr-14 04:16 adi_py/process.py
 -rw-r--r--  2.0 unx    41649 b- defN 24-Mar-11 17:14 adi_py/utils.py
 -rw-r--r--  2.0 unx     4154 b- defN 24-Mar-11 17:14 adi_py/xarray_accessors.py
 -rw-r--r--  2.0 unx       49 b- defN 24-Apr-27 16:41 cds3/__init__.py
--rwxr-xr-x  2.0 unx   330976 b- defN 24-May-14 18:30 cds3/core.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    50568 b- defN 24-May-14 18:30 cds3/enums.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   330976 b- defN 24-May-13 21:02 cds3/core.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    50568 b- defN 24-May-13 21:02 cds3/enums.cpython-39-x86_64-linux-gnu.so
 -rw-r--r--  2.0 unx       55 b- defN 24-Mar-11 17:14 dsproc3/__init__.py
--rwxr-xr-x  2.0 unx   868424 b- defN 24-May-14 18:31 dsproc3/core.cpython-39-x86_64-linux-gnu.so
--rwxr-xr-x  2.0 unx    77184 b- defN 24-May-14 18:31 dsproc3/enums.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx   868424 b- defN 24-May-13 21:02 dsproc3/core.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx    77184 b- defN 24-May-13 21:02 dsproc3/enums.cpython-39-x86_64-linux-gnu.so
 -rw-r--r--  2.0 unx       26 b- defN 24-Mar-11 17:14 trans/__init__.py
--rwxr-xr-x  2.0 unx    38576 b- defN 24-May-14 18:31 trans/core.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx       53 b- defN 24-May-14 18:31 arm_adi-3.21.1.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 24-May-14 18:31 arm_adi-3.21.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 24-May-14 18:31 arm_adi-3.21.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1549 b- defN 24-May-14 18:31 arm_adi-3.21.1.dist-info/RECORD
-19 files, 1493198 bytes uncompressed, 458264 bytes compressed:  69.3%
+-rwxr-xr-x  2.0 unx    38576 b- defN 24-May-13 21:02 trans/core.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx       56 b- defN 24-May-13 21:02 arm_adi-3.21.1rc0.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 24-May-13 21:02 arm_adi-3.21.1rc0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       26 b- defN 24-May-13 21:02 arm_adi-3.21.1rc0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1561 b- defN 24-May-13 21:02 arm_adi-3.21.1rc0.dist-info/RECORD
+19 files, 1493213 bytes uncompressed, 458270 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: trans/__init__.py
 Comment: 
 
 Filename: trans/core.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: arm_adi-3.21.1.dist-info/METADATA
+Filename: arm_adi-3.21.1rc0.dist-info/METADATA
 Comment: 
 
-Filename: arm_adi-3.21.1.dist-info/WHEEL
+Filename: arm_adi-3.21.1rc0.dist-info/WHEEL
 Comment: 
 
-Filename: arm_adi-3.21.1.dist-info/top_level.txt
+Filename: arm_adi-3.21.1rc0.dist-info/top_level.txt
 Comment: 
 
-Filename: arm_adi-3.21.1.dist-info/RECORD
+Filename: arm_adi-3.21.1rc0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `arm_adi-3.21.1.dist-info/RECORD` & `arm_adi-3.21.1rc0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 cds3/core.cpython-39-x86_64-linux-gnu.so,sha256=5g2h7G615W4TnDXOQNaFMLS68rK48fsU-FQCxW_MSno,330976
 cds3/enums.cpython-39-x86_64-linux-gnu.so,sha256=AfwMj_vPfq_a2qFsZv8_CAtAx07OuOfHd5lrJJP36Dk,50568
 dsproc3/__init__.py,sha256=cVAVQcV-V7E6RWvZOtk2zzUjF0Kx3D1SSd2oIJIQ-J8,55
 dsproc3/core.cpython-39-x86_64-linux-gnu.so,sha256=wweMHz2tzy2gmCLSxfUE1uDBAOYgmwPHwH_Jl-Cc8vc,868424
 dsproc3/enums.cpython-39-x86_64-linux-gnu.so,sha256=vgNwKOsViKUN_-a_st5hP2b2eTz99I5jtobQB5lG4eY,77184
 trans/__init__.py,sha256=Eqb6lUmJNljei5ehgzdAjMHWye92E-jL7jHJezpEglI,26
 trans/core.cpython-39-x86_64-linux-gnu.so,sha256=uiAkhxhcNZnEMag61wvj6XdpeQKmM-JxTKyWtZ1DXqE,38576
-arm_adi-3.21.1.dist-info/METADATA,sha256=9YJDusQUruRrIB80oLQaGUAg9lAYF-t6-Y-ZHxsn06o,53
-arm_adi-3.21.1.dist-info/WHEEL,sha256=S6BHKTEP8NjWsdyBMQb12wPxDFPBE-J7vg1aUoGOwJY,108
-arm_adi-3.21.1.dist-info/top_level.txt,sha256=-qlPwWrGKOSHxoluVqcX8LROk0Ks7aXq3s8bP4mTLvk,26
-arm_adi-3.21.1.dist-info/RECORD,,
+arm_adi-3.21.1rc0.dist-info/METADATA,sha256=AOT7GJm_CSV_PnN4RFP_DNux1r9qGFIFJ8Twg63Nvww,56
+arm_adi-3.21.1rc0.dist-info/WHEEL,sha256=S6BHKTEP8NjWsdyBMQb12wPxDFPBE-J7vg1aUoGOwJY,108
+arm_adi-3.21.1rc0.dist-info/top_level.txt,sha256=-qlPwWrGKOSHxoluVqcX8LROk0Ks7aXq3s8bP4mTLvk,26
+arm_adi-3.21.1rc0.dist-info/RECORD,,
```

