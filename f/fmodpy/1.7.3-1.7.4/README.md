# Comparing `tmp/fmodpy-1.7.3.tar.gz` & `tmp/fmodpy-1.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmodpy-1.7.3.tar", last modified: Wed Mar  6 08:55:36 2024, max compression
+gzip compressed data, was "fmodpy-1.7.4.tar", last modified: Tue May 14 03:37:49 2024, max compression
```

## Comparing `fmodpy-1.7.3.tar` & `fmodpy-1.7.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.778183 fmodpy-1.7.3/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1072 2022-03-18 19:21:33.000000 fmodpy-1.7.3/LICENSE.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       27 2022-07-26 13:43:21.000000 fmodpy-1.7.3/MANIFEST.in
--rw-r--r--   0 thomaslux   (501) staff       (20)      780 2024-03-06 08:55:36.778112 fmodpy-1.7.3/PKG-INFO
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.765733 fmodpy-1.7.3/fmodpy/
--rw-r--r--   0 thomaslux   (501) staff       (20)      658 2022-07-18 14:21:02.000000 fmodpy-1.7.3/fmodpy/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1148 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/__main__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.767703 fmodpy-1.7.3/fmodpy/about/
--rw-r--r--   0 thomaslux   (501) staff       (20)       47 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/author.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)      607 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/classifiers.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       72 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/description.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       31 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/keywords.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        5 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/on_pypi.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       12 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/about/requirements.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        6 2024-03-06 08:46:26.000000 fmodpy-1.7.3/fmodpy/about/version.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)     5705 2024-03-06 08:55:34.000000 fmodpy-1.7.3/fmodpy/about/version_history.md
--rw-r--r--   0 thomaslux   (501) staff       (20)    12323 2023-06-16 04:39:57.000000 fmodpy-1.7.3/fmodpy/config.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.768363 fmodpy-1.7.3/fmodpy/development/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1136 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/development/strange_type_example.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)     5060 2022-04-09 14:56:15.000000 fmodpy-1.7.3/fmodpy/development/todo.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      874 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/development/type.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      522 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/exceptions.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    34638 2024-03-06 08:52:18.000000 fmodpy-1.7.3/fmodpy/fmodpy.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.771331 fmodpy-1.7.3/fmodpy/parsing/
--rw-r--r--   0 thomaslux   (501) staff       (20)    10893 2023-11-17 15:21:16.000000 fmodpy-1.7.3/fmodpy/parsing/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     2926 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/_old_code.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)    43536 2024-01-26 15:08:21.000000 fmodpy-1.7.3/fmodpy/parsing/argument.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1033 2023-06-17 15:43:32.000000 fmodpy-1.7.3/fmodpy/parsing/character.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    15118 2024-01-26 15:18:16.000000 fmodpy-1.7.3/fmodpy/parsing/code.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1600 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/complex.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     6082 2024-03-06 08:25:49.000000 fmodpy-1.7.3/fmodpy/parsing/file.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     2853 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/function.py
--rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/implicit_none.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      162 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/integer.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1563 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/interface.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      950 2023-04-06 04:56:34.000000 fmodpy-1.7.3/fmodpy/parsing/logical.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     7614 2023-06-17 03:34:05.000000 fmodpy-1.7.3/fmodpy/parsing/module.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      118 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/procedure.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      160 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/real.py
--rw-r--r--   0 thomaslux   (501) staff       (20)    22068 2024-01-26 15:25:46.000000 fmodpy-1.7.3/fmodpy/parsing/subroutine.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     6315 2022-05-10 02:34:01.000000 fmodpy-1.7.3/fmodpy/parsing/type.py
--rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/parsing/use.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     6807 2023-11-17 16:31:40.000000 fmodpy-1.7.3/fmodpy/parsing/util.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.771774 fmodpy-1.7.3/fmodpy/test/
--rw-r--r--   0 thomaslux   (501) staff       (20)    53248 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/.coverage
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.772063 fmodpy-1.7.3/fmodpy/test/character/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1522 2023-06-17 16:32:35.000000 fmodpy-1.7.3/fmodpy/test/character/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      807 2023-06-17 16:32:32.000000 fmodpy-1.7.3/fmodpy/test/character/test_character.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.772338 fmodpy-1.7.3/fmodpy/test/complex128/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2311 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex128/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex128/test_complex128.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.772632 fmodpy-1.7.3/fmodpy/test/complex256/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2377 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex256/__init__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.772958 fmodpy-1.7.3/fmodpy/test/complex256/test_complex256/
--rw-r--r--   0 thomaslux   (501) staff       (20)     7751 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)    13250 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3978 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex256/test_complex256.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.773288 fmodpy-1.7.3/fmodpy/test/complex64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2309 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/complex64/test_complex64.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.773545 fmodpy-1.7.3/fmodpy/test/double_precision/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/double_precision/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3626 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/double_precision/test_double_precision.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.773818 fmodpy-1.7.3/fmodpy/test/fixed_format/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1545 2023-11-17 16:28:26.000000 fmodpy-1.7.3/fmodpy/test/fixed_format/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      488 2023-11-17 16:28:09.000000 fmodpy-1.7.3/fmodpy/test/fixed_format/test_fixed_format.f
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.774080 fmodpy-1.7.3/fmodpy/test/int32/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2256 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/int32/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3411 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/int32/test_int32.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.774358 fmodpy-1.7.3/fmodpy/test/int64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2427 2022-08-27 16:58:36.000000 fmodpy-1.7.3/fmodpy/test/int64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     4008 2022-08-27 16:57:13.000000 fmodpy-1.7.3/fmodpy/test/int64/test_int64.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.774650 fmodpy-1.7.3/fmodpy/test/logical/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1435 2022-03-27 18:02:26.000000 fmodpy-1.7.3/fmodpy/test/logical/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      663 2022-03-27 17:59:28.000000 fmodpy-1.7.3/fmodpy/test/logical/test_logical.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.775231 fmodpy-1.7.3/fmodpy/test/misc/
--rw-r--r--   0 thomaslux   (501) staff       (20)      932 2022-05-10 02:37:20.000000 fmodpy-1.7.3/fmodpy/test/misc/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      212 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/misc/implicit_shape.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)      271 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/misc/simple.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)      307 2022-05-10 02:24:48.000000 fmodpy-1.7.3/fmodpy/test/misc/subroutine_with_type.f90
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.775670 fmodpy-1.7.3/fmodpy/test/module/
--rw-r--r--   0 thomaslux   (501) staff       (20)     3173 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/module/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)      173 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/module/extra_module.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     1364 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/module/test_module.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.775995 fmodpy-1.7.3/fmodpy/test/procedure/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1134 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/procedure/__init__.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.776543 fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/
--rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     1624 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure.pyx
--rw-r--r--   0 thomaslux   (501) staff       (20)     2078 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90
--rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/procedure/procedure.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.776879 fmodpy-1.7.3/fmodpy/test/real32/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2261 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/real32/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3368 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/real32/test_real32.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.777154 fmodpy-1.7.3/fmodpy/test/real64/
--rw-r--r--   0 thomaslux   (501) staff       (20)     2497 2024-01-26 15:20:15.000000 fmodpy-1.7.3/fmodpy/test/real64/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     3983 2024-01-26 15:15:55.000000 fmodpy-1.7.3/fmodpy/test/real64/test_real64.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     3781 2023-11-17 16:29:16.000000 fmodpy-1.7.3/fmodpy/test/test.py
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.777701 fmodpy-1.7.3/fmodpy/test/type/
--rw-r--r--   0 thomaslux   (501) staff       (20)     3219 2023-06-17 22:23:55.000000 fmodpy-1.7.3/fmodpy/test/type/__init__.py
--rw-r--r--   0 thomaslux   (501) staff       (20)     1373 2022-03-18 19:21:33.000000 fmodpy-1.7.3/fmodpy/test/type/derived_type_error.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)     4828 2023-06-17 22:22:44.000000 fmodpy-1.7.3/fmodpy/test/type/test_type.f03
--rw-r--r--   0 thomaslux   (501) staff       (20)      134 2023-06-17 21:31:36.000000 fmodpy-1.7.3/fmodpy/test/type/test_type_aux.f03
-drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-03-06 08:55:36.777891 fmodpy-1.7.3/fmodpy.egg-info/
--rw-r--r--   0 thomaslux   (501) staff       (20)      780 2024-03-06 08:55:36.000000 fmodpy-1.7.3/fmodpy.egg-info/PKG-INFO
--rw-r--r--   0 thomaslux   (501) staff       (20)     2688 2024-03-06 08:55:36.000000 fmodpy-1.7.3/fmodpy.egg-info/SOURCES.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        1 2024-03-06 08:55:36.000000 fmodpy-1.7.3/fmodpy.egg-info/dependency_links.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)       12 2024-03-06 08:55:36.000000 fmodpy-1.7.3/fmodpy.egg-info/requires.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)        7 2024-03-06 08:55:36.000000 fmodpy-1.7.3/fmodpy.egg-info/top_level.txt
--rw-r--r--   0 thomaslux   (501) staff       (20)      108 2024-03-06 08:55:36.778408 fmodpy-1.7.3/setup.cfg
--rw-r--r--   0 thomaslux   (501) staff       (20)     2652 2022-03-18 19:21:33.000000 fmodpy-1.7.3/setup.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.284642 fmodpy-1.7.4/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1072 2022-03-18 19:21:33.000000 fmodpy-1.7.4/LICENSE.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       27 2022-07-26 13:43:21.000000 fmodpy-1.7.4/MANIFEST.in
+-rw-r--r--   0 thomaslux   (501) staff       (20)      780 2024-05-14 03:37:49.284563 fmodpy-1.7.4/PKG-INFO
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.268658 fmodpy-1.7.4/fmodpy/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      658 2022-07-18 14:21:02.000000 fmodpy-1.7.4/fmodpy/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1148 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/__main__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.270754 fmodpy-1.7.4/fmodpy/about/
+-rw-r--r--   0 thomaslux   (501) staff       (20)       47 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/author.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)      607 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/classifiers.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       72 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/description.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       31 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/keywords.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        5 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/on_pypi.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       12 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/about/requirements.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        6 2024-03-06 08:55:38.000000 fmodpy-1.7.4/fmodpy/about/version.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)     5810 2024-05-14 03:37:46.000000 fmodpy-1.7.4/fmodpy/about/version_history.md
+-rw-r--r--   0 thomaslux   (501) staff       (20)    12323 2023-06-16 04:39:57.000000 fmodpy-1.7.4/fmodpy/config.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.271376 fmodpy-1.7.4/fmodpy/development/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1136 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/development/strange_type_example.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)     5060 2022-04-09 14:56:15.000000 fmodpy-1.7.4/fmodpy/development/todo.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      874 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/development/type.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      522 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/exceptions.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    34638 2024-03-06 08:52:18.000000 fmodpy-1.7.4/fmodpy/fmodpy.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.274720 fmodpy-1.7.4/fmodpy/parsing/
+-rw-r--r--   0 thomaslux   (501) staff       (20)    10893 2023-11-17 15:21:16.000000 fmodpy-1.7.4/fmodpy/parsing/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2926 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/_old_code.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)    44195 2024-05-14 03:36:08.000000 fmodpy-1.7.4/fmodpy/parsing/argument.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1033 2023-06-17 15:43:32.000000 fmodpy-1.7.4/fmodpy/parsing/character.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    15118 2024-01-26 15:18:16.000000 fmodpy-1.7.4/fmodpy/parsing/code.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1600 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/complex.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6082 2024-03-06 08:25:49.000000 fmodpy-1.7.4/fmodpy/parsing/file.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2853 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/function.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/implicit_none.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      162 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/integer.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1563 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/interface.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      950 2023-04-06 04:56:34.000000 fmodpy-1.7.4/fmodpy/parsing/logical.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     7614 2023-06-17 03:34:05.000000 fmodpy-1.7.4/fmodpy/parsing/module.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      118 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/procedure.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      160 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/real.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)    22068 2024-01-26 15:25:46.000000 fmodpy-1.7.4/fmodpy/parsing/subroutine.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6315 2022-05-10 02:34:01.000000 fmodpy-1.7.4/fmodpy/parsing/type.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)        0 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/parsing/use.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     6807 2023-11-17 16:31:40.000000 fmodpy-1.7.4/fmodpy/parsing/util.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.275481 fmodpy-1.7.4/fmodpy/test/
+-rw-r--r--   0 thomaslux   (501) staff       (20)    53248 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/.coverage
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.276015 fmodpy-1.7.4/fmodpy/test/character/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1522 2023-06-17 16:32:35.000000 fmodpy-1.7.4/fmodpy/test/character/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      807 2023-06-17 16:32:32.000000 fmodpy-1.7.4/fmodpy/test/character/test_character.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.276470 fmodpy-1.7.4/fmodpy/test/complex128/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2311 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex128/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex128/test_complex128.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.276819 fmodpy-1.7.4/fmodpy/test/complex256/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2377 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex256/__init__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.277189 fmodpy-1.7.4/fmodpy/test/complex256/test_complex256/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     7751 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)    13250 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3978 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex256/test_complex256.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.277555 fmodpy-1.7.4/fmodpy/test/complex64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2309 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3655 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/complex64/test_complex64.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.277895 fmodpy-1.7.4/fmodpy/test/double_precision/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2252 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/double_precision/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3626 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/double_precision/test_double_precision.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.278328 fmodpy-1.7.4/fmodpy/test/fixed_format/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1545 2023-11-17 16:28:26.000000 fmodpy-1.7.4/fmodpy/test/fixed_format/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      488 2023-11-17 16:28:09.000000 fmodpy-1.7.4/fmodpy/test/fixed_format/test_fixed_format.f
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.278743 fmodpy-1.7.4/fmodpy/test/int32/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2256 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/int32/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3411 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/int32/test_int32.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.279207 fmodpy-1.7.4/fmodpy/test/int64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2427 2022-08-27 16:58:36.000000 fmodpy-1.7.4/fmodpy/test/int64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     4008 2022-08-27 16:57:13.000000 fmodpy-1.7.4/fmodpy/test/int64/test_int64.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.279654 fmodpy-1.7.4/fmodpy/test/logical/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1435 2022-03-27 18:02:26.000000 fmodpy-1.7.4/fmodpy/test/logical/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      663 2022-03-27 17:59:28.000000 fmodpy-1.7.4/fmodpy/test/logical/test_logical.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.280451 fmodpy-1.7.4/fmodpy/test/misc/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      932 2022-05-10 02:37:20.000000 fmodpy-1.7.4/fmodpy/test/misc/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      212 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/misc/implicit_shape.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)      271 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/misc/simple.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)      307 2022-05-10 02:24:48.000000 fmodpy-1.7.4/fmodpy/test/misc/subroutine_with_type.f90
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.281098 fmodpy-1.7.4/fmodpy/test/module/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3173 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/module/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)      173 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/module/extra_module.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1364 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/module/test_module.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.281499 fmodpy-1.7.4/fmodpy/test/procedure/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1134 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/procedure/__init__.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.282060 fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1624 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure.pyx
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2078 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1253 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/procedure/procedure.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.282447 fmodpy-1.7.4/fmodpy/test/real32/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2261 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/real32/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3368 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/real32/test_real32.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.283038 fmodpy-1.7.4/fmodpy/test/real64/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2497 2024-01-26 15:20:15.000000 fmodpy-1.7.4/fmodpy/test/real64/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3983 2024-01-26 15:15:55.000000 fmodpy-1.7.4/fmodpy/test/real64/test_real64.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3781 2023-11-17 16:29:16.000000 fmodpy-1.7.4/fmodpy/test/test.py
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.283956 fmodpy-1.7.4/fmodpy/test/type/
+-rw-r--r--   0 thomaslux   (501) staff       (20)     3219 2023-06-17 22:23:55.000000 fmodpy-1.7.4/fmodpy/test/type/__init__.py
+-rw-r--r--   0 thomaslux   (501) staff       (20)     1373 2022-03-18 19:21:33.000000 fmodpy-1.7.4/fmodpy/test/type/derived_type_error.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)     4828 2023-06-17 22:22:44.000000 fmodpy-1.7.4/fmodpy/test/type/test_type.f03
+-rw-r--r--   0 thomaslux   (501) staff       (20)      134 2023-06-17 21:31:36.000000 fmodpy-1.7.4/fmodpy/test/type/test_type_aux.f03
+drwxr-xr-x   0 thomaslux   (501) staff       (20)        0 2024-05-14 03:37:49.284298 fmodpy-1.7.4/fmodpy.egg-info/
+-rw-r--r--   0 thomaslux   (501) staff       (20)      780 2024-05-14 03:37:49.000000 fmodpy-1.7.4/fmodpy.egg-info/PKG-INFO
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2688 2024-05-14 03:37:49.000000 fmodpy-1.7.4/fmodpy.egg-info/SOURCES.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        1 2024-05-14 03:37:49.000000 fmodpy-1.7.4/fmodpy.egg-info/dependency_links.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)       12 2024-05-14 03:37:49.000000 fmodpy-1.7.4/fmodpy.egg-info/requires.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)        7 2024-05-14 03:37:49.000000 fmodpy-1.7.4/fmodpy.egg-info/top_level.txt
+-rw-r--r--   0 thomaslux   (501) staff       (20)      108 2024-05-14 03:37:49.284934 fmodpy-1.7.4/setup.cfg
+-rw-r--r--   0 thomaslux   (501) staff       (20)     2652 2022-03-18 19:21:33.000000 fmodpy-1.7.4/setup.py
```

### Comparing `fmodpy-1.7.3/LICENSE.txt` & `fmodpy-1.7.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/PKG-INFO` & `fmodpy-1.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fmodpy
-Version: 1.7.3
+Version: 1.7.4
 Summary: A lightweight, efficient, highly automated, fortran wrapper for python.
 Home-page: https://github.com/tchlux/fmodpy
