# Comparing `tmp/JaqalPaq-extras-1.2.0a1.tar.gz` & `tmp/jaqalpaq_extras-1.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/build-jaqal/jaqalpaq-extras/dist/.tmp-1x1tnq_t/JaqalPaq-extras-1.2.0a1.tar", last modified: Fri May 19 23:35:44 2023, max compression
+gzip compressed data, was "jaqalpaq_extras-1.3.0a1.tar", last modified: Tue May 14 11:01:58 2024, max compression
```

## Comparing `JaqalPaq-extras-1.2.0a1.tar` & `jaqalpaq_extras-1.3.0a1.tar`

### file list

```diff
@@ -1,79 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/
--rw-rw-r--   0 root         (0) root         (0)    11358 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       51 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)      197 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4204 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3230 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/ftdetect/
--rw-rw-r--   0 root         (0) root         (0)       64 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/ftdetect/jaqal.vim
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/
--rw-rw-r--   0 root         (0) root         (0)     4448 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/jaqal.vim
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/examples/Tutorials/
--rw-rw-r--   0 root         (0) root         (0)    30905 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/examples/Tutorials/Transpiler_Demo.ipynb
--rw-rw-r--   0 root         (0) root         (0)      111 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     2676 2023-05-19 23:35:44.000000 JaqalPaq-extras-1.2.0a1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4204 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1973 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      283 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/
--rw-rw-r--   0 root         (0) root         (0)      275 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8957 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/
--rw-rw-r--   0 root         (0) root         (0)      304 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5032 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/cirq/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/
--rw-rw-r--   0 root         (0) root         (0)      302 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8717 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/
--rw-rw-r--   0 root         (0) root         (0)      715 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15645 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/frontend.py
--rw-rw-r--   0 root         (0) root         (0)     8777 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/gates.py
--rw-rw-r--   0 root         (0) root         (0)     3558 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/instance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/
--rw-rw-r--   0 root         (0) root         (0)      402 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2850 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/frontend.py
--rw-rw-r--   0 root         (0) root         (0)     7648 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py
--rw-rw-r--   0 root         (0) root         (0)     1453 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/
--rw-rw-r--   0 root         (0) root         (0)      437 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7744 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/backend.py
--rw-rw-r--   0 root         (0) root         (0)    13877 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/frontend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     8510 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/scheduler/test_scheduler.py
--rw-rw-r--   0 root         (0) root         (0)      321 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/test_smoke.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/test_cirq_transpiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1326 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/test_projectq_transpiler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      719 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_backend.py
--rw-rw-r--   0 root         (0) root         (0)     1248 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_gates.py
--rw-rw-r--   0 root         (0) root         (0)     1322 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2411 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2640 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_unroller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2749 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/test_quil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 23:35:43.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      564 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_backend.py
--rw-rw-r--   0 root         (0) root         (0)      967 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py
--rw-rw-r--   0 root         (0) root         (0)     2176 2023-05-19 23:29:52.000000 JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.177310 jaqalpaq_extras-1.3.0a1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4708 2024-05-14 11:01:58.177310 jaqalpaq_extras-1.3.0a1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3214 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/contrib/vim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/contrib/vim/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.165310 jaqalpaq_extras-1.3.0a1/contrib/vim/addons/ftdetect/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/contrib/vim/addons/ftdetect/jaqal.vim
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.165310 jaqalpaq_extras-1.3.0a1/contrib/vim/addons/syntax/
+-rw-r--r--   0 root         (0) root         (0)     4448 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/contrib/vim/addons/syntax/jaqal.vim
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.165310 jaqalpaq_extras-1.3.0a1/examples/Tutorials/
+-rw-r--r--   0 root         (0) root         (0)    31140 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/examples/Tutorials/Transpiler_Demo.ipynb
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     2679 2024-05-14 11:01:58.177310 jaqalpaq_extras-1.3.0a1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.173310 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4708 2024-05-14 11:01:57.000000 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2016 2024-05-14 11:01:58.000000 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 11:01:57.000000 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      286 2024-05-14 11:01:57.000000 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-14 11:01:58.000000 jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.161310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.165310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/cirq/
+-rw-r--r--   0 root         (0) root         (0)      538 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/cirq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9972 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/cirq/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/projectq/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/projectq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8661 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/projectq/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/
+-rw-r--r--   0 root         (0) root         (0)      839 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20458 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/frontend.py
+-rw-r--r--   0 root         (0) root         (0)     8771 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/gates.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/instance.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/sampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/
+-rw-r--r--   0 root         (0) root         (0)      402 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/frontend.py
+-rw-r--r--   0 root         (0) root         (0)     7797 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/
+-rw-r--r--   0 root         (0) root         (0)      437 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7687 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/backend.py
+-rw-r--r--   0 root         (0) root         (0)    13877 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/frontend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/tests/scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8500 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/scheduler/test_scheduler.py
+-rw-r--r--   0 root         (0) root         (0)      321 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/test_smoke.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/tests/transpilers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.169310 jaqalpaq_extras-1.3.0a1/tests/transpilers/cirq/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/cirq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11387 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/cirq/test_cirq_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.173310 jaqalpaq_extras-1.3.0a1/tests/transpilers/projectq/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/projectq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/projectq/test_projectq_transpiler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.173310 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_backend.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_gates.py
+-rw-r--r--   0 root         (0) root         (0)     1135 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_transpiler.py
+-rw-r--r--   0 root         (0) root         (0)     3007 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_unroller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.173310 jaqalpaq_extras-1.3.0a1/tests/transpilers/quil/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/quil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/quil/test_quil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 11:01:58.173310 jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      552 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_backend.py
+-rw-r--r--   0 root         (0) root         (0)      929 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py
+-rw-r--r--   0 root         (0) root         (0)     2346 2024-05-14 11:01:39.000000 jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_transpiler.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `JaqalPaq-extras-1.2.0a1/LICENSE` & `jaqalpaq_extras-1.3.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.2.0a1/PKG-INFO` & `jaqalpaq_extras-1.3.0a1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,44 @@
-Metadata-Version: 2.1
-Name: JaqalPaq-extras
-Version: 1.2.0a1
-Summary: Python tools for Jaqal (extras)
-Home-page: https://qscout.sandia.gov
-Author: Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
-Author-email: qscout@sandia.gov
-License: Apache
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6.5
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: qiskit
-Provides-Extra: pyquil
-Provides-Extra: cirq
-Provides-Extra: projectq
-Provides-Extra: pytket
-Provides-Extra: tutorial
-License-File: LICENSE
-License-File: NOTICE
-
 # JaqalPaq-Extras
+
 JaqalPaq-Extras contains extensions to the
 [JaqalPaq](https://gitlab.com/jaqal/jaqalpaq/) python package, which itself is
 used to parse, manipulate, emulate, and generate quantum assembly code written
 in
 [Jaqal](https://qscout.sandia.gov/jaqal) (Just another quantum assembly
 language).  The purpose of JaqalPaq-Extras is to facilitate the conversion of
 programs written in other quantum assembly languages into Jaqal circuit objects
 in JaqalPaq.  JaqalPaq-Extras is supported on a "best effort" basis, and
 quality cannot be guaranteed.
 
-Because some other quantum assembly languages do not support explicit
-scheduling like Jaqal does, JaqalPaq-Extras also contains some basic quantum
+Because some other quantum assembly languages do not support explicit scheduling as Jaqal does, JaqalPaq-Extras also contains some basic quantum
 circuit scheduling routines.  Furthermore, to facilitate execution on the
 [QSCOUT](https://qscout.sandia.gov/) (Quantum Scientific Computing Open User
 Testbed) platform, JaqalPaq-Extras also includes extensions for third-party
 quantum software toolchains that support the QSCOUT hardware model (including
 its native gate set and scheduling constraints).  In summary, JaqalPaq-Extras
 contains the following functionalities:
 
-
 * Conversion of quantum assembly data structures into JaqalPaq circuit objects
   from:
-    * IBM's [Qiskit](https://github.com/Qiskit)
-    * Rigetti's [pyquil](https://github.com/rigetti/pyquil)
-    * Google's [Cirq](https://github.com/quantumlib/Cirq)
-    * ETH Zurich's [ProjectQ](https://github.com/ProjectQ-Framework/ProjectQ)
-    * CQC's [pytket](https://github.com/CQCL/pytket)
+  * IBM's [Qiskit](https://github.com/Qiskit)
+  * Rigetti's [pyquil](https://github.com/rigetti/pyquil)
+  * Google's [Cirq](https://github.com/quantumlib/Cirq)
+  * ETH Zurich's [ProjectQ](https://github.com/ProjectQ-Framework/ProjectQ)
+  * CQC's [pytket](https://github.com/CQCL/pytket)
 * Basic routines for scheduling unscheduled quantum assembly programs.
-* Extensions to these packages above, as needed, to support to the QSCOUT
+* Extensions to these packages above, as needed, to support the QSCOUT
   hardware model.
 
 ## Installation
 
 JaqalPaq-Extras is available on
 [GitLab](https://gitlab.com/jaqal/jaqalpaq-extras).  It requires JaqalPaq to be
-installed first, which is also  available on
-[GitLab](https://gitlab.com/jaqal/jaqalpaq).  JaqalPaq-Extras requires JaqalPaq
-itself be installed first.
+installed first, which is also available on
+[GitLab](https://gitlab.com/jaqal/jaqalpaq).  JaqalPaq-Extras requires JaqalPaq itself to be installed first.
 Both JaqalPaq and its extensions can be installed with
 [pip](https://pip.pypa.io/en/stable/):
 
 ```bash
 pip install jaqalpaq
 pip install jaqalpaq-extras
 ```
@@ -77,19 +47,19 @@
 However, to make use of the transpiler subpackages, one or more other software
 toolchains
 must be installed. As of this writing, all five supported toolchains can be
 installed via
 pip as follows, with the supported versions of these packages indicated:
 
 ```bash
