# Comparing `tmp/penguindashboard-1.0.8.tar.gz` & `tmp/penguindashboard-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penguindashboard-1.0.8.tar", last modified: Mon May 13 21:18:19 2024, max compression
+gzip compressed data, was "penguindashboard-1.0.9.tar", last modified: Mon May 13 21:19:33 2024, max compression
```

## Comparing `penguindashboard-1.0.8.tar` & `penguindashboard-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:18:19.535136 penguindashboard-1.0.8/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.8/LICENSE.txt
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 21:18:19.535136 penguindashboard-1.0.8/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.8/README.md
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:18:19.519137 penguindashboard-1.0.8/penguindashboard/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2516 2024-05-13 20:59:25.000000 penguindashboard-1.0.8/penguindashboard/AntiBERTa2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4052 2024-05-13 20:51:49.000000 penguindashboard-1.0.8/penguindashboard/BLAST_phylo.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3486 2024-05-13 20:51:04.000000 penguindashboard-1.0.8/penguindashboard/ESM2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2829 2024-05-13 20:55:20.000000 penguindashboard-1.0.8/penguindashboard/ProteinMPNN_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3402 2024-05-13 20:55:23.000000 penguindashboard-1.0.8/penguindashboard/SaProt_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.8/penguindashboard/__init__.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.8/penguindashboard/edit_mutcompute_output.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.8/penguindashboard/esm_fold.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4992 2024-05-13 21:07:11.000000 penguindashboard-1.0.8/penguindashboard/pipeline.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.8/penguindashboard/score.py
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:18:19.531136 penguindashboard-1.0.8/penguindashboard.egg-info/
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 21:18:19.000000 penguindashboard-1.0.8/penguindashboard.egg-info/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 21:18:19.000000 penguindashboard-1.0.8/penguindashboard.egg-info/SOURCES.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 21:18:19.000000 penguindashboard-1.0.8/penguindashboard.egg-info/dependency_links.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 21:18:19.000000 penguindashboard-1.0.8/penguindashboard.egg-info/entry_points.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 21:18:19.000000 penguindashboard-1.0.8/penguindashboard.egg-info/top_level.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 21:18:19.535136 penguindashboard-1.0.8/setup.cfg
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 21:18:03.000000 penguindashboard-1.0.8/setup.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:19:33.039438 penguindashboard-1.0.9/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.9/LICENSE.txt
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 21:19:33.039438 penguindashboard-1.0.9/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.9/README.md
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:19:33.023439 penguindashboard-1.0.9/penguindashboard/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2516 2024-05-13 20:59:25.000000 penguindashboard-1.0.9/penguindashboard/AntiBERTa2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4052 2024-05-13 20:51:49.000000 penguindashboard-1.0.9/penguindashboard/BLAST_phylo.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3486 2024-05-13 20:51:04.000000 penguindashboard-1.0.9/penguindashboard/ESM2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2829 2024-05-13 20:55:20.000000 penguindashboard-1.0.9/penguindashboard/ProteinMPNN_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3402 2024-05-13 20:55:23.000000 penguindashboard-1.0.9/penguindashboard/SaProt_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.9/penguindashboard/__init__.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.9/penguindashboard/edit_mutcompute_output.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.9/penguindashboard/esm_fold.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4968 2024-05-13 21:19:10.000000 penguindashboard-1.0.9/penguindashboard/pipeline.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.9/penguindashboard/score.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 21:19:33.035438 penguindashboard-1.0.9/penguindashboard.egg-info/
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 21:19:32.000000 penguindashboard-1.0.9/penguindashboard.egg-info/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 21:19:32.000000 penguindashboard-1.0.9/penguindashboard.egg-info/SOURCES.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 21:19:32.000000 penguindashboard-1.0.9/penguindashboard.egg-info/dependency_links.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 21:19:32.000000 penguindashboard-1.0.9/penguindashboard.egg-info/entry_points.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 21:19:32.000000 penguindashboard-1.0.9/penguindashboard.egg-info/top_level.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 21:19:33.039438 penguindashboard-1.0.9/setup.cfg
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 21:19:28.000000 penguindashboard-1.0.9/setup.py
```

### Comparing `penguindashboard-1.0.8/LICENSE.txt` & `penguindashboard-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/PKG-INFO` & `penguindashboard-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.8
+Version: 1.0.9
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.8/README.md` & `penguindashboard-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/AntiBERTa2_getLogits.py` & `penguindashboard-1.0.9/penguindashboard/AntiBERTa2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/BLAST_phylo.py` & `penguindashboard-1.0.9/penguindashboard/BLAST_phylo.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/ESM2_getLogits.py` & `penguindashboard-1.0.9/penguindashboard/ESM2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/ProteinMPNN_getLogits.py` & `penguindashboard-1.0.9/penguindashboard/ProteinMPNN_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/SaProt_getLogits.py` & `penguindashboard-1.0.9/penguindashboard/SaProt_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/edit_mutcompute_output.py` & `penguindashboard-1.0.9/penguindashboard/edit_mutcompute_output.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/esm_fold.py` & `penguindashboard-1.0.9/penguindashboard/esm_fold.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard/pipeline.py` & `penguindashboard-1.0.9/penguindashboard/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
 
     if args.saprot:
         os.makedirs(f"{args.output_dir}/foldseek", exist_ok=True)
         subprocess.run(f"foldseek createdb {pdb_file} {args.output_dir}/foldseek/{name} -v 1", shell=True)
         subprocess.run(f"foldseek lndb {args.output_dir}/foldseek/{name}_h {args.output_dir}/foldseek/{name}_ss_h -v 1", shell=True)
         subprocess.run(f"foldseek convert2fasta {args.output_dir}/foldseek/{name}_ss {args.output_dir}/foldseek/{name}_ss.fasta -v 1", shell=True)
         print("Running SaProt...")
-        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str {seq} --foldseek_tokens {args.output_dir}/foldseek/{name}_ss.fasta 
-                       --output_prefix {args.output_dir}/{name}", shell=True)
+        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str {seq} --foldseek_tokens {args.output_dir}/foldseek/{name}_ss.fasta --output_prefix {args.output_dir}/{name}", shell=True)
 
     if args.antiberta:
         print("Running AntiBERTa2...")
         subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str {seq} --output_prefix {args.output_dir}/{name}", shell=True)
 
     if args.esm:
         print("Running ESM2 (650M)...")
```

### Comparing `penguindashboard-1.0.8/penguindashboard/score.py` & `penguindashboard-1.0.9/penguindashboard/score.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/penguindashboard.egg-info/PKG-INFO` & `penguindashboard-1.0.9/penguindashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.8
+Version: 1.0.9
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.8/penguindashboard.egg-info/SOURCES.txt` & `penguindashboard-1.0.9/penguindashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.8/setup.py` & `penguindashboard-1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 # Text of the README file
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='penguindashboard',
-    version='1.0.8',
+    version='1.0.9',
     author='Aaron Feller, Phillip Woolley',
     author_email='aaronleefeller@gmail.com, prwoolley@utexas.edu',
     description='PEngUIN: Protein Engineering Using Independent Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AaronFeller/PEngUIN',
     license='MIT',
```

