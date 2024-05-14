# Comparing `tmp/drex-0.0.2434.tar.gz` & `tmp/drex-0.0.244.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drex-0.0.2434.tar", last modified: Thu Apr 18 09:06:35 2024, max compression
+gzip compressed data, was "drex-0.0.244.tar", last modified: Fri Apr 26 18:14:01 2024, max compression
```

## Comparing `drex-0.0.2434.tar` & `drex-0.0.244.tar`

### file list

```diff
@@ -1,39 +1,58 @@
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       98 2024-03-29 18:39:48.000000 drex-0.0.2434/.gitignore
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      721 2024-04-18 09:06:35.259033 drex-0.0.2434/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-04 15:50:32.000000 drex-0.0.2434/README.md
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.255033 drex-0.0.2434/data/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2912 2024-03-26 20:01:38.000000 drex-0.0.2434/data/10MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7032 2024-03-26 20:01:41.000000 drex-0.0.2434/data/1MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.2434/data/200MB.csv
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1303 2024-03-26 20:01:44.000000 drex-0.0.2434/data/50MB.csv
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.255033 drex-0.0.2434/drex/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.2434/drex/__init__.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/drex/schedulers/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      576 2024-04-17 08:25:26.000000 drex-0.0.2434/drex/schedulers/algorithm1.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1438 2024-04-17 09:15:25.000000 drex-0.0.2434/drex/schedulers/algorithm2.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3158 2024-04-17 09:28:40.000000 drex-0.0.2434/drex/schedulers/algorithm3.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1686 2024-04-17 10:28:07.000000 drex-0.0.2434/drex/schedulers/random.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/drex/utils/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.2434/drex/utils/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      784 2024-03-26 21:04:00.000000 drex-0.0.2434/drex/utils/load_data.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.2434/drex/utils/poibin.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/drex/utils/reliability/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.2434/drex/utils/reliability/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.2434/drex/utils/reliability/fragment_handler.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7971 2024-04-18 09:02:32.000000 drex-0.0.2434/drex/utils/reliability/ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.2434/drex/utils/reliability/utils.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5350 2024-04-15 08:30:49.000000 drex-0.0.2434/drex/utils/tool_functions.py
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/drex.egg-info/
--rw-r--r--   0 domizzi   (1000) domizzi   (1000)      721 2024-04-18 09:06:35.000000 drex-0.0.2434/drex.egg-info/PKG-INFO
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      670 2024-04-18 09:06:35.000000 drex-0.0.2434/drex.egg-info/SOURCES.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-04-18 09:06:35.000000 drex-0.0.2434/drex.egg-info/dependency_links.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       12 2024-04-18 09:06:35.000000 drex-0.0.2434/drex.egg-info/requires.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-04-18 09:06:35.000000 drex-0.0.2434/drex.egg-info/top_level.txt
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      596 2024-04-18 09:06:16.000000 drex-0.0.2434/pyproject.toml
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-04-18 09:06:35.259033 drex-0.0.2434/setup.cfg
-drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-18 09:06:35.259033 drex-0.0.2434/test/
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 11:45:13.000000 drex-0.0.2434/test/__init__.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2150 2024-04-17 08:36:19.000000 drex-0.0.2434/test/drex-test.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      327 2024-04-17 15:00:11.000000 drex-0.0.2434/test/test-ida.py
--rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      328 2024-04-17 15:00:41.000000 drex-0.0.2434/test/test-ida2.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.546252 drex-0.0.244/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       98 2024-03-29 18:39:48.000000 drex-0.0.244/.gitignore
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-04-26 18:14:01.546252 drex-0.0.244/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      335 2024-04-04 15:50:32.000000 drex-0.0.244/README.md
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.518252 drex-0.0.244/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4011 2024-04-19 16:55:19.000000 drex-0.0.244/data/100MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2929 2024-04-22 09:11:47.000000 drex-0.0.244/data/10MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2933 2024-04-22 09:11:39.000000 drex-0.0.244/data/1MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2903 2024-03-26 20:01:25.000000 drex-0.0.244/data/200MB.csv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3915 2024-04-22 09:06:02.000000 drex-0.0.244/data/50MB.csv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.518252 drex-0.0.244/drex/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:09:29.000000 drex-0.0.244/drex/__init__.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.518252 drex-0.0.244/drex/inputs/
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.534252 drex-0.0.244/drex/inputs/data/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)  3971043 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/data/FB-samples-combined.json
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      260 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/data/README.md
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      333 2024-04-25 20:22:04.000000 drex-0.0.244/drex/inputs/data/data.json
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.538252 drex-0.0.244/drex/inputs/data/raw/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   198743 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_0.tsv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   223858 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/data/raw/FB-2009_samples_24_times_1hr_1.tsv
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)   898688 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/data/raw/FB-2010_samples_24_times_1hr_0.tsv
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.542252 drex-0.0.244/drex/inputs/nodes/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      209 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/nodes/README.md
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1541 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/nodes/nodes_1.json
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.542252 drex-0.0.244/drex/inputs/parsing_code/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2385 2024-04-26 07:52:45.000000 drex-0.0.244/drex/inputs/parsing_code/parse_SWIM_map_reduce.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.542252 drex-0.0.244/drex/schedulers/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      955 2024-04-25 10:11:30.000000 drex-0.0.244/drex/schedulers/algorithm1.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8261 2024-04-26 08:50:19.000000 drex-0.0.244/drex/schedulers/algorithm2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3561 2024-04-26 09:11:46.000000 drex-0.0.244/drex/schedulers/algorithm3.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     7683 2024-04-26 08:52:11.000000 drex-0.0.244/drex/schedulers/algorithm4.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1803 2024-04-25 10:11:30.000000 drex-0.0.244/drex/schedulers/random.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.546252 drex-0.0.244/drex/utils/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:13.000000 drex-0.0.244/drex/utils/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1486 2024-04-25 20:04:38.000000 drex-0.0.244/drex/utils/load_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    10547 2024-03-26 19:02:20.000000 drex-0.0.244/drex/utils/poibin.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2034 2024-04-26 09:10:23.000000 drex-0.0.244/drex/utils/prediction.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.546252 drex-0.0.244/drex/utils/reliability/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-03-28 21:06:19.000000 drex-0.0.244/drex/utils/reliability/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     5214 2024-03-28 16:17:33.000000 drex-0.0.244/drex/utils/reliability/fragment_handler.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     8647 2024-04-18 11:31:42.000000 drex-0.0.244/drex/utils/reliability/ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     4913 2024-03-28 16:17:33.000000 drex-0.0.244/drex/utils/reliability/utils.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)    15563 2024-04-25 10:11:30.000000 drex-0.0.244/drex/utils/tool_functions.py
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.546252 drex-0.0.244/drex.egg-info/
+-rw-r--r--   0 domizzi   (1000) domizzi   (1000)      770 2024-04-26 18:14:01.000000 drex-0.0.244/drex.egg-info/PKG-INFO
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     1163 2024-04-26 18:14:01.000000 drex-0.0.244/drex.egg-info/SOURCES.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        1 2024-04-26 18:14:01.000000 drex-0.0.244/drex.egg-info/dependency_links.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       32 2024-04-26 18:14:01.000000 drex-0.0.244/drex.egg-info/requires.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        5 2024-04-26 18:14:01.000000 drex-0.0.244/drex.egg-info/top_level.txt
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      629 2024-04-26 18:13:31.000000 drex-0.0.244/pyproject.toml
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)       38 2024-04-26 18:14:01.546252 drex-0.0.244/setup.cfg
+drwxrwxr-x   0 domizzi   (1000) domizzi   (1000)        0 2024-04-26 18:14:01.546252 drex-0.0.244/test/
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)        0 2024-04-17 11:45:13.000000 drex-0.0.244/test/__init__.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     3528 2024-04-26 09:11:31.000000 drex-0.0.244/test/drex-test.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      414 2024-04-25 20:04:38.000000 drex-0.0.244/test/filter_data.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      325 2024-04-18 11:31:59.000000 drex-0.0.244/test/test-ida.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)      328 2024-04-17 15:00:41.000000 drex-0.0.244/test/test-ida2.py
+-rw-rw-r--   0 domizzi   (1000) domizzi   (1000)     2757 2024-04-26 09:02:34.000000 drex-0.0.244/test/test_linearregression.py
```

### Comparing `drex-0.0.2434/PKG-INFO` & `drex-0.0.244/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.2434
+Version: 0.0.244
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # D-rex
 
 Dynamic replication for heterogeneous storage nodes.
 
 Maxime GONTHIER - Dante - Haochen
