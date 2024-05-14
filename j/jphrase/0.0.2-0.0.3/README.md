# Comparing `tmp/jphrase-0.0.2.tar.gz` & `tmp/jphrase-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jphrase-0.0.2.tar", last modified: Sun May 12 15:23:57 2024, max compression
+gzip compressed data, was "jphrase-0.0.3.tar", last modified: Tue May 14 15:00:07 2024, max compression
```

## Comparing `jphrase-0.0.2.tar` & `jphrase-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.850169 jphrase-0.0.2/
--rw-r--r--   0 jiro       (501) staff       (20)     1069 2024-05-09 08:54:48.000000 jphrase-0.0.2/LICENSE
--rw-r--r--   0 jiro       (501) staff       (20)     7500 2024-05-12 15:23:57.849900 jphrase-0.0.2/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)     7057 2024-05-12 15:18:47.000000 jphrase-0.0.2/README.md
--rw-r--r--   0 jiro       (501) staff       (20)       38 2024-05-12 15:23:57.850223 jphrase-0.0.2/setup.cfg
--rw-r--r--   0 jiro       (501) staff       (20)      827 2024-05-12 15:18:47.000000 jphrase-0.0.2/setup.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.847506 jphrase-0.0.2/src/
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.848560 jphrase-0.0.2/src/jphrase/
--rw-r--r--   0 jiro       (501) staff       (20)       74 2024-05-09 14:29:27.000000 jphrase-0.0.2/src/jphrase/__init__.py
--rw-r--r--   0 jiro       (501) staff       (20)     7175 2024-05-12 15:18:47.000000 jphrase-0.0.2/src/jphrase/phrase_splitter.py
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.849612 jphrase-0.0.2/src/jphrase.egg-info/
--rw-r--r--   0 jiro       (501) staff       (20)     7500 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/PKG-INFO
--rw-r--r--   0 jiro       (501) staff       (20)      251 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/SOURCES.txt
--rw-r--r--   0 jiro       (501) staff       (20)        1 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/dependency_links.txt
--rw-r--r--   0 jiro       (501) staff       (20)        8 2024-05-12 15:23:57.000000 jphrase-0.0.2/src/jphrase.egg-info/top_level.txt
-drwxr-xr-x   0 jiro       (501) staff       (20)        0 2024-05-12 15:23:57.849391 jphrase-0.0.2/tests/
--rw-r--r--   0 jiro       (501) staff       (20)     3380 2024-05-12 15:18:47.000000 jphrase-0.0.2/tests/test_phrase_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:07.466427 jphrase-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 14:59:58.000000 jphrase-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-14 15:00:07.466427 jphrase-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-14 14:59:58.000000 jphrase-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:00:07.466427 jphrase-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 14:59:58.000000 jphrase-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:07.466427 jphrase-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:07.466427 jphrase-0.0.3/src/jphrase/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-14 14:59:58.000000 jphrase-0.0.3/src/jphrase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-05-14 14:59:58.000000 jphrase-0.0.3/src/jphrase/phrase_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:00:07.466427 jphrase-0.0.3/src/jphrase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-14 15:00:07.000000 jphrase-0.0.3/src/jphrase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-14 15:00:07.000000 jphrase-0.0.3/src/jphrase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:00:07.000000 jphrase-0.0.3/src/jphrase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:00:07.000000 jphrase-0.0.3/src/jphrase.egg-info/top_level.txt
```

### Comparing `jphrase-0.0.2/LICENSE` & `jphrase-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jphrase-0.0.2/PKG-INFO` & `jphrase-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jphrase
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Japanese phrase tokenizer
 Home-page: https://github.com/jiroshimaya/jphrase
 Author: shimajiroxyz
 Author-email: shimaya.jiro@irl.sys.es.osaka-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jphrase
 jphraseは、日本語のテキストを文節に分割するためのライブラリです。
 形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します。
 
@@ -83,15 +83,17 @@
 consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
-python tests/test_phrase_splitter.py
+pip install -r requirements.txt
+pip install -e .
+pytest
 ```
 
 # Rule for phrase splitting
 jphraseでは形態素解析結果の品詞情報に基づいて文節の境界を決定します。
 
 ipadicの辞書を用いて形態素解析を行うと、各単語につき、以下の情報が得られます。
```

### Comparing `jphrase-0.0.2/README.md` & `jphrase-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,17 @@
 consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
-python tests/test_phrase_splitter.py
+pip install -r requirements.txt
+pip install -e .
+pytest
 ```
 
 # Rule for phrase splitting
 jphraseでは形態素解析結果の品詞情報に基づいて文節の境界を決定します。
 
 ipadicの辞書を用いて形態素解析を行うと、各単語につき、以下の情報が得られます。
```

### Comparing `jphrase-0.0.2/setup.py` & `jphrase-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jphrase",  # PyPIに登録するパッケージ名
-    version="0.0.2",
+    version="0.0.3",
     packages=find_packages(where='src'),  # パッケージはsrcディレクトリ内にある
     package_dir={'': 'src'},  # パッケージのルートディレクトリをsrcに設定
     install_requires=[],
     author="shimajiroxyz",
     author_email="shimaya.jiro@irl.sys.es.osaka-u.ac.jp",
     description="A Japanese phrase tokenizer",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/jiroshimaya/jphrase",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.11',
 )
```

### Comparing `jphrase-0.0.2/src/jphrase/phrase_splitter.py` & `jphrase-0.0.3/src/jphrase/phrase_splitter.py`

 * *Files identical despite different names*

### Comparing `jphrase-0.0.2/src/jphrase.egg-info/PKG-INFO` & `jphrase-0.0.3/src/jphrase.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: jphrase
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Japanese phrase tokenizer
 Home-page: https://github.com/jiroshimaya/jphrase
 Author: shimajiroxyz
 Author-email: shimaya.jiro@irl.sys.es.osaka-u.ac.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # jphrase
 jphraseは、日本語のテキストを文節に分割するためのライブラリです。
 形態素解析から得られた単語の品詞情報に基づき、ルールベースで文節を決定します。
 
@@ -83,15 +83,17 @@
 consider_non_independent_nouns_and_verbs_as_breaks引数は、非自立な名詞や動詞を文節の区切りとして扱うかどうかを制御します。この引数がTrueに設定されている場合、非自立な名詞や動詞の前で新しい文節が始まります。Falseの場合、非自立な名詞や動詞は前の文節に含まれ続けます。
 
 またこれらのオプション引数はPhraseSplitterのインスタンス作成時にも指定することができ、指定した場合は、split_text実行時のデフォルト値として扱われます。
 
 # Testing
 
 ```Python
-python tests/test_phrase_splitter.py
+pip install -r requirements.txt
+pip install -e .
+pytest
 ```
 
 # Rule for phrase splitting
 jphraseでは形態素解析結果の品詞情報に基づいて文節の境界を決定します。
 
 ipadicの辞書を用いて形態素解析を行うと、各単語につき、以下の情報が得られます。
```

