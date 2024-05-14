# Comparing `tmp/AutoGitSemVer-0.7.2-py3-none-any.whl.zip` & `tmp/AutoGitSemVer-0.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 16214 bytes, number of entries: 11
--rw-r--r--  2.0 unx     2433 b- defN 24-Apr-29 22:54 BuildBinary.py
--rw-r--r--  2.0 unx     2756 b- defN 24-Apr-29 22:54 AutoGitSemVer/AutoGitSemVerSchema.json
--rw-r--r--  2.0 unx     6207 b- defN 24-Apr-29 22:54 AutoGitSemVer/EntryPoint.py
--rw-r--r--  2.0 unx    23413 b- defN 24-Apr-29 22:54 AutoGitSemVer/Lib.py
--rw-r--r--  2.0 unx      882 b- defN 24-Apr-29 22:54 AutoGitSemVer/__init__.py
--rw-r--r--  2.0 unx     1071 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    18050 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       63 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       26 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      931 b- defN 24-Apr-29 22:54 AutoGitSemVer-0.7.2.dist-info/RECORD
-11 files, 55924 bytes uncompressed, 14630 bytes compressed:  73.8%
+Zip file size: 15266 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     2756 b- defN 24-May-14 18:03 AutoGitSemVer/AutoGitSemVerSchema.json
+-rw-r--r--  2.0 unx     6207 b- defN 24-May-14 18:03 AutoGitSemVer/EntryPoint.py
+-rw-r--r--  2.0 unx    23413 b- defN 24-May-14 18:03 AutoGitSemVer/Lib.py
+-rw-r--r--  2.0 unx      882 b- defN 24-May-14 18:04 AutoGitSemVer/__init__.py
+-rw-r--r--  2.0 unx     1071 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    18050 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       63 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      860 b- defN 24-May-14 18:04 AutoGitSemVer-0.7.3.dist-info/RECORD
+10 files, 53408 bytes uncompressed, 13786 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
-Filename: BuildBinary.py
-Comment: 
-
 Filename: AutoGitSemVer/AutoGitSemVerSchema.json
 Comment: 
 
 Filename: AutoGitSemVer/EntryPoint.py
 Comment: 
 
 Filename: AutoGitSemVer/Lib.py
 Comment: 
 
 Filename: AutoGitSemVer/__init__.py
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/LICENSE.txt
+Filename: AutoGitSemVer-0.7.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/METADATA
+Filename: AutoGitSemVer-0.7.3.dist-info/METADATA
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/WHEEL
+Filename: AutoGitSemVer-0.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/entry_points.txt
+Filename: AutoGitSemVer-0.7.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/top_level.txt
+Filename: AutoGitSemVer-0.7.3.dist-info/top_level.txt
 Comment: 
 
-Filename: AutoGitSemVer-0.7.2.dist-info/RECORD
+Filename: AutoGitSemVer-0.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AutoGitSemVer/__init__.py

```diff
@@ -13,11 +13,11 @@
 # ----------------------------------------------------------------------
 # pylint: disable=missing-module-docstring,invalid-name
 
 # ----------------------------------------------------------------------
 # Note that this value will be overwritten by calls to `python ../../Build.py update_version` based
 # on changes observed in the git repository. The default value below will be used until the value
 # here is explicitly updated as part of a commit.
-__version__ = "0.7.2"
+__version__ = "0.7.3"
 
 
 from .Lib import GenerateStyle, GetSemanticVersion, GetSemanticVersionResult
```

## Comparing `AutoGitSemVer-0.7.2.dist-info/LICENSE.txt` & `AutoGitSemVer-0.7.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `AutoGitSemVer-0.7.2.dist-info/METADATA` & `AutoGitSemVer-0.7.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoGitSemVer
-Version: 0.7.2
+Version: 0.7.3
 Summary: Calculates a semantic version based on git changes.
 Author-email: David Brownell <db@DavidBrownell.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/davidbrownell/AutoGitSemVer
 Project-URL: Documentation, https://github.com/davidbrownell/AutoGitSemVer
 Project-URL: Repository, https://github.com/davidbrownell/AutoGitSemVer
 Classifier: Development Status :: 4 - Beta
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AutoGitSemVer Version: 0.7.2 Summary: Calculates a
+Metadata-Version: 2.1 Name: AutoGitSemVer Version: 0.7.3 Summary: Calculates a
 semantic version based on git changes. Author-email: David Brownell
 DavidBrownell.com> License: MIT License Project-URL: Homepage, https://
 github.com/davidbrownell/AutoGitSemVer Project-URL: Documentation, https://
 github.com/davidbrownell/AutoGitSemVer Project-URL: Repository, https://
 github.com/davidbrownell/AutoGitSemVer Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Natural Language :: English Classifier:
```

## Comparing `AutoGitSemVer-0.7.2.dist-info/RECORD` & `AutoGitSemVer-0.7.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-BuildBinary.py,sha256=CrOg39LilVUF-xy1KIP8o3KI2m_cYP_VCzBQUDI6-Dc,2433
 AutoGitSemVer/AutoGitSemVerSchema.json,sha256=2n2DRw-JReiYcD9jmw3mjbsKNZjheKIvhVdQz6FmP2s,2756
 AutoGitSemVer/EntryPoint.py,sha256=jpe3CRtmgYl8yu4W0XfqVnJ7IXcJ47oCf0D_EsXcE_s,6207
 AutoGitSemVer/Lib.py,sha256=vaR0ovpm219oCIJ14vXYLnMsl1s-3H9ruqP-DQuD3wA,23413
-AutoGitSemVer/__init__.py,sha256=q3ClVk8B-b_Pliu_RuoscWhBB8Qdo_ufz_FT2X8wjq4,882
-AutoGitSemVer-0.7.2.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
-AutoGitSemVer-0.7.2.dist-info/METADATA,sha256=fBuEj5q-CIBlGGmnTA_46hjcDgpfogR72ME7NG8Ss1g,18050
-AutoGitSemVer-0.7.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-AutoGitSemVer-0.7.2.dist-info/entry_points.txt,sha256=G8GOzgDIIgHgBzYb4RuCBwRUQtSLd7SW-DihP0oTU9Y,63
-AutoGitSemVer-0.7.2.dist-info/top_level.txt,sha256=Q6jMBQnUOSQS-cq3i7AjILoN-JIyZe1D8FBCnOXgKXQ,26
-AutoGitSemVer-0.7.2.dist-info/RECORD,,
+AutoGitSemVer/__init__.py,sha256=QEHsvpvrnFCyBv83n0JFE0DOfrNb5yRTgceOMhXx7PU,882
+AutoGitSemVer-0.7.3.dist-info/LICENSE.txt,sha256=6ycKI8SWG920Saey4PGi5YUVLX0C_8hfqJr7Q0sqGI8,1071
+AutoGitSemVer-0.7.3.dist-info/METADATA,sha256=h6JX09r13BBZ-Rh0tiyL32-k5snpzIe14bddlMO33rI,18050
+AutoGitSemVer-0.7.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+AutoGitSemVer-0.7.3.dist-info/entry_points.txt,sha256=G8GOzgDIIgHgBzYb4RuCBwRUQtSLd7SW-DihP0oTU9Y,63
+AutoGitSemVer-0.7.3.dist-info/top_level.txt,sha256=uoFTKJr0qTooZ8HV80Q-dR0UcRsQeKA4zDMnDK9KDAs,14
+AutoGitSemVer-0.7.3.dist-info/RECORD,,
```