```

### Comparing `drex-0.0.2434/data/10MB.csv` & `drex-0.0.244/data/10MB.csv`

 * *Files 16% similar despite different names*

```diff
@@ -1,129 +1,113 @@
 n	k	avg_time
-2	1	27.50726233
-3	1	34.59417131
 3	2	19.28857229
-4	1	43.37876928
 4	2	24.63187528
 4	3	17.51573498
-5	1	52.97134509
 5	2	29.44641221
 5	3	21.37515559
 5	4	17.3750212
-6	1	62.36370463
 6	2	34.81844056
 6	3	24.92258263
 6	4	20.41700473
 6	5	17.87465532
-7	1	70.10816665
 7	2	39.46366694
 7	3	28.42925556
 7	4	23.5203069
 7	5	20.58486915
 7	6	18.13726401
-8	1	78.68930581
 8	2	44.67001181
 8	3	32.21036627
 8	4	26.65605915
 8	5	23.32587898
 8	6	20.62390769
 8	7	18.97838035
-9	1	88.89513476
 9	2	50.27725115
 9	3	36.13663659
 9	4	29.67597663
 9	5	26.10830185
 9	6	23.00774615
 9	7	21.1340075
 9	8	19.62892175
-10	1	105.525432
 10	2	59.11700723
 10	3	43.1504004
 10	4	35.57954094
 10	5	30.60855808
 10	6	27.40350852
 10	7	25.48838179
 10	8	23.49809713
 10	9	21.73158543
