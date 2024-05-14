# Comparing `tmp/bacgwastatlearn-0.1.1.tar.gz` & `tmp/bacgwastatlearn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacgwastatlearn-0.1.1.tar", last modified: Fri May 10 05:21:44 2024, max compression
+gzip compressed data, was "bacgwastatlearn-0.1.2.tar", last modified: Tue May 14 20:47:10 2024, max compression
```

## Comparing `bacgwastatlearn-0.1.1.tar` & `bacgwastatlearn-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.700783 bacgwastatlearn-0.1.1/
--rw-r--r--   0 paulmacos   (501) staff       (20)      496 2024-05-10 05:21:44.700413 bacgwastatlearn-0.1.1/PKG-INFO
--rw-r--r--   0 paulmacos   (501) staff       (20)      322 2024-05-10 04:28:48.000000 bacgwastatlearn-0.1.1/README.md
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.694456 bacgwastatlearn-0.1.1/bacGWAStatLearn/
--rwxr-xr--   0 paulmacos   (501) staff       (20)     4377 2024-05-09 21:21:50.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/ClassIndexing.py
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.696349 bacgwastatlearn-0.1.1/bacGWAStatLearn/FeatureSelect/
--rwxr-xr--   0 paulmacos   (501) staff       (20)    10737 2024-05-09 21:24:10.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/FeatureSelect/ClassFeatureSelection.py
--rw-r--r--   0 paulmacos   (501) staff       (20)      112 2024-05-07 04:18:58.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/FeatureSelect/__init__.py
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.697428 bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/
--rwxr-xr--   0 paulmacos   (501) staff       (20)    13648 2024-05-09 21:21:28.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/ClassParamAnalysis.py
--rwxr-xr--   0 paulmacos   (501) staff       (20)     6236 2024-05-07 04:15:49.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/ClassTuning.py
--rw-r--r--   0 paulmacos   (501) staff       (20)      112 2024-05-07 04:01:51.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/__init__.py
--rw-r--r--   0 paulmacos   (501) staff       (20)      145 2024-05-08 18:34:39.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/__init__.py
--rw-r--r--   0 paulmacos   (501) staff       (20)      991 2024-05-09 21:22:43.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/main.py
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.699691 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/
--rwxr--r--   0 paulmacos   (501) staff       (20)     1853 2024-05-09 21:16:57.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_PreFilter_script0.py
--rwxr-xr--   0 paulmacos   (501) staff       (20)     3339 2024-05-09 21:17:58.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Ranking_script4.py
--rwxr-xr--   0 paulmacos   (501) staff       (20)     6471 2024-05-09 21:19:06.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_ReTuning_script3.py
--rwxr-xr--   0 paulmacos   (501) staff       (20)     3508 2024-05-09 21:16:35.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Selection_script2.py
--rwxr-xr--   0 paulmacos   (501) staff       (20)     8347 2024-05-09 21:20:12.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Tuning_script1.py
--rw-r--r--   0 paulmacos   (501) staff       (20)      113 2024-05-10 03:45:11.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/__init__.py
-drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-10 05:21:44.700029 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/
--rw-r--r--   0 paulmacos   (501) staff       (20)      496 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/PKG-INFO
--rw-r--r--   0 paulmacos   (501) staff       (20)      840 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/SOURCES.txt
--rw-r--r--   0 paulmacos   (501) staff       (20)        1 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/dependency_links.txt
--rw-r--r--   0 paulmacos   (501) staff       (20)       62 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/entry_points.txt
--rw-r--r--   0 paulmacos   (501) staff       (20)      117 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/requires.txt
--rw-r--r--   0 paulmacos   (501) staff       (20)       16 2024-05-10 05:21:44.000000 bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/top_level.txt
--rw-r--r--   0 paulmacos   (501) staff       (20)       38 2024-05-10 05:21:44.700873 bacgwastatlearn-0.1.1/setup.cfg
--rw-r--r--   0 paulmacos   (501) staff       (20)      798 2024-05-10 05:21:05.000000 bacgwastatlearn-0.1.1/setup.py
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.902108 bacgwastatlearn-0.1.2/
+-rw-r--r--   0 paulmacos   (501) staff       (20)     1073 2024-05-14 17:10:16.000000 bacgwastatlearn-0.1.2/LICENSE
+-rw-r--r--   0 paulmacos   (501) staff       (20)      593 2024-05-14 20:47:10.901832 bacgwastatlearn-0.1.2/PKG-INFO
+-rw-r--r--   0 paulmacos   (501) staff       (20)     1423 2024-05-13 20:37:23.000000 bacgwastatlearn-0.1.2/README.md
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.895438 bacgwastatlearn-0.1.2/bacGWAStatLearn/
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     4377 2024-05-09 21:21:50.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/ClassIndexing.py
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.897516 bacgwastatlearn-0.1.2/bacGWAStatLearn/FeatureSelect/
+-rwxr-xr--   0 paulmacos   (501) staff       (20)    10737 2024-05-09 21:24:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/FeatureSelect/ClassFeatureSelection.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)      112 2024-05-07 04:18:58.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/FeatureSelect/__init__.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)     6071 2024-05-14 20:43:13.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/Snakefile.py
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.898659 bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/
+-rwxr-xr--   0 paulmacos   (501) staff       (20)    13648 2024-05-09 21:21:28.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/ClassParamAnalysis.py
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     6236 2024-05-07 04:15:49.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/ClassTuning.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)      112 2024-05-07 04:01:51.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/__init__.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)      145 2024-05-08 18:34:39.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/__init__.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)      991 2024-05-09 21:22:43.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/main.py
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.900940 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/
+-rwxr--r--   0 paulmacos   (501) staff       (20)     1853 2024-05-09 21:16:57.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_PreFilter_script0.py
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     3339 2024-05-09 21:17:58.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Ranking_script4.py
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     6471 2024-05-09 21:19:06.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_ReTuning_script3.py
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     3508 2024-05-09 21:16:35.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Selection_script2.py
+-rwxr-xr--   0 paulmacos   (501) staff       (20)     8347 2024-05-09 21:20:12.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Tuning_script1.py
+-rw-r--r--   0 paulmacos   (501) staff       (20)      113 2024-05-10 03:45:11.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/__init__.py
+drwxr-xr-x   0 paulmacos   (501) staff       (20)        0 2024-05-14 20:47:10.901330 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/
+-rw-r--r--   0 paulmacos   (501) staff       (20)      593 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/PKG-INFO
+-rw-r--r--   0 paulmacos   (501) staff       (20)      877 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/SOURCES.txt
+-rw-r--r--   0 paulmacos   (501) staff       (20)        1 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/dependency_links.txt
+-rw-r--r--   0 paulmacos   (501) staff       (20)       62 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/entry_points.txt
+-rw-r--r--   0 paulmacos   (501) staff       (20)      117 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/requires.txt
+-rw-r--r--   0 paulmacos   (501) staff       (20)       16 2024-05-14 20:47:10.000000 bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/top_level.txt
+-rw-r--r--   0 paulmacos   (501) staff       (20)       38 2024-05-14 20:47:10.902176 bacgwastatlearn-0.1.2/setup.cfg
+-rw-r--r--   0 paulmacos   (501) staff       (20)      928 2024-05-14 20:46:49.000000 bacgwastatlearn-0.1.2/setup.py
```

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/ClassIndexing.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/ClassIndexing.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/FeatureSelect/ClassFeatureSelection.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/FeatureSelect/ClassFeatureSelection.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/ClassParamAnalysis.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/ClassParamAnalysis.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/TreeTune/ClassTuning.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/TreeTune/ClassTuning.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/main.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/main.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_PreFilter_script0.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_PreFilter_script0.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Ranking_script4.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Ranking_script4.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_ReTuning_script3.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_ReTuning_script3.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Selection_script2.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Selection_script2.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn/scripts/GWAS_Tuning_script1.py` & `bacgwastatlearn-0.1.2/bacGWAStatLearn/scripts/GWAS_Tuning_script1.py`

 * *Files identical despite different names*

