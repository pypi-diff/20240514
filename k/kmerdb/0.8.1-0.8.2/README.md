# Comparing `tmp/kmerdb-0.8.1.tar.gz` & `tmp/kmerdb-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kmerdb-0.8.1.tar", last modified: Thu May  9 20:24:48 2024, max compression
+gzip compressed data, was "kmerdb-0.8.2.tar", last modified: Tue May 14 00:19:22 2024, max compression
```

## Comparing `kmerdb-0.8.1.tar` & `kmerdb-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/
--rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.1/LICENSE.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.1/MANIFEST.in
--rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-09 20:24:48.833375 kmerdb-0.8.1/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    13884 2024-04-13 02:30:35.000000 kmerdb-0.8.1/README.md
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.829375 kmerdb-0.8.1/kmerdb/
--rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.1/kmerdb/CITATION.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)   107575 2024-05-09 20:17:53.000000 kmerdb-0.8.1/kmerdb/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.1/kmerdb/__main__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    59984 2024-05-09 20:21:21.000000 kmerdb-0.8.1/kmerdb/appmap.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.1/kmerdb/banners.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    13805 2024-05-09 20:22:40.000000 kmerdb-0.8.1/kmerdb/config.py
--rw-rw-r--   0 matt      (1000) matt      (1000)  1166202 2024-05-09 20:18:07.000000 kmerdb-0.8.1/kmerdb/distance.c
--rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.1/kmerdb/distance.pyx
--rw-rw-r--   0 matt      (1000) matt      (1000)    40090 2024-05-08 05:07:56.000000 kmerdb-0.8.1/kmerdb/fileutil.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    53348 2024-05-08 05:01:16.000000 kmerdb-0.8.1/kmerdb/graph.py
--rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.1/kmerdb/index.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/kmer.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.1/kmerdb/legacy.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/logger.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    19969 2024-04-13 20:20:14.000000 kmerdb-0.8.1/kmerdb/parse.py
--rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.1/kmerdb/probability.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5632 2024-04-13 02:29:52.000000 kmerdb-0.8.1/kmerdb/python_distances.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.1/kmerdb/util.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/kmerdb.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/entry_points.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/not-zip-safe
--rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-05-09 20:24:48.000000 kmerdb-0.8.1/kmerdb.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)     4635 2024-05-09 20:23:12.000000 kmerdb-0.8.1/pyproject.toml
--rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-05-09 20:24:48.833375 kmerdb-0.8.1/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-05-09 20:23:01.000000 kmerdb-0.8.1/setup.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-09 20:24:48.833375 kmerdb-0.8.1/test/
--rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.1/test/test_kmer.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.213420 kmerdb-0.8.2/
+-rw-r--r--   0 matt      (1000) matt      (1000)    11346 2021-01-20 15:15:28.000000 kmerdb-0.8.2/LICENSE.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       28 2024-01-28 00:42:24.000000 kmerdb-0.8.2/MANIFEST.in
+-rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-14 00:19:22.213420 kmerdb-0.8.2/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13884 2024-04-13 02:30:35.000000 kmerdb-0.8.2/README.md
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/kmerdb/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      428 2024-01-28 00:42:24.000000 kmerdb-0.8.2/kmerdb/CITATION.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)   108276 2024-05-13 23:36:34.000000 kmerdb-0.8.2/kmerdb/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      798 2024-01-28 00:42:24.000000 kmerdb-0.8.2/kmerdb/__main__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    60779 2024-05-13 23:14:16.000000 kmerdb-0.8.2/kmerdb/appmap.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1291 2024-03-29 16:31:32.000000 kmerdb-0.8.2/kmerdb/banners.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    14003 2024-05-13 23:07:17.000000 kmerdb-0.8.2/kmerdb/config.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)  1166202 2024-05-13 23:33:04.000000 kmerdb-0.8.2/kmerdb/distance.c
+-rw-r-----   0 matt      (1000) matt      (1000)     2778 2022-07-13 21:42:45.000000 kmerdb-0.8.2/kmerdb/distance.pyx
+-rw-rw-r--   0 matt      (1000) matt      (1000)    40091 2024-05-10 03:18:55.000000 kmerdb-0.8.2/kmerdb/fileutil.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    53348 2024-05-08 05:01:16.000000 kmerdb-0.8.2/kmerdb/graph.py
+-rw-r--r--   0 matt      (1000) matt      (1000)    10823 2021-01-20 15:15:31.000000 kmerdb-0.8.2/kmerdb/index.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    22817 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/kmer.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1497 2024-04-03 23:33:05.000000 kmerdb-0.8.2/kmerdb/legacy.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4594 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/logger.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    19969 2024-04-13 20:20:14.000000 kmerdb-0.8.2/kmerdb/parse.py
+-rw-r--r--   0 matt      (1000) matt      (1000)     6817 2021-01-20 15:15:31.000000 kmerdb-0.8.2/kmerdb/probability.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5632 2024-04-13 02:29:52.000000 kmerdb-0.8.2/kmerdb/python_distances.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1702 2024-04-06 05:24:31.000000 kmerdb-0.8.2/kmerdb/util.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/kmerdb.egg-info/
+-rw-r--r--   0 matt      (1000) matt      (1000)    29907 2024-05-14 00:19:21.000000 kmerdb-0.8.2/kmerdb.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)      624 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/entry_points.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2024-05-09 20:24:48.000000 kmerdb-0.8.2/kmerdb.egg-info/not-zip-safe
+-rw-rw-r--   0 matt      (1000) matt      (1000)      301 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        7 2024-05-14 00:19:22.000000 kmerdb-0.8.2/kmerdb.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4635 2024-05-10 03:20:49.000000 kmerdb-0.8.2/pyproject.toml
+-rw-rw-r--   0 matt      (1000) matt      (1000)      129 2024-05-14 00:19:22.213420 kmerdb-0.8.2/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7003 2024-05-10 03:21:06.000000 kmerdb-0.8.2/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2024-05-14 00:19:22.209420 kmerdb-0.8.2/test/
+-rw-r--r--   0 matt      (1000) matt      (1000)     2575 2021-01-20 15:15:31.000000 kmerdb-0.8.2/test/test_kmer.py
```

### Comparing `kmerdb-0.8.1/LICENSE.txt` & `kmerdb-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/PKG-INFO` & `kmerdb-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.1
+Version: 0.8.2
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `kmerdb-0.8.1/README.md` & `kmerdb-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/__init__.py` & `kmerdb-0.8.2/kmerdb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,15 +211,14 @@
 
 
     from kmerdb import fileutil, config, util, distances
 
 
 
 
-
     global feature
     global step
 
 
     
 
     has_cython = False
@@ -331,28 +330,37 @@
             logger.log_it(e.__str__(), "ERROR")
             logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
             
             raise e
         profiles = np.array(df)
         #profiles = np.transpose(np.array(df))
         columns = list(df.columns)
-        assert profiles.shape[0] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
+
+
+
+        # profiles.shape = [row number, column number]
+        #
+        
+        assert profiles.shape[1] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
         n = len(columns)
 
     elif len(arguments.input) == 1 and (os.path.splitext(arguments.input[0])[-1] == ".tsv" or os.path.splitext(arguments.input[0])[-1] == ".csv"):
 
         feature = 2
         step = 2
         
         try:
             df = pd.read_csv(arguments.input[0], sep=arguments.delimiter)
         except pd.errors.EmptyDataError as e:
-            logger.log_it(e, "ERROR")
             logger.log_it("Pandas error on DataFrame reading. Perhaps a null dataset being read?", "ERROR")
             raise e
+        except FileNotFoundError as e:
+            logger.log_it(e.__str__(), "ERROR")
+            logger.log_it("Input file not found", "ERROR")
+            raise e
         #profiles = np.transpose(np.array(df))
         profiles = np.array(df)
         columns = list(df.columns) # I'm sorry I ever made this line. Please forgive me.
         # This is just gratuitous code and language. I'm really really not sure what I want to express here.
         #assert profiles.shape[0] == len(columns), "distance | Number of columns of dataframe did not match the number of rows of the profile"
         n = len(columns)
     elif len(arguments.input) == 1 and os.path.splitext(arguments.input[0])[-1] == ".kdb":
@@ -763,19 +771,19 @@
         plt.savefig(config.pca_variance_fig_filepath)
 
         if arguments.n is not None:
             logger.log_it("Using selected PCA dimensionality to reduce the transpose matrix/DataFrame again for use in 'kdb kmeans'", "INFO")
             pca = PCA(n_components=arguments.n)
             pca.fit(np.transpose(df))
             sys.stderr.write("\n\n\n")
-            sys.stderr.write("-"*30)
+            sys.stderr.write("-"*30+ "\n")
             
             sys.stderr.write("Explained variances: {0}\n".format(pca.explained_variance_ratio_))
-            sys.stderr.write("Log-likelihoods: {0}\n".format(pca.score_samples(normalized)))
-            sys.stderr.write("Log-likelihood of all samples: {0}\n".format(pca.score(normalized)))
+            sys.stderr.write("Log-likelihoods: {0}\n".format(pca.score_samples(np.transpose(df))))
+            sys.stderr.write("Log-likelihood of all samples: {0}\n".format(pca.score(np.transpose(df))))
             sys.stderr.write("MLE estimate of components for dimensionality reduction produced this shape: {0}\n".format(pca.components_.shape))
 
             score_matrix = pca.transform(np.transpose(df))
             score_df = pd.DataFrame(np.transpose(score_matrix), columns=columns)
 
             #score_df.to_csv(sys.stdout, sep=arguments.delimiter, index=arguments.with_index)
             final_df = score_df
@@ -1103,45 +1111,46 @@
     Another end-user function that takes an argparse Namespace object.
     This function just reads the metadata header, can print in json.
     """
     from kmerdb import fileutil, config, util, graph
 
     sfx = os.path.splitext(arguments.kdb)[-1]
     metadata = None
-    
+
     if sfx != ".kdb" and sfx != ".kdbg": # A filepath with invalid suffix
         raise IOError("Viewable .kdb(g) filepath does not end in '.kdb' or '.kdbg'")
     elif not os.path.exists(arguments.kdb):
         raise IOError("Input .kdb(g) filepath '{0}' does not exist on the filesystem".format(arguments.kdb_in))
 
     if sfx == ".kdb":
-        kdb = fileutil.open(arguments.kdb, mode='r', sort=arguments.re_sort, slurp=True)
+        kdb = fileutil.open(arguments.kdb, mode='r', sort=False, slurp=False)
         metadata = kdb.metadata
             
         kmer_ids_dtype = metadata["kmer_ids_dtype"]
         N = 4**metadata["k"]
         if metadata["version"] != config.VERSION:
             logger.log_it(".kdb version is out of date, may be incompatible with current KDBReader class", "WARNING")
 
         assert kdb.kmer_ids.size == N, "view | read kmer_ids size did not match N from the header metadata"
         assert kdb.counts.size == N, "view | read counts size did not match N from the header metadata"
         assert kdb.frequencies.size == N, "view | read frequencies size did not match N from the header metadata"
         metadata = kdb.metadata
     elif sfx == ".kdbg":
-        kdb = graph.open(arguments.kdb, mode='r')
+        kdb = graph.open(arguments.kdb, mode='r', slurp=False)
         if kdb.metadata["version"] != config.VERSION:
             logger.log_it(".kdb file version is out of date, may be incompatible with current fileutil.KDBReader class", "WARNING")
 
 
             
         N = 4**kdb.metadata["k"]
         metadata = kdb.metadata
 
     else:
         raise ValueError("Input to 'kmerdb header' is a .kdb or .kdbg (gzipped .tsv) file of a count vector or a graph. Requires YAML metadata header.Try creating a k-mer count profile with 'kmerdb profile' or edge list with 'kmerdb graph'")
+
     if arguments.json:
         print(dict(kdb.metadata))
     else:
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
         print(yaml.dump(metadata))
         print(config.header_delimiter)
             
@@ -1204,15 +1213,15 @@
             
             kmer_ids_dtype = metadata["kmer_ids_dtype"]
             N = 4**metadata["k"]
             if metadata["version"] != config.VERSION:
                 logger.log_it("KDB version is out of date, may be incompatible with current KDBReader class", "WARNING")
             if arguments.kdb_out is None or (arguments.kdb_out == "/dev/stdout" or arguments.kdb_out == "STDOUT"): # Write to stdout, uncompressed
                 if arguments.header:
-                    yaml.add_representer(OrderedDict, util.represent_ordereddict)
+                    yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
                     print(yaml.dump(metadata, sort_keys=False))
                     print(config.header_delimiter)
             logger.log_it("Reading from file...", "INFO")
 
             
             
             try:
@@ -1949,22 +1958,22 @@
         np.dtype(metadata["count_dtype"])
         np.dtype(metadata["frequencies_dtype"])
     except TypeError as e:
         logger.log_it(e.__str__(), "ERROR")
 
         raise TypeError("Incorrect dtype.")
 
-    logger.log_it("Initializing Numpy array of {0} uint zeroes for the final composite profile...".format(total_kmers), "ERROR")
+    logger.log_it("Initializing Numpy array of {0} uint zeroes for the final composite profile...".format(total_kmers), "DEBUG")
     
     kmer_ids = np.array(range(N), dtype=metadata["kmer_ids_dtype"])
     profile = np.array(range(N), dtype=metadata["profile_dtype"])
     counts = np.array(counts, dtype=metadata["count_dtype"])
     frequencies = np.divide(counts, metadata["total_kmers"])
     
-    logger.log_it("Initialization of profile completed, using approximately {0} bytes per profile".format(counts.nbytes), "INFO")
+    logger.log_it("Initialization of profile completed, using approximately {0} bytes for profile".format(counts.nbytes), "INFO")
     
     yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
     sys.stderr.write(yaml.dump(metadata, sort_keys=False))
 
     
     step += 1
 
@@ -2057,15 +2066,15 @@
         if citation == "":
             return
         else:
             sys.stderr.write("Printing citation notice to stderr. This will not interfere with the execution of the program in any way. Please see CITATION_FAQ.md for any questions.\n")
             sys.stderr.write(citation + "\n\n\n")
             sys.stderr.write("Run 'kmerdb citation' to silence.\n")
     else:
-        sys.stderr.write("Thanks for using/citing kmerdb")
+        sys.stderr.write("Thanks for using/citing kmerdb\n")
     # else:
     #     raise IOError("Cannot locate the extra package data file 'kmerdb/CITATION', which should have been distributed with the program")
 
 
 def get_program_header(arguments):
     import appmap
     import sys
@@ -2339,14 +2348,15 @@
     citation_parser.add_argument("-v", "--verbose", help="Prints warnings to the console by default", default=0, action="count")
     citation_parser.add_argument("--debug", action="store_true", default=False, help="Debug mode. Do not format errors and condense log")
     citation_parser.add_argument("-nl", "--num-log-lines", type=int, choices=config.default_logline_choices, default=50, help=argparse.SUPPRESS)
     citation_parser.add_argument("-l", "--log-file", type=str, default="kmerdb.log", help="Destination path to log file")
     citation_parser.set_defaults(func=citation)
 
     args=parser.parse_args()
+    
     global logger
     global exit_code
 
     
     global step
     global feature
 
@@ -2377,40 +2387,44 @@
     logger = kdbLogger.Loggah(logfile=args.log_file or None, level=args.verbose)
         
 
     from kmerdb import appmap
     kmerdb_appmap = appmap.kmerdb_appmap( argv , logger )
     kmerdb_appmap.print_program_header()
 
-    sys.stderr.write("Beginning program...\n")
 
 
+    
+    sys.stderr.write("Beginning program...\n")
+
     if args.debug is True:
         args.func(args)
     else:
+        logger.log_it("Running with error summary feature enabled, bypass with --debug for vague/invalid exceptions", "DEBUG")
+        
         try:
-
             args.func(args)
+            
             exit_code = 0
 
         except TypeError as e:
-
-            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 1
         
             raise e
         except ValueError as e:
         
-            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 2
         
             raise e
         except KeyError as e:
         
-            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, traceback=traceback, step=step, feature=feature, logs=logger.logs, n_logs=args["n_logs"])
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 3
         
             raise e
         except RuntimeError as e:
         
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 4
@@ -2419,29 +2433,35 @@
         except OSError as e:
 
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 5
         
             raise e
         except ArgumentError as e:
-        
+
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 6
         
             raise e
         except AssertionError as e:
-        
+
+            print("CAUGHT ASSERTION ERROR")
+            
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = 7
         
             raise e
+        except FileNotFoundError as e:
+            exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
+            
+            exit_code = 8
+            raise e
         except Exception as e:
             exit_summary = kmerdb_appmap.exit_gracefully(e , subcommand=subcommand_name, step=step, feature=feature, logs=logger.logs, n_logs=args.num_log_lines or None)
             exit_code = -1
         
             raise e
         finally:
-
             sys.stderr.write("Program ran for {0} seconds...\n\n\n".format(time.time() - start))
             sys.stderr.write(config.thanks)
             sys.stderr.write(config.DONE)
             sys.exit(exit_code)
```