-11	1	114.7657544
 11	2	63.5997299
 11	3	46.39869664
 11	4	38.18506873
 11	5	33.21130819
 11	6	29.51571648
 11	7	27.31433845
 11	8	25.19853089
 11	9	23.67360761
 11	10	22.16234727
-12	1	122.3155661
 12	2	68.77895272
 12	3	50.09316421
 12	4	41.41727896
 12	5	35.97136669
 12	6	31.70952106
 12	7	29.25295751
 12	8	26.92114942
 12	9	25.27613308
 12	10	24.25048747
 12	11	23.2385983
-13	1	132.0129851
 13	2	74.16346159
 13	3	53.63010974
 13	4	44.61490149
 13	5	38.43130074
 13	6	34.27011006
 13	7	31.64965792
 13	8	29.38081841
 13	9	27.44176791
 13	10	25.9118037
 13	11	24.86320188
 13	12	24.27593825
-14	1	141.4833059
 14	2	79.22456033
 14	3	57.70378568
 14	4	47.75547981
 14	5	41.40831852
 14	6	36.94921858
 14	7	33.91865425
 14	8	31.43874211
 14	9	29.39926147
 14	10	27.89450591
 14	11	26.81508698
 14	12	25.62994623
 14	13	24.67593851
-15	1	149.7832485
 15	2	84.18207154
 15	3	61.1492851
 15	4	50.93052766
 15	5	43.92759881
 15	6	38.9887219
 15	7	35.98457351
 15	8	33.22814164
 15	9	31.26360462
 15	10	29.47478187
 15	11	28.37652071
 15	12	27.22030218
 15	13	26.29118917
 15	14	25.47776577
-16	1	157.3746848
 16	2	88.49745917
 16	3	64.92435288
 16	4	53.60662386
 16	5	46.55044444
 16	6	41.50835936
 16	7	38.29206824
 16	8	35.4055815
 16	9	33.44836681
 16	10	31.34017265
 16	11	30.09953465
 16	12	29.15431724
 16	13	28.23515463
 16	14	26.96458404
 16	15	26.28225818
-17	1	168.4061772
 17	2	94.15699201
 17	3	68.83617799
 17	4	57.09932086
 17	5	49.39344168
 17	6	43.94601259
 17	7	40.38456755
 17	8	37.31013703
@@ -131,15 +115,14 @@
 17	10	33.3193783
 17	11	31.96704876
 17	12	30.84052215
 17	13	29.70041993
 17	14	28.84377487
 17	15	28.00013449
 17	16	27.47714698
-18	1	177.8612285
 18	2	99.62128704
 18	3	72.79515088
 18	4	59.99926398
 18	5	52.00514002
 18	6	46.24584134
 18	7	42.62798321
 18	8	39.55885375
@@ -148,15 +131,14 @@
 18	11	33.73327897
 18	12	32.54492466
 18	13	31.23344355
 18	14	30.35891287
 18	15	29.47791488
 18	16	28.92824888
 18	17	28.20483863
-19	1	186.5779243
 19	2	104.833914
 19	3	75.88183944
 19	4	63.05892231
 19	5	54.76809702
 19	6	48.83276606
 19	7	44.84178591
 19	8	41.44248042
@@ -165,8 +147,26 @@
 19	11	35.62865603
 19	12	34.37410672
 19	13	33.0395345
 19	14	31.92266037
 19	15	31.13155241
 19	16	30.70206103
 19	17	29.52286403