-Download-URL: https://github.com/tchlux/fmodpy/archive/1.7.3.tar.gz
+Download-URL: https://github.com/tchlux/fmodpy/archive/1.7.4.tar.gz
 Author: Thomas C.H. Lux
 Author-email: thomas.ch.lux@gmail.com
 License: MIT
 Keywords: python,python3,fortran,wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fmodpy-1.7.3/fmodpy/__init__.py` & `fmodpy-1.7.4/fmodpy/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/__main__.py` & `fmodpy-1.7.4/fmodpy/__main__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/about/classifiers.txt` & `fmodpy-1.7.4/fmodpy/about/classifiers.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/about/version_history.md` & `fmodpy-1.7.4/fmodpy/about/version_history.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,7 +27,8 @@
 | 1.5.6<br>March 2023 | Making some 'os.remove' operations safer by checking <br> for path existence. Refactored 'f_compiler_args' <br> into two more parts, 'optimization_level' and <br> 'shared_object_args', so that the typical '-fPIC <br> -shared' do not need to be included when adding <br> custom compilation arguments. |
 | 1.5.7<br>April 2023 | Delayed warning message about LOGICAL arrays until <br> those arguments actually have a python interface <br> generated. This is to prevent parsed-but-unused <br> subroutine arguments from creating noise. |
 | 1.6.0<br>June 2023 | Added support for Fortran strings. Updated the <br> generated codes to automatically check for source <br> code modifications when loading and recompile if the <br> source code was modified. |
 | 1.7.0<br>November 2023 | Added support for parsing PARAMETER lines in fixed <br> format Fortran. |
 | 1.7.1<br>January 2024 | Fixed bug in type of return argument for allocatable <br> arrays. Updated messaging about implicit typing to <br> be more useful. |
 | 1.7.2<br>March 2024 | Updating command execution to use a list of <br> arguments instead of string join and 'shell=True'. <br> Moved compile options to the end of the argument <br> list to ensure that libraries are included correctly <br> in compiled shared object. |
 | 1.7.3<br>March 2024 | A commensurate update to size check compilations <br> that was made in the previous update. Moving library <br> specification to the back of the list of arguments <br> for the compiler to ensure dependencies are included <br> correctly. |
