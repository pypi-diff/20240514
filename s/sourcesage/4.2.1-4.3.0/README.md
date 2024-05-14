# Comparing `tmp/sourcesage-4.2.1.tar.gz` & `tmp/sourcesage-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourcesage-4.2.1.tar", last modified: Sat May 11 21:47:05 2024, max compression
+gzip compressed data, was "sourcesage-4.3.0.tar", last modified: Tue May 14 15:07:27 2024, max compression
```

## Comparing `sourcesage-4.2.1.tar` & `sourcesage-4.3.0.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.631350 sourcesage-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-11 21:47:01.000000 sourcesage-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-11 21:47:05.631350 sourcesage-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-11 21:47:01.000000 sourcesage-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 21:47:05.631350 sourcesage-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-11 21:47:01.000000 sourcesage-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.623350 sourcesage-4.2.1/sourcesage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.627350 sourcesage-4.2.1/sourcesage/config/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/.SourceSageignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.627350 sourcesage-4.2.1/sourcesage/config/ISSUES_RESOLVE/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.627350 sourcesage-4.2.1/sourcesage/config/STAGE_INFO/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/config/language_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.627350 sourcesage-4.2.1/sourcesage/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/ChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/ChangelogUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/DiffChangelogGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/EnvFileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/GitHubIssueRetrieve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/GitHubUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/IssuesToMarkdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/StageInfoGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/StagedDiffGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/markdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-11 21:47:01.000000 sourcesage-4.2.1/sourcesage/modules/source_sage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.631350 sourcesage-4.2.1/sourcesage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19635 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 21:47:05.000000 sourcesage-4.2.1/sourcesage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 21:47:05.631350 sourcesage-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-11 21:47:01.000000 sourcesage-4.2.1/tests/test_sourcesage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-14 15:07:22.000000 sourcesage-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-14 15:07:27.612118 sourcesage-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19252 2024-05-14 15:07:22.000000 sourcesage-4.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:07:27.612118 sourcesage-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-05-14 15:07:23.000000 sourcesage-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.604118 sourcesage-4.3.0/sourcesage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/.SourceSageignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/config/language_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6334 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.608118 sourcesage-4.3.0/sourcesage/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ChangelogUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/DiffChangelogGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/EnvFileHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/GitHubIssueRetrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/GitHubUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/IssuesToMarkdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/ReleaseDiffReportGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/StageInfoGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/StagedDiffGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/markdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-14 15:07:23.000000 sourcesage-4.3.0/sourcesage/modules/source_sage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/sourcesage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19660 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-14 15:07:27.000000 sourcesage-4.3.0/sourcesage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:07:27.612118 sourcesage-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3139 2024-05-14 15:07:23.000000 sourcesage-4.3.0/tests/test_sourcesage.py
```

### Comparing `sourcesage-4.2.1/LICENSE` & `sourcesage-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/PKG-INFO` & `sourcesage-4.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.2.1
+Version: 4.3.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 Requires-Dist: art
+Requires-Dist: termcolor
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.3.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
+Requires-Dist: termcolor
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
   _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]][[!![[SSoouurrcceeSSaaggee -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////
```

### Comparing `sourcesage-4.2.1/README.md` & `sourcesage-4.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/setup.py` & `sourcesage-4.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    required = f.read().splitlines()
 
 setup(
     # パッケージの名前
     name='sourcesage',
     
     # パッケージのバージョン
-    version='4.2.1',
+    version='4.3.0',
     
     # パッケージに含めるモジュールを自動的に探す
     packages=find_packages(),
     
     # パッケージの分類情報
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -51,9 +51,10 @@
     # パッケージのインストールに必要な依存関係
     # install_requires=required,
     install_requires=[
             'loguru',
             'GitPython',
             'requests',
             'art',
+            'termcolor',
     ],
 )
```

### Comparing `sourcesage-4.2.1/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md` & `sourcesage-4.3.0/sourcesage/config/ISSUES_RESOLVE/ISSUES_RESOLVE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md` & `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_AND_ISSUES_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md` & `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md` & `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_EMOJI.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md` & `sourcesage-4.3.0/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/config/constants.py` & `sourcesage-4.3.0/sourcesage/config/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.SOURCE_SAGE_MD = "DocuMind.md"
         self.CHANGELOG_DIR = "Changelog"
         self.STAGED_DIFF_MD = "STAGED_DIFF.md"
 
         self.set_output_dir(output_dir)
 
     def set_output_dir(self, output_dir):
-        self.SOURCE_SAGE_ASSETS_DIR = os.path.join(output_dir, "SourceSageAssets")
+        self.SOURCE_SAGE_ASSETS_DIR = os.path.join(output_dir, ".SourceSageAssets")
         self.ISSUE_LOG_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_LOG")
         self.ISSUES_RESOLVE_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "ISSUE_WISE/ISSUES_RESOLVE")
         self.STAGE_INFO_DIR = os.path.join(self.SOURCE_SAGE_ASSETS_DIR, "COMMIT_CRAFT/STAGE_INFO")
 
         self.TEMPLATE_ISSUES_RESOLVE_DIR = os.path.join(self.DOCS_DIR, "ISSUES_RESOLVE")
         self.ISSUES_RESOLVE_TEMPLATE_MD = "ISSUES_RESOLVE_TEMPLATE.md"
```

### Comparing `sourcesage-4.2.1/sourcesage/config/language_map.json` & `sourcesage-4.3.0/sourcesage/config/language_map.json`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/core.py` & `sourcesage-4.3.0/sourcesage/core.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/ChangelogGenerator.py` & `sourcesage-4.3.0/sourcesage/modules/ChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/ChangelogUtils.py` & `sourcesage-4.3.0/sourcesage/modules/ChangelogUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/DiffChangelogGenerator.py` & `sourcesage-4.3.0/sourcesage/modules/DiffChangelogGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/EnvFileHandler.py` & `sourcesage-4.3.0/sourcesage/modules/EnvFileHandler.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/GitHubIssueRetrieve.py` & `sourcesage-4.3.0/sourcesage/modules/GitHubIssueRetrieve.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/GitHubUtils.py` & `sourcesage-4.3.0/sourcesage/modules/GitHubUtils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/IssuesToMarkdown.py` & `sourcesage-4.3.0/sourcesage/modules/IssuesToMarkdown.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/StageInfoGenerator.py` & `sourcesage-4.3.0/sourcesage/modules/StageInfoGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/StagedDiffGenerator.py` & `sourcesage-4.3.0/sourcesage/modules/StagedDiffGenerator.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/file_utils.py` & `sourcesage-4.3.0/sourcesage/modules/file_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/markdown_utils.py` & `sourcesage-4.3.0/sourcesage/modules/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage/modules/source_sage.py` & `sourcesage-4.3.0/sourcesage/modules/source_sage.py`

 * *Files identical despite different names*

### Comparing `sourcesage-4.2.1/sourcesage.egg-info/PKG-INFO` & `sourcesage-4.3.0/sourcesage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: sourcesage
-Version: 4.2.1
+Version: 4.3.0
 Home-page: https://github.com/Sunwood-ai-labs/SourceSage
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru
 Requires-Dist: GitPython
 Requires-Dist: requests
 Requires-Dist: art
+Requires-Dist: termcolor
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/SourceSage_icon4.png" width="100%">
 <br>
 <h1 align="center">SourceSage</h1>
 <h2 align="center">
   ～Transforming code for AI～
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-Metadata-Version: 2.1 Name: sourcesage Version: 4.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: sourcesage Version: 4.3.0 Home-page: https://
 github.com/Sunwood-ai-labs/SourceSage Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 loguru Requires-Dist: GitPython Requires-Dist: requests Requires-Dist: art
+Requires-Dist: termcolor
  [https://raw.githubusercontent.com/Sunwood-ai-labs/SourceSage/main/docs/icon/
                              SourceSage_icon4.png]
                            ************ SSoouurrcceeSSaaggee ************
                      ********** ?ï?½?TTrraannssffoorrmmiinngg ccooddee ffoorr AAII?ï?½?
  [[PPyyPPII -- VVeerrssiioonn]][[PPyyPPII -- FFoorrmmaatt]][[PPyyPPII -- IImmpplleemmeennttaattiioonn]][[PPyyPPII -- SSttaattuuss]][[PPyyPPII --
    DDoowwnnllooaaddss]][[PPyyPPII -- DDoowwnnllooaaddss]]_[[_hh_tt_tt_pp_ss_::_//_//_aa_pp_pp_.._cc_oo_dd_aa_cc_yy_.._cc_oo_mm_//_pp_rr_oo_jj_ee_cc_tt_//_bb_aa_dd_gg_ee_//_GG_rr_aa_dd_ee_//
   _77_77_aa_bb_77_77_11_55_dd_dd_22_33_44_99_99_dd_88_22_cc_aa_cc_aa_44_ee_77_ee_aa_33_bb_00_99_33_]][[!![[SSoouurrcceeSSaaggee -- SSuunnwwoooodd--aaii--llaabbss]]((hhttttppss::////
```

### Comparing `sourcesage-4.2.1/sourcesage.egg-info/SOURCES.txt` & `sourcesage-4.3.0/sourcesage.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 sourcesage/modules/ChangelogGenerator.py
 sourcesage/modules/ChangelogUtils.py
 sourcesage/modules/DiffChangelogGenerator.py
 sourcesage/modules/EnvFileHandler.py
 sourcesage/modules/GitHubIssueRetrieve.py
 sourcesage/modules/GitHubUtils.py
 sourcesage/modules/IssuesToMarkdown.py
+sourcesage/modules/ReleaseDiffReportGenerator.py
 sourcesage/modules/StageInfoGenerator.py
 sourcesage/modules/StagedDiffGenerator.py
 sourcesage/modules/__init__.py
 sourcesage/modules/file_utils.py
 sourcesage/modules/markdown_utils.py
 sourcesage/modules/source_sage.py
 tests/test_sourcesage.py
```

### Comparing `sourcesage-4.2.1/tests/test_sourcesage.py` & `sourcesage-4.3.0/tests/test_sourcesage.py`

 * *Files identical despite different names*

