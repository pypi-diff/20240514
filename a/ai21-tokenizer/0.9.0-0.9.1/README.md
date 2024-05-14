# Comparing `tmp/ai21_tokenizer-0.9.0.tar.gz` & `tmp/ai21_tokenizer-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21_tokenizer-0.9.0.tar", max compression
+gzip compressed data, was "ai21_tokenizer-0.9.1.tar", max compression
```

## Comparing `ai21_tokenizer-0.9.0.tar` & `ai21_tokenizer-0.9.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/LICENSE
--rw-r--r--   0        0        0     2620 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/README.md
--rw-r--r--   0        0        0      499 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/ai21_tokenizer/__init__.py
--rw-r--r--   0        0        0     2189 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/ai21_tokenizer/base_tokenizer.py
--rw-r--r--   0        0        0     2822 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/ai21_tokenizer/jamba_instruct_tokenizer.py
--rw-r--r--   0        0        0     9103 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/ai21_tokenizer/jurassic_tokenizer.py
--rw-r--r--   0        0        0      223 2024-03-28 16:09:08.972587 ai21_tokenizer-0.9.0/ai21_tokenizer/resources/j2-tokenizer/config.json
--rw-r--r--   0        0        0  6659225 2024-03-28 16:09:09.008587 ai21_tokenizer-0.9.0/ai21_tokenizer/resources/j2-tokenizer/j2-tokenizer.model
--rw-r--r--   0        0        0     1188 2024-03-28 16:09:09.008587 ai21_tokenizer-0.9.0/ai21_tokenizer/tokenizer_factory.py
--rw-r--r--   0        0        0      647 2024-03-28 16:09:09.008587 ai21_tokenizer-0.9.0/ai21_tokenizer/utils.py
--rw-r--r--   0        0        0       18 2024-03-28 16:09:09.008587 ai21_tokenizer-0.9.0/ai21_tokenizer/version.py
--rw-r--r--   0        0        0     2392 2024-03-28 16:09:09.008587 ai21_tokenizer-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3218 1970-01-01 00:00:00.000000 ai21_tokenizer-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2620 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/README.md
+-rw-r--r--   0        0        0      499 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/ai21_tokenizer/__init__.py
+-rw-r--r--   0        0        0     2189 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/ai21_tokenizer/base_tokenizer.py
+-rw-r--r--   0        0        0     2822 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/ai21_tokenizer/jamba_instruct_tokenizer.py
+-rw-r--r--   0        0        0     9103 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/ai21_tokenizer/jurassic_tokenizer.py
+-rw-r--r--   0        0        0      223 2024-05-14 18:29:17.562830 ai21_tokenizer-0.9.1/ai21_tokenizer/resources/j2-tokenizer/config.json
+-rw-r--r--   0        0        0  6659225 2024-05-14 18:29:17.598830 ai21_tokenizer-0.9.1/ai21_tokenizer/resources/j2-tokenizer/j2-tokenizer.model
+-rw-r--r--   0        0        0     1188 2024-05-14 18:29:17.598830 ai21_tokenizer-0.9.1/ai21_tokenizer/tokenizer_factory.py
+-rw-r--r--   0        0        0      647 2024-05-14 18:29:17.598830 ai21_tokenizer-0.9.1/ai21_tokenizer/utils.py
+-rw-r--r--   0        0        0       18 2024-05-14 18:29:17.598830 ai21_tokenizer-0.9.1/ai21_tokenizer/version.py
+-rw-r--r--   0        0        0     2403 2024-05-14 18:29:17.602830 ai21_tokenizer-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3217 1970-01-01 00:00:00.000000 ai21_tokenizer-0.9.1/PKG-INFO
```

### Comparing `ai21_tokenizer-0.9.0/LICENSE` & `ai21_tokenizer-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/README.md` & `ai21_tokenizer-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/base_tokenizer.py` & `ai21_tokenizer-0.9.1/ai21_tokenizer/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/jamba_instruct_tokenizer.py` & `ai21_tokenizer-0.9.1/ai21_tokenizer/jamba_instruct_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/jurassic_tokenizer.py` & `ai21_tokenizer-0.9.1/ai21_tokenizer/jurassic_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/resources/j2-tokenizer/j2-tokenizer.model` & `ai21_tokenizer-0.9.1/ai21_tokenizer/resources/j2-tokenizer/j2-tokenizer.model`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/tokenizer_factory.py` & `ai21_tokenizer-0.9.1/ai21_tokenizer/tokenizer_factory.py`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/ai21_tokenizer/utils.py` & `ai21_tokenizer-0.9.1/ai21_tokenizer/utils.py`

 * *Files identical despite different names*

### Comparing `ai21_tokenizer-0.9.0/pyproject.toml` & `ai21_tokenizer-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -55,26 +55,26 @@
 name = "cz_customize"
 
 [tool.commitizen.customize]
 schema_pattern = "(build|ci|docs|feat|fix|perf|refactor|style|test|chore|revert|bump):(\\s.*)"
 
 [tool.poetry]
 name = "ai21-tokenizer"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21_tokenizer" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-sentencepiece = "^0.2.0"