+| 1.7.4<br>May 2024 | Add support for 'size(a,1,kind=int64)' style size <br> specifications of inputs. |
```

### Comparing `fmodpy-1.7.3/fmodpy/config.py` & `fmodpy-1.7.4/fmodpy/config.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/development/strange_type_example.f90` & `fmodpy-1.7.4/fmodpy/development/strange_type_example.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/development/todo.py` & `fmodpy-1.7.4/fmodpy/development/todo.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/development/type.py` & `fmodpy-1.7.4/fmodpy/development/type.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/exceptions.py` & `fmodpy-1.7.4/fmodpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/fmodpy.py` & `fmodpy-1.7.4/fmodpy/fmodpy.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/__init__.py` & `fmodpy-1.7.4/fmodpy/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/_old_code.txt` & `fmodpy-1.7.4/fmodpy/parsing/_old_code.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/argument.py` & `fmodpy-1.7.4/fmodpy/parsing/argument.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,14 +669,24 @@
                     for i in range(len(slices)):
                         if (slices[i].strip() == ":"): continue
                         try:
                             slices[i] = str(int(slices[i])-1)
                         except ValueError:
                             slices[i] += "-1"
                     func_replacement = f"{name}[{','.join(slices)}].size"
+                # If this is formatted as "<slice>[,<slice>][,<kind>]", translate the slice(s)..
+                elif (re.match(r"^\s*(:|[\w]+)\s*(,\s*(:|([\w]+(=\s*\w+\s*)?)))*$", argument) is not None):
+                    slices = argument.split(",")[:2]
+                    for i in range(min(len(slices), 2)):  # Skip "KIND=..." optional third argument.
+                        if (slices[i].strip() == ":"): continue
+                        try:
+                            slices[i] = str(int(slices[i])-1)
+                        except ValueError:
+                            slices[i] += "-1"
+                    func_replacement = ','.join(slices)
                 # Otherwise, the contents of `SIZE(...)` cannot be parsed successfully.
                 else:
                     raise(NotImplementedError("The contents of 'SIZE' could not be parsed successfully. If this is valid Fortran syntax, consider raising an issue with a minimum necessary example from this code.\n\n  "+size))
                 # Replace float division with integer division in python.
                 size = before_call + func_replacement + after_call
             # Append this NumPy size.
             sizes.append(size)