### Comparing `kmerdb-0.8.1/kmerdb/__main__.py` & `kmerdb-0.8.2/kmerdb/__main__.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/appmap.py` & `kmerdb-0.8.2/kmerdb/appmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1866,20 +1866,77 @@
             "description": "(Deprecated)"
         })
 
     ]
 
 })
 
+ALL_PARAMS = {
+    "profile": COMMAND_1_PARAMS["items"],
+    "make_graph": COMMAND_2_PARAMS["items"],
+    "get_matrix": COMMAND_3_PARAMS["items"],
+    "distance": COMMAND_4_PARAMS["items"],
+    "view": COMMAND_5_PARAMS["items"],
+    "header": COMMAND_6_PARAMS["items"],
+    "kmeans": COMMAND_7_PARAMS["items"],
+    "hierarchical": COMMAND_8_PARAMS["items"],
+    "index": COMMAND_9_PARAMS["items"],
+    "shuf": COMMAND_10_PARAMS["items"]
+
+}
+
+ALL_INPUTS = {
+    "profile": COMMAND_1_INPUTS["items"],
+    "make_graph": COMMAND_2_INPUTS["items"],
+    "get_matrix": COMMAND_3_INPUTS["items"],
+    "distance": COMMAND_4_INPUTS["items"],
+    "view": COMMAND_5_INPUTS["items"],
+    "header": COMMAND_6_INPUTS["items"],
+    "kmeans": COMMAND_7_INPUTS["items"],
+    "hierarchical": COMMAND_8_INPUTS["items"],
+    "index": COMMAND_9_INPUTS["items"],
+    "shuf": COMMAND_10_INPUTS["items"]
+}
+
+ALL_FEATURES = {
+    "profile": COMMAND_1_FEATURES["items"],
+    "make_graph": COMMAND_2_FEATURES["items"],
+    "get_matrix": COMMAND_3_FEATURES["items"],
+    "distances": COMMAND_4_FEATURES["items"],
+    "view": COMMAND_5_FEATURES["items"],
+    "header": COMMAND_6_FEATURES["items"],
+    "kmeans": COMMAND_7_FEATURES["items"],
+    "hierarchical": COMMAND_8_FEATURES["items"],
+    "index": COMMAND_9_FEATURES["items"],
+    "shuf": COMMAND_10_FEATURES["items"]
+
+
+}
+
+
+ALL_STEPS = {
+
+    "profile": COMMAND_1_STEPS["items"],
+    "make_graph": COMMAND_2_STEPS["items"],
+    "get_matrix": COMMAND_3_STEPS["items"],
+    "distances": COMMAND_4_STEPS["items"],
+    "view": COMMAND_5_STEPS["items"],
+    "header": COMMAND_6_STEPS["items"],
+    "kmeans": COMMAND_7_STEPS["items"],
+    "hierarchical": COMMAND_8_STEPS["items"],
+    "index": COMMAND_9_STEPS["items"],
+    "shuf": COMMAND_10_STEPS["items"]
+}
 
