# Comparing `tmp/visualtest_python-1.9.0-py3-none-any.whl.zip` & `tmp/visualtest_python-1.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 29105 bytes, number of entries: 12
--rw-r--r--  2.0 unx      121 b- defN 24-May-10 16:02 sbvt/__init__.py
--rw-r--r--  2.0 unx    12832 b- defN 24-May-09 10:07 sbvt/api.py
--rw-r--r--  2.0 unx    11350 b- defN 24-May-10 16:02 sbvt/app.py
--rw-r--r--  2.0 unx    50235 b- defN 24-May-09 10:06 sbvt/browser.py
--rw-r--r--  2.0 unx     7465 b- defN 24-Mar-12 12:03 sbvt/imagetools.py
--rw-r--r--  2.0 unx      548 b- defN 23-May-11 09:06 sbvt/timer.py
--rw-r--r--  2.0 unx    22097 b- defN 24-May-09 10:07 sbvt/visualtest.py
--rw-r--r--  2.0 unx     1073 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3898 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      938 b- defN 24-May-10 16:03 visualtest_python-1.9.0.dist-info/RECORD
-12 files, 110654 bytes uncompressed, 27549 bytes compressed:  75.1%
+Zip file size: 29116 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      121 b- defN 24-May-14 16:15 sbvt/__init__.py
+-rw-r--r--  2.0 unx    12832 b- defN 24-May-09 17:02 sbvt/api.py
+-rw-r--r--  2.0 unx    11350 b- defN 24-May-09 17:02 sbvt/app.py
+-rw-r--r--  2.0 unx    50235 b- defN 24-May-09 17:02 sbvt/browser.py
+-rw-r--r--  2.0 unx     7465 b- defN 24-Mar-06 17:50 sbvt/imagetools.py
+-rw-r--r--  2.0 unx      548 b- defN 23-May-11 15:13 sbvt/timer.py
+-rw-r--r--  2.0 unx    22097 b- defN 24-May-09 17:02 sbvt/visualtest.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-14 16:18 visualtest_python-1.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3933 b- defN 24-May-14 16:18 visualtest_python-1.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 16:18 visualtest_python-1.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 24-May-14 16:18 visualtest_python-1.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      938 b- defN 24-May-14 16:18 visualtest_python-1.9.1.dist-info/RECORD
+12 files, 110689 bytes uncompressed, 27560 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: sbvt/timer.py
 Comment: 
 
 Filename: sbvt/visualtest.py
 Comment: 
 
-Filename: visualtest_python-1.9.0.dist-info/LICENSE
+Filename: visualtest_python-1.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: visualtest_python-1.9.0.dist-info/METADATA
+Filename: visualtest_python-1.9.1.dist-info/METADATA
 Comment: 
 
-Filename: visualtest_python-1.9.0.dist-info/WHEEL
+Filename: visualtest_python-1.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: visualtest_python-1.9.0.dist-info/top_level.txt
+Filename: visualtest_python-1.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: visualtest_python-1.9.0.dist-info/RECORD
+Filename: visualtest_python-1.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sbvt/__init__.py

```diff
@@ -1,4 +1,4 @@
 # this import statement is here for context.py in tests folder
 from .visualtest import VisualTest
 
-__version__ = '1.9.0'
+__version__ = '1.9.1'
```

## Comparing `visualtest_python-1.9.0.dist-info/LICENSE` & `visualtest_python-1.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `visualtest_python-1.9.0.dist-info/METADATA` & `visualtest_python-1.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visualtest-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Python SDK for SmartBear VisualTest via Selenium WebDriver
 Home-page: https://github.com/SmartBear/visualtest-python
 Author: Luke Kende
 Author-email: luke.kende@smartbear.com
 Keywords: visual testing,UI testing,GUI testing,UX testing,screenshots,full page screenshots,image comparisons,regression testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -18,14 +18,15 @@
 Requires-Dist: requests
 Requires-Dist: Pillow
 Requires-Dist: numpy
 Requires-Dist: python-dotenv
 Requires-Dist: packaging
 Requires-Dist: colorama
 Requires-Dist: colour
+Requires-Dist: axe-selenium-python
 
 #  VisualTest
 
 This Python SDK extends the functionality of Selenium WebDriver enabling the script to capture screenshots of the device under test, including fullpage, viewport, and element screenshots for regression testing or manual review of the UI.
 
 ```pip install visualtest-python```
```

## Comparing `visualtest_python-1.9.0.dist-info/RECORD` & `visualtest_python-1.9.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-sbvt/__init__.py,sha256=VqnerJ4XyRrD0_POqFjyQMVWoj1OWmaLzidY6VmZR4w,121
+sbvt/__init__.py,sha256=9rQkZp_dlaSsbdTmW-v0Ok1hJIXEmKF4E8T0GbD-kps,121
 sbvt/api.py,sha256=Jr1MeG78U1wrx4dQqV5mdLpC-IrzLV_QTKi-owJqSIc,12832
 sbvt/app.py,sha256=l2mHhvztiSZBiI4Y0EPFmgsxl4qRg9nAehdaUd66DWE,11350
 sbvt/browser.py,sha256=gTKjkahOAcICuAyNLHz_bPv-Io4dmbtWxheBTl574-Y,50235
 sbvt/imagetools.py,sha256=Gtbq9yAyv42Hh8yS60zIK50RfKcJTMUknnmrq64VGTM,7465
 sbvt/timer.py,sha256=ciQJQUYSTChdIbsLiYiEzPa6yw8YwSqaeWc7DU4gSrE,548
 sbvt/visualtest.py,sha256=ht8oWYdiHHvLOKFkp0EHTbQFF_Pb3Z3bFtRqJt96MWY,22097
-visualtest_python-1.9.0.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
-visualtest_python-1.9.0.dist-info/METADATA,sha256=_TdBpUDdty1X4dHo-Ht9SGCVXmsZDvWVwM9YMMnz8gI,3898
-visualtest_python-1.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-visualtest_python-1.9.0.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
-visualtest_python-1.9.0.dist-info/RECORD,,
+visualtest_python-1.9.1.dist-info/LICENSE,sha256=8vhEBNg7g2MxrQdwP-_ugxe3PDk5EbsBeMa--tc1xEA,1073
+visualtest_python-1.9.1.dist-info/METADATA,sha256=wMeFjjig62OO6XbzFuSpz0pna3629iN35yqQB6G9_Gk,3933
+visualtest_python-1.9.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+visualtest_python-1.9.1.dist-info/top_level.txt,sha256=t2tNJSI9vPU6KzikQCU2NYIJmbBaVTvOSJajc6IoRD0,5
+visualtest_python-1.9.1.dist-info/RECORD,,
```

