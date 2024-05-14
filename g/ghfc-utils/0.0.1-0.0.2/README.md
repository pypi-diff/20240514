# Comparing `tmp/ghfc_utils-0.0.1.tar.gz` & `tmp/ghfc_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghfc_utils-0.0.1.tar", last modified: Tue May 14 09:56:05 2024, max compression
+gzip compressed data, was "ghfc_utils-0.0.2.tar", last modified: Tue May 14 11:35:48 2024, max compression
```

## Comparing `ghfc_utils-0.0.1.tar` & `ghfc_utils-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        0 2024-05-14 09:56:05.117791 ghfc_utils-0.0.1/
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)     1070 2024-04-26 11:45:27.000000 ghfc_utils-0.0.1/LICENSE
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)     5492 2024-05-14 09:56:05.117716 ghfc_utils-0.0.1/PKG-INFO
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)     4967 2024-05-13 13:21:47.000000 ghfc_utils-0.0.1/README.md
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)       94 2024-05-14 09:52:59.000000 ghfc_utils-0.0.1/pyproject.toml
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)      805 2024-05-14 09:56:05.118211 ghfc_utils-0.0.1/setup.cfg
-drwxr-xr-x   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        0 2024-05-14 09:56:05.110796 ghfc_utils-0.0.1/src/
-drwxr-xr-x   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        0 2024-05-14 09:56:05.114831 ghfc_utils-0.0.1/src/ghfc_utils/
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        0 2024-04-26 13:11:07.000000 ghfc_utils-0.0.1/src/ghfc_utils/__init__.py
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)       79 2024-04-26 13:12:52.000000 ghfc_utils-0.0.1/src/ghfc_utils/slivar_dnm.py
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)    11917 2024-05-06 14:46:14.000000 ghfc_utils-0.0.1/src/ghfc_utils/slivar_reannotator.py
-drwxr-xr-x   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        0 2024-05-14 09:56:05.117123 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)     5492 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/PKG-INFO
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)      365 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)        1 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)       71 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/entry_points.txt
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)       22 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/requires.txt
--rw-r--r--   0 fcliquet (1943789240) PASTEUR\Domain Users (1414054825)       11 2024-05-14 09:56:05.000000 ghfc_utils-0.0.1/src/ghfc_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4736 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       94 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.174895 ghfc_utils-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/src/ghfc_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/src/ghfc_utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12125 2024-05-14 11:35:35.000000 ghfc_utils-0.0.2/src/ghfc_utils/slivar_reannotator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:35:48.178895 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5285 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      336 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-14 11:35:48.000000 ghfc_utils-0.0.2/src/ghfc_utils.egg-info/top_level.txt
```

### Comparing `ghfc_utils-0.0.1/LICENSE` & `ghfc_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghfc_utils-0.0.1/PKG-INFO` & `ghfc_utils-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: ghfc_utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various tools and scripts used in the GHFC lab
 Home-page: https://gitlab.pasteur.fr/ghfc/ghfc-utils
 Author: Freddy Cliquet
 Author-email: freddy.cliquet@pasteur.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: argparse
+Requires-Dist: pyranges
 
 # ghfc-utils
 
 set of small tools designed to help automatize simple task locally or on Pasteur's cluster.
 
 **ghfc-reannotate** for the postprocessing of slivar files including filtering and geneset reannotation.
 
 ## Installation
 
 ```
-pip install git+https://{token_username}:{generated_token}@gitlab.pasteur.fr/ghfc/ghfc-utils.git
-```
-
-when on maestro:
-```
-module load Python/3.9.18
-pip install --user git+https://maestro_tok_FC:rSUDdAJWZutsZTJseJ3V@gitlab.pasteur.fr/ghfc/ghfc-utils.git
+pip install ghfc_utils
 ```
 
 ## slivar reannotator
 
 A tool to filter and reannotate slivar files according to various parameters and genesets. The goal is to produce a more generic kind of slivar files and to use this for the user to run their own filtering.
 
 ```
```

### Comparing `ghfc_utils-0.0.1/README.md` & `ghfc_utils-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,15 @@
 set of small tools designed to help automatize simple task locally or on Pasteur's cluster.
 
 **ghfc-reannotate** for the postprocessing of slivar files including filtering and geneset reannotation.
 
 ## Installation
 
 ```
-pip install git+https://{token_username}:{generated_token}@gitlab.pasteur.fr/ghfc/ghfc-utils.git
-```
-
-when on maestro:
-```
-module load Python/3.9.18
-pip install --user git+https://maestro_tok_FC:rSUDdAJWZutsZTJseJ3V@gitlab.pasteur.fr/ghfc/ghfc-utils.git
+pip install ghfc_utils
 ```
 
 ## slivar reannotator
 
 A tool to filter and reannotate slivar files according to various parameters and genesets. The goal is to produce a more generic kind of slivar files and to use this for the user to run their own filtering.
 
 ```
```