```

### Comparing `fmodpy-1.7.3/fmodpy/parsing/character.py` & `fmodpy-1.7.4/fmodpy/parsing/character.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/code.py` & `fmodpy-1.7.4/fmodpy/parsing/code.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/complex.py` & `fmodpy-1.7.4/fmodpy/parsing/complex.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/file.py` & `fmodpy-1.7.4/fmodpy/parsing/file.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/function.py` & `fmodpy-1.7.4/fmodpy/parsing/function.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/interface.py` & `fmodpy-1.7.4/fmodpy/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/logical.py` & `fmodpy-1.7.4/fmodpy/parsing/logical.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/module.py` & `fmodpy-1.7.4/fmodpy/parsing/module.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/subroutine.py` & `fmodpy-1.7.4/fmodpy/parsing/subroutine.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/type.py` & `fmodpy-1.7.4/fmodpy/parsing/type.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/parsing/util.py` & `fmodpy-1.7.4/fmodpy/parsing/util.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/.coverage` & `fmodpy-1.7.4/fmodpy/test/.coverage`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/character/__init__.py` & `fmodpy-1.7.4/fmodpy/test/character/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/character/test_character.f03` & `fmodpy-1.7.4/fmodpy/test/character/test_character.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex128/__init__.py` & `fmodpy-1.7.4/fmodpy/test/complex128/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex128/test_complex128.f03` & `fmodpy-1.7.4/fmodpy/test/complex128/test_complex128.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex256/__init__.py` & `fmodpy-1.7.4/fmodpy/test/complex256/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90` & `fmodpy-1.7.4/fmodpy/test/complex256/test_complex256/test_complex256_c_wrapper.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py` & `fmodpy-1.7.4/fmodpy/test/complex256/test_complex256/test_complex256_python_wrapper.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex256/test_complex256.f03` & `fmodpy-1.7.4/fmodpy/test/complex256/test_complex256.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex64/__init__.py` & `fmodpy-1.7.4/fmodpy/test/complex64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/complex64/test_complex64.f03` & `fmodpy-1.7.4/fmodpy/test/complex64/test_complex64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/double_precision/__init__.py` & `fmodpy-1.7.4/fmodpy/test/double_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/double_precision/test_double_precision.f03` & `fmodpy-1.7.4/fmodpy/test/double_precision/test_double_precision.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/fixed_format/__init__.py` & `fmodpy-1.7.4/fmodpy/test/fixed_format/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/int32/__init__.py` & `fmodpy-1.7.4/fmodpy/test/int32/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/int32/test_int32.f03` & `fmodpy-1.7.4/fmodpy/test/int32/test_int32.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/int64/__init__.py` & `fmodpy-1.7.4/fmodpy/test/int64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/int64/test_int64.f03` & `fmodpy-1.7.4/fmodpy/test/int64/test_int64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/logical/__init__.py` & `fmodpy-1.7.4/fmodpy/test/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/logical/test_logical.f03` & `fmodpy-1.7.4/fmodpy/test/logical/test_logical.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/misc/__init__.py` & `fmodpy-1.7.4/fmodpy/test/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/module/__init__.py` & `fmodpy-1.7.4/fmodpy/test/module/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/module/test_module.f03` & `fmodpy-1.7.4/fmodpy/test/module/test_module.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/procedure/__init__.py` & `fmodpy-1.7.4/fmodpy/test/procedure/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure.f03` & `fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure.pyx` & `fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure.pyx`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90` & `fmodpy-1.7.4/fmodpy/test/procedure/og_procedure/procedure_c_to_f.f90`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/procedure/procedure.f03` & `fmodpy-1.7.4/fmodpy/test/procedure/procedure.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/real32/__init__.py` & `fmodpy-1.7.4/fmodpy/test/real32/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/real32/test_real32.f03` & `fmodpy-1.7.4/fmodpy/test/real32/test_real32.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/real64/__init__.py` & `fmodpy-1.7.4/fmodpy/test/real64/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/real64/test_real64.f03` & `fmodpy-1.7.4/fmodpy/test/real64/test_real64.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/test.py` & `fmodpy-1.7.4/fmodpy/test/test.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/type/__init__.py` & `fmodpy-1.7.4/fmodpy/test/type/__init__.py`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/type/derived_type_error.f03` & `fmodpy-1.7.4/fmodpy/test/type/derived_type_error.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy/test/type/test_type.f03` & `fmodpy-1.7.4/fmodpy/test/type/test_type.f03`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/fmodpy.egg-info/PKG-INFO` & `fmodpy-1.7.4/fmodpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fmodpy
-Version: 1.7.3
+Version: 1.7.4
 Summary: A lightweight, efficient, highly automated, fortran wrapper for python.
 Home-page: https://github.com/tchlux/fmodpy
-Download-URL: https://github.com/tchlux/fmodpy/archive/1.7.3.tar.gz
+Download-URL: https://github.com/tchlux/fmodpy/archive/1.7.4.tar.gz
 Author: Thomas C.H. Lux
 Author-email: thomas.ch.lux@gmail.com
 License: MIT
 Keywords: python,python3,fortran,wrapper
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fmodpy-1.7.3/fmodpy.egg-info/SOURCES.txt` & `fmodpy-1.7.4/fmodpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmodpy-1.7.3/setup.py` & `fmodpy-1.7.4/setup.py`

 * *Files identical despite different names*