-class kmerdb_appmap:
 
 
 
         
+class kmerdb_appmap:
+
 
 
     
     def __init__(self, argv, logger=None):
 
 
         if logger is not None:
@@ -1924,70 +1981,14 @@
 
 
 
 
         
 
 
-        self.ALL_PARAMS = {
-            "profile": COMMAND_1_PARAMS["items"],
-            "make_graph": COMMAND_2_PARAMS["items"],
-            "get_matrix": COMMAND_3_PARAMS["items"],
-            "distance": COMMAND_4_PARAMS["items"],
-            "view": COMMAND_5_PARAMS["items"],
-            "header": COMMAND_6_PARAMS["items"],
-            "kmeans": COMMAND_7_PARAMS["items"],
-            "hierarchical": COMMAND_8_PARAMS["items"],
-            "index": COMMAND_9_PARAMS["items"],
-            "shuf": COMMAND_10_PARAMS["items"]
-
-        }
-
-        ALL_INPUTS = {
-            "profile": COMMAND_1_INPUTS["items"],
-            "make_graph": COMMAND_2_INPUTS["items"],
-            "get_matrix": COMMAND_3_INPUTS["items"],
-            "distance": COMMAND_4_INPUTS["items"],
-            "view": COMMAND_5_INPUTS["items"],
-            "header": COMMAND_6_INPUTS["items"],
-            "kmeans": COMMAND_7_INPUTS["items"],
-            "hierarchical": COMMAND_8_INPUTS["items"],
-            "index": COMMAND_9_INPUTS["items"],
-            "shuf": COMMAND_10_INPUTS["items"]
-        }
-
-        ALL_FEATURES = {
-            "profile": COMMAND_1_FEATURES["items"],
-            "make_graph": COMMAND_2_FEATURES["items"],
-            "get_matrix": COMMAND_3_FEATURES["items"],
-            "distance": COMMAND_4_FEATURES["items"],
-            "view": COMMAND_5_FEATURES["items"],
-            "header": COMMAND_6_FEATURES["items"],
-            "kmeans": COMMAND_7_FEATURES["items"],
-            "hierarchical": COMMAND_8_FEATURES["items"],
-            "index": COMMAND_9_FEATURES["items"],
-            "shuf": COMMAND_10_FEATURES["items"]
-
-
-        }
-
-
-        ALL_STEPS = {
-
-            "profile": COMMAND_1_STEPS["items"],
-            "make_graph": COMMAND_2_STEPS["items"],
-            "get_matrix": COMMAND_3_STEPS["items"],
-            "distance": COMMAND_4_STEPS["items"],
-            "view": COMMAND_5_STEPS["items"],
-            "header": COMMAND_6_STEPS["items"],
-            "kmeans": COMMAND_7_STEPS["items"],
-            "hierarchical": COMMAND_8_STEPS["items"],
-            "index": COMMAND_9_STEPS["items"],
-            "shuf": COMMAND_10_STEPS["items"]
-        }
         
         # KMEANS_BANNER = """
         #                   name : kmeans
         #            description : 
         # """
 
         # HIERARCHICAL_BANNER = """
