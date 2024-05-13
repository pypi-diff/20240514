# Comparing `tmp/spyder_index-0.2.0.tar.gz` & `tmp/spyder_index-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_index-0.2.0.tar", last modified: Fri May 10 11:49:29 2024, max compression
+gzip compressed data, was "spyder_index-0.2.1.tar", last modified: Mon May 13 22:06:47 2024, max compression
```

## Comparing `spyder_index-0.2.0.tar` & `spyder_index-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.792106 spyder_index-0.2.0/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-07 19:51:35.000000 spyder_index-0.2.0/LICENSE
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9471 2024-05-10 11:49:29.790828 spyder_index-0.2.0/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     8242 2024-05-10 11:38:25.000000 spyder_index-0.2.0/README.md
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1309 2024-05-10 11:44:39.000000 spyder_index-0.2.0/pyproject.toml
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-10 11:49:29.792353 spyder_index-0.2.0/setup.cfg
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.693249 spyder_index-0.2.0/spyder_index/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-10 11:44:46.000000 spyder_index-0.2.0/spyder_index/__init__.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.684346 spyder_index-0.2.0/spyder_index/core/
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.735169 spyder_index-0.2.0/spyder_index/core/document/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-07 19:52:45.000000 spyder_index-0.2.0/spyder_index/core/document/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2168 2024-05-10 11:01:20.000000 spyder_index-0.2.0/spyder_index/core/document/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.738903 spyder_index-0.2.0/spyder_index/core/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-07 19:53:08.000000 spyder_index-0.2.0/spyder_index/core/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-09 16:51:50.000000 spyder_index-0.2.0/spyder_index/core/embeddings/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.748732 spyder_index-0.2.0/spyder_index/core/readers/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)       86 2024-05-09 21:26:45.000000 spyder_index-0.2.0/spyder_index/core/readers/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      533 2024-05-09 20:15:29.000000 spyder_index-0.2.0/spyder_index/core/readers/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.755622 spyder_index-0.2.0/spyder_index/core/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-07 19:53:25.000000 spyder_index-0.2.0/spyder_index/core/vector_stores/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-09 11:34:49.000000 spyder_index-0.2.0/spyder_index/core/vector_stores/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.760419 spyder_index-0.2.0/spyder_index/embeddings/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-07 19:54:12.000000 spyder_index-0.2.0/spyder_index/embeddings/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-07 20:24:21.000000 spyder_index-0.2.0/spyder_index/embeddings/huggingface.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.765832 spyder_index-0.2.0/spyder_index/readers/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      165 2024-05-10 11:39:21.000000 spyder_index-0.2.0/spyder_index/readers/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1918 2024-05-10 10:52:51.000000 spyder_index-0.2.0/spyder_index/readers/directory.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.771624 spyder_index-0.2.0/spyder_index/readers/file/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      163 2024-05-10 11:40:17.000000 spyder_index-0.2.0/spyder_index/readers/file/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1112 2024-05-10 01:42:18.000000 spyder_index-0.2.0/spyder_index/readers/file/json.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      812 2024-05-10 01:44:20.000000 spyder_index-0.2.0/spyder_index/readers/file/pdf.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1595 2024-05-10 10:49:23.000000 spyder_index-0.2.0/spyder_index/readers/s3.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.782528 spyder_index-0.2.0/spyder_index/text_splitters/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-07 19:55:01.000000 spyder_index-0.2.0/spyder_index/text_splitters/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-07 19:55:07.000000 spyder_index-0.2.0/spyder_index/text_splitters/semantic.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     1371 2024-05-10 11:27:40.000000 spyder_index-0.2.0/spyder_index/text_splitters/sentence.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.785606 spyder_index-0.2.0/spyder_index/vector_stores/
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-07 19:55:30.000000 spyder_index-0.2.0/spyder_index/vector_stores/__init__.py
--rw-rw-r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-07 19:55:41.000000 spyder_index-0.2.0/spyder_index/vector_stores/elasticsearch.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-10 11:49:29.789024 spyder_index-0.2.0/spyder_index.egg-info/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9471 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1021 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/SOURCES.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/dependency_links.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      237 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/requires.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-10 11:49:29.000000 spyder_index-0.2.0/spyder_index.egg-info/top_level.txt
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.341586 spyder_index-0.2.1/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-13 20:08:52.000000 spyder_index-0.2.1/LICENSE
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)    10265 2024-05-13 22:06:47.340342 spyder_index-0.2.1/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9007 2024-05-13 22:04:23.000000 spyder_index-0.2.1/README.md
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1333 2024-05-13 21:02:14.000000 spyder_index-0.2.1/pyproject.toml
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-13 22:06:47.341841 spyder_index-0.2.1/setup.cfg
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.268308 spyder_index-0.2.1/spyder_index/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/__init__.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.254254 spyder_index-0.2.1/spyder_index/core/
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.283589 spyder_index-0.2.1/spyder_index/core/document/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/document/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2168 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/document/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.288905 spyder_index-0.2.1/spyder_index/core/embeddings/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/embeddings/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/embeddings/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.293167 spyder_index-0.2.1/spyder_index/core/readers/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       86 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/readers/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      533 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/readers/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.298167 spyder_index-0.2.1/spyder_index/core/vector_stores/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/vector_stores/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.304127 spyder_index-0.2.1/spyder_index/embeddings/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/embeddings/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/embeddings/huggingface.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.311582 spyder_index-0.2.1/spyder_index/readers/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      165 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2086 2024-05-13 20:49:18.000000 spyder_index-0.2.1/spyder_index/readers/directory.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.325353 spyder_index-0.2.1/spyder_index/readers/file/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      311 2024-05-13 20:44:59.000000 spyder_index-0.2.1/spyder_index/readers/file/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      815 2024-05-13 20:33:50.000000 spyder_index-0.2.1/spyder_index/readers/file/docx.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      831 2024-05-13 20:44:21.000000 spyder_index-0.2.1/spyder_index/readers/file/html.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1112 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/file/json.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      812 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/file/pdf.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      703 2024-05-13 20:59:47.000000 spyder_index-0.2.1/spyder_index/readers/file/unstructured.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1595 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/s3.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.330024 spyder_index-0.2.1/spyder_index/text_splitters/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/semantic.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1371 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/sentence.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.335156 spyder_index-0.2.1/spyder_index/vector_stores/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/vector_stores/elasticsearch.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.338239 spyder_index-0.2.1/spyder_index.egg-info/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)    10265 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1131 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      251 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/requires.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/top_level.txt
```

### Comparing `spyder_index-0.2.0/LICENSE` & `spyder_index-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/PKG-INFO` & `spyder_index-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.2.0
+Version: 0.2.1
 Summary: Spyder Index is an open-source framework for building LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
 Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
 Requires-Dist: ibm-cos-sdk~=2.13.2
 Requires-Dist: jq~=1.7.0
