# Comparing `tmp/fast2q-2.5.4.tar.gz` & `tmp/fast2q-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fast2q-2.5.4.tar", last modified: Fri Sep  1 13:40:04 2023, max compression
+gzip compressed data, was "dist\fast2q-2.5.5.tar", last modified: Tue Sep  5 08:45:39 2023, max compression
```

## Comparing `fast2q-2.5.4.tar` & `fast2q-2.5.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-09-01 13:40:04.000000 fast2q-2.5.4/
--rw-rw-rw-   0        0        0    11539 2023-09-01 13:40:04.000000 fast2q-2.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-08-03 08:39:02.000000 fast2q-2.5.4/README.txt
-drwxrwxrwx   0        0        0        0 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q/
--rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.4/fast2q/__init__.py
--rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.4/fast2q/__main__.py
--rw-rw-rw-   0        0        0    49907 2023-09-01 12:06:47.000000 fast2q-2.5.4/fast2q/fast2q.py
-drwxrwxrwx   0        0        0        0 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/
--rw-rw-rw-   0        0        0    11539 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-09-01 13:40:04.000000 fast2q-2.5.4/fast2q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-01 13:40:04.000000 fast2q-2.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1446 2023-09-01 13:38:52.000000 fast2q-2.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-05 08:45:39.000000 fast2q-2.5.5/
+-rw-rw-rw-   0        0        0    11653 2023-09-05 08:45:39.000000 fast2q-2.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-08-03 08:39:02.000000 fast2q-2.5.5/README.txt
+drwxrwxrwx   0        0        0        0 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q/
+-rw-rw-rw-   0        0        0        0 2021-05-14 10:49:48.000000 fast2q-2.5.5/fast2q/__init__.py
+-rw-rw-rw-   0        0        0       76 2021-09-02 14:00:47.000000 fast2q-2.5.5/fast2q/__main__.py
+-rw-rw-rw-   0        0        0    49277 2023-09-05 08:42:02.000000 fast2q-2.5.5/fast2q/fast2q.py
+drwxrwxrwx   0        0        0        0 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/
+-rw-rw-rw-   0        0        0    11653 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-09-05 08:45:39.000000 fast2q-2.5.5/fast2q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-09-05 08:45:39.000000 fast2q-2.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1446 2023-09-05 08:45:08.000000 fast2q-2.5.5/setup.py
```

### Comparing `fast2q-2.5.4/PKG-INFO` & `fast2q-2.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.4
+Version: 2.5.5
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -13,15 +13,17 @@
         
         2FAST2Q can work with any classic CRISPRi experimental setup, or be used for any kind of sequence extraction from FASTQ files.
         
         Check out my GitHub for the source files: https://github.com/afombravo/2FAST2Q
         
         2FAST2Q is published as part of a CRISPRi-seq protocol: https://www.nature.com/articles/s41596-021-00639-6
         
-        A more in depth description of the program is also available as a preprint: https://www.biorxiv.org/content/10.1101/2021.12.17.473121v1
+        A more in depth description of the program is also available:
+        
+        Bravo AM, Typas A, Veening J. 2022. 2FAST2Q: a general-purpose sequence search and counting program for FASTQ files. PeerJ 10:e14041 : https://peerj.com/articles/14041/
         
         
         # How to use it
         
         
         There are two versions of the program, with and without a basic user interface.
```

### Comparing `fast2q-2.5.4/fast2q/fast2q.py` & `fast2q-2.5.5/fast2q/fast2q.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     Every read is trimmed based on the indicated feature positioning. 
     The quality of the obtained trimmed read is crossed against the indicated
     Phred score for quality control.
     If the read has a perfect match with a feature, the respective feature gets a 
     read increase of 1 (done by calling .counts from the respective feature class 
     from the feature class dictionary).
     If the read doesnt have a perfect match, it is sent for mismatch comparison
-    via the "imperfect_alignment" function.
+    via the "mismatch_search_handler" function.
     """
 
     def binary_converter(features):
 
         """ Parses the input features into numba dictionaries with int8 layout. 
         Converts all DNA sequences to their respective binary array forms. 
         This gives some computing speed advantages with mismatches."""
@@ -244,18 +244,15 @@
 
                     if len(param['quality_set'].intersection(quality)) == 0:
 
                         if param['Running Mode']=='C':
                             if seq in features:
                                 features[seq].counts += 1
                                 perfect_counter += 1
-                                if features['G'].counts == 1:
-                                    print(reading,3)
-                                    break
-                            
+
                             elif mismatch != []:
                                 features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter=\
                                 mismatch_search_handler(seq,mismatch,\
                                                         failed_reads,binary_features,\
                                                         imperfect_counter,features,\
                                                         passed_reads,ram_clearance,non_aligned_counter)
 
@@ -370,55 +367,43 @@
                     return
     if found==1:
         return found_guide
 
 def mismatch_search_handler(seq,mismatch,failed_reads,binary_features,imperfect_counter,features,passed_reads,ram_clearance,non_aligned_counter):
     
     """Converts a read into numpy int 8 form. Runs the imperfect alignment 