@@ -2353,96 +2354,120 @@
         
 
     def exit_gracefully(self, e:Exception, subcommand:str=None, step:int=None, feature:int=None, logs:list=None, n_logs:int=None):
         """
         We need to handle exit gracefully. The 'step' and 'feature' categories/flags/ints are passed from __init__ or down its callstack to 
         """
         import traceback
-        
 
-        if e is None:
-            raise ValueError("Need an error to exit")
-        elif not isinstance(e, Exception):
-            raise ValueError("Need an error to exit")
+
+        # if e is None:
+        #     raise ValueError("Need an error to exit")
+        # elif not isinstance(e, Exception):
+        #     raise ValueError("Need an error to exit")
 
         
-        if n_logs is None or type(n_logs) is not int:
-            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument n_logs to be a int")
-        elif logs is None or type(logs) is not list:
-            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument logs to be a list")
-        elif feature is not None and type(feature) is not int:
-            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument feature to be a int")
-        elif step is not None and type(step) is not int:
-            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument step to be a int")
-        elif subcommand is not None and type(subcommand) is not str:
-            raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument subcommand to be a str")
+        # if n_logs is None or type(n_logs) is not int:
+        #     raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument n_logs to be a int")
+        # elif logs is None or type(logs) is not list:
+        #     raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument logs to be a list")
+        # elif feature is not None and type(feature) is not int:
+        #     raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument feature to be a int")
+        # elif step is not None and type(step) is not int:
+        #     raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument step to be a int")
+        # elif subcommand is not None and type(subcommand) is not str:
+        #     raise TypeError("kmerdb.appmap.exit_gracefully expects the keyword argument subcommand to be a str")
 
 
 
         
-        N = len(logs) 
-        loggable_line = N
-        assert subcommand in config.subcommands, "Unknown subcommand"
-
-
+        N = min(len(logs), n_logs)
 
