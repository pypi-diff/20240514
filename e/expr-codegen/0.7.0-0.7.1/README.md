# Comparing `tmp/expr_codegen-0.7.0.tar.gz` & `tmp/expr_codegen-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expr_codegen-0.7.0.tar", last modified: Mon May 13 04:19:34 2024, max compression
+gzip compressed data, was "expr_codegen-0.7.1.tar", last modified: Tue May 14 07:07:48 2024, max compression
```

## Comparing `expr_codegen-0.7.0.tar` & `expr_codegen-0.7.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.675872 expr_codegen-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/expr_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/expr_codegen/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/latex/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/expr_codegen/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/pandas/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/pandas/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/pandas/template.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/expr_codegen/polars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/polars/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/polars/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/polars/template.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8718 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/expr_codegen/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 04:19:34.671872 expr_codegen-0.7.0/expr_codegen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-13 04:19:34.000000 expr_codegen-0.7.0/expr_codegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-13 04:19:34.000000 expr_codegen-0.7.0/expr_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 04:19:34.000000 expr_codegen-0.7.0/expr_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 04:19:34.000000 expr_codegen-0.7.0/expr_codegen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 04:19:34.000000 expr_codegen-0.7.0/expr_codegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 04:19:30.000000 expr_codegen-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 04:19:34.675872 expr_codegen-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.551120 expr_codegen-0.7.1/expr_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8206 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14665 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/expr_codegen/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/latex/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/expr_codegen/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/pandas/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/pandas/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/pandas/template.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/expr_codegen/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/polars/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/polars/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/polars/template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/expr_codegen/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/expr_codegen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-14 07:07:48.000000 expr_codegen-0.7.1/expr_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-14 07:07:48.000000 expr_codegen-0.7.1/expr_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:07:48.000000 expr_codegen-0.7.1/expr_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-14 07:07:48.000000 expr_codegen-0.7.1/expr_codegen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-14 07:07:48.000000 expr_codegen-0.7.1/expr_codegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-14 07:07:43.000000 expr_codegen-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:07:48.555120 expr_codegen-0.7.1/setup.cfg
```

### Comparing `expr_codegen-0.7.0/LICENSE` & `expr_codegen-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/PKG-INFO` & `expr_codegen-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.7.0
+Version: 0.7.1
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
@@ -85,40 +85,43 @@
 from polars_ta.prefix.ta import *  # noqa
 from polars_ta.prefix.tdx import *  # noqa
 from polars_ta.prefix.wq import *  # noqa
 
 from expr_codegen.tool import codegen_exec
 
 
-def _code_block_():
-    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+def _code_block_1():
+   # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+   LOG_MC_ZS = cs_mad_zscore(log1p(market_cap))
+
+
+def _code_block_2():
+   # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
+   # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
+   from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
+
+   # 1. 下划线开头的变量只是中间变量,会被自动更名，最终输出时会被剔除
+   # 2. 下划线开头的变量可以重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
+   _avg = ts_mean(corr, 20)
+   _std = ts_std_dev(corr, 20)
+   _beta = ts_LINEARREG_SLOPE(corr, 20)
+
+   # 3. 下划线开头的变量有环循环赋值。在调试时可快速用注释进行切换
+   _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
+   _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
+   # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
 
-    # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
-    # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
-    from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
-
-    # 1. 下划线开头的变量是中间变量,会被自动更名，最终输出时会被剔除
-    # 2. 下划线开头的变量可重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
-    _avg = ts_mean(corr, 20)
-    _std = ts_std_dev(corr, 20)
-    _beta = ts_LINEARREG_SLOPE(corr, 20)
-
-    # 3. 下划线开头的变量支持有环循环赋值。在调试时可快速用注释进行切换
-    _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
-    _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
-    # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
-
-    _corr = cs_zscore(_avg) + cs_zscore(_std)
-    CPV = cs_zscore(_corr) + cs_zscore(_beta)
+   _corr = cs_zscore(_avg) + cs_zscore(_std)
+   CPV = cs_zscore(_corr) + cs_zscore(_beta)
 
 
 df = None  # 替换成真实的polars数据
