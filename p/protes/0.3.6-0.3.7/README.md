# Comparing `tmp/protes-0.3.6.tar.gz` & `tmp/protes-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protes-0.3.6.tar", last modified: Sun Dec 10 18:02:48 2023, max compression
+gzip compressed data, was "protes-0.3.7.tar", last modified: Tue May 14 11:39:18 2024, max compression
```

## Comparing `protes-0.3.6.tar` & `protes-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-10 18:02:48.836528 protes-0.3.6/
--rw-r--r--   0 andrei     (501) staff       (20)       63 2023-08-15 14:13:10.000000 protes-0.3.6/MANIFEST.in
--rw-r--r--   0 andrei     (501) staff       (20)    10074 2023-12-10 18:02:48.835899 protes-0.3.6/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)     7907 2023-12-10 18:02:16.000000 protes-0.3.6/README.md
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-10 18:02:48.832868 protes-0.3.6/protes/
--rw-r--r--   0 andrei     (501) staff       (20)      127 2023-12-10 18:02:09.000000 protes-0.3.6/protes/__init__.py
--rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.6/protes/animation.py
--rw-r--r--   0 andrei     (501) staff       (20)     6214 2023-12-10 17:13:10.000000 protes-0.3.6/protes/protes.py
--rw-r--r--   0 andrei     (501) staff       (20)     5442 2023-08-15 15:24:56.000000 protes-0.3.6/protes/protes_general.py
-drwxr-xr-x   0 andrei     (501) staff       (20)        0 2023-12-10 18:02:48.835146 protes-0.3.6/protes.egg-info/
--rw-r--r--   0 andrei     (501) staff       (20)    10074 2023-12-10 18:02:48.000000 protes-0.3.6/protes.egg-info/PKG-INFO
--rw-r--r--   0 andrei     (501) staff       (20)      277 2023-12-10 18:02:48.000000 protes-0.3.6/protes.egg-info/SOURCES.txt
--rw-r--r--   0 andrei     (501) staff       (20)        1 2023-12-10 18:02:48.000000 protes-0.3.6/protes.egg-info/dependency_links.txt
--rw-r--r--   0 andrei     (501) staff       (20)      309 2023-12-10 18:02:48.000000 protes-0.3.6/protes.egg-info/requires.txt
--rw-r--r--   0 andrei     (501) staff       (20)        7 2023-12-10 18:02:48.000000 protes-0.3.6/protes.egg-info/top_level.txt
--rw-r--r--   0 andrei     (501) staff       (20)      539 2023-12-10 16:50:58.000000 protes-0.3.6/requirements.txt
--rw-r--r--   0 andrei     (501) staff       (20)       38 2023-12-10 18:02:48.836624 protes-0.3.6/setup.cfg
--rw-r--r--   0 andrei     (501) staff       (20)     2590 2023-12-10 16:09:13.000000 protes-0.3.6/setup.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-05-14 11:39:18.959339 protes-0.3.7/
+-rw-r--r--   0 andrei     (501) staff       (20)       63 2023-08-15 14:13:10.000000 protes-0.3.7/MANIFEST.in
+-rw-r--r--   0 andrei     (501) staff       (20)    10074 2024-05-14 11:39:18.958998 protes-0.3.7/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)     7907 2024-05-14 11:33:22.000000 protes-0.3.7/README.md
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-05-14 11:39:18.956391 protes-0.3.7/protes/
+-rw-r--r--   0 andrei     (501) staff       (20)      127 2024-05-14 11:34:04.000000 protes-0.3.7/protes/__init__.py
+-rw-r--r--   0 andrei     (501) staff       (20)     4670 2023-05-18 16:29:00.000000 protes-0.3.7/protes/animation.py
+-rw-r--r--   0 andrei     (501) staff       (20)     6199 2024-05-14 11:31:27.000000 protes-0.3.7/protes/protes.py
+-rw-r--r--   0 andrei     (501) staff       (20)     5427 2024-05-14 11:31:33.000000 protes-0.3.7/protes/protes_general.py
+drwxr-xr-x   0 andrei     (501) staff       (20)        0 2024-05-14 11:39:18.958371 protes-0.3.7/protes.egg-info/
+-rw-r--r--   0 andrei     (501) staff       (20)    10074 2024-05-14 11:39:18.000000 protes-0.3.7/protes.egg-info/PKG-INFO
+-rw-r--r--   0 andrei     (501) staff       (20)      277 2024-05-14 11:39:18.000000 protes-0.3.7/protes.egg-info/SOURCES.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        1 2024-05-14 11:39:18.000000 protes-0.3.7/protes.egg-info/dependency_links.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      309 2024-05-14 11:39:18.000000 protes-0.3.7/protes.egg-info/requires.txt
+-rw-r--r--   0 andrei     (501) staff       (20)        7 2024-05-14 11:39:18.000000 protes-0.3.7/protes.egg-info/top_level.txt
+-rw-r--r--   0 andrei     (501) staff       (20)      539 2023-12-10 16:50:58.000000 protes-0.3.7/requirements.txt
+-rw-r--r--   0 andrei     (501) staff       (20)       38 2024-05-14 11:39:18.959414 protes-0.3.7/setup.cfg
+-rw-r--r--   0 andrei     (501) staff       (20)     2590 2023-12-10 16:09:13.000000 protes-0.3.7/setup.py
```

### Comparing `protes-0.3.6/PKG-INFO` & `protes-0.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.6
+Version: 0.3.7
 Summary: Method PROTES (PRobabilistic Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization gradient-free method multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -45,17 +45,17 @@
 ## Description
 
 Method **PROTES** (**PR**obabilistic **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip:
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` - `3.10`, then, the package can be installed via pip:
 ```bash
-pip install protes==0.3.6
+pip install protes==0.3.7
 ```
 
 > To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`. Also note that `requirements.txt` contains `jax[cpu]`; if you need the GPU version of the `jax`, please install it yourself.
 
 
 ## Usage
```

### Comparing `protes-0.3.6/README.md` & `protes-0.3.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 ## Description
 
 Method **PROTES** (**PR**obabilistic **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip:
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` - `3.10`, then, the package can be installed via pip:
 ```bash
-pip install protes==0.3.6
+pip install protes==0.3.7
 ```
 
 > To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`. Also note that `requirements.txt` contains `jax[cpu]`; if you need the GPU version of the `jax`, please install it yourself.
 
 
 ## Usage
```

### Comparing `protes-0.3.6/protes/animation.py` & `protes-0.3.7/protes/animation.py`

 * *Files identical despite different names*

### Comparing `protes-0.3.6/protes/protes.py` & `protes-0.3.7/protes/protes.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         info['m'] += y.shape[0]
 
         is_new = _process(P, I, y, info, with_info_i_opt_list, with_info_full)
 
         if info['m_max'] and info['m'] >= info['m_max']:
             break
 
-        ind = jnp.argsort(y, kind='stable')
+        ind = jnp.argsort(y)
         ind = (ind[::-1] if is_max else ind)[:k_top]
 
         for _ in range(k_gd):
             state, P = optimize(state, P, I[ind, :])
         
         if with_info_p:
             info['P'] = P
```

### Comparing `protes-0.3.6/protes/protes_general.py` & `protes-0.3.7/protes/protes_general.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         info['m'] += y.shape[0]
 
         is_new = _process(P, I, y, info, with_info_i_opt_list, with_info_full)
 
         if info['m_max'] and info['m'] >= info['m_max']:
             break
 
-        ind = jnp.argsort(y, kind='stable')
+        ind = jnp.argsort(y)
         ind = (ind[::-1] if is_max else ind)[:k_top]
 
         for _ in range(k_gd):
             state, P = optimize(state, P, I[ind, :])
 
         info['t'] = tpc() - time
         _log(info, log, is_new)
```

### Comparing `protes-0.3.6/protes.egg-info/PKG-INFO` & `protes-0.3.7/protes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protes
-Version: 0.3.6
+Version: 0.3.7
 Summary: Method PROTES (PRobabilistic Optimizer with TEnsor Sampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format
 Home-page: https://github.com/anabatsh/PROTES
 Author: Andrei Chertkov
 Author-email: andre.chertkov@gmail.com
 Project-URL: Source, https://github.com/anabatsh/PROTES
 Keywords: Derivative-free optimization gradient-free method multidimensional optimization low-rank representation tensor train format
 Classifier: Development Status :: 4 - Beta
@@ -45,17 +45,17 @@
 ## Description
 
 Method **PROTES** (**PR**obabilistic **O**ptimizer with **TE**nsor **S**ampling) for derivative-free optimization of the multidimensional arrays and discretized multivariate functions based on the tensor train (TT) format.
 
 
 ## Installation
 
-To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` or `3.9`, then, the package can be installed via pip:
+To use this package, please install manually first the [python](https://www.python.org) programming language of the version `3.8` - `3.10`, then, the package can be installed via pip:
 ```bash
-pip install protes==0.3.6
+pip install protes==0.3.7
 ```
 
 > To ensure version stability, we recommend working in a virtual environment, as described in the `workflow.md`. Also note that `requirements.txt` contains `jax[cpu]`; if you need the GPU version of the `jax`, please install it yourself.
 
 
 ## Usage
```

### Comparing `protes-0.3.6/requirements.txt` & `protes-0.3.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `protes-0.3.6/setup.py` & `protes-0.3.7/setup.py`

 * *Files identical despite different names*