+        tb = traceback.extract_tb(e.__traceback__)
+        last_traceback_FrameSummary = tb[-1]
+        error_file_name = last_traceback_FrameSummary.filename
+        error_line_number = last_traceback_FrameSummary.lineno
 
         
+        #assert subcommand in config.subcommand_functions, "Unknown subcommand"
 
+        if self._loggable:
+            self.logger.log_it("Program error! Collecting error metadata and formatting...", "ERROR")
         # This is the "Error blocks" metadata
-        exit_summary = OrderedDict({
+
+        # print(subcommand)
+        # print(config.VERSION)
+        # print(config.REQUIRES_PYTHON)
+        # print(feature)
+        # print(ALL_FEATURES[subcommand][feature]["name"])
+        # print(ALL_FEATURES[subcommand][feature]["shortname"])
+        # print(ALL_FEATURES[subcommand][feature]["description"])
+        # print(step)
+        # print(ALL_STEPS[subcommand][step]["name"])
+        # print(ALL_STEPS[subcommand][step]["shortname"])
+        # print(ALL_STEPS[subcommand][step]["description"])
+        #     # The *total* number of logged lines produced by the program and returned to the global 'logs' var in __init__.py
+        # print(self.logfile)
+        # print(str(tb))
+        # print(error_file_name)
+        # print(error_line_number)
+        # print(e.__str__())
+
+        
+        e_sum = {
             "subcommand": subcommand,
             "kmerdb-version": config.VERSION,
             "python-version": config.REQUIRES_PYTHON,
             "feature": feature,
-            "feature_name": self.ALL_FEATURES[subcommand][feature]["name"],
-            "feature_shortname": self.ALL_FEATURES[subcommand][feature]["shortname"],
-            "feature_description": self.ALL_FEATURES[subcommand][feature]["description"],
+            "feature_name": ALL_FEATURES[subcommand][feature]["name"],
+            "feature_shortname": ALL_FEATURES[subcommand][feature]["shortname"],
+            "feature_description": ALL_FEATURES[subcommand][feature]["description"],
             "step" : step,
-            "step_name": self.ALL_STEPS[subcommand][step]["name"],
-            "step_shortname": self.ALL_STEPS[subcommand][step]["shortname"],
-            "step_description": self.ALL_STEPS[subcommand][step]["description"],
+            "step_name": ALL_STEPS[subcommand][step]["name"],
+            "step_shortname": ALL_STEPS[subcommand][step]["shortname"],
+            "step_description": ALL_STEPS[subcommand][step]["description"],
             # The *total* number of logged lines produced by the program and returned to the global 'logs' var in __init__.py
             "log_file": self.logfile,
-            "traceback": str(traceback.extract_tb(e.__traceback__)),
-            "last_logged_line": loggable_line, 
+            "traceback": str(tb),
+            "error_file_name": error_file_name,
+            "error_line_number": error_line_number,
             "error": e.__str__(),
-        })
+        }
 
