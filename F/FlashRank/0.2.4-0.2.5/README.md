# Comparing `tmp/FlashRank-0.2.4.tar.gz` & `tmp/FlashRank-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlashRank-0.2.4.tar", last modified: Tue Apr 30 10:37:33 2024, max compression
+gzip compressed data, was "FlashRank-0.2.5.tar", last modified: Tue May 14 14:22:15 2024, max compression
```

## Comparing `FlashRank-0.2.4.tar` & `FlashRank-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:37:33.544893 FlashRank-0.2.4/
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:37:33.543132 FlashRank-0.2.4/FlashRank.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:37:33.000000 FlashRank-0.2.4/FlashRank.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-04-30 10:37:33.000000 FlashRank-0.2.4/FlashRank.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-30 10:37:33.000000 FlashRank-0.2.4/FlashRank.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       68 2024-04-30 10:37:33.000000 FlashRank-0.2.4/FlashRank.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-04-30 10:37:33.000000 FlashRank-0.2.4/FlashRank.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.4/LICENSE
--rw-r--r--   0 prithivida   (501) staff       (20)    10278 2024-04-30 10:37:33.544701 FlashRank-0.2.4/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     9757 2024-03-19 01:23:34.000000 FlashRank-0.2.4/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-30 10:37:33.544366 FlashRank-0.2.4/flashrank/
--rw-r--r--   0 prithivida   (501) staff       (20)      724 2024-04-30 10:04:33.000000 FlashRank-0.2.4/flashrank/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)    10031 2024-04-30 10:36:20.000000 FlashRank-0.2.4/flashrank/Ranker.py
--rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.4/flashrank/Rankerb.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.4/flashrank/Rankerc.py
--rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.4/flashrank/__init__.py
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-30 10:37:33.544937 FlashRank-0.2.4/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      855 2024-04-30 10:37:07.000000 FlashRank-0.2.4/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-05-14 14:22:15.442371 FlashRank-0.2.5/
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-05-14 14:22:15.440614 FlashRank-0.2.5/FlashRank.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)    11744 2024-05-14 14:22:15.000000 FlashRank-0.2.5/FlashRank.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      294 2024-05-14 14:22:15.000000 FlashRank-0.2.5/FlashRank.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-05-14 14:22:15.000000 FlashRank-0.2.5/FlashRank.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       68 2024-05-14 14:22:15.000000 FlashRank-0.2.5/FlashRank.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       10 2024-05-14 14:22:15.000000 FlashRank-0.2.5/FlashRank.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)    11357 2023-12-04 14:24:33.000000 FlashRank-0.2.5/LICENSE
+-rw-r--r--   0 prithivida   (501) staff       (20)    11744 2024-05-14 14:22:15.442179 FlashRank-0.2.5/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)    11222 2024-05-03 06:55:22.000000 FlashRank-0.2.5/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-05-14 14:22:15.441879 FlashRank-0.2.5/flashrank/
+-rw-r--r--   0 prithivida   (501) staff       (20)      724 2024-04-30 10:04:33.000000 FlashRank-0.2.5/flashrank/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)    10450 2024-05-14 14:20:14.000000 FlashRank-0.2.5/flashrank/Ranker.py
+-rw-r--r--   0 prithivida   (501) staff       (20)    10457 2023-12-13 12:36:57.000000 FlashRank-0.2.5/flashrank/Rankerb.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6093 2024-01-29 14:51:57.000000 FlashRank-0.2.5/flashrank/Rankerc.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       41 2024-04-30 09:25:26.000000 FlashRank-0.2.5/flashrank/__init__.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-05-14 14:22:15.442409 FlashRank-0.2.5/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      855 2024-05-14 14:20:29.000000 FlashRank-0.2.5/setup.py
```

### Comparing `FlashRank-0.2.4/FlashRank.egg-info/PKG-INFO` & `FlashRank-0.2.5/FlashRank.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [IMPORTANT UPDATE]
+
+<img src=./images/logo.png width=100%>
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11093524.svg)](https://doi.org/10.5281/zenodo.11093524)
+
+## [IMPORTANT UPDATE]
 
 ~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
 
 This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
-# 🏎️ FlashRank
-Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
+# 🏎️ What is it?
+Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA LLMs and cross-encoders, with gratitude to all the model owners. 
+
+Supports:
+
+- Pairwise / Pointwise rerankers. (Cross encoder based)
+- Listwise LLM based rerankers. (LLM based)
+(see below for full list of supported models)
+
+# Table of Contents  
+
+1. [Features](#features)  
+2. [Installation](#installation)
+3. [Getting started](#getting-started)
+4. [Deployment patterns](#deployment-patterns)
+5. [How to Cite?](#how-to-cite)
+5. [Papers citing flashrank](#papers-citing-flashrank) 
+
+
+## Features
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
     
 2. ⏱️ **Super-fast**:
     - Rerank speed is a function of **# of tokens in passages, query + model depth (layers)**
@@ -40,25 +64,27 @@
     - How good are Zero-shot rerankers - look at the reference section.
     - Below are the list of models supported as of now.
         * `ms-marco-TinyBERT-L-2-v2` (default) [Model card](https://huggingface.co/cross-encoder/ms-marco-TinyBERT-L-2)
         * `ms-marco-MiniLM-L-12-v2` [Model card](https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-12-v2)
         * `rank-T5-flan` (Best non cross-encoder reranker) [Model card](https://huggingface.co/bergum/rank-T5-flan)
         * `ms-marco-MultiBERT-L-12`  (Multi-lingual, [supports 100+ languages](https://github.com/google-research/bert/blob/master/multilingual.md#list-of-languages))
         * `ce-esci-MiniLM-L12-v2` [FT on Amazon ESCI dataset](https://github.com/amazon-science/esci-data) (This is interesting because most models are FT on MSFT MARCO Bing queries) [Model card](https://huggingface.co/metarank/ce-esci-MiniLM-L12-v2)
+        * `rank_zephyr_7b_v1_full` (4-bit-quantised GGUF) [Model card](https://huggingface.co/castorini/rank_zephyr_7b_v1_full) (Offers very competitive performance, with large context window and relatively faster for a 4GB model).
+            - **Important note:** Our current integration of `rank_zephyr` supports a max of 20 passages in one pass. The sliding window logic support is yet to be added.
     - Models in roadmap:
         * InRanker
-    - Why only sleeker models? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
+    - Why sleeker models are preferred ? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
 
 
-## 🚀 Installation:
+## Installation:
 ```python 
 pip install flashrank
 ```
 
-## Usage:
+## Getting started:
 ```python
 from flashrank import Ranker, RerankRequest
 
 # Nano (~4MB), blazing fast model & competitive performance (ranking precision).
 ranker = Ranker()
 
 or 
@@ -71,14 +97,18 @@
 # Medium (~110MB), slower model with best zeroshot performance (ranking precision) on out of domain data.
 ranker = Ranker(model_name="rank-T5-flan", cache_dir="/opt")
 
 or 
 
 # Medium (~150MB), slower model with competitive performance (ranking precision) for 100+ languages  (don't use for english)
 ranker = Ranker(model_name="ms-marco-MultiBERT-L-12", cache_dir="/opt")
+
+or 
+
+ranker = Ranker(model_name="rank_zephyr_7b_v1_full", max_length=1024) # adjust max_length based on your passage length
 ```
 
 ```python
 # Metadata is optional, Id can be your DB ids from your retrieval stage or simple numeric indices.
 query = "How to speedup LLMs?"
 passages = [
    {
@@ -192,10 +222,19 @@
 
 <br/>
 
 2. **In-domain and Zeroshot performance of RankT5 fine-tuned on MS-MARCO**
   <center><img src="./images/RankT5_BEIR.png" width=450/></center>
 <br/>
 
-## How to Cite
+## How to Cite?
 
 To cite this repository in your work please click the "cite this repository" link on the right side (bewlow repo descriptions and tags)
+
+
+## Papers citing flashrank
+
+- [Bryndza at ClimateActivism 2024: Stance, Target and Hate Event
+Detection via Retrieval-Augmented GPT-4 and LLaMA](https://arxiv.org/pdf/2402.06549)
+
+- [Stance and Hate Event Detection in Tweets Related to
+Climate Activism - Shared Task at CASE 2024](https://aclanthology.org/2024.case-1.33.pdf)
```

### Comparing `FlashRank-0.2.4/LICENSE` & `FlashRank-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.4/PKG-INFO` & `FlashRank-0.2.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,54 @@
 Metadata-Version: 2.1
 Name: FlashRank
-Version: 0.2.4
+Version: 0.2.5
 Summary: Ultra lite & Super fast SoTA cross-encoder based re-ranking for your search & retrieval pipelines.
 Home-page: https://github.com/PrithivirajDamodaran/FlashRank
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# [IMPORTANT UPDATE]
+
+<img src=./images/logo.png width=100%>
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11093524.svg)](https://doi.org/10.5281/zenodo.11093524)
+
+## [IMPORTANT UPDATE]
 
 ~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
 
 This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
-# 🏎️ FlashRank
-Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
+# 🏎️ What is it?
+Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA LLMs and cross-encoders, with gratitude to all the model owners. 
+
+Supports:
+
+- Pairwise / Pointwise rerankers. (Cross encoder based)
+- Listwise LLM based rerankers. (LLM based)
+(see below for full list of supported models)
+
+# Table of Contents  
+
+1. [Features](#features)  
+2. [Installation](#installation)
+3. [Getting started](#getting-started)
+4. [Deployment patterns](#deployment-patterns)
+5. [How to Cite?](#how-to-cite)
+5. [Papers citing flashrank](#papers-citing-flashrank) 
+
+
+## Features
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
     
 2. ⏱️ **Super-fast**:
     - Rerank speed is a function of **# of tokens in passages, query + model depth (layers)**
@@ -40,25 +64,27 @@
     - How good are Zero-shot rerankers - look at the reference section.
     - Below are the list of models supported as of now.
         * `ms-marco-TinyBERT-L-2-v2` (default) [Model card](https://huggingface.co/cross-encoder/ms-marco-TinyBERT-L-2)
         * `ms-marco-MiniLM-L-12-v2` [Model card](https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-12-v2)
         * `rank-T5-flan` (Best non cross-encoder reranker) [Model card](https://huggingface.co/bergum/rank-T5-flan)
         * `ms-marco-MultiBERT-L-12`  (Multi-lingual, [supports 100+ languages](https://github.com/google-research/bert/blob/master/multilingual.md#list-of-languages))
         * `ce-esci-MiniLM-L12-v2` [FT on Amazon ESCI dataset](https://github.com/amazon-science/esci-data) (This is interesting because most models are FT on MSFT MARCO Bing queries) [Model card](https://huggingface.co/metarank/ce-esci-MiniLM-L12-v2)
+        * `rank_zephyr_7b_v1_full` (4-bit-quantised GGUF) [Model card](https://huggingface.co/castorini/rank_zephyr_7b_v1_full) (Offers very competitive performance, with large context window and relatively faster for a 4GB model).
+            - **Important note:** Our current integration of `rank_zephyr` supports a max of 20 passages in one pass. The sliding window logic support is yet to be added.
     - Models in roadmap:
         * InRanker
-    - Why only sleeker models? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
+    - Why sleeker models are preferred ? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
 
 
-## 🚀 Installation:
+## Installation:
 ```python 
 pip install flashrank
 ```
 
-## Usage:
+## Getting started:
 ```python
 from flashrank import Ranker, RerankRequest
 
 # Nano (~4MB), blazing fast model & competitive performance (ranking precision).
 ranker = Ranker()
 
 or 
@@ -71,14 +97,18 @@
 # Medium (~110MB), slower model with best zeroshot performance (ranking precision) on out of domain data.
 ranker = Ranker(model_name="rank-T5-flan", cache_dir="/opt")
 
 or 
 
 # Medium (~150MB), slower model with competitive performance (ranking precision) for 100+ languages  (don't use for english)
 ranker = Ranker(model_name="ms-marco-MultiBERT-L-12", cache_dir="/opt")
+
+or 
+
+ranker = Ranker(model_name="rank_zephyr_7b_v1_full", max_length=1024) # adjust max_length based on your passage length
 ```
 
 ```python
 # Metadata is optional, Id can be your DB ids from your retrieval stage or simple numeric indices.
 query = "How to speedup LLMs?"
 passages = [
    {
@@ -192,10 +222,19 @@
 
 <br/>
 
 2. **In-domain and Zeroshot performance of RankT5 fine-tuned on MS-MARCO**
   <center><img src="./images/RankT5_BEIR.png" width=450/></center>
 <br/>
 
-## How to Cite
+## How to Cite?
 
 To cite this repository in your work please click the "cite this repository" link on the right side (bewlow repo descriptions and tags)
+
+
+## Papers citing flashrank
+
+- [Bryndza at ClimateActivism 2024: Stance, Target and Hate Event
+Detection via Retrieval-Augmented GPT-4 and LLaMA](https://arxiv.org/pdf/2402.06549)
+
+- [Stance and Hate Event Detection in Tweets Related to
+Climate Activism - Shared Task at CASE 2024](https://aclanthology.org/2024.case-1.33.pdf)
```

### Comparing `FlashRank-0.2.4/README.md` & `FlashRank-0.2.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,39 @@
-# [IMPORTANT UPDATE]
+
+<img src=./images/logo.png width=100%>
+
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11093524.svg)](https://doi.org/10.5281/zenodo.11093524)
+
+## [IMPORTANT UPDATE]
 
 ~~*A clone library called **SwiftRank is pointing to our model buckets, we are working on a interim solution to avoid this stealing**. Thank you for patience and understanding.*~~
 
 This issue is resolved, the models are in HF now. **please upgrade to continue** pip install -U flashrank. Thank you for patience and understanding
 
-# 🏎️ FlashRank
-Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA cross-encoders, with gratitude to all the model owners.
+# 🏎️ What is it?
+Ultra-lite &amp; Super-fast Python library to add re-ranking to your existing search &amp; retrieval pipelines. It is based on SoTA LLMs and cross-encoders, with gratitude to all the model owners. 
+
+Supports:
+
+- Pairwise / Pointwise rerankers. (Cross encoder based)
+- Listwise LLM based rerankers. (LLM based)
+(see below for full list of supported models)
+
+# Table of Contents  
+
+1. [Features](#features)  
+2. [Installation](#installation)
+3. [Getting started](#getting-started)
+4. [Deployment patterns](#deployment-patterns)
+5. [How to Cite?](#how-to-cite)
+5. [Papers citing flashrank](#papers-citing-flashrank) 
+
+
+## Features
 
 1. ⚡ **Ultra-lite**: 
     - **No Torch or Transformers** needed. Runs on CPU.
     - Boasts the **tiniest reranking model in the world, ~4MB**.
     
 2. ⏱️ **Super-fast**:
     - Rerank speed is a function of **# of tokens in passages, query + model depth (layers)**
@@ -25,25 +49,27 @@
     - How good are Zero-shot rerankers - look at the reference section.
     - Below are the list of models supported as of now.
         * `ms-marco-TinyBERT-L-2-v2` (default) [Model card](https://huggingface.co/cross-encoder/ms-marco-TinyBERT-L-2)
         * `ms-marco-MiniLM-L-12-v2` [Model card](https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-12-v2)
         * `rank-T5-flan` (Best non cross-encoder reranker) [Model card](https://huggingface.co/bergum/rank-T5-flan)
         * `ms-marco-MultiBERT-L-12`  (Multi-lingual, [supports 100+ languages](https://github.com/google-research/bert/blob/master/multilingual.md#list-of-languages))
         * `ce-esci-MiniLM-L12-v2` [FT on Amazon ESCI dataset](https://github.com/amazon-science/esci-data) (This is interesting because most models are FT on MSFT MARCO Bing queries) [Model card](https://huggingface.co/metarank/ce-esci-MiniLM-L12-v2)
+        * `rank_zephyr_7b_v1_full` (4-bit-quantised GGUF) [Model card](https://huggingface.co/castorini/rank_zephyr_7b_v1_full) (Offers very competitive performance, with large context window and relatively faster for a 4GB model).
+            - **Important note:** Our current integration of `rank_zephyr` supports a max of 20 passages in one pass. The sliding window logic support is yet to be added.
     - Models in roadmap:
         * InRanker
-    - Why only sleeker models? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
+    - Why sleeker models are preferred ? Reranking is the final leg of larger retrieval pipelines, idea is to avoid any extra overhead especially for user-facing scenarios. To that end models with really small footprint that doesn't need any specialised hardware and yet offer competitive performance are chosen. Feel free to raise issues to add support for a new models as you see fit.
 
 
-## 🚀 Installation:
+## Installation:
 ```python 
 pip install flashrank
 ```
 
-## Usage:
+## Getting started:
 ```python
 from flashrank import Ranker, RerankRequest
 
 # Nano (~4MB), blazing fast model & competitive performance (ranking precision).
 ranker = Ranker()
 
 or 
@@ -56,14 +82,18 @@
 # Medium (~110MB), slower model with best zeroshot performance (ranking precision) on out of domain data.
 ranker = Ranker(model_name="rank-T5-flan", cache_dir="/opt")
 
 or 
 
 # Medium (~150MB), slower model with competitive performance (ranking precision) for 100+ languages  (don't use for english)
 ranker = Ranker(model_name="ms-marco-MultiBERT-L-12", cache_dir="/opt")
+
+or 
+
+ranker = Ranker(model_name="rank_zephyr_7b_v1_full", max_length=1024) # adjust max_length based on your passage length
 ```
 
 ```python
 # Metadata is optional, Id can be your DB ids from your retrieval stage or simple numeric indices.
 query = "How to speedup LLMs?"
 passages = [
    {
@@ -177,10 +207,19 @@
 
 <br/>
 
 2. **In-domain and Zeroshot performance of RankT5 fine-tuned on MS-MARCO**
   <center><img src="./images/RankT5_BEIR.png" width=450/></center>
 <br/>
 
-## How to Cite
+## How to Cite?
 
 To cite this repository in your work please click the "cite this repository" link on the right side (bewlow repo descriptions and tags)
+
+
+## Papers citing flashrank
+
+- [Bryndza at ClimateActivism 2024: Stance, Target and Hate Event
+Detection via Retrieval-Augmented GPT-4 and LLaMA](https://arxiv.org/pdf/2402.06549)
+
+- [Stance and Hate Event Detection in Tweets Related to
+Climate Activism - Shared Task at CASE 2024](https://aclanthology.org/2024.case-1.33.pdf)
```

### Comparing `FlashRank-0.2.4/flashrank/Config.py` & `FlashRank-0.2.5/flashrank/Config.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.4/flashrank/Ranker.py` & `FlashRank-0.2.5/flashrank/Ranker.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import zipfile
 import requests
 from tqdm import tqdm
 from flashrank.Config import default_model, default_cache_dir, model_url, model_file_map, listwise_rankers
 import collections
 from typing import Optional, List, Dict, Any
-from llama_cpp import Llama
+import logging
 
 class RerankRequest:
     """ Represents a reranking request with a query and a list of passages. 
     
     Attributes:
         query (Optional[str]): The query for which the passages need to be reranked.
         passages (List[Dict[str, Any]]): The list of passages to be reranked.
@@ -30,29 +30,36 @@
     Attributes:
         cache_dir (Path): Path to the cache directory where models are stored.
         model_dir (Path): Path to the directory of the specific model being used.
         session (ort.InferenceSession): The ONNX runtime session for making inferences.
         tokenizer (Tokenizer): The tokenizer for text processing.
     """
 
-    def __init__(self, model_name: str = default_model, cache_dir: str = default_cache_dir, max_length: int = 512):
+    def __init__(self, model_name: str = default_model, cache_dir: str = default_cache_dir, max_length: int = 512, log_level: str = "INFO"):
         """ Initializes the Ranker class with specified model and cache settings.
 
         Args:
             model_name (str): The name of the model to be used.
             cache_dir (str): The directory where models are cached.
             max_length (int): The maximum length of the tokens.
+            log_level (str): Logging level (DEBUG, INFO, WARNING, ERROR, CRITICAL).
         """
+        
+        # Setting up logging
+        logging.basicConfig(level=getattr(logging, log_level.upper(), logging.INFO))
+        self.logger = logging.getLogger(__name__)
+
         self.cache_dir: Path = Path(cache_dir)
         self.model_dir: Path = self.cache_dir / model_name
         self._prepare_model_dir(model_name)
         model_file = model_file_map[model_name]
 
         self.llm_model = None
         if model_name in listwise_rankers:
+            from llama_cpp import Llama
             self.llm_model = Llama(
               model_path=str(self.model_dir / model_file),
               n_ctx=max_length,  
               n_threads=8,          
             ) 
         else:
             self.session = ort.InferenceSession(str(self.model_dir / model_file))
@@ -61,19 +68,19 @@
     def _prepare_model_dir(self, model_name: str):
         """ Ensures the model directory is prepared by downloading and extracting the model if not present.
 
         Args:
             model_name (str): The name of the model to be prepared.
         """
         if not self.cache_dir.exists():
-            print(f"Cache directory {self.cache_dir} not found. Creating it..")
+            self.logger.debug(f"Cache directory {self.cache_dir} not found. Creating it..")
             self.cache_dir.mkdir(parents=True, exist_ok=True)
         
         if not self.model_dir.exists():
-            print(f"Downloading {model_name}...")
+            self.logger.info(f"Downloading {model_name}...")
             self._download_model_files(model_name)
 
     def _download_model_files(self, model_name: str):
         """ Downloads and extracts the model files from a specified URL.
 
         Args:
             model_name (str): The name of the model to download.
@@ -171,15 +178,15 @@
             List[Dict[str, Any]]: The reranked list of passages with added scores.
         """
         query = request.query
         passages = request.passages
 
         # self.llm_model will be instantiated for GGUF based Listwise LLM models
         if self.llm_model is not None:
-            print("Running listwise ranking..")
+            self.logger.debug("Running listwise ranking..")
             num_of_passages = len(passages)
             messages = self._get_prefix_prompt(query, num_of_passages)
 
             result_map = {}
             for rank, passage in enumerate(passages):
                 messages.append(
                     {
@@ -201,15 +208,15 @@
             results = []
             for rank in raw_ranks["choices"][0]["message"]["content"].split(" > "):
                 results.append(result_map[int(rank[1])])
             return results    
 
         # self.session will be instantiated for ONNX based pairwise CE models
         else:
-            print("Running pairwise ranking..")
+            self.logger.debug("Running pairwise ranking..")
             query_passage_pairs = [[query, passage["text"]] for passage in passages]
 
             input_text = self.tokenizer.encode_batch(query_passage_pairs)
             input_ids = np.array([e.ids for e in input_text])
             token_type_ids = np.array([e.type_ids for e in input_text])
             attention_mask = np.array([e.attention_mask for e in input_text])
 
@@ -217,15 +224,20 @@
 
             onnx_input = {"input_ids": input_ids.astype(np.int64), "attention_mask": attention_mask.astype(np.int64)}
             if use_token_type_ids:
                 onnx_input["token_type_ids"] = token_type_ids.astype(np.int64)
 
             outputs = self.session.run(None, onnx_input)
 
-            scores = np.exp(outputs[0]) / (1 + np.exp(outputs[0])) if outputs[0].shape[1] > 1 else np.exp(outputs[0].flatten()) / (1 + np.exp(outputs[0].flatten()))
-            scores = scores.tolist()
+            logits = outputs[0]
+
+            if logits.shape[1] == 1:
+                scores = 1 / (1 + np.exp(-logits.flatten()))
+            else:
+                exp_logits = np.exp(logits)
+                scores = exp_logits[:, 1] / np.sum(exp_logits, axis=1)
 
             for score, passage in zip(scores, passages):
                 passage["score"] = score
 
             passages.sort(key=lambda x: x["score"], reverse=True)
             return passages
```

### Comparing `FlashRank-0.2.4/flashrank/Rankerb.py` & `FlashRank-0.2.5/flashrank/Rankerb.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.4/flashrank/Rankerc.py` & `FlashRank-0.2.5/flashrank/Rankerc.py`

 * *Files identical despite different names*

### Comparing `FlashRank-0.2.4/setup.py` & `FlashRank-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FlashRank', 
-    version='0.2.4', 
+    version='0.2.5', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime',
         'numpy',
         'requests',
         'tqdm',
```