### Comparing `bacgwastatlearn-0.1.1/bacGWAStatLearn.egg-info/SOURCES.txt` & `bacgwastatlearn-0.1.2/bacGWAStatLearn.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+LICENSE
 README.md
 setup.py
 bacGWAStatLearn/ClassIndexing.py
+bacGWAStatLearn/Snakefile.py
 bacGWAStatLearn/__init__.py
 bacGWAStatLearn/main.py
 bacGWAStatLearn.egg-info/PKG-INFO
 bacGWAStatLearn.egg-info/SOURCES.txt
 bacGWAStatLearn.egg-info/dependency_links.txt
 bacGWAStatLearn.egg-info/entry_points.txt
 bacGWAStatLearn.egg-info/requires.txt
```

### Comparing `bacgwastatlearn-0.1.1/setup.py` & `bacgwastatlearn-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # from bacGWAStatLearn import  _program
 _program = "bacGWAStatLearn"
 # Call setup function
 setup(
     author="Paul Phillips",
     description="A machine learning approach for conducting genome wide association studies (GWAS) on bacteria",
     name="bacGWAStatLearn",
-    packages=find_packages(include=["bacGWAStatLearn", "bacGWAStatLearn.*"]),
-    version="0.1.1",
+    packages=find_packages(include=["bacGWAStatLearn", "bacGWAStatLearn.*", "bacGWAStatLearn.Snakefile"]),
+    version="0.1.2",
     install_requires=['pandas', 'scipy', 'statsmodels','numpy==1.23.5', 'scikit-learn', 'xgboost', 'matplotlib', 'joblib', 'snakemake', 'Boruta', 'shap', 'seaborn','plotnine'],
-    # packages=["bacGWASim"],
+    # py_modules=['Snakefile', 'ClassIndexing.py'],
+    url="https://github.com/PaulDanPhillips/bacGWAStatLearn",
+    license="MIT",
     entry_points="""
     [console_scripts]
     {program} = bacGWAStatLearn.main:main
     """.format(program=_program),
     include_package_data=True,
-)
-
+)
```