+        
+        exit_summary = OrderedDict(e_sum)
 
+        
         yaml.add_representer(OrderedDict, util.represent_yaml_from_collections_dot_OrderedDict)
         
 
         try:
             jsonschema.validate(instance=exit_summary, schema=config.exit_summary_schema)
         except jsonschema.ValidationError as e:
             sys.stderr.write("Failed to validate the exit summary. Internal Error.\n")
             raise e
                 
-
-
-
-
-
-
-
         self.print_github_block()
 
         """
         Print last n lines of log
         """
-        for i in range(n_logs):
+
+
+
+        
+        for i in range(N):
 
             try:
                 if self._loggable:
                     sys.stderr.write("{0} - last line of log\n".format(n_logs - i))
                     self.logger.log_it(logs[i], "ERROR")
                 else:
                     sys.stderr.write("{0} - last line of log\n".format(n_logs - i))
-                    sys.stderr.write(logs[i], "ERROR")
+                    sys.stderr.write(logs[i])
             except Exception as e:
                 raise e
                 
         sys.stderr.write("-" * 80 + "\n")
         if self._loggable:
             
             self.logger.log_it("...displaying last {0} lines of the log. Please see '{1}' for more details...".format(n_logs, self.logfile), "ERROR")
```

### Comparing `kmerdb-0.8.1/kmerdb/banners.py` & `kmerdb-0.8.2/kmerdb/banners.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/config.py` & `kmerdb-0.8.2/kmerdb/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,24 +13,26 @@
    See the License for the specific language governing permissions and
    limitations under the License.
 
 '''
 
 
 
-VERSION="0.8.1"
+VERSION="0.8.2"
 REQUIRES_PYTHON="3.7.4"
 header_delimiter = "\n" + ("="*24) + "\n"
 
 
-requirements_count = 8
-requirements_dev_count = 14 # 4/9/24 there are some duplicates sure, but the requirements evolve faster than the dev do, are more essential for function, and I dont change the -dev file much. 
+requirements_count = 9
+requirements_dev_count = 9 # 4/9/24 there are some duplicates sure, but the requirements evolve faster than the dev do, are more essential for function, and I dont change the -dev file much. 
 
 subcommands = ["usage", "help", "profile", "graph", "index", "shuf", "matrix", "distance"] # kmeans and hierarchical and probability commands deprecated
-subcommand_functions = ("profile", "make_graph", "get_matrix", "index_file", "distances", "kmeans", "hierarchical",)
+subcommand_functions = ["expanded_help", "profile", "make_graph", "get_matrix", "index_file", "shuf", "get_matrix", "distances"]
+
+#subcommand_functions = ("profile", "make_graph", "get_matrix", "index_file", "distances", "kmeans", "hierarchical",)
 default_logline_choices = (20, 50, 100, 200)
 KDB_COLUMN_NUMBER = 4
 
 
 
 graph_schema = {
     "type": "object",
@@ -146,18 +148,19 @@
         "feature_description": {"type": "string"},
         "step": {"type": "number"},
         "step_name": {"type": "string"},
         "step_shortname": {"type": "string"},
         "step_description": {"type": "string"},
         "log_file": {"type": "string"},
         "traceback": {"type": "string"},
-        "last_logged_line": {"type": "number"},
+        "error_file_name": {"type": "string"},
+        "error_line_number": {"type": "number"},
         "error": {"type": "string"},        
     },
-    "required": ["subcommand", "kmerdb-version", "python-version", "feature", "feature_name", "feature_shortname", "feature_description", "step", "step_name", "step_shortname", "step_description", "traceback", "last_logged_line", "error", ]
+    "required": ["subcommand", "kmerdb-version", "python-version", "feature", "feature_name", "feature_shortname", "feature_description", "step", "step_name", "step_shortname", "step_description", "traceback", "error_file_name", "error_line_number", "error", ]
 }
```

### Comparing `kmerdb-0.8.1/kmerdb/distance.c` & `kmerdb-0.8.2/kmerdb/distance.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/core/include"
+            "/_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "kmerdb.distance",
         "sources": [
             "kmerdb/distance.pyx"
         ]
     },
     "module_name": "kmerdb.distance"
@@ -1674,177 +1674,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1877,42 +1877,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18030,261 +18030,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18293,29 +18293,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18326,15 +18326,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18343,29 +18343,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18376,15 +18376,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18393,29 +18393,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18426,15 +18426,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18443,29 +18443,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18476,15 +18476,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18493,29 +18493,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18526,217 +18526,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 970, __pyx_L1_error)
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18752,15 +18752,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18768,68 +18768,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 982, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18837,15 +18837,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18860,15 +18860,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18884,15 +18884,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18900,68 +18900,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 988, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18969,15 +18969,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18992,15 +18992,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19016,15 +19016,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19032,68 +19032,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 994, __pyx_L3_error)
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19101,15 +19101,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19124,170 +19124,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22077,26 +22077,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-ns374l82/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../_dev/hot/_10+/tmp/pip-build-env-5qsf0315/overlay/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 990, __pyx_L1_error)
```

### Comparing `kmerdb-0.8.1/kmerdb/distance.pyx` & `kmerdb-0.8.2/kmerdb/distance.pyx`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/fileutil.py` & `kmerdb-0.8.2/kmerdb/fileutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,15 +394,15 @@
 
 {0}
 
  ...then try again to view the header with 'kmerdb header' or the whole file : 'kmerdb view -H kmer_count_vector.12.kdb'
 
 
 
-""".format(appmap.command_1_usage, "ERROR")
+""".format(appmap.command_1_usage, "ERROR"))
 
                 self.logger.log_it(e.__str__, "ERROR")
             raise ValueError("Requires kmerdb v{0} format YAML header. Body is .tsv format table, .bgzf file.      - k-mer count vector        (idx, k-mer id, count, frequency)".format(config.VERSION))
```

### Comparing `kmerdb-0.8.1/kmerdb/graph.py` & `kmerdb-0.8.2/kmerdb/graph.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/index.py` & `kmerdb-0.8.2/kmerdb/index.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/kmer.py` & `kmerdb-0.8.2/kmerdb/kmer.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/legacy.py` & `kmerdb-0.8.2/kmerdb/legacy.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/logger.py` & `kmerdb-0.8.2/kmerdb/logger.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/parse.py` & `kmerdb-0.8.2/kmerdb/parse.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/probability.py` & `kmerdb-0.8.2/kmerdb/probability.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/python_distances.py` & `kmerdb-0.8.2/kmerdb/python_distances.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb/util.py` & `kmerdb-0.8.2/kmerdb/util.py`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/kmerdb.egg-info/PKG-INFO` & `kmerdb-0.8.2/kmerdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: kmerdb
-Version: 0.8.1
+Version: 0.8.2
 Summary: Yet another corretion to the 'yet another correction to just a k-mer counter...'
 Home-page: https://github.com/MatthewRalston/kmerdb
-Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz
+Download-URL: https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz
 Author: fross
 Author-email: "Matt Ralston <mralston.development@gmail.com>" <mralston.development@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `kmerdb-0.8.1/kmerdb.egg-info/SOURCES.txt` & `kmerdb-0.8.2/kmerdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kmerdb-0.8.1/pyproject.toml` & `kmerdb-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # requires numpy and cython for custom cython correlation function
 
 requires = ["setuptools>=69.2.0", "numpy>=1.21.2", "Cython>=3.0.8"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kmerdb"
-version = "0.8.1"
+version = "0.8.2"
 description = "Yet another corretion to the 'yet another correction to just a k-mer counter...'"
 readme = "README.md"
 authors = [{name="Matt Ralston <mralston.development@gmail.com>", email="mralston.development@gmail.com"}]
 license = { file = "LICENSE.txt" }
 classifiers = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
```

### Comparing `kmerdb-0.8.1/setup.py` & `kmerdb-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,20 +105,20 @@
         return None
                 
 # Package meta-data.
 NAME = 'kmerdb'
 DESCRIPTION = 'Yet another kmer library for Python'
 long_description = 'See README.md for details'
 URL = 'https://github.com/MatthewRalston/kmerdb'
-CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.8.1.tar.gz"
+CURRENT_RELEASE = "https://github.com/MatthewRalston/kmerdb/archive/v0.8.2.tar.gz"
 EMAIL = 'mralston.development@gmail.com'
 AUTHOR = 'fross'
 REQUIRES_PYTHON = ">=3.7.4"
 #REQUIRES_PYTHON = '>=3.12.2'
-VERSION = "0.8.1"
+VERSION = "0.8.2"
 KEYWORDS = ["bioinformatics", "fastq", "fasta", "k-mer", "kmer"]
 CLASSIFIERS = [
 	    "Development Status :: 1 - Planning",
 	    "Development Status :: 2 - Pre-Alpha",
 	    "Development Status :: 7 - Inactive",
 	    "Environment :: Console",
 	    "Intended Audience :: Developers",
```

### Comparing `kmerdb-0.8.1/test/test_kmer.py` & `kmerdb-0.8.2/test/test_kmer.py`

 * *Files identical despite different names*