-df = codegen_exec(_code_block_, df, output_file=sys.stdout)  # 打印代码
-df = codegen_exec(_code_block_, df, output_file="output.py")  # 保存到文件
-df = codegen_exec(_code_block_, df)  # 只执行，不保存代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file=sys.stdout)  # 打印代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file="output.py")  # 保存到文件
+df = codegen_exec(df, _code_block_1, _code_block_2)  # 只执行，不保存代码
 
 ```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
```

### Comparing `expr_codegen-0.7.0/README.md` & `expr_codegen-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -35,40 +35,43 @@
 from polars_ta.prefix.ta import *  # noqa
 from polars_ta.prefix.tdx import *  # noqa
 from polars_ta.prefix.wq import *  # noqa
 
 from expr_codegen.tool import codegen_exec
 
 
-def _code_block_():
-    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+def _code_block_1():
+   # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+   LOG_MC_ZS = cs_mad_zscore(log1p(market_cap))
+
+
+def _code_block_2():
+   # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
+   # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
+   from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
+
+   # 1. 下划线开头的变量只是中间变量,会被自动更名，最终输出时会被剔除
+   # 2. 下划线开头的变量可以重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
+   _avg = ts_mean(corr, 20)
+   _std = ts_std_dev(corr, 20)
+   _beta = ts_LINEARREG_SLOPE(corr, 20)
+
+   # 3. 下划线开头的变量有环循环赋值。在调试时可快速用注释进行切换
+   _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
+   _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
+   # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
 
-    # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
-    # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
-    from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
-
-    # 1. 下划线开头的变量是中间变量,会被自动更名，最终输出时会被剔除
-    # 2. 下划线开头的变量可重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
-    _avg = ts_mean(corr, 20)
-    _std = ts_std_dev(corr, 20)
-    _beta = ts_LINEARREG_SLOPE(corr, 20)
-
-    # 3. 下划线开头的变量支持有环循环赋值。在调试时可快速用注释进行切换
-    _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
-    _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
-    # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
-
-    _corr = cs_zscore(_avg) + cs_zscore(_std)
-    CPV = cs_zscore(_corr) + cs_zscore(_beta)
+   _corr = cs_zscore(_avg) + cs_zscore(_std)
+   CPV = cs_zscore(_corr) + cs_zscore(_beta)
 
 
 df = None  # 替换成真实的polars数据
-df = codegen_exec(_code_block_, df, output_file=sys.stdout)  # 打印代码
-df = codegen_exec(_code_block_, df, output_file="output.py")  # 保存到文件
-df = codegen_exec(_code_block_, df)  # 只执行，不保存代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file=sys.stdout)  # 打印代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file="output.py")  # 保存到文件
+df = codegen_exec(df, _code_block_1, _code_block_2)  # 只执行，不保存代码
 
 ```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
```

### Comparing `expr_codegen-0.7.0/expr_codegen/codes.py` & `expr_codegen-0.7.1/expr_codegen/codes.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/dag.py` & `expr_codegen-0.7.1/expr_codegen/dag.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/expr.py` & `expr_codegen-0.7.1/expr_codegen/expr.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/latex/printer.py` & `expr_codegen-0.7.1/expr_codegen/latex/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/model.py` & `expr_codegen-0.7.1/expr_codegen/model.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/pandas/code.py` & `expr_codegen-0.7.1/expr_codegen/pandas/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/pandas/printer.py` & `expr_codegen-0.7.1/expr_codegen/pandas/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/pandas/template.py.j2` & `expr_codegen-0.7.1/expr_codegen/pandas/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/polars/code.py` & `expr_codegen-0.7.1/expr_codegen/polars/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/polars/printer.py` & `expr_codegen-0.7.1/expr_codegen/polars/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/polars/template.py.j2` & `expr_codegen-0.7.1/expr_codegen/polars/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/expr_codegen/tool.py` & `expr_codegen-0.7.1/expr_codegen/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         self.exprs_dict = self.reduce(repl, new_redu)
 
         # with open("exprs.pickle", "wb") as file:
         #     pickle.dump(exprs_dict, file)
 
         return self.exprs_dict
 