+Requires-Dist: docx2txt~=0.8
 
 # 🕸️ Spyder Index
 
 ![PyPI - Version](https://img.shields.io/pypi/v/spyder-index)
 ![PyPI - License](https://img.shields.io/pypi/l/spyder-index)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/spyder-index)
 
@@ -41,14 +42,16 @@
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Readers
   - [Directory](#readers-directory)
+  - [Docx File](#readers-docx)
+  - [HTML File](#readers-html)
   - [JSON File](#readers-json)
   - [PDF File](#readers-pdf)
   - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
@@ -132,14 +135,56 @@
 - `jq_schema` (str): The jq schema to use to extract the data from the JSON.
 - `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
+## Readers: Docx
+
+### Overview
+
+Loads data from Microsoft Word (Docx) format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import DocxReader
+```
+
+##### **`DocxReader(input_file: str)`**
+
+Initialize an DocxReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: HTML
+
+### Overview
+
+Loads data from HTML format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import HTMLReader
+```
+
+##### **`HTMLReader(input_file: str)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
 ## Readers: PDF
 
 ### Overview
 
 Loads data from PDF.
 
 ### API Reference
```

### Comparing `spyder_index-0.2.0/README.md` & `spyder_index-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Readers
   - [Directory](#readers-directory)
+  - [Docx File](#readers-docx)
+  - [HTML File](#readers-html)
   - [JSON File](#readers-json)
   - [PDF File](#readers-pdf)
   - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
@@ -103,14 +105,56 @@
 - `jq_schema` (str): The jq schema to use to extract the data from the JSON.
 - `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
+## Readers: Docx
+
+### Overview
+
+Loads data from Microsoft Word (Docx) format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import DocxReader
+```
+
+##### **`DocxReader(input_file: str)`**
+
+Initialize an DocxReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: HTML
+
+### Overview
+
+Loads data from HTML format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import HTMLReader
+```
+
+##### **`HTMLReader(input_file: str)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
 ## Readers: PDF
 
 ### Overview
 
 Loads data from PDF.
 
 ### API Reference
```

### Comparing `spyder_index-0.2.0/pyproject.toml` & `spyder_index-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyder-index"
-version = "0.2.0"
+version = "0.2.1"
 description = "Spyder Index is an open-source framework for building LLM applications"
 readme = "README.md"
 authors = [{ name = "Leonardo Furnielis" }]
 license = {text = "MIT License"}
 keywords = ["framework", "RAG", "index", "data", "LLM", "AI", "semantic search"]
 dependencies = [
     "langchain-core ~= 0.1.48",
@@ -17,15 +17,16 @@
     "langchain-experimental ~= 0.0.57",
     "sentence-transformers ~= 2.7.0",
     "pydantic ~= 2.7.1",
     "pypdf ~= 4.2.0",
     "torch == 2.1.0",
     "elasticsearch ~= 8.13.0",
     "ibm-cos-sdk ~= 2.13.2",
-    "jq ~= 1.7.0"
+    "jq ~= 1.7.0",
+    "docx2txt ~= 0.8"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
```

### Comparing `spyder_index-0.2.0/spyder_index/core/document/base.py` & `spyder_index-0.2.1/spyder_index/core/document/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/core/embeddings/base.py` & `spyder_index-0.2.1/spyder_index/core/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/core/readers/base.py` & `spyder_index-0.2.1/spyder_index/core/readers/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/embeddings/huggingface.py` & `spyder_index-0.2.1/spyder_index/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/readers/directory.py` & `spyder_index-0.2.1/spyder_index/readers/directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,21 @@
 
 from spyder_index.core.readers import BaseReader
 from spyder_index.core.document import Document
 
 from langchain_community.document_loaders import DirectoryLoader
 
 def _loading_default_file_readers():
+    from spyder_index.readers.file import DocxReader
+    from spyder_index.readers.file import HTMLReader
     from spyder_index.readers.file import PDFReader
 
     default_file_reader_cls: dict[str, Type[BaseReader]] = {
+        ".docx": DocxReader,
+        ".html": HTMLReader,
         ".pdf": PDFReader,
     }
     
     return default_file_reader_cls
 
 
 class DirectoryReader(BaseReader):
```

### Comparing `spyder_index-0.2.0/spyder_index/readers/file/json.py` & `spyder_index-0.2.1/spyder_index/readers/file/json.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/readers/file/pdf.py` & `spyder_index-0.2.1/spyder_index/readers/file/pdf.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/readers/s3.py` & `spyder_index-0.2.1/spyder_index/readers/s3.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/text_splitters/semantic.py` & `spyder_index-0.2.1/spyder_index/text_splitters/semantic.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/text_splitters/sentence.py` & `spyder_index-0.2.1/spyder_index/text_splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index/vector_stores/elasticsearch.py` & `spyder_index-0.2.1/spyder_index/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.0/spyder_index.egg-info/PKG-INFO` & `spyder_index-0.2.1/spyder_index.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spyder-index
-Version: 0.2.0
+Version: 0.2.1
 Summary: Spyder Index is an open-source framework for building LLM applications
 Author: Leonardo Furnielis
 License: MIT License
 Project-URL: Homepage, https://github.com/leonardofurnielis/spyder_index
 Project-URL: Issues, https://github.com/leonardofurnielis/spyder_index/issues
 Keywords: framework,RAG,index,data,LLM,AI,semantic search
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 Requires-Dist: sentence-transformers~=2.7.0
 Requires-Dist: pydantic~=2.7.1
 Requires-Dist: pypdf~=4.2.0
 Requires-Dist: torch==2.1.0
 Requires-Dist: elasticsearch~=8.13.0
 Requires-Dist: ibm-cos-sdk~=2.13.2
 Requires-Dist: jq~=1.7.0
+Requires-Dist: docx2txt~=0.8
 
 # 🕸️ Spyder Index
 
 ![PyPI - Version](https://img.shields.io/pypi/v/spyder-index)
 ![PyPI - License](https://img.shields.io/pypi/l/spyder-index)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/spyder-index)
 
@@ -41,14 +42,16 @@
 
 ## Table of Contents
 
 - Embeddings
   - [HuggingFace](#embeddings-huggingface)
 - Readers
   - [Directory](#readers-directory)
+  - [Docx File](#readers-docx)
+  - [HTML File](#readers-html)
   - [JSON File](#readers-json)
   - [PDF File](#readers-pdf)
   - [S3](#readers-s3)
 - Text Splitter
   - [Semantic Splitter](#text-splitter-semantic-splitter)
   - [Sentence Splitter](#text-splitter-sentence-splitter)
 - Vector Store
@@ -132,14 +135,56 @@
 - `jq_schema` (str): The jq schema to use to extract the data from the JSON.
 - `text_content` (bool): Flag to indicate whether the content is in string format. Default is `False`
 
 ##### **`load_data() -> List[Document]`**
 
 Loads data from the specified directory.
 
+## Readers: Docx
+
+### Overview
+
+Loads data from Microsoft Word (Docx) format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import DocxReader
+```
+
+##### **`DocxReader(input_file: str)`**
+
+Initialize an DocxReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
+## Readers: HTML
+
+### Overview
+
+Loads data from HTML format.
+
+### API Reference
+
+```py 
+from spyder_index.readers.file import HTMLReader
+```
+
+##### **`HTMLReader(input_file: str)`**
+
+Initialize an JSONReader object.
+- `input_file` (str): File path to read.
+
+##### **`load_data() -> List[Document]`**
+
+Loads data from the specified directory.
+
 ## Readers: PDF
 
 ### Overview
 
 Loads data from PDF.
 
 ### API Reference
```

### Comparing `spyder_index-0.2.0/spyder_index.egg-info/SOURCES.txt` & `spyder_index-0.2.1/spyder_index.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 spyder_index/core/vector_stores/base.py
 spyder_index/embeddings/__init__.py
 spyder_index/embeddings/huggingface.py
 spyder_index/readers/__init__.py
 spyder_index/readers/directory.py
 spyder_index/readers/s3.py
 spyder_index/readers/file/__init__.py
+spyder_index/readers/file/docx.py
+spyder_index/readers/file/html.py
 spyder_index/readers/file/json.py
 spyder_index/readers/file/pdf.py
+spyder_index/readers/file/unstructured.py
 spyder_index/text_splitters/__init__.py
 spyder_index/text_splitters/semantic.py
 spyder_index/text_splitters/sentence.py
 spyder_index/vector_stores/__init__.py
 spyder_index/vector_stores/elasticsearch.py
```

