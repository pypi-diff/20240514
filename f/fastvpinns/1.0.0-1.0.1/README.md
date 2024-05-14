# Comparing `tmp/fastvpinns-1.0.0.tar.gz` & `tmp/fastvpinns-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastvpinns-1.0.0.tar", last modified: Sat May 11 11:27:02 2024, max compression
+gzip compressed data, was "fastvpinns-1.0.1.tar", last modified: Tue May 14 13:29:38 2024, max compression
```

## Comparing `fastvpinns-1.0.0.tar` & `fastvpinns-1.0.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)      298 2024-04-22 12:11:53.000000 fastvpinns-1.0.0/CHANGELOG
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     5202 2024-05-03 06:32:46.000000 fastvpinns-1.0.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1081 2024-04-30 11:07:45.000000 fastvpinns-1.0.0/CONTRIBUTING.md
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1107 2024-04-27 16:26:49.000000 fastvpinns-1.0.0/LICENSE
--rw-rw-r--   0 thivin    (1001) thivin    (1001)       47 2024-04-22 07:47:55.000000 fastvpinns-1.0.0/MANIFEST.in
--rw-rw-r--   0 thivin    (1001) thivin    (1001)      465 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/PKG-INFO
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     5524 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/README.md
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/FE/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    11557 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/FE2D_Cell.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    11796 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Chebyshev_2.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    11172 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Jacobi.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    10431 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Legendre.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    10075 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Legendre_Special.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     4024 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_function_2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     3372 2024-05-07 05:50:35.000000 fastvpinns-1.0.0/fastvpinns/FE/basis_function_3d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     5134 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/fe2d_setup_main.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     3120 2024-05-11 10:52:47.000000 fastvpinns-1.0.0/fastvpinns/FE/fe_transformation_2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     3314 2024-05-07 05:41:24.000000 fastvpinns-1.0.0/fastvpinns/FE/fe_transformation_3d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     9893 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/fespace.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    26953 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/fespace2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     6207 2024-05-11 10:52:47.000000 fastvpinns-1.0.0/fastvpinns/FE/quad_affine.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     6307 2024-05-11 10:52:47.000000 fastvpinns-1.0.0/fastvpinns/FE/quad_bilinear.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1388 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/quadratureformulas.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     6270 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/FE/quadratureformulas_quad2d.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/Geometry/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.0/fastvpinns/Geometry/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     2074 2024-05-04 08:48:19.000000 fastvpinns-1.0.0/fastvpinns/Geometry/geometry.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    21564 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/Geometry/geometry_2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.0/fastvpinns/__init__.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/data/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-22 09:57:24.000000 fastvpinns-1.0.0/fastvpinns/data/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     4544 2024-05-03 12:24:07.000000 fastvpinns-1.0.0/fastvpinns/data/datahandler.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     9329 2024-05-03 13:54:55.000000 fastvpinns-1.0.0/fastvpinns/data/datahandler2d.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/model/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.0/fastvpinns/model/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    12048 2024-05-07 05:38:52.000000 fastvpinns-1.0.0/fastvpinns/model/model.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    12788 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/model/model_hard.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    13700 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/model/model_inverse.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)    14082 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/model/model_inverse_domain.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/physics/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-22 09:57:37.000000 fastvpinns-1.0.0/fastvpinns/physics/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     2584 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/cd2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     2914 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/cd2d_inverse.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     3047 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/cd2d_inverse_domain.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     2219 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/helmholtz2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1109 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/poisson2d.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     2277 2024-04-27 14:40:21.000000 fastvpinns-1.0.0/fastvpinns/physics/poisson2d_inverse.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/tests/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-27 14:45:42.000000 fastvpinns-1.0.0/fastvpinns/tests/__init__.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns/utils/
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.0/fastvpinns/utils/__init__.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     6705 2024-04-23 20:05:51.000000 fastvpinns-1.0.0/fastvpinns/utils/compute_utils.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     8719 2024-04-27 15:15:48.000000 fastvpinns-1.0.0/fastvpinns/utils/plot_utils.py
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1272 2024-04-23 20:05:51.000000 fastvpinns-1.0.0/fastvpinns/utils/print_utils.py
-drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/fastvpinns.egg-info/
--rw-r--r--   0 thivin    (1001) thivin    (1001)      465 2024-05-11 11:27:02.000000 fastvpinns-1.0.0/fastvpinns.egg-info/PKG-INFO
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1649 2024-05-11 11:27:02.000000 fastvpinns-1.0.0/fastvpinns.egg-info/SOURCES.txt
--rw-rw-r--   0 thivin    (1001) thivin    (1001)        1 2024-05-11 11:27:02.000000 fastvpinns-1.0.0/fastvpinns.egg-info/dependency_links.txt
--rw-rw-r--   0 thivin    (1001) thivin    (1001)      182 2024-05-11 11:27:02.000000 fastvpinns-1.0.0/fastvpinns.egg-info/requires.txt
--rw-rw-r--   0 thivin    (1001) thivin    (1001)       11 2024-05-11 11:27:02.000000 fastvpinns-1.0.0/fastvpinns.egg-info/top_level.txt
--rw-rw-r--   0 thivin    (1001) thivin    (1001)     1831 2024-05-11 11:25:48.000000 fastvpinns-1.0.0/pyproject.toml
--rw-rw-r--   0 thivin    (1001) thivin    (1001)      187 2024-04-29 15:27:33.000000 fastvpinns-1.0.0/requirements.txt
--rw-rw-r--   0 thivin    (1001) thivin    (1001)       79 2024-05-11 11:27:02.418644 fastvpinns-1.0.0/setup.cfg
--rw-rw-r--   0 thivin    (1001) thivin    (1001)      686 2024-05-11 11:23:11.000000 fastvpinns-1.0.0/setup.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.625684 fastvpinns-1.0.1/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)      298 2024-04-22 12:11:53.000000 fastvpinns-1.0.1/CHANGELOG
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     5202 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1081 2024-04-30 11:07:45.000000 fastvpinns-1.0.1/CONTRIBUTING.md
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1107 2024-04-27 16:26:49.000000 fastvpinns-1.0.1/LICENSE
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)       47 2024-04-22 07:47:55.000000 fastvpinns-1.0.1/MANIFEST.in
+-rw-r--r--   0 thivin    (1001) thivin    (1001)     7768 2024-05-14 13:29:38.625684 fastvpinns-1.0.1/PKG-INFO
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     5717 2024-05-14 13:03:55.000000 fastvpinns-1.0.1/README.md
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/FE/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    11557 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/FE2D_Cell.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    11796 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Chebyshev_2.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    11172 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Jacobi.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    10431 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Legendre.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    10075 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Legendre_Special.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     4024 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_function_2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     3372 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/basis_function_3d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     5134 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/fe2d_setup_main.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     3120 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/fe_transformation_2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     3314 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/fe_transformation_3d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     9893 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/fespace.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    26953 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/fespace2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     6207 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/quad_affine.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     6307 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/quad_bilinear.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1388 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/quadratureformulas.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     6270 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/FE/quadratureformulas_quad2d.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/Geometry/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.1/fastvpinns/Geometry/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     2074 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/Geometry/geometry.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    21564 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/Geometry/geometry_2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.1/fastvpinns/__init__.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/data/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-22 09:57:24.000000 fastvpinns-1.0.1/fastvpinns/data/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     4544 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/data/datahandler.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     9329 2024-05-14 12:18:13.000000 fastvpinns-1.0.1/fastvpinns/data/datahandler2d.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/model/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.1/fastvpinns/model/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    12048 2024-05-07 05:38:52.000000 fastvpinns-1.0.1/fastvpinns/model/model.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    12788 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/model/model_hard.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    13700 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/model/model_inverse.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)    14082 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/model/model_inverse_domain.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/physics/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-22 09:57:37.000000 fastvpinns-1.0.1/fastvpinns/physics/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     2584 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/cd2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     2914 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/cd2d_inverse.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     3047 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/cd2d_inverse_domain.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     2219 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/helmholtz2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1109 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/poisson2d.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     2277 2024-04-27 14:40:21.000000 fastvpinns-1.0.1/fastvpinns/physics/poisson2d_inverse.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns/tests/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-27 14:45:42.000000 fastvpinns-1.0.1/fastvpinns/tests/__init__.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.625684 fastvpinns-1.0.1/fastvpinns/utils/
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        0 2024-04-21 18:01:35.000000 fastvpinns-1.0.1/fastvpinns/utils/__init__.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     6705 2024-04-23 20:05:51.000000 fastvpinns-1.0.1/fastvpinns/utils/compute_utils.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     8719 2024-04-27 15:15:48.000000 fastvpinns-1.0.1/fastvpinns/utils/plot_utils.py
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1272 2024-04-23 20:05:51.000000 fastvpinns-1.0.1/fastvpinns/utils/print_utils.py
+drwxrwxr-x   0 thivin    (1001) thivin    (1001)        0 2024-05-14 13:29:38.621684 fastvpinns-1.0.1/fastvpinns.egg-info/
+-rw-r--r--   0 thivin    (1001) thivin    (1001)     7768 2024-05-14 13:29:38.000000 fastvpinns-1.0.1/fastvpinns.egg-info/PKG-INFO
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1649 2024-05-14 13:29:38.000000 fastvpinns-1.0.1/fastvpinns.egg-info/SOURCES.txt
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)        1 2024-05-14 13:29:38.000000 fastvpinns-1.0.1/fastvpinns.egg-info/dependency_links.txt
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)      182 2024-05-14 13:29:38.000000 fastvpinns-1.0.1/fastvpinns.egg-info/requires.txt
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)       11 2024-05-14 13:29:38.000000 fastvpinns-1.0.1/fastvpinns.egg-info/top_level.txt
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)     1981 2024-05-14 13:10:48.000000 fastvpinns-1.0.1/pyproject.toml
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)      187 2024-04-29 15:27:33.000000 fastvpinns-1.0.1/requirements.txt
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)       79 2024-05-14 13:29:38.625684 fastvpinns-1.0.1/setup.cfg
+-rw-rw-r--   0 thivin    (1001) thivin    (1001)      861 2024-05-14 12:52:07.000000 fastvpinns-1.0.1/setup.py
```

### Comparing `fastvpinns-1.0.0/CODE_OF_CONDUCT.md` & `fastvpinns-1.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/CONTRIBUTING.md` & `fastvpinns-1.0.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/LICENSE` & `fastvpinns-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/README.md` & `fastvpinns-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 [![Unit tests](https://github.com/cmgcds/fastvpinns/actions/workflows/unit-tests.yml/badge.svg)](https://github.com/cmgcds/fastvpinns/actions/workflows/unit-tests.yml)
 [![Integration tests](https://github.com/cmgcds/fastvpinns/actions/workflows/integration-tests.yml/badge.svg)](https://github.com/cmgcds/fastvpinns/actions/workflows/integration-tests.yml)
 [![Compatability check](https://github.com/cmgcds/fastvpinns/actions/workflows/compatibility-tests.yml/badge.svg)](https://github.com/cmgcds/fastvpinns/actions/workflows/compatibility-tests.yml)
 [![codecov](https://codecov.io/gh/cmgcds/fastvpinns/graph/badge.svg?token=NI9G37R2Q7)](https://codecov.io/gh/cmgcds/fastvpinns)
+[![PyPI](https://badge.fury.io/py/fastvpinns.svg)](https://badge.fury.io/py/fastvpinns)
 
 [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 ![Python Versions](https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11-blue)
 
 
 
@@ -24,26 +25,14 @@
     <br />
 
   </p>
 </div>
 
 A robust tensor-based deep learning framework for solving PDE's using hp-Variational Physics-Informed Neural Networks (hp-VPINNs). The framework is based on the work by [FastVPINNs Paper](https://arxiv.org/abs/2404.12063).
 
-```bibtex
-@misc{anandh2024fastvpinns,
-      title={FastVPINNs: Tensor-Driven Acceleration
-             of VPINNs for Complex Geometries}, 
-      author={Thivin Anandh, Divij Ghose, Himanshu Jain
-               and Sashikumaar Ganesan},
-      year={2024},
-      eprint={2404.12063},
-      archivePrefix={arXiv},
-      primaryClass={cs.LG}
-}
-```
 
 *This library is an highly optimised version of the the initial implementation of hp-VPINNs by [kharazmi](https://github.com/ehsankharazmi/hp-VPINNs). Ref [hp-VPINNs Paper](https://arxiv.org/abs/2003.05385).*
 
 ## Authors 👨‍💻
 ---
 
 [Thivin Anandh](https://github.com/thivinanandh), [Divij Ghose](https://divijghose.github.io/), [Sashikumaar Ganesan](https://cds.iisc.ac.in/faculty/sashi)
@@ -64,14 +53,32 @@
  On ubuntu systems with libGL issues caused due to matplotlib or gmsh, please run the following command to install the required dependencies:
 ```bash
 sudo apt-get install -y libglu1-mesa 
 ```
 
 For more information on the installation process, please refer to our documentation [here](https://cmgcds.github.io/fastvpinns/).
 
+## Citing 📜
+---
+
+If you use this code in your research, please consider citing the following paper:
+
+```bibtex
+@misc{anandh2024fastvpinns,
+      title={FastVPINNs: Tensor-Driven Acceleration
+             of VPINNs for Complex Geometries}, 
+      author={Thivin Anandh, Divij Ghose, Himanshu Jain
+               and Sashikumaar Ganesan},
+      year={2024},
+      eprint={2404.12063},
+      archivePrefix={arXiv},
+      primaryClass={cs.LG}
+}
+```
+
 ## Usage 🚀
 ---
 
 For detailed usage, please refer to our documentation [here](https://cmgcds.github.io/fastvpinns/).
 
 The package provides a simple API to train and solve PDE using VPINNs. The following code snippet demonstrates how to train a hp-VPINN model for the 2D Poisson equation for a structured grid. We could observe that we can solve a PDE using fastvpinns using 15 lines of code.
```

#### html2text {}

```diff
@@ -3,47 +3,49 @@
 unit-tests.yml) [![Integration tests](https://github.com/cmgcds/fastvpinns/
 actions/workflows/integration-tests.yml/badge.svg)](https://github.com/cmgcds/
 fastvpinns/actions/workflows/integration-tests.yml) [![Compatability check]
 (https://github.com/cmgcds/fastvpinns/actions/workflows/compatibility-
 tests.yml/badge.svg)](https://github.com/cmgcds/fastvpinns/actions/workflows/
 compatibility-tests.yml) [![codecov](https://codecov.io/gh/cmgcds/fastvpinns/
 graph/badge.svg?token=NI9G37R2Q7)](https://codecov.io/gh/cmgcds/fastvpinns) [!
-[MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://
-opensource.org/licenses/MIT) [![Code style: black](https://img.shields.io/
-badge/code%20style-black-000000.svg)](https://github.com/psf/black) ![Python
-Versions](https://img.shields.io/badge/python-
+[PyPI](https://badge.fury.io/py/fastvpinns.svg)](https://badge.fury.io/py/
+fastvpinns) [![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)]
+(https://opensource.org/licenses/MIT) [![Code style: black](https://
+img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
+black) ![Python Versions](https://img.shields.io/badge/python-
 3.8%20|%203.9%20|%203.10%20|%203.11-blue)
                                _[_F_a_s_t_V_P_I_N_N_s_ _l_o_g_o_]
     ******** TTeennssoorr--ddrriivveenn aacccceelleerraatteedd ffrraammeewwoorrkk ffoorr hhpp--vvaarriiaattiioonnaall ppiinnnnss ********
 
                           _LL_ii_nn_kk_ _tt_oo_ _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn_ _?ð_?_?_?
 A robust tensor-based deep learning framework for solving PDE's using hp-
 Variational Physics-Informed Neural Networks (hp-VPINNs). The framework is
 based on the work by [FastVPINNs Paper](https://arxiv.org/abs/2404.12063).
-```bibtex @misc{anandh2024fastvpinns, title={FastVPINNs: Tensor-Driven
-Acceleration of VPINNs for Complex Geometries}, author={Thivin Anandh, Divij
-Ghose, Himanshu Jain and Sashikumaar Ganesan}, year={2024}, eprint=
-{2404.12063}, archivePrefix={arXiv}, primaryClass={cs.LG} } ``` *This library
-is an highly optimised version of the the initial implementation of hp-VPINNs
-by [kharazmi](https://github.com/ehsankharazmi/hp-VPINNs). Ref [hp-VPINNs
-Paper](https://arxiv.org/abs/2003.05385).* ## Authors ð¨âð» --- [Thivin
-Anandh](https://github.com/thivinanandh), [Divij Ghose](https://
+*This library is an highly optimised version of the the initial implementation
+of hp-VPINNs by [kharazmi](https://github.com/ehsankharazmi/hp-VPINNs). Ref
+[hp-VPINNs Paper](https://arxiv.org/abs/2003.05385).* ## Authors ð¨âð» --
+- [Thivin Anandh](https://github.com/thivinanandh), [Divij Ghose](https://
 divijghose.github.io/), [Sashikumaar Ganesan](https://cds.iisc.ac.in/faculty/
 sashi) STARS Lab, Department of Computational and Data Sciences, Indian
 Institute of Science, Bangalore, India ## Installation ð ï¸ --- The build of
 the code is currently tested on Python versions (3.8, 3.9, 3.10, 3.11), on OS
 Ubuntu 20.04 and Ubuntu 22.04, Macos-latest and Windows-latest (refer
 compatibility build [Compatability check](https://github.com/cmgcds/fastvpinns/
 actions/workflows/compatibility-tests.yml)). You can install the package using
 pip as follows: ```bash pip install fastvpinns ``` On ubuntu systems with libGL
 issues caused due to matplotlib or gmsh, please run the following command to
 install the required dependencies: ```bash sudo apt-get install -y libglu1-mesa
 ``` For more information on the installation process, please refer to our
-documentation [here](https://cmgcds.github.io/fastvpinns/). ## Usage ð --
-- For detailed usage, please refer to our documentation [here](https://
+documentation [here](https://cmgcds.github.io/fastvpinns/). ## Citing ð --
+- If you use this code in your research, please consider citing the following
+paper: ```bibtex @misc{anandh2024fastvpinns, title={FastVPINNs: Tensor-Driven
+Acceleration of VPINNs for Complex Geometries}, author={Thivin Anandh, Divij
+Ghose, Himanshu Jain and Sashikumaar Ganesan}, year={2024}, eprint=
+{2404.12063}, archivePrefix={arXiv}, primaryClass={cs.LG} } ``` ## Usage ð -
+-- For detailed usage, please refer to our documentation [here](https://
 cmgcds.github.io/fastvpinns/). The package provides a simple API to train and
 solve PDE using VPINNs. The following code snippet demonstrates how to train a
 hp-VPINN model for the 2D Poisson equation for a structured grid. We could
 observe that we can solve a PDE using fastvpinns using 15 lines of code.
 ```python #load the geometry domain = Geometry_2D("quadrilateral", "internal",
 100, 100, "./") cells, boundary_points = domain.generate_quad_mesh_internal
 (x_limits=[0, 1],y_limits=[0, 1],n_cells_x=4, n_cells_y=4,
```

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/FE2D_Cell.py` & `fastvpinns-1.0.1/fastvpinns/FE/FE2D_Cell.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Chebyshev_2.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Chebyshev_2.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Jacobi.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Jacobi.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Legendre.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Legendre.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_2d_QN_Legendre_Special.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_2d_QN_Legendre_Special.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_function_2d.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_function_2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/basis_function_3d.py` & `fastvpinns-1.0.1/fastvpinns/FE/basis_function_3d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/fe2d_setup_main.py` & `fastvpinns-1.0.1/fastvpinns/FE/fe2d_setup_main.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/fe_transformation_2d.py` & `fastvpinns-1.0.1/fastvpinns/FE/fe_transformation_2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/fe_transformation_3d.py` & `fastvpinns-1.0.1/fastvpinns/FE/fe_transformation_3d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/fespace.py` & `fastvpinns-1.0.1/fastvpinns/FE/fespace.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/fespace2d.py` & `fastvpinns-1.0.1/fastvpinns/FE/fespace2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/quad_affine.py` & `fastvpinns-1.0.1/fastvpinns/FE/quad_affine.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/quad_bilinear.py` & `fastvpinns-1.0.1/fastvpinns/FE/quad_bilinear.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/quadratureformulas.py` & `fastvpinns-1.0.1/fastvpinns/FE/quadratureformulas.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/FE/quadratureformulas_quad2d.py` & `fastvpinns-1.0.1/fastvpinns/FE/quadratureformulas_quad2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/Geometry/geometry.py` & `fastvpinns-1.0.1/fastvpinns/Geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/Geometry/geometry_2d.py` & `fastvpinns-1.0.1/fastvpinns/Geometry/geometry_2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/data/datahandler.py` & `fastvpinns-1.0.1/fastvpinns/data/datahandler.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/data/datahandler2d.py` & `fastvpinns-1.0.1/fastvpinns/data/datahandler2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/model/model.py` & `fastvpinns-1.0.1/fastvpinns/model/model.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/model/model_hard.py` & `fastvpinns-1.0.1/fastvpinns/model/model_hard.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/model/model_inverse.py` & `fastvpinns-1.0.1/fastvpinns/model/model_inverse.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/model/model_inverse_domain.py` & `fastvpinns-1.0.1/fastvpinns/model/model_inverse_domain.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/cd2d.py` & `fastvpinns-1.0.1/fastvpinns/physics/cd2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/cd2d_inverse.py` & `fastvpinns-1.0.1/fastvpinns/physics/cd2d_inverse.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/cd2d_inverse_domain.py` & `fastvpinns-1.0.1/fastvpinns/physics/cd2d_inverse_domain.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/helmholtz2d.py` & `fastvpinns-1.0.1/fastvpinns/physics/helmholtz2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/poisson2d.py` & `fastvpinns-1.0.1/fastvpinns/physics/poisson2d.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/physics/poisson2d_inverse.py` & `fastvpinns-1.0.1/fastvpinns/physics/poisson2d_inverse.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/utils/compute_utils.py` & `fastvpinns-1.0.1/fastvpinns/utils/compute_utils.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/utils/plot_utils.py` & `fastvpinns-1.0.1/fastvpinns/utils/plot_utils.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns/utils/print_utils.py` & `fastvpinns-1.0.1/fastvpinns/utils/print_utils.py`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/fastvpinns.egg-info/SOURCES.txt` & `fastvpinns-1.0.1/fastvpinns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastvpinns-1.0.0/pyproject.toml` & `fastvpinns-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools==68.2.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastvpinns"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Thivin Anandh", email="thivinanandh@gmail.com" },
   { name="Divij Ghose", email="divijghose@gmail.com" },
   { name="Sashikumaar Ganesan", email="sashi@iisc.ac.in" }
 ]
 description = "A fast tensor-driven variational physics-informed neural network library for solving PDEs."
 readme = "README.md"
 requires-python = ">=3.8"
+keywords = ["PDE", "Neural Networks", "Physics", "AI", "Machine Learning","variational PINNs", "VPINNs", "PINNs", "Physics-informed neural networks"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `fastvpinns-1.0.0/setup.py` & `fastvpinns-1.0.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup, find_packages
+import os
 
 # Read the requirements from the requirements.txt file
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
+
+# Moved all the metadata to the pyproject.toml file
 setup(
     name="fastvpinns",
-    version="1.0.0",
-    author="Thivin Anandh, Divij Ghose, Sashikumaar Ganesan",
-    author_email="thivinanandh@gmail.com",
-    description="An Efficient tensor-based implementation of hp-Variational Physics-informed Neural Networks (VPINNs) for solving PDEs",
+    # version="1.0.5",
+    # author="Thivin Anandh, Divij Ghose, Sashikumaar Ganesan",
+    # author_email="thivinanandh@gmail.com",
+    # description="An Efficient tensor-based implementation of hp-Variational Physics-informed Neural Networks (VPINNs) for solving PDEs",
     packages=find_packages(),
+    # long_description=read_file('README.md'),
+    # home_page="https://cmgcds.github.io/fastvpinns",
     # license="MIT",
     install_requires=requirements,
-    keywords=['variational PINNs', 'VPINNs', 'PINNs', 'Physics-informed neural networks', 'Deep learning', 'Machine learning']
+    # keywords=['variational PINNs', 'VPINNs', 'PINNs', 'Physics-informed neural networks', 'Deep learning', 'Machine learning']
 )
```