-    def dag(self, merge):
+    def dag(self, merge: bool):
         """生成DAG"""
         G = dag_start(self.exprs_dict, self.get_current_func, self.get_current_func_kwargs)
         if merge:
             G = dag_middle(G, self.exprs_names, self.get_current_func, self.get_current_func_kwargs)
         return dag_end(G)
 
     def all(self, exprs_src, style: str = 'polars', template_file: str = 'template.py.j2',
@@ -220,61 +220,87 @@
 
         """
         globals_ = {'df_input': df_input}
         exec(codes, globals_)
         return globals_['df_output']
 
     @lru_cache(maxsize=64)
-    def _get_codes(self, source: str, extra_codes: str, output_file: str,
-                   style='polars', template_file='template.py.j2',
-                   date='date', asset='asset') -> str:
+    def _get_code(self,
+                  source: str, *more_sources: str,
+                  extra_codes: str, output_file: str,
+                  style='polars', template_file='template.py.j2',
+                  date='date', asset='asset') -> str:
         """通过字符串生成代码， 加了缓存，多次调用不重复生成"""
-        raw, exprs_dict = sources_to_exprs(self.globals_, source, safe=False)
+        raw, exprs_dict = sources_to_exprs(self.globals_, source, *more_sources, safe=False)
 
         # 生成代码
-        codes, G = _TOOL_.all(exprs_dict, style=style, template_file=template_file,
-                              replace=True, regroup=True, format=True,
-                              date=date, asset=asset,
-                              # 复制了需要使用的函数，还复制了最原始的表达式
-                              extra_codes=(raw,
-                                           # 传入多个列的方法
-                                           extra_codes,
-                                           ))
+        code, G = _TOOL_.all(exprs_dict, style=style, template_file=template_file,
+                             replace=True, regroup=True, format=True,
+                             date=date, asset=asset,
+                             # 复制了需要使用的函数，还复制了最原始的表达式
+                             extra_codes=(raw,
+                                          # 传入多个列的方法
+                                          extra_codes,
+                                          ))
         if isinstance(output_file, TextIOWrapper):
-            output_file.write(codes)
+            output_file.write(code)
         elif output_file is not None:
             with open(output_file, 'w', encoding='utf-8') as f:
-                f.write(codes)
+                f.write(code)
 
-        return codes
+        return code
 
 
 _TOOL_ = ExprTool()
 
 
-def codegen_exec(code_block,
-                 df_input,
+def codegen_exec(df,
+                 *codes,
                  extra_codes: str = r'CS_SW_L1 = pl.col(r"^sw_l1_\d+$")',
                  output_file: Optional[str] = None,
                  style: str = 'polars', template_file: str = 'template.py.j2',
                  date: str = 'date', asset: str = 'asset'
                  ):
-    """快速转换源代码并执行"""
+    """快速转换源代码并执行
+
+    Parameters
+    ----------
+    df: pl.DataFrame
+        输入DataFrame
+    codes:
+        函数体。此部分中的表达式会被翻译成目标代码
+    extra_codes: str
+        额外代码。不做处理，会被直接复制到目标代码中
+    output_file: str
+        保存生成的目标代码到文件中
+    style: str
+        代码风格。可选值 ('polars', 'pandas')
+    template_file: str
+        代码模板
+    date: str
+        时间字段
+    asset: str
+        资产字段
+
+    Returns
+    -------
+    pl.DataFrame
+
+    """
     # 此代码来自于sympy.var
     frame = inspect.currentframe().f_back
     _TOOL_.globals_ = frame.f_globals.copy()
     del frame
 
-    if isinstance(code_block, str):
-        source = code_block
-    else:
-        source = inspect.getsource(code_block)
+    more_sources = [c if isinstance(c, str) else inspect.getsource(c) for c in codes]
 
-    codes = _TOOL_._get_codes(source, extra_codes, output_file,
-                              style=style, template_file=template_file,
-                              date=date, asset=asset,
-                              )
+    code = _TOOL_._get_code(
+        *more_sources, extra_codes=extra_codes,
+        output_file=output_file,
+        style=style, template_file=template_file,
+        date=date, asset=asset,
+    )
 
-    if df_input is None:
-        return df_input
+    if df is None:
+        return df
     else:
-        return _TOOL_.exec(codes, df_input)
+        return _TOOL_.exec(code, df)
```

### Comparing `expr_codegen-0.7.0/expr_codegen.egg-info/PKG-INFO` & `expr_codegen-0.7.1/expr_codegen.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.7.0
+Version: 0.7.1
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
@@ -85,40 +85,43 @@
 from polars_ta.prefix.ta import *  # noqa
 from polars_ta.prefix.tdx import *  # noqa
 from polars_ta.prefix.wq import *  # noqa
 
 from expr_codegen.tool import codegen_exec
 
 
-def _code_block_():
-    # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+def _code_block_1():
+   # 因子编辑区，可利用IDE的智能提示在此区域编辑因子
+   LOG_MC_ZS = cs_mad_zscore(log1p(market_cap))
+
+
+def _code_block_2():
+   # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
+   # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
+   from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
+
+   # 1. 下划线开头的变量只是中间变量,会被自动更名，最终输出时会被剔除
+   # 2. 下划线开头的变量可以重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
+   _avg = ts_mean(corr, 20)
+   _std = ts_std_dev(corr, 20)
+   _beta = ts_LINEARREG_SLOPE(corr, 20)
+
+   # 3. 下划线开头的变量有环循环赋值。在调试时可快速用注释进行切换
+   _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
+   _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
+   # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
 
-    # 模板中已经默认导入了from polars_ta.prefix下大量的算子，但
-    # talib在模板中没有默认导入。这种写法可实现在生成的代码中导入
-    from polars_ta.prefix.talib import ts_LINEARREG_SLOPE  # noqa
-
-    # 1. 下划线开头的变量是中间变量,会被自动更名，最终输出时会被剔除
-    # 2. 下划线开头的变量可重复使用。多个复杂因子多行书写时有重复中间变时不再冲突
-    _avg = ts_mean(corr, 20)
-    _std = ts_std_dev(corr, 20)
-    _beta = ts_LINEARREG_SLOPE(corr, 20)
-
-    # 3. 下划线开头的变量支持有环循环赋值。在调试时可快速用注释进行切换
-    _avg = cs_mad_zscore_resid(_avg, LOG_MC_ZS, ONE)
-    _std = cs_mad_zscore_resid(_std, LOG_MC_ZS, ONE)
-    # _beta = cs_mad_zscore_resid(_beta, LOG_MC_ZS, ONE)
-
-    _corr = cs_zscore(_avg) + cs_zscore(_std)
-    CPV = cs_zscore(_corr) + cs_zscore(_beta)
+   _corr = cs_zscore(_avg) + cs_zscore(_std)
+   CPV = cs_zscore(_corr) + cs_zscore(_beta)
 
 
 df = None  # 替换成真实的polars数据
-df = codegen_exec(_code_block_, df, output_file=sys.stdout)  # 打印代码
-df = codegen_exec(_code_block_, df, output_file="output.py")  # 保存到文件
-df = codegen_exec(_code_block_, df)  # 只执行，不保存代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file=sys.stdout)  # 打印代码
+df = codegen_exec(df, _code_block_1, _code_block_2, output_file="output.py")  # 保存到文件
+df = codegen_exec(df, _code_block_1, _code_block_2)  # 只执行，不保存代码
 
 ```
 
 ## 目录结构
 
 ```commandline
 │  requirements.txt # 通过`pip install -r requirements.txt`安装依赖
```

### Comparing `expr_codegen-0.7.0/expr_codegen.egg-info/SOURCES.txt` & `expr_codegen-0.7.1/expr_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.7.0/pyproject.toml` & `expr_codegen-0.7.1/pyproject.toml`

 * *Files identical despite different names*