-tokenizers = "^0.15.2"
+sentencepiece = ">=0.2.0,<1.0.0"
+tokenizers = ">=0.15.0,<1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 invoke = "*"
 isort = "*"
 mypy = "*"
 safety = "*"
@@ -98,19 +98,14 @@
 
 [tool.semantic_release.branches.main]
 match = "(main)"
 
 [tool.semantic_release.changelog.environment]
 newline_sequence = "\n"
 
-
-
-
-
-
 [tool.poetry.group.test.dependencies]
 coverage = "^7.1.0"
 pytest = "7.4.4"
 pytest-cov = "4.0.0"
 pytest-mock = "3.11.1"
 
 [[tool.poetry.source]]
```

### Comparing `ai21_tokenizer-0.9.0/PKG-INFO` & `ai21_tokenizer-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: ai21-tokenizer
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sentencepiece (>=0.2.0,<0.3.0)
-Requires-Dist: tokenizers (>=0.15.2,<0.16.0)
+Requires-Dist: sentencepiece (>=0.2.0,<1.0.0)
+Requires-Dist: tokenizers (>=0.15.0,<1.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <a href="https://github.com/AI21Labs/ai21-tokenizer">AI21 Labs Tokenizer</a>
 </h1>
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: ai21-tokenizer Version: 0.9.0 Summary: Author: AI21
+Metadata-Version: 2.1 Name: ai21-tokenizer Version: 0.9.1 Summary: Author: AI21
 Labs Requires-Python: >=3.7,<4.0 Classifier: Programming Language :: Python ::
 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: sentencepiece (>=0.2.0,<0.3.0) Requires-Dist: tokenizers
-(>=0.15.2,<0.16.0) Description-Content-Type: text/markdown
+Requires-Dist: sentencepiece (>=0.2.0,<1.0.0) Requires-Dist: tokenizers
+(>=0.15.0,<1.0.0) Description-Content-Type: text/markdown
                        ************ _AA_II_22_11_ _LL_aa_bb_ss_ _TT_oo_kk_ee_nn_ii_zz_ee_rr ************
     AA SSeenntteenncceePPiieeccee bbaasseedd ttookkeenniizzeerr ffoorr pprroodduuccttiioonn uusseess wwiitthh AAII2211''ss mmooddeellss
   _[_T_e_s_t_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
                               _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 --- ## Installation ### pip ```bash pip install ai21-tokenizer ``` ### poetry
 ```bash poetry add ai21-tokenizer ``` ## Usage ### Tokenizer Creation ```python
 from ai21_tokenizer import Tokenizer tokenizer = Tokenizer.get_tokenizer() #
```