-    function for all number of inputed mismatches."""
+    search for all number of inputed mismatches."""
+    
+    if seq in failed_reads:
+        non_aligned_counter += 1
+        return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
+    
+    if seq in passed_reads:
+        features[passed_reads[seq]].counts += 1
+        imperfect_counter += 1
+        return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
     
     read=seq2bin(seq)                         
     for miss in mismatch:
 
-        # we already know this read is going to pass
-        if seq in passed_reads:
-            features[passed_reads[seq]].counts += 1
+        feature = features_all_vs_all(binary_features, read, miss)
+        
+        if feature is not None:
+            features[feature].counts += 1
             imperfect_counter += 1
+            passed_reads[seq] = feature
             return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
-        
-        elif seq not in failed_reads:
-            features,imperfect_counter,feature=\
-                imperfect_alignment(read,binary_features,\
-                                    miss, imperfect_counter,\
-                                    features)
-            if feature is None:
+    
+        else: 
+            if miss == mismatch[-1]:
+                #if function reaches here its because nothing was aligned anywhere
                 if ram_clearance:
                     failed_reads.add(seq)
-            else:
-                passed_reads[seq] = feature
-                imperfect_counter += 1
+                non_aligned_counter += 1
                 return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
-    
-    #if function reaches here its because nothing was aligned anywhere
-    non_aligned_counter += 1
-
-    return features,imperfect_counter,failed_reads,passed_reads,non_aligned_counter
-
-def imperfect_alignment(read,binary_features, mismatch, counter, features):
-    
-    """ for the inputed read sequence, this compares if there is a feature 
-    with a sequence that is similar to it, to the indicated mismatch degree"""
-
-    feature = features_all_vs_all(binary_features, read, mismatch)
-    
-    if feature is not None:
-        features[feature].counts += 1
-        counter += 1
-
-    return features,counter,feature
 
 def aligner(raw,i,o,features,param,cpu,failed_reads,passed_reads):
 
     """ Runs the main read to sgRNA associating function "reads_counter".
     Creates some visual prompts to alert the user that the samples are being
     processed. Some on the fly quality control is possible (such as making sure 
     the total number of samples is correct, getting an estimate of the total
@@ -694,15 +679,15 @@
     return param
 
 def input_parser():
     
     """ Handles the cmd line interface, and all the parameter inputs"""
     
     global version
-    version = "2.5.4"
+    version = "2.5.5"
     
     def current_dir_path_handling(param):
         if param[0] is None:
             parameters[param[1]]=os.getcwd()
             if param[1] == 'feature':
                 file = path_finder(os.getcwd(), ["*.csv"])
                 if parameters['Running Mode']!="EC":
```

### Comparing `fast2q-2.5.4/fast2q.egg-info/PKG-INFO` & `fast2q-2.5.5/fast2q.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast2q
-Version: 2.5.4
+Version: 2.5.5
 Summary: A Python3 program that counts sequence occurences in fastq files.
 Home-page: https://github.com/afombravo/2FAST2Q
 Author: Afonso M Bravo
 Author-email: <afonsombravo@hotmail.com>
 License: UNKNOWN
 Description: # Welcome to 2FAST2Q
         A Python3 based program that counts sequence occurrences in FASTQ files
@@ -13,15 +13,17 @@
         
         2FAST2Q can work with any classic CRISPRi experimental setup, or be used for any kind of sequence extraction from FASTQ files.
         
         Check out my GitHub for the source files: https://github.com/afombravo/2FAST2Q
         
         2FAST2Q is published as part of a CRISPRi-seq protocol: https://www.nature.com/articles/s41596-021-00639-6
         
-        A more in depth description of the program is also available as a preprint: https://www.biorxiv.org/content/10.1101/2021.12.17.473121v1
+        A more in depth description of the program is also available:
+        
+        Bravo AM, Typas A, Veening J. 2022. 2FAST2Q: a general-purpose sequence search and counting program for FASTQ files. PeerJ 10:e14041 : https://peerj.com/articles/14041/
         
         
         # How to use it
         
         
         There are two versions of the program, with and without a basic user interface.
```

### Comparing `fast2q-2.5.4/setup.py` & `fast2q-2.5.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '2.5.4' 
+VERSION = '2.5.5' 
 DESCRIPTION = """A Python3 program that counts sequence occurences in fastq files."""
 
 setup(
         name="fast2q", 
         version=VERSION,
         author="Afonso M Bravo",
         author_email="<afonsombravo@hotmail.com>",
```