-pip install qiskit>=0.27.0,<0.28.0
-pip install pyquil>=2.21.0,<3.0.0
-pip install cirq>=0.11.0,<0.12.0
-pip install projectq>=0.5.1,<0.7.0
-pip install pytket>=0.5.6,<0.13.0
+pip install qiskit>=0.27.0,<1.1.0
+pip install pyquil>=2.21.0,<4.9.0
+pip install cirq>=0.11.0,<1.4.0
+pip install projectq>=0.5.1,<0.9.0
+pip install pytket>=1.0.1,<2.0.0
 ```
 
 Additionally, a gate-set specification is required for all of the transpiler
 subpackages.
 Currently, we provide the QSCOUT native gate models, which is also available on
 [GitLab](https://gitlab.com/jaqal/qscout-gatemodels/) and can be installed via
 [pip](https://pip.pypa.io/en/stable/):
@@ -99,15 +69,15 @@
 ```
 
 ## Documentation
 
 Online documentation is hosted on [Read the
 Docs](https://jaqalpaq.readthedocs.io).
 
-
 ## License
+
 [Apache 2.0](https://choosealicense.com/licenses/apache-2.0/)
 
 ## Questions?
 
 For help and support, please contact
 [qscout@sandia.gov](mailto:qscout@sandia.gov).
```

### Comparing `JaqalPaq-extras-1.2.0a1/contrib/vim/addons/syntax/jaqal.vim` & `jaqalpaq_extras-1.3.0a1/contrib/vim/addons/syntax/jaqal.vim`

 * *Files identical despite different names*

### Comparing `JaqalPaq-extras-1.2.0a1/examples/Tutorials/Transpiler_Demo.ipynb` & `jaqalpaq_extras-1.3.0a1/examples/Tutorials/Transpiler_Demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994107744107744%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, 'from jaqalpaq.transpilers.cirq.frontend import "*

 * *            "jaqal_circuit_from_cirq_circuit\\n')], delete: [1]}}, 3: {'outputs': {0: {'text': "*

 * *            "['0: ───PhX(1)───MS(0.25π)───PhX(-0.5)^0.5───S^-1───\\n', '               │\\n', '1: "*

 * *            "────────────MS(0.25π)───PhX(1)^0.5─────────────\\n']}}, 'source': {insert: [(0, "*

 * *            "'try:\\n'), (1, '    cirq_ion_bell = "*

 * *            "cirq.ConvertToIonGates().convert_circuit(cirq_bell)\\n'), (2, ' […]*

```diff
@@ -18,15 +18,15 @@
                     "shell.execute_reply": "1970-01-01T00:00:00.000000Z"
                 },
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "import cirq\n",
-                "from jaqalpaq.transpilers.cirq import jaqal_circuit_from_cirq_circuit\n",
+                "from jaqalpaq.transpilers.cirq.frontend import jaqal_circuit_from_cirq_circuit\n",
                 "from jaqalpaq.generator import generate_jaqal_program"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
@@ -70,22 +70,28 @@
                 "tags": []
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0: \u2500\u2500\u2500PhX(1)\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500MS(0.25\u03c0)\u2500\u2500\u2500PhX(-0.5)^0.5\u2500\u2500\u2500S^-1\u2500\u2500\u2500\n",
-                        "                       \u2502\n",
-                        "1: \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500MS(0.25\u03c0)\u2500\u2500\u2500PhX(1)^0.5\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\n"
+                        "0: \u2500\u2500\u2500PhX(1)\u2500\u2500\u2500MS(0.25\u03c0)\u2500\u2500\u2500PhX(-0.5)^0.5\u2500\u2500\u2500S^-1\u2500\u2500\u2500\n",
+                        "               \u2502\n",
+                        "1: \u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500MS(0.25\u03c0)\u2500\u2500\u2500PhX(1)^0.5\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\u2500\n"
                     ]
                 }
             ],
             "source": [
-                "cirq_ion_bell = cirq.ConvertToIonGates().convert_circuit(cirq_bell)\n",
+                "try:\n",
+                "    cirq_ion_bell = cirq.ConvertToIonGates().convert_circuit(cirq_bell)\n",
+                "except AttributeError:\n",
+                "    from jaqalpaq.transpilers.cirq.frontend import QSCOUTTargetGateset\n",
+                "    cirq_ion_bell = cirq.optimize_for_target_gateset(\n",
+                "                cirq_bell, gateset=QSCOUTTargetGateset()\n",
+                "            )\n",
                 "print(cirq_ion_bell)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {
```

### Comparing `JaqalPaq-extras-1.2.0a1/setup.cfg` & `jaqalpaq_extras-1.3.0a1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = JaqalPaq-extras
 author = Benjamin C. A. Morrison, Jay Wesley Van Der Wall, Daniel Lobser, Antonio Russo, Kenneth Rudinger, Peter Maunz
 author_email = qscout@sandia.gov
 description = Python tools for Jaqal (extras)
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache
-version = 1.2.0a1
+version = 1.3.0a1
 home_page = https://qscout.sandia.gov
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
@@ -18,30 +18,30 @@
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Unix
 
 [options]
 packages = find_namespace:
 package_dir = 
 	=src
-install_requires = JaqalPaq==1.2.0a1; QSCOUT-gatemodels>=1.2.0a1
+install_requires = JaqalPaq==1.3.0a1; QSCOUT-gatemodels>=1.3.0a1
 python_requires = >=3.6.5
 platforms = any
 
 [options.packages.find]
 include = 
 	jaqalpaq.scheduler
 	jaqalpaq.transpilers
 	jaqalpaq.transpilers.*
 where = src
 
 [options.extras_require]
 tests = pytest
-qiskit = qiskit>=0.27.0,<0.37.0
-pyquil = pyquil>=2.21.0,<3.0.0
-cirq = cirq>=0.11.0,<0.15.0
+qiskit = qiskit>=0.27.0,<1.1.0
+pyquil = pyquil>=2.21.0,<4.9.0
+cirq = cirq-core>=0.11.0,<1.4.0
 projectq = projectq>=0.5.1,<0.8.0
 pytket = pytket>=1.0.1,<2.0.0
 tutorial = pytket-qiskit==0.24.0; qiskit-nature[pyscf]==0.3.2
 
 [options.data_files]
 share/jaqalpaq/tests = 
 	tests/test_smoke.py
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt` & `jaqalpaq_extras-1.3.0a1/src/JaqalPaq_extras.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 src/jaqalpaq/transpilers/cirq/frontend.py
 src/jaqalpaq/transpilers/projectq/__init__.py
 src/jaqalpaq/transpilers/projectq/frontend.py
 src/jaqalpaq/transpilers/qiskit/__init__.py
 src/jaqalpaq/transpilers/qiskit/frontend.py
 src/jaqalpaq/transpilers/qiskit/gates.py
 src/jaqalpaq/transpilers/qiskit/instance.py
+src/jaqalpaq/transpilers/qiskit/sampler.py
 src/jaqalpaq/transpilers/quil/__init__.py
 src/jaqalpaq/transpilers/quil/frontend.py
 src/jaqalpaq/transpilers/quil/ioncompiler.py
 src/jaqalpaq/transpilers/quil/qscoutam.py
 src/jaqalpaq/transpilers/tket/__init__.py
 src/jaqalpaq/transpilers/tket/backend.py
 src/jaqalpaq/transpilers/tket/frontend.py
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/scheduler/scheduler.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/scheduler/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
 from jaqalpaq.core import (
     BlockStatement,
     LoopStatement,
     GateStatement,
-    ParamType,
     Circuit,
 )
 from jaqalpaq.core.block import UnscheduledBlockStatement
 from jaqalpaq.core.algorithm.visitor import Visitor
 from jaqalpaq.core.algorithm.used_qubit_visitor import UsedQubitIndicesVisitor
 from jaqalpaq.error import JaqalError
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/projectq/frontend.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/projectq/frontend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
-import projectq
 from projectq.setups import restrictedgateset, trapped_ion_decomposer
 from projectq.ops import (
     Rx,
     Ry,
     Rz,
     Rxx,
     Ryy,
@@ -17,15 +16,14 @@
     Allocate,
     Deallocate,
     Barrier,
     BarrierGate,
 )
 from projectq.cengines import BasicEngine
 from projectq.meta import get_control_count
-from projectq.types import WeakQubitRef
 
 from jaqalpaq.core import CircuitBuilder
 from jaqalpaq.core.circuitbuilder import UnscheduledBlockBuilder
 from jaqalpaq.error import JaqalError
 
 import numpy as np
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/frontend.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/frontend.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,398 +1,345 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
-from jaqalpaq.core import CircuitBuilder, GateStatement, Macro
-from jaqalpaq.core.circuitbuilder import UnscheduledBlockBuilder
+from pytket.circuit import OpType, Circuit, QubitRegister, Bit
+
+from jaqalpaq.core.circuitbuilder import (
+    CircuitBuilder,
+    UnscheduledBlockBuilder,
+    SequentialBlockBuilder,
+)
+
+from jaqalpaq.core import Macro
+
 from jaqalpaq.core.algorithm import expand_subcircuits, expand_macros
 from jaqalpaq.core.algorithm.visitor import Visitor
 from jaqalpaq.core.algorithm.fill_in_map import fill_in_map
 
-# from qscoutlib import MSGate, QasmGate, IonUnroller
-from qiskit.converters import dag_to_circuit
-from jaqalpaq.error import JaqalError
-
-# from sympy.core.evalf import N
 import numpy as np
 
-from qiskit.transpiler.passes import UnrollCustomDefinitions, BasisTranslator
-from qiskit.qasm import pi
-from qiskit.circuit.library.standard_gates.p import PhaseGate
-from qiskit.circuit.library.standard_gates.r import RGate
-from qiskit.circuit.library.standard_gates.x import CXGate
-from qiskit.circuit.library.standard_gates.u import UGate
-from qiskit.circuit.library.standard_gates.h import HGate
-from qiskit.circuit.library.standard_gates.rxx import RXXGate
-from qiskit.circuit import (
-    QuantumRegister,
-    QuantumCircuit,
-    Parameter,
-    EquivalenceLibrary,
-)
-from qiskit.circuit.library.standard_gates.equivalence_library import (
-    StandardEquivalenceLibrary,
-)
-from .gates import JaqalMSGate, SYGate, SYdgGate, JaqalRGate
-from qiskit.transpiler import PassManager
-
+from jaqalpaq.error import JaqalError
 
-_QISKIT_NAMES = {
-    "jaqalr": "R",
-    "sx": "Sx",
-    "sxdg": "Sxd",
-    "sy": "Sy",
-    "sydg": "Syd",
-    "s": "Sz",
-    "sdg": "Szd",
-    "x": "Px",
-    "y": "Py",
-    "z": "Pz",
-    "rz": "Rz",
-    "jaqalms": "MS",
-    "sxx": "Sxx",
+_TKET_NAMES = {
+    OpType.PhasedX: lambda q, alpha, beta: ("R", q, beta, alpha),
+    OpType.Rz: lambda q, theta: ("Rz", q, theta),
+    OpType.XXPhase: lambda q1, q2, theta: ("MS", q1, q2, 0, theta),
 }
 
-_PARAM_MAPS = {
-    "*": lambda targets, args: args,
+_REVERSE_TKET_NAMES = {
+    "R": lambda q, beta, alpha: [(OpType.PhasedX, [alpha, beta], [q])],
+    "Sx": lambda q: [(OpType.SX, [q])],
+    "Sxd": lambda q: [(OpType.SXdg, [q])],
+    "Sy": lambda q: [(OpType.Ry, 0.5, [q])],
+    "Syd": lambda q: [(OpType.Ry, -0.5, [q])],
+    "Sz": lambda q: [(OpType.S, [q])],
+    "Szd": lambda q: [(OpType.Sdg, [q])],
+    "Px": lambda q: [(OpType.X, [q])],
+    "Py": lambda q: [(OpType.Y, [q])],
+    "Pz": lambda q: [(OpType.Z, [q])],
+    "Rz": lambda q, theta: [(OpType.Rz, theta, [q])],
+    "MS": lambda q1, q2, phi, theta: [
+        (OpType.Rz, phi, [q1]),
+        (OpType.Rz, phi, [q2]),
+        (OpType.XXPhase, theta, [q1, q2]),
+        (OpType.Rz, -phi, [q1]),
+        (OpType.Rz, -phi, [q2]),
+    ],
+    "Sxx": lambda q1, q2: [(OpType.XXPhase, 0.5, [q1, q2])],
 }
 
 
-def jaqal_circuit_from_dag_circuit(dag):
-    """
-    Converts a Qiskit directed-acyclic-graph representation of a circuit to a
-    :class:`jaqalpaq.core.Circuit`.
-    See :func:`jaqal_circuit_from_qiskit_circuit` for details.
-
-    :param qiskit.dagcircuit.DAGCircuit dag: The directed acyclic graph circuit to convert.
-    :returns: The same quantum circuit, converted to JaqalPaq.
-    :rtype: jaqalpaq.core.Circuit
-    """
-    return jaqal_circuit_from_qiskit_circuit(dag_to_circuit(dag))
-
-
-def jaqal_circuit_from_qiskit_circuit(
-    circuit, names=None, native_gates=None, param_maps=None
+def jaqal_circuit_from_tket_circuit(
+    tkc, native_gates=None, names=None, remove_measurements=False
 ):
-    """
-    Converts a Qiskit circuit to a :class:`jaqalpaq.core.Circuit`. The circuit
-    will be structured into a sequence of unscheduled blocks. All instructions between one
-    barrier statement and the next will be put into an unscheduled block together. If the
-    :mod:`qscout.scheduler` is run on the circuit, as many as possible of those gates will
-    be parallelized within each block, while maintaining the order of the blocks.
-    Otherwise, the circuit will be treated as a fully sequential circuit.
-
-    Measurement and reset commands are supported, but only if applied to every qubit in
-    the circuit in immediate succession. If so, they will be mapped to a prepare_all or
-    measure_all gate. If the circuit does not end with a measurement, then a measure_all
-    gate will be appended to it.
+    """Converts a pytket Circuit object to a :class:`jaqalpaq.core.Circuit`.
+    The circuit will be structured as a sequence of parallel blocks, one for each Cirq
+    Moment in the input. The circuit will be structured into a sequence of unscheduled
+    blocks. All instructions between one barrier statement and the next will be put into
+    an unscheduled block together. If the :mod:`jaqalpaq.scheduler` is run on the circuit,
+    as many as possible of those gates will be parallelized within each block, while
+    maintaining the order of the blocks. Otherwise, the circuit will be treated as a fully
+    sequential circuit.
+
+    Measurement commands are supported, but only if applied to every qubit in the circuit
+    in immediate succession. If so, they will be mapped to a measure_all gate. If the
+    circuit does not end with a measurement, then a measure_all gate will be appended to
+    it.
 
     Circuits containing multiple quantum registers will be converted to circuits with a
     single quantum register, containing all the qubits from each register. The parts of
     that larger register that correspond to each of the original registers will be mapped
-    with the appropriate names.
-
-    :param qiskit.circuit.QuantumCircuit circuit: The circuit to convert.
-    :param names: A mapping from names of Qiskit gates to the corresponding native Jaqal
-        gate names. If omitted, maps jaqalr
-        (:class:`jaqalpaq.transpilers.qiskit.JaqalRGate`), sx, sxdg, sy
-        (:class:`jaqalpaq.qiskit.SYGate`), sydg (:class:`jaqalpaq.qiskit.SYdgGate`), s,
-        sdg, x, y, z, rz, jaqalms (:class:`jaqalpaq.qiskit.JaqalMSGate`), and sxx
-        (:class:`jaqalpaq.qiskit.SXXGate`) to their QSCOUT counterparts.
+    with the appropriate names. Circuits containing multiple-index qubits will have each
+    such qubit mapped to a single-qubit register named with the indices separated by
+    underscore characters.
+
+    Measurements are supported, but only if applied to every qubit in the circuit in the
+    same moment. If so, they will be mapped to a measure_all gate. If the measure_all gate
+    is not the last gate in the circuit, a prepare_all gate will be inserted after it.
+    Additionally, a prepare_all gate will be inserted before the first moment. If the
+    circuit does not end with a measurement, then a measure_all gate will be appended.
+
+    :param pytket.circuit.Circuit tkc: The Circuit to convert.
+    :param names: A mapping from pytket OpTypes to functions taking qubits and gate
+        angle parameters and returning a tuple of arguments for
+        :meth:`jaqalpaq.core.Circuit.build_gate`. If omitted, maps
+        ``pytket.OpType.PhasedX`` to the QSCOUT ``R`` gate, ``pytket.OpType.Rz`` to the
+        QSCOUT ``Rz`` gate, and ``pytket.OpType.XXPhase`` to the QSCOUT ``MS`` gate. The
+        ``pytket.passes.SynthesiseUMD`` compilation pass will compile a circuit into this
+        basis.
     :type names: dict or None
     :param native_gates: The native gate set to target. If None, target the QSCOUT native
         gates.
     :type native_gates: dict or None
+    :param bool remove_measurements: Ignore any measure statements in the original circuit
+        and append a measure_all gate instead. Defaults to False.
     :returns: The same quantum circuit, converted to JaqalPaq.
     :rtype: jaqalpaq.core.Circuit
-    :raises JaqalError: If any instruction acts on a qubit from a register other than the
-        circuit's qregs.
-    :raises JaqalError: If the circuit includes a snapshot instruction.
-    :raises JaqalError: If the user tries to measure or reset only some of the qubits,
-        rather than all of them.
     :raises JaqalError: If the circuit includes a gate not included in `names`.
     """
+    qreg_sizes = {}
+    for qb in tkc.qubits:
+        if len(qb.index) != 1:
+            qreg_sizes[qb.reg_name + "_".join([str(x) for x in qb.index])] = 1
+        elif qb.reg_name in qreg_sizes:
+            qreg_sizes[qb.reg_name] = max(qreg_sizes[qb.reg_name], qb.index[0] + 1)
+        else:
+            qreg_sizes[qb.reg_name] = qb.index[0] + 1
+    n = sum(qreg_sizes.values())
     if native_gates is None:
         from qscout.v1.std.jaqal_gates import ALL_GATES as native_gates
-    n = sum([qreg.size for qreg in circuit.qregs])
+
     qsc = CircuitBuilder(native_gates=native_gates)
     if names is None:
-        names = _QISKIT_NAMES
-    if param_maps is None:
-        param_maps = _PARAM_MAPS
+        names = _TKET_NAMES
     baseregister = qsc.register("baseregister", n)
     offset = 0
     registers = {}
-    for qreg in circuit.qregs:
-        registers[qreg.name] = qsc.map(
-            qreg.name, baseregister, slice(offset, offset + qreg.size)
+    for qreg in qreg_sizes:
+        registers[qreg] = qsc.map(
+            qreg, baseregister, slice(offset, offset + qreg_sizes[qreg])
         )
-        offset += qreg.size
+        offset += qreg_sizes[qreg]
     # We're going to divide the circuit up into blocks. Each block will contain every gate
     # between one barrier statement and the next. If the circuit is output with no further
     # processing, then the gates in each block will be run in sequence. However, if the
     # circuit is passed to the scheduler, it'll try to parallelize as many of the gates
     # within each block as possible, while keeping the blocks themselves sequential.
     block = UnscheduledBlockBuilder()
     qsc.expression.append(block.expression)
     block.gate("prepare_all")
     measure_accumulator = set()
-    reset_accumulator = set()
-    in_preamble = True
-    for instr in circuit.data:
-        if reset_accumulator:
-            if instr[0].name == "reset":
-                target = instr[1][0]
-                if target.register.name in registers:
-                    reset_accumulator.add(
-                        registers[target.register.name].resolve_qubit(target.index)[1]
-                    )
-                else:
-                    raise JaqalError("Register %s invalid!" % target.register.name)
-                if len(reset_accumulator) == n:
-                    block.gate("prepare_all")
-                    reset_accumulator = {}
-                continue
-            else:
-                raise JaqalError(
-                    "Cannot reset only qubits %s and not whole register."
-                    % reset_accumulator
-                )
-                # reset_accumulator = set()
-        if measure_accumulator:
-            if instr[0].name == "measure":
-                target = instr[1][0]
-                if target.register.name in registers:
-                    measure_accumulator.add(
-                        registers[target.register.name].resolve_qubit(target.index)[1]
-                    )
+    for command in tkc:
+        block, measure_accumulator = convert_command(
+            command,
+            qsc,
+            block,
+            names,
+            measure_accumulator,
+            n,
+            registers,
+            remove_measurements,
+        )
+    block.gate("measure_all", no_duplicate=True)
+    return qsc.build()
+
+
+def convert_command(
+    command,
+    qsc,
+    block,
+    names,
+    measure_accumulator,
+    n,
+    registers,
+    remove_measurements,
+    remaps=None,
+):
+    if remaps is None:
+        remaps = range(n)
+    op_type = command.op.type
+    if measure_accumulator:
+        if op_type == OpType.Measure:
+            qb = command.qubits[0]
+            if qb.reg_name in registers:
+                if len(qb.index) != 1:
+                    target = registers[
+                        qb.reg_name + "_".join([str(x) for x in qb.index])
+                    ][0]
                 else:
-                    raise JaqalError("Register %s invalid!" % target.register.name)
-                if len(measure_accumulator) == n:
-                    block.gate("measure_all")
-                    measure_accumulator = {}
-                continue
-            else:
-                raise JaqalError(
-                    "Cannot measure only qubits %s and not whole register."
-                    % reset_accumulator
-                )
-                # measure_accumulator = set()
-        if instr[0].name == "measure":
-            in_preamble = False
-            target = instr[1][0]
-            if target.register.name in registers:
-                measure_accumulator = {
-                    registers[target.register.name].resolve_qubit(target.index)[1]
-                }
-                if len(measure_accumulator) == n:
-                    block.gate("measure_all")
-                    measure_accumulator = {}
-                continue
+                    target = registers[qb.reg_name][qb.index[0]]
+                measure_accumulator.add(target.resolve_qubit()[1])
             else:
                 raise JaqalError("Register %s invalid!" % target.register.name)
-        elif instr[0].name == "reset":
-            if not in_preamble:
-                target = instr[1][0]
-                if target.register.name in registers:
-                    reset_accumulator = {
-                        registers[target.register.name].resolve_qubit(target.index)[1]
-                    }
-                    if len(reset_accumulator) == n:
-                        block.gate("prepare_all")
-                        reset_accumulator = {}
-                else:
-                    raise JaqalError("Register %s invalid!" % target.register.name)
-        elif instr[0].name == "barrier":
-            block = UnscheduledBlockBuilder()
-            qsc.expression.append(block.expression)
-            # Use barriers to inform the scheduler, as explained above.
-        elif instr[0].name == "snapshot":
+            if len(measure_accumulator) == n:
+                block.gate("measure_all")
+                measure_accumulator = set()
+            return block, measure_accumulator
+        else:
             raise JaqalError(
-                "Physical hardware does not support snapshot instructions."
+                "Cannot measure only qubits %s and not whole register."
+                % measure_accumulator
             )
-        elif instr[0].name in names:
-            in_preamble = False
-            if instr[0].name in param_maps:
-                param_map = param_maps[instr[0].name]
+            # measure_accumulator = set()
+    if op_type == OpType.Measure:
+        if not remove_measurements:
+            qb = command.qubits[0]
+            if len(qb.index) != 1:
+                target = registers[qb.reg_name + "_".join([str(x) for x in qb.index])][
+                    0
+                ]
             else:
-                param_map = param_maps["*"]
-            targets = instr[1]
-            for target in targets:
-                if target.register.name not in registers:
-                    raise JaqalError("Gate register %s invalid!" % target.register.name)
-            block.gate(
-                names[instr[0].name],
-                *[registers[target.register.name][target.index] for target in targets],
-                *param_map(targets, (float(param) for param in instr[0].params))
+                target = registers[qb.reg_name][qb.index[0]]
+            measure_accumulator = {target.resolve_qubit()[1]}
+            if len(measure_accumulator) == n:
+                block.gate("measure_all")
+                measure_accumulator = set()
+    elif op_type == OpType.Reset and remove_measurements:
+        pass
+    elif op_type == OpType.Barrier:
+        block = UnscheduledBlockBuilder()
+        qsc.expression.append(block.expression)
+        # Use barriers to inform the scheduler, as explained above.
+    elif op_type in (OpType.CircBox, OpType.ExpBox, OpType.PauliExpBox):
+        new_remaps = [remaps[qb.index[0]] for qb in command.qubits]
+        macro_block = SequentialBlockBuilder()
+        subcirq = command.op.get_circuit()
+        for cmd in subcirq:
+            convert_command(
+                cmd,
+                qsc,
+                macro_block,
+                names,
+                set(),
+                n,
+                registers,
+                remove_measurements,
+                new_remaps,
             )
-        else:
-            raise JaqalError(
-                "Instruction %s not available on trapped ion hardware; try unrolling first."
-                % instr[0].name
+        macro_name = f"macro_{len(qsc.macros)}"
+        qsc.macro(macro_name, [], macro_block)
+        block.append(qsc.build_gate(macro_name))
+        # TODO: Re-use macros when the same circuit block appears in multiple places.
+    elif op_type in names:
+        targets = command.qubits
+        qb_targets = []
+        for qb in targets:
+            if (
+                len(qb.index) != 1
+            ):  # TODO: Figure out how to pass multi-index qubits in macros.
+                qb_targets.append(
+                    registers[qb.reg_name + "_".join([str(x) for x in qb.index])][0]
+                )
+            else:
+                qb_targets.append(registers[qb.reg_name][remaps[qb.index[0]]])
+        block.gate(
+            *names[op_type](
+                *qb_targets,
+                *[float(param) * np.pi for param in command.op.params],
             )
-    block.gate("measure_all", no_duplicate=True)
-    return qsc.build()
+        )
+    else:
+        raise JaqalError(
+            "Instruction %s not available on trapped ion hardware; try unrolling first."
+            % op_type
+        )
+    return block, measure_accumulator
 
 
-def qiskit_circuit_from_jaqal_circuit(circuit, names=None):
+def tket_circuit_from_jaqal_circuit(circuit, names=None):
     """
-    Converts a :class:`jaqalpaq.core.Circuit` to a Qiskit circuit. All scheduling
-    information in the circuit will be lost in conversion.
+    Converts a :class:`jaqalpaq.core.Circuit` to a pytket circuit. All scheduling
+    information in the circuit will be lost in conversion. Loop statements and macros will
+    be unrolled.
 
     :param jaqalpaq.core.Circuit circuit: The circuit to convert.
-    :param names: A mapping from names of native Jaqal gates to the corresponding Qiskit
-        gate names. If omitted, maps R (:class:`jaqalpaq.transpilers.qiskit.JaqalRGate`),
-        Sx, Sxd, Sy (:class:`jaqalpaq.qiskit.SYGate`), Syd
-        (:class:`jaqalpaq.qiskit.SYdgGate`), Sz, Szd, Px, Py, Pz, Rz, MS
-        (:class:`jaqalpaq.qiskit.JaqalMSGate`), and Sxx
-        (:class:`jaqalpaq.qiskit.SXXGate`) to their Qiskit counterparts.
+    :param names: A mapping from names of native Jaqal gates to the corresponding pytket
+        gate names. If omitted, maps R, Sx, Sxd, Sz, Szd, Px, Py, Pz, Rz, and Sxx
+        to their pytket counterparts; and Sy, Syd, and MS to equivalent sequences of
+        pytket gates.
     :type names: dict or None
     :returns: The same quantum circuit, converted to Qiskit.
     :rtype: qiskit.circuit.QuantumCircuit
     """
     if names is None:
-        names = {v: k for k, v in _QISKIT_NAMES.items()}
+        names = _REVERSE_TKET_NAMES
 
-    qkr = {
-        reg.name: QuantumRegister(size=reg.size, name=reg.name)
+    tkr = {
+        reg.name: QubitRegister(name=reg.name, size=reg.size)
         for reg in circuit.registers.values()
         if reg.fundamental
     }
     expanded_circuit = fill_in_map(expand_subcircuits(expand_macros(circuit)))
-    visitor = QiskitTranspilationVisitor()
-    visitor.registers = qkr
+    visitor = TketTranspilationVisitor()
+    visitor.registers = tkr
     visitor.names = names
     return visitor.visit(expanded_circuit)
 
 
-class QiskitTranspilationVisitor(Visitor):
+class TketTranspilationVisitor(Visitor):
     registers = {}
     names = {}
 
     def visit_default(self, obj, *args, **kwargs):
         return obj
 
     def visit_LoopStatement(self, obj, circ):
-        subcirc = QuantumCircuit(*self.registers.values())
-        circ.compose(
-            self.visit(obj.statements, subcirc).repeat(obj.iterations), inplace=True
-        )
+        subcirc = Circuit()
+        for qreg in self.registers.values():
+            subcirc.add_q_register(qreg)
+        self.visit(obj.statements, subcirc)
+        for i in range(obj.iterations):
+            circ.append(subcirc)
         return circ
+        # TODO: This is inefficient, but at the moment I don't have a more efficient approach.
+        # If pytket implements a similar iteration construct, this should definitely be changed to use it.
 
     def visit_BlockStatement(self, obj, circ):
         for stmt in obj.statements:
             self.visit(stmt, circ)
         return circ
 
     def visit_Circuit(self, obj, circ=None):
-        circ = QuantumCircuit(*self.registers.values())
+        circ = Circuit()
+        for qreg in self.registers.values():
+            circ.add_q_register(qreg)
         return self.visit(obj.body, circ)
 
     def visit_GateStatement(self, obj, circ):
         # Note: The code originally checked if a gate was a native gate, macro, or neither,
         # and raised an exception if neither. This assumes everything not a macro is a native gate.
-        # Note: This could be more elegant with a is_macro method on gates
+        # Note: This could be more elegant with a is_macro method on gates.
         if isinstance(obj.gate_def, Macro):
             raise JaqalError("Expand macros before transpilation.")
         elif obj.name == "prepare_all":
             for reg in self.registers.values():
-                circ.reset(reg)
+                for qb in reg:
+                    circ.add_gate(OpType.Reset, [qb])
         elif obj.name == "measure_all":
-            circ.measure_all()
+            for qreg in self.registers.values():
+                for bit in qreg:
+                    cbit = Bit(len(circ.bits))
+                    circ.add_bit(cbit)
+                    circ.Measure(bit, cbit)
         else:
             classical_params = []
             quantum_params = []
             for pname, pval in obj.parameters.items():
                 if pname in [
                     cparam.name for cparam in obj.gate_def.classical_parameters
                 ]:
                     classical_params.append(self.visit(pval))
                 else:
                     quantum_params.append(self.visit(pval))
-            getattr(circ, self.names[obj.name])(*classical_params, *quantum_params)
+            [
+                circ.add_gate(*gate_data)
+                for gate_data in self.names[obj.name](
+                    *quantum_params, *classical_params
+                )
+            ]
 
     def visit_Parameter(self, obj):
         return self.visit(obj.resolve_value())
 
     def visit_NamedQubit(self, obj):
         reg, idx = obj.resolve_qubit()
         return self.registers[reg.name][idx]
-
-
-def ion_equivalence_library():
-    """
-    Constructs a `qiskit.circuit.EquivalenceLibrary` containing a few standard identities
-    for converting superconducting gates to equivalent sequences of trapped-ion gates.
-    In particular, we use an implementation of the CNOT gate taken from Maslov (2017).
-    This function is intended for internal use, but may be of utility to users designing
-    their own transpilation protocols.
-
-    :returns: The equivalence library.
-    :rtype: qiskit.circuit.EquivalenceLibrary
-    """
-    el = EquivalenceLibrary(base=StandardEquivalenceLibrary)
-    q1 = QuantumRegister(1, "q")
-    q2 = QuantumRegister(2, "q")
-    theta = Parameter("theta")
-    phi = Parameter("phi")
-    lam = Parameter("lam")
-
-    circuit = QuantumCircuit(q1, global_phase=theta / 2)
-    circuit.rz(theta, 0)
-    el.set_entry(PhaseGate(theta), [circuit])
-
-    circuit = QuantumCircuit(q1)
-    circuit.jaqalr(phi, theta, 0)
-    el.set_entry(RGate(theta, phi), [circuit])
-
-    circuit = QuantumCircuit(q1)
-    circuit.rz(lam, 0)
-    circuit.jaqalr(pi / 2, theta, 0)
-    circuit.rz(phi, 0)
-    el.set_entry(UGate(theta, phi, lam), [circuit])
-
-    circuit = QuantumCircuit(q1)
-    circuit.z(0)
-    circuit.sy(0)
-    el.set_entry(HGate(), [circuit])
-
-    circuit = QuantumCircuit(q2)
-    circuit.jaqalms(0, theta, 0, 1)
-    el.set_entry(RXXGate(theta), [circuit])
-
-    # // controlled-NOT as per Maslov (2017); this implementation takes s = v = +1
-    # gate cx a,b
-    # {
-    # ry(pi/2) a;
-    # ms(pi/2, 0) a,b;
-    # rx(-pi/2) a;
-    # rx(-pi/2) b;
-    # ry(-pi/2) a;
-    # }
-    circuit = QuantumCircuit(q2)
-    circuit.sy(0)
-    circuit.jaqalms(0, pi / 2, 0, 1)
-    circuit.sxdg(0)
-    circuit.sxdg(1)
-    circuit.sydg(0)
-    el.set_entry(CXGate(), [circuit])
-
-    return el
-
-
-def ion_pass_manager():
-    """
-    Constructs a `qiskit.transpiler.PassManager` that will unroll a circuit into the
-    QSCOUT standard gate set. Pass a `qiskit.circuit.Circuit` object into its `run` method
-    to perform the unrolling.
-
-    :returns: The pass manager.
-    :rtype: qiskit.transpiler.PassManager
-    """
-    pm = PassManager()
-    basis_gates = _QISKIT_NAMES.keys()
-    el = ion_equivalence_library()
-
-    pm.append(
-        [UnrollCustomDefinitions(el, basis_gates), BasisTranslator(el, basis_gates)]
-    )
-    return pm
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/gates.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/gates.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from qiskit.circuit import Gate, QuantumCircuit, QuantumRegister
 from qiskit.circuit.library.standard_gates.u3 import U3Gate
 from qiskit.circuit.library.standard_gates.rx import RXGate
 from qiskit.circuit.library.standard_gates.ry import RYGate
 from qiskit.circuit.library.standard_gates.rz import RZGate
 from qiskit.circuit.library.standard_gates.rxx import RXXGate
-from qiskit.qasm import pi
+from numpy import pi
 
 
 class JaqalMSGate(Gate):
     """
     The two-parameter Mølmer-Sørensen gate, as implemented on QSCOUT hardware.
     Note that this is *not* equivalent to Qiskit's MSGate. It's equivalent to ::
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/qiskit/instance.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/qiskit/instance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-from qiskit.result.result import Result
-from qiskit.providers.basejob import BaseJob
-from qiskit.providers.basebackend import BaseBackend
-from qiskit.providers.jobstatus import JobStatus
-from qiskit import Aer
 from qiskit.utils import QuantumInstance
 from .frontend import jaqal_circuit_from_qiskit_circuit, ion_pass_manager
-from qiskit.transpiler import PassManager
 from jaqalpaq.emulator import run_jaqal_circuit
 import numpy as np
 from collections import Counter
 
+try:
+    from qiskit_aer import AerSimulator
+
+    aer_simulator = True
+
+except ImportError:
+    from qiskit import Aer
+
+    aer_simulator = False
+
 
 class IonResult:
     def __init__(self, counts):
         self.counts = counts
 
     def get_counts(self, name=None):
         if len(self.counts) == 1:
@@ -87,8 +91,10 @@
     :param jaqal_backend: Pass a backend instance to use. If omitted, instantiates a new
         :class:`jaqalpaq.emulator.UnitarySerializedEmulator`, which in practice should
         usually be the desired usage.
     :type jaqal_backend: :class:`jaqalpaq.emulator.AbstractBackend` or None
     :returns: A Qiskit representation of the Jaqal emulator.
     :rtype: `qiskit.utils.QuantumInstance`
     """
-    return IonInstance(Aer.get_backend("qasm_simulator"), jaqal_backend=jaqal_backend)
+    if aer_simulator:
+        return IonInstance(AerSimulator(), jaqal_backend=jaqal_backend)
+    return IonInstance(Aer.get_backend("aer_simulator"), jaqal_backend=jaqal_backend)
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/frontend.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/frontend.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
-from jaqalpaq.error import JaqalError
 import networkx as nx
-from pyquil.device import NxDevice
+import pyquil
 from pyquil.api import QuantumComputer
 from pyquil.quilbase import Gate
 from pyquil.quilatom import unpack_qubit
 from .ioncompiler import IonCompiler
 from .qscoutam import QSCOUTAM
-import numpy as np
-import pyquil
+
+pyquil_version = [int(part) for part in pyquil.__version__.split(".")]
+
+if pyquil_version >= [3]:
+    from pyquil.quantum_processor import NxQuantumProcessor
+else:
+    from pyquil.device import NxDevice
 
 
 def get_ion_device(num_qubits):
-    return NxDevice(nx.complete_graph(num_qubits))
+    if pyquil_version >= [3]:
+        return NxQuantumProcessor(nx.complete_graph(num_qubits))
+    else:
+        return NxDevice(nx.complete_graph(num_qubits))
 
 
 def get_ion_qam():
     return QSCOUTAM()
 
 
 def get_ion_qc(num_qubits):
@@ -28,20 +35,27 @@
     be submitted to be run on the actual QSCOUT device).
 
     :param int num_qubits: How many qubits in the trap will be used.
     :returns: The quantum computer object for compilation.
     :rtype: pyquil.api.QuantumComputer
     """
     device = get_ion_device(num_qubits)
-    return QuantumComputer(
-        name="QSCOUT-%d" % num_qubits,
-        qam=get_ion_qam(),
-        device=device,
-        compiler=IonCompiler(device),
-    )
+    if pyquil_version >= [3]:
+        return QuantumComputer(
+            name="QSCOUT-%d" % num_qubits,
+            qam=get_ion_qam(),
+            compiler=IonCompiler(device),
+        )
+    else:
+        return QuantumComputer(
+            name="QSCOUT-%d" % num_qubits,
+            qam=get_ion_qam(),
+            device=device,
+            compiler=IonCompiler(device),
+        )
 
 
 def quil_gates(native_gates=None):
     """Generates quil versions of a gate set (the QSCOUT native gates, by default).
 
     :returns: A mapping of gate names to functions that take classical parameters and
         qubit indices and build pyquil gates.
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/ioncompiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
-from pyquil.api._qac import AbstractCompiler
+import pyquil
 from typing import Optional
 from pyquil.quil import Program, Gate
 from pyquil.quilbase import Measurement, ResetQubit, Reset, Declare
 from jaqalpaq.core import CircuitBuilder, Circuit
 from jaqalpaq.core.circuitbuilder import UnscheduledBlockBuilder
 from jaqalpaq.error import JaqalError
-import numpy as np
+
+pyquil_version = [int(part) for part in pyquil.__version__.split(".")]
+
+if pyquil_version >= [3]:
+    from pyquil.api import AbstractCompiler
+else:
+    from pyquil.api._qac import AbstractCompiler
 
 # We automatically map gates that have the same name up to case; for example, any gate
 # generated by quil_gates.
 
 _QUIL_NAMES = {
     "X": "Px",
     "Y": "Py",
@@ -129,15 +135,15 @@
                     )
                     # measure_accumulator = set()
             if isinstance(instr, Gate):
                 if instr.name in self.names:
                     block.gate(
                         self.names[instr.name],
                         *[qreg[qubit.index] for qubit in instr.qubits],
-                        *[float(p) for p in instr.params]
+                        *[float(p) for p in instr.params],
                     )
                     in_preamble = False
                 else:
                     raise JaqalError("Gate %s not in native gate set." % instr.name)
             elif isinstance(instr, Reset):
                 if not in_preamble:
                     block.gate("prepare_all")
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/quil/qscoutam.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,73 @@
 # Copyright 2020 National Technology & Engineering Solutions of Sandia, LLC (NTESS).
 # Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains
 # certain rights in this software.
+import pyquil
 from pyquil.api import QAM
-
 from jaqalpaq.error import JaqalError
 
+pyquil_version = [int(part) for part in pyquil.__version__.split(".")]
+
 
 class QSCOUTAM(QAM):
     """
     Quantum Abstract Machine representing the QSCOUT hardware. It will refuse to load or
     run programs, but can be used as a compilation target. Instead of using the Quil API
     to load and run programs, instead compile them to Jaqal files and submit them to
     the QSCOUT team directly.
     """
 
-    def load(self, executable):
-        """
-        Does not load a Jaqal program onto an abstraction of the QSCOUT hardware.
+    if pyquil_version >= [3]:
 
-        :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
-        """
-        raise JaqalError(
-            "QSCOUT cannot run programs through the Quil API. Generate a Jaqal file with compile() and submit it directly to the QSCOUT team."
-        )
+        def execute(
+            self,
+            executable,
+            memory_map,
+            **kwargs,
+        ):
+            """
+            Does not load a Jaqal program onto an abstraction of the QSCOUT hardware.
+
+            :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
+            """
+            raise JaqalError(
+                "QSCOUT cannot run programs through the Quil API. Generate a Jaqal file with compile() and submit it directly to the QSCOUT team."
+            )
+
+        def execute_with_memory_map_batch(self, executable, memory_maps, **kwargs):
+            """
+            Does not load a Jaqal program onto an abstraction of the QSCOUT hardware.
+
+            :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
+            """
+            raise JaqalError(
+                "QSCOUT cannot run programs through the Quil API. Generate a Jaqal file with compile() and submit it directly to the QSCOUT team."
+            )
+
+        def get_result(self, execute_response):
+            """
+            Does not load a Jaqal program onto an abstraction of the QSCOUT hardware.
+
+            :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
+            """
+            raise JaqalError(
+                "QSCOUT cannot run programs through the Quil API. Generate a Jaqal file with compile() and submit it directly to the QSCOUT team."
+            )
+
+    else:
+
+        def load(self, executable):
+            """
+            Does not load a Jaqal program onto an abstraction of the QSCOUT hardware.
+
+            :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
+            """
+            raise JaqalError(
+                "QSCOUT cannot run programs through the Quil API. Generate a Jaqal file with compile() and submit it directly to the QSCOUT team."
+            )
 
     def run(self):
         """
         Does not run a previously loaded Jaqal program on an abstraction of the QSCOUT hardware.
 
         :raises JaqalError: Because the Quil API should not be used to try to execute programs on QSCOUT.
         """
```

### Comparing `JaqalPaq-extras-1.2.0a1/src/jaqalpaq/transpilers/tket/backend.py` & `jaqalpaq_extras-1.3.0a1/src/jaqalpaq/transpilers/tket/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 # certain rights in this software.
 
 # Portions of this work are derived from the pytket extension modules which are
 # copyright 2020-2021 Cambridge Quantum Computing and used under the Apache License 2.0.
 
 from typing import (
     Any,
-    Callable,
     Dict,
     List,
     Optional,
     Sequence,
-    Tuple,
-    TypeVar,
     Union,
     cast,
-    TYPE_CHECKING,
     Set,
 )
 
 from numpy.random import default_rng
 
 from pytket.backends import Backend, CircuitStatus, ResultHandle
 from pytket.backends.backendresult import BackendResult
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/scheduler/test_scheduler.py` & `jaqalpaq_extras-1.3.0a1/tests/scheduler/test_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import unittest, pytest
-import jaqalpaq
+import unittest
+import pytest
 from jaqalpaq.core.circuitbuilder import build
 from jaqalpaq.scheduler import schedule_circuit
 
 qscout = pytest.importorskip("qscout")
 from qscout.v1.std.jaqal_gates import ALL_GATES as native_gates
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/cirq/test_cirq_transpiler.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_reverse_transpiler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-import unittest, pytest
+import unittest
+import pytest
+from jaqalpaq.core import CircuitBuilder
+from math import pi
 
-import jaqalpaq
+qiskit = pytest.importorskip("qiskit")
+from qiskit.circuit import QuantumCircuit, QuantumRegister
+from jaqalpaq.transpilers.qiskit import qiskit_circuit_from_jaqal_circuit
+from qscout.v1.std import jaqal_gates
 
-cirq = pytest.importorskip("cirq")
 
-from jaqalpaq.transpilers.cirq import jaqal_circuit_from_cirq_circuit
-from jaqalpaq.generator import generate_jaqal_program
-from math import pi
-from jaqalpaq.core import CircuitBuilder
+class PytketReverseTranspilerTester(unittest.TestCase):
+    def test_prepare_bell_pairs(self):
+        jcirc = CircuitBuilder(jaqal_gates.ALL_GATES)
+        reg1 = jcirc.register("q", 2)
+        block = jcirc.block()
+        block.gate("prepare_all")
+        block.gate("MS", reg1[0], reg1[1], pi / 4, pi / 2)
+        block.gate("measure_all")
+        built = jcirc.build()
+        transpiled = qiskit_circuit_from_jaqal_circuit(built)
 
+        qr = QuantumRegister(2, "q")
+        qkc = QuantumCircuit(qr)
+        qkc.reset(range(2))
+        qkc.jaqalms(pi / 4, pi / 2, qr[0], qr[1])
+        qkc.measure_all()
 
-class CirqTranspilerTester(unittest.TestCase):
-    def test_transpile_line_circuit(self):
-        c = cirq.Circuit()
-        qubits = [cirq.LineQubit(0), cirq.LineQubit(1)]
-        c.append(cirq.H.on(qubits[0]))
-        c.append(cirq.CNOT(*qubits))
-        ic = cirq.ConvertToIonGates().convert_circuit(c)
-        ic.append(
-            cirq.measure_each(*qubits),
-            strategy=cirq.circuits.InsertStrategy.NEW_THEN_INLINE,
-        )
-        jc = jaqal_circuit_from_cirq_circuit(ic)
-        jcirc = CircuitBuilder()
-        reg = jcirc.register("allqubits", 2)
-        jcirc.gate("prepare_all")
-        jcirc.gate("R", reg[0], pi, pi)
-        jcirc.gate("MS", reg[0], reg[1], 0, pi / 2)
-        block = jcirc.block(True)
-        block.gate("R", reg[0], -1.5707963267948972, pi / 2)
-        # Last few digits are off if we just use -pi/2
-        block.gate("R", reg[1], pi, pi / 2)
-        jcirc.gate("Rz", reg[0], -pi / 2)
-        jcirc.gate("measure_all")
-        self.assertEqual(
-            generate_jaqal_program(jcirc.build()), generate_jaqal_program(jc)
-        )
+        self.assertEqual(str(qkc.draw()), str(transpiled.draw()))
+        # We compare the circuit diagrams because comparing the QASM means that we miss circuits that have the same gates re-ordered in a commuting way.
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/projectq/test_projectq_transpiler.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/projectq/test_projectq_transpiler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-import unittest, pytest
-
-import jaqalpaq
+import unittest
+import pytest
 
 projectq = pytest.importorskip("projectq")
 
-import projectq
-from projectq.cengines import MainEngine, DummyEngine
-from projectq.ops import SqrtX, H, CNOT, Rz, Measure, Rx, Ry, Rxx, Ryy, All, Barrier
+from projectq.cengines import MainEngine
+from projectq.ops import SqrtX, Measure, Rxx, All, Barrier
 from jaqalpaq.transpilers.projectq import get_engine_list, JaqalBackend
 from jaqalpaq.generator import generate_jaqal_program
-from math import pi
 from jaqalpaq.core import CircuitBuilder
 
 
 class ProjectQTranspilerTester(unittest.TestCase):
     def test_transpile_circuit(self):
         backend = JaqalBackend()
         engine_list = get_engine_list()
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/qiskit/test_qiskit_gates.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/qiskit/test_qiskit_gates.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import unittest, pytest
-
-import jaqalpaq
+import unittest
+import pytest
+from math import pi
 
 qiskit = pytest.importorskip("qiskit")
-
-from jaqalpaq.transpilers.qiskit import JaqalMSGate, SYGate, SYdgGate, JaqalRGate
 from qiskit.circuit import QuantumCircuit, QuantumRegister
-from math import pi
 
 
 class QiskitGateTester(unittest.TestCase):
     def test_msgate(self):
         qr = QuantumRegister(2)
         circ = QuantumCircuit(qr)
         circ.jaqalms(pi / 4, pi / 4, qr[0], qr[1])
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/quil/test_quil.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/quil/test_quil.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import unittest, pytest
-import jaqalpaq
+import unittest
+import pytest
+from jaqalpaq.core import CircuitBuilder
+from jaqalpaq.generator import generate_jaqal_program
 
 pyquil = pytest.importorskip("pyquil")
-
+from jaqalpaq.transpilers.quil import *
 from pyquil import Program
 from pyquil.gates import *
-from numpy import pi
-from jaqalpaq.transpilers.quil import *
-from jaqalpaq.core import CircuitBuilder
-from jaqalpaq.generator import generate_jaqal_program
 
 
 class QuilTranspilerTester(unittest.TestCase):
     def test_1_ion_compilation(self):
         p = Program()
         ro = p.declare("ro", "BIT", 3)
         p += X(0)
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_backend.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-import unittest, pytest
-
-import jaqalpaq
+import unittest
+import pytest
 
 pytket = pytest.importorskip("pytket")
-
 from jaqalpaq.transpilers.tket import JaqalBackend
 from pytket import Circuit
 
 
 class PytketBackendTester(unittest.TestCase):
     def test_prepare_bell_pairs(self):
         circ = Circuit(2, 2)
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_reverse_transpiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import unittest, pytest
-
-import jaqalpaq
+import unittest
+import pytest
+from jaqalpaq.core import CircuitBuilder
+from math import pi
 
 pytket = pytest.importorskip("pytket")
-
-from jaqalpaq.core import CircuitBuilder
 from jaqalpaq.transpilers.tket import JaqalBackend, tket_circuit_from_jaqal_circuit
-from pytket import Circuit
-from math import pi
+
 from qscout.v1.std import jaqal_gates
 
 
 class PytketReverseTranspilerTester(unittest.TestCase):
     def test_prepare_bell_pairs(self):
         jcirc = CircuitBuilder(jaqal_gates.ALL_GATES)
         reg1 = jcirc.register("q", 2)
```

### Comparing `JaqalPaq-extras-1.2.0a1/tests/transpilers/tket/test_tket_transpiler.py` & `jaqalpaq_extras-1.3.0a1/tests/transpilers/tket/test_tket_transpiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import unittest, pytest
-
-import jaqalpaq
+import unittest
+import pytest
+from jaqalpaq.generator import generate_jaqal_program
+from math import pi
+from jaqalpaq.core import CircuitBuilder
 
 pytket = pytest.importorskip("pytket")
-
 from jaqalpaq.transpilers.tket import jaqal_circuit_from_tket_circuit
-from jaqalpaq.generator import generate_jaqal_program
-from numpy import pi
-from jaqalpaq.core import CircuitBuilder
 from pytket import Circuit
 
+pytket_version = [int(part) for part in pytket.__version__.split(".")]
+
 
 class PytketTranspilerTester(unittest.TestCase):
     def test_transpile_1q_circuit(self):
         c = Circuit(1, 1)
         c.Rz(1, 0)
         c.add_barrier([0])
         c.Measure(0, 0)
@@ -47,15 +47,18 @@
         block.gate("measure_all")
         self.assertEqual(
             generate_jaqal_program(jcirc.build()), generate_jaqal_program(qsc)
         )
 
     def test_transpile_grid_circuit(self):
         c = Circuit()
-        qb = pytket._tket.circuit.Qubit("grid", 0, 0)
+        if pytket_version <= [1, 11, 0]:
+            qb = pytket._tket.circuit.Qubit("grid", 0, 0)
+        else:
+            qb = pytket.unit_id.Qubit("grid", 0, 0)
         c.add_qubit(qb)
         c.Rz(1, qb)
         qsc = jaqal_circuit_from_tket_circuit(c)
         jcirc = CircuitBuilder()
         reg = jcirc.register("baseregister", 1)
         reg2 = jcirc.map("grid0_0", reg, slice(0, 1, 1))
         block = jcirc.block()
```