-19	18	28.97082686
+19	18	28.97082686
+19	2	104.833914
+19	3	75.88183944
+19	4	63.05892231
+19	5	54.76809702
+19	6	48.83276606
+19	7	44.84178591
+19	8	41.44248042
+19	9	39.3036458
+19	10	37.01061871
+19	11	35.62865603
+19	12	34.37410672
+19	13	33.0395345
+19	14	31.92266037
+19	15	31.13155241
+19	16	30.70206103
+19	17	29.52286403
+19	18	28.97082686
+20	19	28.97082686
```

### Comparing `drex-0.0.2434/data/200MB.csv` & `drex-0.0.244/data/200MB.csv`

 * *Files identical despite different names*

### Comparing `drex-0.0.2434/drex/schedulers/algorithm3.py` & `drex-0.0.244/drex/schedulers/algorithm3.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,86 @@
 from drex.utils.tool_functions import *
-import time, sys, numpy
 
-def algorithm3(number_of_nodes, reliability_of_nodes, bandwidths, reliability_threshold, file_size, real_records):
+import time
+import sys
+import numpy
+
+
+
+def algorithm3(number_of_nodes, reliability_of_nodes, bandwidths, reliability_threshold, file_size, real_records, node_sizes, predictor):
+	"""
+	Uses a pareto front to find best N with biggest K possible
+	"""
 	start = time.time()
+
 	# 1. Get set of N, K and associated nodes that match the reliability and put them in a list, with fastest N when multiple set of nodes can staisfy the reliability
 	min_K = 0
 	set_of_nodes_chosen = []
 	set_of_nodes = list(range(0, number_of_nodes))
 	set_of_possible_solutions = []
 	time_and_space_from_set_of_possible_solution = []
+
 	for i in range(2, number_of_nodes + 1):
 		min_time = sys.maxsize
 		for set_of_nodes_chosen in itertools.combinations(set_of_nodes, i):
 			reliability_of_nodes_chosen = []
 			bandwidth_of_nodes_chosen = []
 			for j in range(0, len(set_of_nodes_chosen)):
-				reliability_of_nodes_chosen.append(reliability_of_nodes[set_of_nodes_chosen[j]])
+				reliability_of_nodes_chosen.append(
+				    reliability_of_nodes[set_of_nodes_chosen[j]])
 				bandwidth_of_nodes_chosen.append(bandwidths[set_of_nodes_chosen[j]])
-			K = get_max_K_from_reliability_threshold_and_nodes_chosen(i, reliability_threshold, reliability_of_nodes_chosen)
-			if (K != -1):
-				replication_and_write_time = replication_and_chuncking_time(i, K, file_size, bandwidth_of_nodes_chosen, real_records)
+			K = get_max_K_from_reliability_threshold_and_nodes_chosen(
+			    i, reliability_threshold, reliability_of_nodes_chosen)
+			if (K != -1 and nodes_can_fit_new_data(set_of_nodes_chosen, node_sizes, file_size/K)):
+				#replication_and_write_time = replication_and_chuncking_time(i, K, file_size, bandwidth_of_nodes_chosen, real_records)
+				replication_and_write_time = predictor.predict(
+				    file_size, i, K, bandwidth_of_nodes_chosen)
+				
 				set_of_possible_solutions.append((i, K, set_of_nodes_chosen, replication_and_write_time, (file_size/K)*i))
 				time_and_space_from_set_of_possible_solution.append([replication_and_write_time, (file_size/K)*i])
 
+	if (len(time_and_space_from_set_of_possible_solution) == 0):
+		print("ERROR: Algorithm 3 could not find a solution that would not overflow the memory of the nodes")
+		exit(1)
+	
 	# 2. Take those that are on the pareto front
 	costs = numpy.asarray(time_and_space_from_set_of_possible_solution)
 	set_of_solution_on_pareto = is_pareto_efficient(costs, False)
-	# ~ print("Set on pareto front is", set_of_solution_on_pareto)
 
 	time_on_pareto = []
 	for i in range (0, len(set_of_solution_on_pareto)):
 		time_on_pareto.append(time_and_space_from_set_of_possible_solution[set_of_solution_on_pareto[i]][0])
 		
 	# 3. Finding the solution on the plateau
 	# Get min and max
-	time_on_pareto.sort()
+	# ~ time_on_pareto.sort() # Already sorted by time anyway as it's the first value
 	size = len(time_on_pareto) - 1
-	# ~ print(time_on_pareto[0], time_on_pareto[size])
+	
+	max_time = max(time_on_pareto)
+	min_time = min(time_on_pareto)
 	
 	# Start from smallest time and stop when 10% degradation of time has been made and keep the index