### Comparing `ghfc_utils-0.0.1/setup.cfg` & `ghfc_utils-0.0.2/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ghfc_utils
-version = 0.0.1
+version = v0.0.2
 author = Freddy Cliquet
 author_email = freddy.cliquet@pasteur.fr
 description = Various tools and scripts used in the GHFC lab
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.pasteur.fr/ghfc/ghfc-utils
 licence = MIT License
@@ -19,14 +19,15 @@
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
 	numpy
 	pandas
 	argparse
+	pyranges
 
 [options.package_data]
 * = *.yaml
 
 [options.entry_points]
 console_scripts = 
 	ghfc-reannotate = ghfc_utils:slivar_reannotator.main
```

### Comparing `ghfc_utils-0.0.1/src/ghfc_utils/slivar_reannotator.py` & `ghfc_utils-0.0.2/src/ghfc_utils/slivar_reannotator.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,15 +134,16 @@
             df['impact-category'] = df['impact'].map(dict_rev_impacts, na_action='ignore')
             df['impact-category'] = pd.Categorical(df['impact-category'], categories = ['lof_high','lof_med', 'genic_high', 'genic_med', 'genic_low', 'other_high', 'other_low'], ordered = True)
             df['canonical'] = pd.Categorical(df['canonical'], categories = ['YES', ''], ordered = True)
             df['loftee'] = pd.Categorical(df['loftee'], categories = ['HC', 'OS', '', 'LC'], ordered = True)
             df.sort_values(['sample_id', 'chr:pos:ref:alt', 'ENSG']+config['ordering-priority'], inplace=True)
 
             # aggregating transcripts is done by droping duplicates and keeping only the first (as we sorted using our preferences)
-            df.drop_duplicates(subset = ['sample_id', 'chr:pos:ref:alt', 'ENSG'], keep = 'first', inplace=True)
+            if not args.keep_all:
+                df.drop_duplicates(subset = ['sample_id', 'chr:pos:ref:alt', 'ENSG'], keep = 'first', inplace=True)
             print('after remerging transcripts:', len(df), 'variant/gene/sample')
 
             # filtering on pext
             if 'pext-filter' in config and (len(df)>0):
                 df[['chr', 'position', 'ref', 'alt']] = df['chr:pos:ref:alt'].str.split(':', expand=True)
                 def variant_len(variant):
                         v = variant.split(':')
@@ -187,9 +188,10 @@
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument('configuration', help='config file')
     parser.add_argument('slivar', help='slivar file to reannotate')
     parser.add_argument('output', help='annotated slivar file')
     parser.add_argument('--chunksize', default=100000, help='size of the chunks read from the input (default 100000)', type=int)
+    parser.add_argument('-k', '--keep-all-transcripts', dest='keep_all', help='to keep all impacted transcript instead of the first', default=False, action='store_true')
 
     reannotate(parser.parse_args(args))
```

### Comparing `ghfc_utils-0.0.1/src/ghfc_utils.egg-info/PKG-INFO` & `ghfc_utils-0.0.2/src/ghfc_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 Metadata-Version: 2.1
 Name: ghfc_utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Various tools and scripts used in the GHFC lab
 Home-page: https://gitlab.pasteur.fr/ghfc/ghfc-utils
 Author: Freddy Cliquet
 Author-email: freddy.cliquet@pasteur.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: argparse
+Requires-Dist: pyranges
 
 # ghfc-utils
 
 set of small tools designed to help automatize simple task locally or on Pasteur's cluster.
 
 **ghfc-reannotate** for the postprocessing of slivar files including filtering and geneset reannotation.
 
 ## Installation
 
 ```
-pip install git+https://{token_username}:{generated_token}@gitlab.pasteur.fr/ghfc/ghfc-utils.git
-```
-
-when on maestro:
-```
-module load Python/3.9.18
-pip install --user git+https://maestro_tok_FC:rSUDdAJWZutsZTJseJ3V@gitlab.pasteur.fr/ghfc/ghfc-utils.git
+pip install ghfc_utils
 ```
 
 ## slivar reannotator
 
 A tool to filter and reannotate slivar files according to various parameters and genesets. The goal is to produce a more generic kind of slivar files and to use this for the user to run their own filtering.
 
 ```
```