-	total_progress = time_on_pareto[size] - time_on_pareto[0]
-	# ~ print("total progress:", total_progress)
+	total_progress = max_time - min_time
 	min_index = -1
 	min_progress = sys.maxsize
 	for i in range (0, size+1):
-		progress = 100 - ((time_on_pareto[i] - time_on_pareto[0])*100)/total_progress
-		# ~ print(time_on_pareto[i], "did", progress, "% of the total progress.")
+		progress = 100 - ((time_on_pareto[i] - min_time)*100)/total_progress
+		# ~ print("progress:", progress, "with", time_on_pareto[i])
 		if progress < 90:
-			# ~ print("Break")
 			break
 		if progress < min_progress:
 			min_progress = progress
 			min_index = i
 	if min_index == -1:
-		# ~ print("No solution found take the fastest N")
 		min_index = 0
-	# ~ print("min_index =", min_index)
 	
 	min_N = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][0]
 	min_K = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][1]
 	min_set_of_nodes_chosen = set_of_possible_solutions[set_of_solution_on_pareto[min_index]][2]
-
+	
+	node_sizes = update_node_sizes(min_set_of_nodes_chosen, min_K, file_size, node_sizes)
+	
 	end = time.time()
+	
 	print("\nAlgorithm 3 chose N =", min_N, "and K =", min_K, "with the set of nodes:", min_set_of_nodes_chosen, "It took", end - start, "seconds.")
-	return list(min_set_of_nodes_chosen), min_N, min_K
+	
+	return list(min_set_of_nodes_chosen), min_N, min_K, node_sizes
```

### Comparing `drex-0.0.2434/drex/utils/poibin.py` & `drex-0.0.244/drex/utils/poibin.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.2434/drex/utils/reliability/fragment_handler.py` & `drex-0.0.244/drex/utils/reliability/fragment_handler.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.2434/drex/utils/reliability/ida.py` & `drex-0.0.244/drex/utils/reliability/ida.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,22 +33,32 @@
         raise ValueError("numToAssemble must be less than numFragments")
     
     # find the prime number greater than n
     # all computations are done modulo p
     p = 257 if n<257 else nextPrime(n)
     
     original_segments = list(itertools.zip_longest(*(iter(data),) * m, fillvalue=0))
-
+    original_segments_arr = np.array(original_segments)
     building_blocks=build_building_blocks(m,n,p)
     fragments=[]
-    for i in range(n): 
-        fragment_arr = [inner_product(building_blocks[i], original_segments[k],p) for k in range(len(original_segments))]
+    for i in range(n):
+        fragment_arr = [np.inner(building_blocks[i], original_segments_arr[k]) % p for k in range(original_segments_arr.shape[0])]
         frag = Fragment(i, fragment_arr, p, n, m)
         fragments.append(frag)
-    
+        #print(fragment_arr)
+        #fragment_arr = [inner_product(building_blocks[i], original_segments[k],p) for k in range(len(original_segments))]
+        #print(fragment_arr)
+        #break
+        #for k in range(original_segments_arr.shape[0]):
+        #    fragment_arr = np.inner(building_blocks[i], original_segments_arr[k])
+        #    print(fragment_arr)
+        #    #fragments.append(frag)
+        #fragment_arr = np.inner(building_blocks[i], original_segments_arr[k])
+    #    fragment_arr = #[inner_product(building_blocks[i], original_segments[k],p) for k in range(len(original_segments))]
+        
     return fragments
 
 
 def split_bytes_v0(data, n, m):
     """
     Inputs: 
     data: bytes to split
```

### Comparing `drex-0.0.2434/drex/utils/reliability/utils.py` & `drex-0.0.244/drex/utils/reliability/utils.py`

 * *Files identical despite different names*

### Comparing `drex-0.0.2434/drex.egg-info/PKG-INFO` & `drex-0.0.244/drex.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: drex
-Version: 0.0.2434
+Version: 0.0.244
 Summary: DRex package
 Author-email: "Maxime, Dante, Haochen" <dantsanc@pa.uc3m.es>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # D-rex
 
 Dynamic replication for heterogeneous storage nodes.
 
 Maxime GONTHIER - Dante - Haochen
```

### Comparing `drex-0.0.2434/pyproject.toml` & `drex-0.0.244/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "drex"
-version = "0.0.2434"
+version = "0.0.244"
 authors = [
   { name="Maxime, Dante, Haochen", email="dantsanc@pa.uc3m.es" },
 ]
 description = "DRex package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
-    "scipy"
+    "scipy",
+    "pandas",
+    "scikit-learn"
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["data*", "Simulation*", "test*"]
 namespaces = false
```

