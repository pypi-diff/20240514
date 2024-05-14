# Comparing `tmp/earthkit-regrid-0.3.0.tar.gz` & `tmp/earthkit_regrid-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "earthkit-regrid-0.3.0.tar", last modified: Wed Mar 27 16:14:43 2024, max compression
+gzip compressed data, was "earthkit_regrid-0.3.1.tar", last modified: Tue May 14 17:08:04 2024, max compression
```

## Comparing `earthkit-regrid-0.3.0.tar` & `earthkit_regrid-0.3.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.499580 earthkit-regrid-0.3.0/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.289635 earthkit-regrid-0.3.0/.github/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.324976 earthkit-regrid-0.3.0/.github/workflows/
--rw-r--r--   0 cgr        (501) staff       (20)     5807 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 cgr        (501) staff       (20)      235 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.github/workflows/label-public-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)      275 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.github/workflows/notify-new-issue.yml
--rw-r--r--   0 cgr        (501) staff       (20)      279 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.github/workflows/notify-new-pr.yml
--rw-r--r--   0 cgr        (501) staff       (20)     7258 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/.gitignore
--rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 cgr        (501) staff       (20)      137 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/.readthedocs.yml
--rw-r--r--   0 cgr        (501) staff       (20)      756 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/Makefile
--rw-r--r--   0 cgr        (501) staff       (20)     1589 2024-03-27 16:14:43.499323 earthkit-regrid-0.3.0/PKG-INFO
--rw-------   0 cgr        (501) staff       (20)     1207 2024-03-27 15:31:57.000000 earthkit-regrid-0.3.0/README.md
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.342829 earthkit-regrid-0.3.0/docs/
--rw-r--r--   0 cgr        (501) staff       (20)      634 2024-02-08 18:57:31.000000 earthkit-regrid-0.3.0/docs/Makefile
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.344973 earthkit-regrid-0.3.0/docs/_static/
--rw-r--r--   0 cgr        (501) staff       (20)        0 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/_static/.gitkeep
--rw-r--r--   0 cgr        (501) staff       (20)      832 2024-03-25 09:47:44.000000 earthkit-regrid-0.3.0/docs/_static/style.css
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.345357 earthkit-regrid-0.3.0/docs/_templates/
--rw-r--r--   0 cgr        (501) staff       (20)        0 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/_templates/.gitkeep
--rw-r--r--   0 cgr        (501) staff       (20)     2638 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/conf.py
--rw-r--r--   0 cgr        (501) staff       (20)     1526 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/development.rst
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.360011 earthkit-regrid-0.3.0/docs/examples/
--rw-r--r--   0 cgr        (501) staff       (20)   246207 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/examples/healpix_fieldlist.ipynb
--rw-r--r--   0 cgr        (501) staff       (20)      230 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/examples/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)     5277 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/examples/interpolation-2.ipynb
--rw-r--r--   0 cgr        (501) staff       (20)    66836 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/examples/numpy_arrays.ipynb
--rw-r--r--   0 cgr        (501) staff       (20)   255769 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/examples/octahedral_fieldlist.ipynb
--rw-r--r--   0 cgr        (501) staff       (20)     1528 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/gridspec.rst
--rw-r--r--   0 cgr        (501) staff       (20)     1258 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)      224 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/install.rst
--rw-r--r--   0 cgr        (501) staff       (20)     2396 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/interpolate.rst
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.370708 earthkit-regrid-0.3.0/docs/inventory/
--rw-r--r--   0 cgr        (501) staff       (20)      118 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/inventory/healpix_nested.rst
--rw-r--r--   0 cgr        (501) staff       (20)      112 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/inventory/healpix_ring.rst
--rw-r--r--   0 cgr        (501) staff       (20)      374 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/inventory/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)      460 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/inventory/pre_gen_warn.rst
--rw-r--r--   0 cgr        (501) staff       (20)       99 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/docs/inventory/reduced_gg.rst
--rw-r--r--   0 cgr        (501) staff       (20)      136 2024-03-22 15:06:09.000000 earthkit-regrid-0.3.0/docs/inventory/reduced_gg_o.rst
--rw-r--r--   0 cgr        (501) staff       (20)      116 2024-03-27 13:42:49.000000 earthkit-regrid-0.3.0/docs/inventory/regular_ll.rst
--rw-r--r--   0 cgr        (501) staff       (20)      813 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/licence.rst
--rw-r--r--   0 cgr        (501) staff       (20)      765 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/docs/make.bat
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.371885 earthkit-regrid-0.3.0/docs/release_notes/
--rw-r--r--   0 cgr        (501) staff       (20)       85 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/release_notes/index.rst
--rw-r--r--   0 cgr        (501) staff       (20)      595 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/docs/release_notes/version_0.3_updates.rst
--rw-r--r--   0 cgr        (501) staff       (20)      147 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.290890 earthkit-regrid-0.3.0/earthkit/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.378535 earthkit-regrid-0.3.0/earthkit/regrid/
--rw-r--r--   0 cgr        (501) staff       (20)      776 2024-03-24 14:14:23.000000 earthkit-regrid-0.3.0/earthkit/regrid/__init__.py
--rw-r--r--   0 cgr        (501) staff       (20)    13204 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/db.py
--rw-r--r--   0 cgr        (501) staff       (20)    11376 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/gridspec.py
--rw-r--r--   0 cgr        (501) staff       (20)     2709 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/interpolate.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.386114 earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/
--rw-r--r--   0 cgr        (501) staff       (20)     3709 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/generate_inventory_rst.py
--rw-r--r--   0 cgr        (501) staff       (20)     2012 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/module_output.py
--rw-r--r--   0 cgr        (501) staff       (20)     1403 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/xref.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.406618 earthkit-regrid-0.3.0/earthkit/regrid/utils/
--rw-r--r--   0 cgr        (501) staff       (20)     1509 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/__init__.py
--rw-r--r--   0 cgr        (501) staff       (20)    34059 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/caching.py
--rw-r--r--   0 cgr        (501) staff       (20)     2850 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/download.py
--rw-r--r--   0 cgr        (501) staff       (20)      588 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/humanize.py
--rw-r--r--   0 cgr        (501) staff       (20)     3480 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/matrix.py
--rw-r--r--   0 cgr        (501) staff       (20)     2038 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/mir.py
--rw-r--r--   0 cgr        (501) staff       (20)     5934 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/stream.py
--rw-r--r--   0 cgr        (501) staff       (20)     1818 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/earthkit/regrid/utils/temporary.py
--rwxrwxrwx   0 cgr        (501) staff       (20)       72 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit/regrid/version.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.498466 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/
--rw-r--r--   0 cgr        (501) staff       (20)     1589 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/PKG-INFO
--rwxrwxrwx   0 cgr        (501) staff       (20)     3915 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/SOURCES.txt
--rwxrwxrwx   0 cgr        (501) staff       (20)        1 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/dependency_links.txt
--rwxrwxrwx   0 cgr        (501) staff       (20)       59 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/requires.txt
--rwxrwxrwx   0 cgr        (501) staff       (20)        9 2024-03-27 16:14:43.000000 earthkit-regrid-0.3.0/earthkit_regrid.egg-info/top_level.txt
--rw-r--r--   0 cgr        (501) staff       (20)      308 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/environment.yml
--rw-r--r--   0 cgr        (501) staff       (20)      400 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/pyproject.toml
--rw-r--r--   0 cgr        (501) staff       (20)      210 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/pytest.ini
--rw-r--r--   0 cgr        (501) staff       (20)      979 2024-03-27 16:14:43.500406 earthkit-regrid-0.3.0/setup.cfg
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.419033 earthkit-regrid-0.3.0/tests/
--rw-r--r--   0 cgr        (501) staff       (20)      910 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/conftest.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.291844 earthkit-regrid-0.3.0/tests/data/
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.434963 earthkit-regrid-0.3.0/tests/data/local/
--rw-r--r--   0 cgr        (501) staff       (20)       15 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/tests/data/local/.gitignore
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.436233 earthkit-regrid-0.3.0/tests/data/local/db/
--rw-r--r--   0 cgr        (501) staff       (20)     9502 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/index.json
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.438303 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/
--rw-r--r--   0 cgr        (501) staff       (20)     8106 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/0efb7cc6060e3365bd2a0c0037e6a339fd2fd71fdba607cd9b6aa13683d01523.npz
--rw-r--r--   0 cgr        (501) staff       (20)     9735 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/2800f6a28606667ff1e20b82b067e6cf94670b854651601f6ee15683e80e4933.npz
--rw-r--r--   0 cgr        (501) staff       (20)     8023 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/4b7e0a8bb9dee07acc5822ad0caa72f0e5fae26e956b981aa707f2dba9bab915.npz
--rw-r--r--   0 cgr        (501) staff       (20)    10122 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/82ef0fa6d7c834016fe52e93f6cd4185a044e0a900c02906f146998c09c2e22e.npz
--rw-r--r--   0 cgr        (501) staff       (20)     3064 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/8d0fbe91fd547ad49d86acd6f31b339163f35cdfd183689367f6864d98d3328d.npz
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.440316 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/
--rw-r--r--   0 cgr        (501) staff       (20)     2655 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/96b820068578d6b778b0e1359d34e0dfa8c65417b6fbe3e3725fb1bc7a90b3c6.npz
--rw-r--r--   0 cgr        (501) staff       (20)     3147 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/bed78a06d90a74c03bd9b7d9dff94ea3c6436ab99bf182f92ac1e5c9b0977708.npz
--rw-r--r--   0 cgr        (501) staff       (20)     3130 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/c0de1f0a5e662a9392c06416df2e0124a75d8a97c497b19360f7bea1e3ab694b.npz
--rw-r--r--   0 cgr        (501) staff       (20)     2655 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/e0a86032fae661b1de48828084ab32c3aee40b50871f0f8cd4b9c1b919991525.npz
--rw-r--r--   0 cgr        (501) staff       (20)     3067 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/f330f076443c96111fab1e6df633ac3c9e605ffec35b4a1a78bc952e6a5925b6.npz
--rw-r--r--   0 cgr        (501) staff       (20)     7085 2024-03-22 11:18:10.000000 earthkit-regrid-0.3.0/tests/data/local/in_5x5.npz
--rw-r--r--   0 cgr        (501) staff       (20)      842 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/in_H4_nested.npz
--rw-r--r--   0 cgr        (501) staff       (20)      829 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/in_H4_ring.npz
--rw-r--r--   0 cgr        (501) staff       (20)    16083 2024-03-22 11:18:10.000000 earthkit-regrid-0.3.0/tests/data/local/in_N32.npz
--rw-r--r--   0 cgr        (501) staff       (20)    13894 2024-03-22 11:18:10.000000 earthkit-regrid-0.3.0/tests/data/local/in_O32.npz
--rw-r--r--   0 cgr        (501) staff       (20)     2011 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_5x5_10x10_linear.npz
--rw-r--r--   0 cgr        (501) staff       (20)     2011 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_5x5_10x10_nearest-neighbour.npz
--rw-r--r--   0 cgr        (501) staff       (20)     4715 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_H4_nested_10x10_linear.npz
--rw-r--r--   0 cgr        (501) staff       (20)     1070 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_H4_nested_10x10_nearest-neighbour.npz
--rw-r--r--   0 cgr        (501) staff       (20)     4711 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_H4_ring_10x10_linear.npz
--rw-r--r--   0 cgr        (501) staff       (20)     1070 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_H4_ring_10x10_nearest-neighbour.npz
--rw-r--r--   0 cgr        (501) staff       (20)     4732 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_N32_10x10_linear.npz
--rw-r--r--   0 cgr        (501) staff       (20)     1984 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_N32_10x10_nearest-neighbour.npz
--rw-r--r--   0 cgr        (501) staff       (20)     4641 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_O32_10x10_linear.npz
--rw-r--r--   0 cgr        (501) staff       (20)     1976 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/data/local/out_O32_10x10_nearest-neighbour.npz
--rw-r--r--   0 cgr        (501) staff       (20)      319 2024-02-05 17:26:14.000000 earthkit-regrid-0.3.0/tests/environment-unit-tests.yml
--rw-r--r--   0 cgr        (501) staff       (20)     5523 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/test_gridspec.py
--rw-r--r--   0 cgr        (501) staff       (20)     6275 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/test_interpolate.py
--rw-r--r--   0 cgr        (501) staff       (20)     7990 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tests/test_local.py
--rw-r--r--   0 cgr        (501) staff       (20)      532 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/tests/test_version.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.490875 earthkit-regrid-0.3.0/tools/
--rw-r--r--   0 cgr        (501) staff       (20)      186 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/.gitignore
--rw-r--r--   0 cgr        (501) staff       (20)     2508 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/tools/make-matrix.sh
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.492363 earthkit-regrid-0.3.0/tools/manage/
--rw-r--r--   0 cgr        (501) staff       (20)     3355 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/manage/build_db.py
--rw-r--r--   0 cgr        (501) staff       (20)     1125 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/manage/build_local_test_db.py
--rw-r--r--   0 cgr        (501) staff       (20)     3796 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/manage/merge_index.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.494953 earthkit-regrid-0.3.0/tools/subset/
--rw-r--r--   0 cgr        (501) staff       (20)      648 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/subset/eccharts_subset_db_conf.yaml
--rw-r--r--   0 cgr        (501) staff       (20)      648 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/subset/subset_db_conf.yaml
--rw-r--r--   0 cgr        (501) staff       (20)     3674 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/subset/subset_remote_db.py
-drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-03-27 16:14:43.498028 earthkit-regrid-0.3.0/tools/utils/
--rw-r--r--   0 cgr        (501) staff       (20)        0 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/tools/utils/__init__.py
--rw-r--r--   0 cgr        (501) staff       (20)      847 2024-03-01 12:33:57.000000 earthkit-regrid-0.3.0/tools/utils/grid.py
--rw-r--r--   0 cgr        (501) staff       (20)     4861 2024-03-27 16:12:10.000000 earthkit-regrid-0.3.0/tools/utils/matrix.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.131457 earthkit_regrid-0.3.1/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.639008 earthkit_regrid-0.3.1/.github/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.674490 earthkit_regrid-0.3.1/.github/workflows/
+-rw-r--r--   0 cgr        (501) staff       (20)     5832 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      235 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/.github/workflows/label-public-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      275 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/.github/workflows/notify-new-issue.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      279 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/.github/workflows/notify-new-pr.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     7258 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/.gitignore
+-rw-r--r--   0 cgr        (501) staff       (20)     1132 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 cgr        (501) staff       (20)      137 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/.readthedocs.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      756 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/Makefile
+-rw-r--r--   0 cgr        (501) staff       (20)     1589 2024-05-14 17:08:04.131255 earthkit_regrid-0.3.1/PKG-INFO
+-rw-r--r--   0 cgr        (501) staff       (20)     1207 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/README.md
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.770403 earthkit_regrid-0.3.1/docs/
+-rw-r--r--   0 cgr        (501) staff       (20)      634 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/Makefile
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.773063 earthkit_regrid-0.3.1/docs/_static/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/_static/.gitkeep
+-rw-r--r--   0 cgr        (501) staff       (20)      832 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/_static/style.css
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.774006 earthkit_regrid-0.3.1/docs/_templates/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/_templates/.gitkeep
+-rw-r--r--   0 cgr        (501) staff       (20)     2638 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/conf.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1526 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/development.rst
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.789719 earthkit_regrid-0.3.1/docs/examples/
+-rw-r--r--   0 cgr        (501) staff       (20)   246207 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/examples/healpix_fieldlist.ipynb
+-rw-r--r--   0 cgr        (501) staff       (20)      230 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/examples/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)     5277 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/examples/interpolation-2.ipynb
+-rw-r--r--   0 cgr        (501) staff       (20)    66836 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/examples/numpy_arrays.ipynb
+-rw-r--r--   0 cgr        (501) staff       (20)   255769 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/examples/octahedral_fieldlist.ipynb
+-rw-r--r--   0 cgr        (501) staff       (20)     1528 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/gridspec.rst
+-rw-r--r--   0 cgr        (501) staff       (20)     1258 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      224 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/install.rst
+-rw-r--r--   0 cgr        (501) staff       (20)     2396 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/interpolate.rst
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.805511 earthkit_regrid-0.3.1/docs/inventory/
+-rw-r--r--   0 cgr        (501) staff       (20)      118 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/healpix_nested.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      112 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/healpix_ring.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      374 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      460 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/pre_gen_warn.rst
+-rw-r--r--   0 cgr        (501) staff       (20)       99 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/reduced_gg.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      136 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/reduced_gg_o.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      116 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/inventory/regular_ll.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      813 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/licence.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      765 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/make.bat
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.820610 earthkit_regrid-0.3.1/docs/release_notes/
+-rw-r--r--   0 cgr        (501) staff       (20)       85 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/release_notes/index.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      842 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/docs/release_notes/version_0.3_updates.rst
+-rw-r--r--   0 cgr        (501) staff       (20)      154 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.640812 earthkit_regrid-0.3.1/earthkit/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.834697 earthkit_regrid-0.3.1/earthkit/regrid/
+-rw-r--r--   0 cgr        (501) staff       (20)      776 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/__init__.py
+-rw-r--r--   0 cgr        (501) staff       (20)    13204 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/db.py
+-rw-r--r--   0 cgr        (501) staff       (20)    11465 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/gridspec.py
+-rw-r--r--   0 cgr        (501) staff       (20)     2709 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/interpolate.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.897216 earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/
+-rw-r--r--   0 cgr        (501) staff       (20)     3812 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/generate_inventory_rst.py
+-rw-r--r--   0 cgr        (501) staff       (20)     2012 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/module_output.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1403 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/xref.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.915798 earthkit_regrid-0.3.1/earthkit/regrid/utils/
+-rw-r--r--   0 cgr        (501) staff       (20)     1509 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/__init__.py
+-rw-r--r--   0 cgr        (501) staff       (20)    34059 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/caching.py
+-rw-r--r--   0 cgr        (501) staff       (20)     2850 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/download.py
+-rw-r--r--   0 cgr        (501) staff       (20)      588 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/humanize.py
+-rw-r--r--   0 cgr        (501) staff       (20)     3480 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/matrix.py
+-rw-r--r--   0 cgr        (501) staff       (20)     2038 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/mir.py
+-rw-r--r--   0 cgr        (501) staff       (20)     5934 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/stream.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1818 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/earthkit/regrid/utils/temporary.py
+-rw-r--r--   0 cgr        (501) staff       (20)       72 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit/regrid/version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.130241 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/
+-rw-r--r--   0 cgr        (501) staff       (20)     1589 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/PKG-INFO
+-rw-r--r--   0 cgr        (501) staff       (20)     3915 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/SOURCES.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        1 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/dependency_links.txt
+-rw-r--r--   0 cgr        (501) staff       (20)       59 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/requires.txt
+-rw-r--r--   0 cgr        (501) staff       (20)        9 2024-05-14 17:08:03.000000 earthkit_regrid-0.3.1/earthkit_regrid.egg-info/top_level.txt
+-rw-r--r--   0 cgr        (501) staff       (20)      315 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/environment.yml
+-rw-r--r--   0 cgr        (501) staff       (20)      400 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/pyproject.toml
+-rw-r--r--   0 cgr        (501) staff       (20)      210 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/pytest.ini
+-rw-r--r--   0 cgr        (501) staff       (20)      979 2024-05-14 17:08:04.132203 earthkit_regrid-0.3.1/setup.cfg
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.005170 earthkit_regrid-0.3.1/tests/
+-rw-r--r--   0 cgr        (501) staff       (20)      910 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/conftest.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:03.641922 earthkit_regrid-0.3.1/tests/data/
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.036966 earthkit_regrid-0.3.1/tests/data/local/
+-rw-r--r--   0 cgr        (501) staff       (20)       15 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/.gitignore
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.039312 earthkit_regrid-0.3.1/tests/data/local/db/
+-rw-r--r--   0 cgr        (501) staff       (20)     9502 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/index.json
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.049294 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/
+-rw-r--r--   0 cgr        (501) staff       (20)     8106 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/0efb7cc6060e3365bd2a0c0037e6a339fd2fd71fdba607cd9b6aa13683d01523.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     9735 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/2800f6a28606667ff1e20b82b067e6cf94670b854651601f6ee15683e80e4933.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     8023 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/4b7e0a8bb9dee07acc5822ad0caa72f0e5fae26e956b981aa707f2dba9bab915.npz
+-rw-r--r--   0 cgr        (501) staff       (20)    10122 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/82ef0fa6d7c834016fe52e93f6cd4185a044e0a900c02906f146998c09c2e22e.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     3064 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/8d0fbe91fd547ad49d86acd6f31b339163f35cdfd183689367f6864d98d3328d.npz
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.055750 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/
+-rw-r--r--   0 cgr        (501) staff       (20)     2655 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/96b820068578d6b778b0e1359d34e0dfa8c65417b6fbe3e3725fb1bc7a90b3c6.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     3147 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/bed78a06d90a74c03bd9b7d9dff94ea3c6436ab99bf182f92ac1e5c9b0977708.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     3130 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/c0de1f0a5e662a9392c06416df2e0124a75d8a97c497b19360f7bea1e3ab694b.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     2655 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/e0a86032fae661b1de48828084ab32c3aee40b50871f0f8cd4b9c1b919991525.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     3067 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/f330f076443c96111fab1e6df633ac3c9e605ffec35b4a1a78bc952e6a5925b6.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     7085 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/in_5x5.npz
+-rw-r--r--   0 cgr        (501) staff       (20)      842 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/in_H4_nested.npz
+-rw-r--r--   0 cgr        (501) staff       (20)      829 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/in_H4_ring.npz
+-rw-r--r--   0 cgr        (501) staff       (20)    16083 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/in_N32.npz
+-rw-r--r--   0 cgr        (501) staff       (20)    13894 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/in_O32.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     2011 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_5x5_10x10_linear.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     2011 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_5x5_10x10_nearest-neighbour.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     4715 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_H4_nested_10x10_linear.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     1070 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_H4_nested_10x10_nearest-neighbour.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     4711 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_H4_ring_10x10_linear.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     1070 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_H4_ring_10x10_nearest-neighbour.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     4732 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_N32_10x10_linear.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     1984 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_N32_10x10_nearest-neighbour.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     4641 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_O32_10x10_linear.npz
+-rw-r--r--   0 cgr        (501) staff       (20)     1976 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/data/local/out_O32_10x10_nearest-neighbour.npz
+-rw-r--r--   0 cgr        (501) staff       (20)      326 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/environment-unit-tests.yml
+-rw-r--r--   0 cgr        (501) staff       (20)     5696 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/tests/test_gridspec.py
+-rw-r--r--   0 cgr        (501) staff       (20)     6275 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/test_interpolate.py
+-rw-r--r--   0 cgr        (501) staff       (20)     8128 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/tests/test_local.py
+-rw-r--r--   0 cgr        (501) staff       (20)      532 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tests/test_version.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.059120 earthkit_regrid-0.3.1/tools/
+-rw-r--r--   0 cgr        (501) staff       (20)      186 2024-05-14 17:04:25.000000 earthkit_regrid-0.3.1/tools/.gitignore
+-rw-r--r--   0 cgr        (501) staff       (20)     2508 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/make-matrix.sh
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.120041 earthkit_regrid-0.3.1/tools/manage/
+-rw-r--r--   0 cgr        (501) staff       (20)     3355 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/manage/build_db.py
+-rw-r--r--   0 cgr        (501) staff       (20)     1125 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/manage/build_local_test_db.py
+-rw-r--r--   0 cgr        (501) staff       (20)     3796 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/manage/merge_index.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.124494 earthkit_regrid-0.3.1/tools/subset/
+-rw-r--r--   0 cgr        (501) staff       (20)      648 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/subset/eccharts_subset_db_conf.yaml
+-rw-r--r--   0 cgr        (501) staff       (20)      648 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/subset/subset_db_conf.yaml
+-rw-r--r--   0 cgr        (501) staff       (20)     3674 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/subset/subset_remote_db.py
+drwxr-xr-x   0 cgr        (501) staff       (20)        0 2024-05-14 17:08:04.129663 earthkit_regrid-0.3.1/tools/utils/
+-rw-r--r--   0 cgr        (501) staff       (20)        0 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/utils/__init__.py
+-rw-r--r--   0 cgr        (501) staff       (20)      847 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/utils/grid.py
+-rw-r--r--   0 cgr        (501) staff       (20)     4861 2024-05-14 17:04:07.000000 earthkit_regrid-0.3.1/tools/utils/matrix.py
```

### Comparing `earthkit-regrid-0.3.0/.github/workflows/ci.yml` & `earthkit_regrid-0.3.1/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -57,42 +57,42 @@
     - name: Install package
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
         make unit-tests
 
-  type-check:
-    needs: [unit-tests]
-    if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
-    runs-on: ubuntu-latest
-    defaults:
-      run:
-        shell: bash -l {0}
-
-    steps:
-    - uses: actions/checkout@v3
-      with:
-        ref: ${{ github.event.pull_request.head.sha || github.ref }}
-    - name: Install Conda environment with Micromamba
-      uses: mamba-org/provision-with-micromamba@v12
-      with:
-        environment-file: environment.yml
-        environment-name: DEVELOP
-        channels: conda-forge
-        cache-env: true
-        cache-env-key: ubuntu-latest-3.10
-        extra-specs: |
-          python=3.10
-    - name: Install package
-      run: |
-        python -m pip install --no-deps -e .
-    - name: Run code quality checks
-      run: |
-        echo type-check not used
+  # type-check:
+  #   needs: [unit-tests]
+  #   if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
+  #   runs-on: ubuntu-latest
+  #   defaults:
+  #     run:
+  #       shell: bash -l {0}
+
+  #   steps:
+  #   - uses: actions/checkout@v3
+  #     with:
+  #       ref: ${{ github.event.pull_request.head.sha || github.ref }}
+  #   - name: Install Conda environment with Micromamba
+  #     uses: mamba-org/provision-with-micromamba@v12
+  #     with:
+  #       environment-file: environment.yml
+  #       environment-name: DEVELOP
+  #       channels: conda-forge
+  #       cache-env: true
+  #       cache-env-key: ubuntu-latest-3.10
+  #       extra-specs: |
+  #         python=3.10
+  #   - name: Install package
+  #     run: |
+  #       python -m pip install --no-deps -e .
+  #   - name: Run code quality checks
+  #     run: |
+  #       echo type-check not used
 
   documentation:
     needs: [unit-tests]
     if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
     runs-on: ubuntu-latest
     defaults:
       run:
@@ -151,15 +151,15 @@
       run: |
         python -m pip install --no-deps -e .
     - name: Run tests
       run: |
         make unit-tests
 
   distribution:
-    needs: [integration-tests, type-check, documentation]
+    needs: [integration-tests, documentation]
     if: ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
       with:
         ref: ${{ github.event.pull_request.head.sha || github.ref }}
@@ -175,15 +175,14 @@
         password: ${{ secrets.PYPI_API_TOKEN }}
 
   notify:
     if: always() && ${{ !github.event.pull_request.head.repo.fork && github.event.action != 'labeled' || github.event.label.name == 'approved-for-ci' }}
     needs:
     - pre-commit
     - unit-tests
-    - type-check
     - documentation
     - integration-tests
     - distribution
     runs-on: ubuntu-latest
     steps:
     - name: Trigger Teams notification
       uses: ecmwf-actions/notify-teams@v1
```

### Comparing `earthkit-regrid-0.3.0/.gitignore` & `earthkit_regrid-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/.pre-commit-config.yaml` & `earthkit_regrid-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/Makefile` & `earthkit_regrid-0.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/PKG-INFO` & `earthkit_regrid-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-regrid
-Version: 0.3.0
+Version: 0.3.1
 Summary: ECMWF python regridding toolkit
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: multiurl
 Requires-Dist: filelock
 Requires-Dist: scipy
 Provides-Extra: test
```

### Comparing `earthkit-regrid-0.3.0/README.md` & `earthkit_regrid-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/Makefile` & `earthkit_regrid-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/_static/style.css` & `earthkit_regrid-0.3.1/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/conf.py` & `earthkit_regrid-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/development.rst` & `earthkit_regrid-0.3.1/docs/development.rst`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/examples/healpix_fieldlist.ipynb` & `earthkit_regrid-0.3.1/docs/examples/healpix_fieldlist.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/examples/interpolation-2.ipynb` & `earthkit_regrid-0.3.1/docs/examples/interpolation-2.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/examples/numpy_arrays.ipynb` & `earthkit_regrid-0.3.1/docs/examples/numpy_arrays.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/examples/octahedral_fieldlist.ipynb` & `earthkit_regrid-0.3.1/docs/examples/octahedral_fieldlist.ipynb`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/gridspec.rst` & `earthkit_regrid-0.3.1/docs/gridspec.rst`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/index.rst` & `earthkit_regrid-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/interpolate.rst` & `earthkit_regrid-0.3.1/docs/interpolate.rst`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/licence.rst` & `earthkit_regrid-0.3.1/docs/licence.rst`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/docs/make.bat` & `earthkit_regrid-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/__init__.py` & `earthkit_regrid-0.3.1/earthkit/regrid/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/db.py` & `earthkit_regrid-0.3.1/earthkit/regrid/db.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/gridspec.py` & `earthkit_regrid-0.3.1/earthkit/regrid/gridspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 RGG_PATTERN = re.compile(r"[OoNn]\d+")
 
 
 # NOTE: this is a temporary code until the full gridspec
 # implementation is available via earthkit-geo.
 
 
-def same_coord(x, y):
-    return abs(x - y) < DEGREE_EPS
+def same_coord(x, y, eps=DEGREE_EPS):
+    return abs(x - y) < eps
 
 
 class GridSpec(dict):
     DEFAULTS = {
         "i_scans_negatively": 0,
         "j_points_consecutive": 0,
         "j_scans_positively": 0,
@@ -82,17 +82,17 @@
 
         if "shape" in self and "shape" in o:
             if self["shape"] != o["shape"]:
                 return False
         return True
 
     @staticmethod
-    def same_area(area1, area2):
+    def same_area(area1, area2, eps=DEGREE_EPS):
         if len(area1) == len(area2):
-            return all(same_coord(v1, v2) for v1, v2 in zip(area1, area2))
+            return all(same_coord(v1, v2, eps=eps) for v1, v2 in zip(area1, area2))
         return False
 
     def has_default_area(self):
         return self.same_area(self["area"], self.DEFAULT_AREA)
 
     @staticmethod
     def normalise_lon(lon, minimum):
@@ -231,27 +231,28 @@
         self.setdefault("area", self.DEFAULT_AREA)
         if self.get("global", 0) or self.has_default_area():
             self._global_ew = True
             self._global_ns = True
 
         self._octahedral = None
         self._N = None
+        self._eps = 0.12
 
     def __eq__(self, o):
         if not super().__eq__(o):
             return False
 
-        if self.same_area(self["area"], o["area"]):
+        if self.same_area(self["area"], o["area"], eps=self._eps):
             return True
 
         # check if west the same for global grids
         if self.is_global() and o.is_global():
             west = self.normalise_lon(self.west, 0)
             west_o = self.normalise_lon(o.west, 0)
-            if same_coord(west, west_o):
+            if same_coord(west, west_o, eps=self._eps):
                 return True
 
         # TODO: add code for non global grids
         return False
 
     @property
     def west(self):
```

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/interpolate.py` & `earthkit_regrid-0.3.1/earthkit/regrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/generate_inventory_rst.py` & `earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/generate_inventory_rst.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,14 +138,17 @@
 
     grid_type = args[0]
 
     gs = {}
     if grid_type == "reduced_gg_o":
         gs["type"] = "reduced_gg"
         gs["octahedral"] = True
+    elif grid_type == "reduced_gg":
+        gs["type"] = "reduced_gg"
+        gs["octahedral"] = False
     elif grid_type == "healpix_ring":
         gs["type"] = "healpix"
         gs["ordering"] = "ring"
     elif grid_type == "healpix_nested":
         gs["type"] = "healpix"
         gs["ordering"] = "nested"
     else:
```

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/module_output.py` & `earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/module_output.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/sphinxext/xref.py` & `earthkit_regrid-0.3.1/earthkit/regrid/sphinxext/xref.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/__init__.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/caching.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/caching.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/download.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/download.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/humanize.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/matrix.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/mir.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/mir.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/stream.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/stream.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit/regrid/utils/temporary.py` & `earthkit_regrid-0.3.1/earthkit/regrid/utils/temporary.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/earthkit_regrid.egg-info/PKG-INFO` & `earthkit_regrid-0.3.1/earthkit_regrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: earthkit-regrid
-Version: 0.3.0
+Version: 0.3.1
 Summary: ECMWF python regridding toolkit
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 Requires-Dist: multiurl
 Requires-Dist: filelock
 Requires-Dist: scipy
 Provides-Extra: test
```

### Comparing `earthkit-regrid-0.3.0/earthkit_regrid.egg-info/SOURCES.txt` & `earthkit_regrid-0.3.1/earthkit_regrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/setup.cfg` & `earthkit_regrid-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/conftest.py` & `earthkit_regrid-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/index.json` & `earthkit_regrid-0.3.1/tests/data/local/db/index.json`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/0efb7cc6060e3365bd2a0c0037e6a339fd2fd71fdba607cd9b6aa13683d01523.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/0efb7cc6060e3365bd2a0c0037e6a339fd2fd71fdba607cd9b6aa13683d01523.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/2800f6a28606667ff1e20b82b067e6cf94670b854651601f6ee15683e80e4933.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/2800f6a28606667ff1e20b82b067e6cf94670b854651601f6ee15683e80e4933.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/4b7e0a8bb9dee07acc5822ad0caa72f0e5fae26e956b981aa707f2dba9bab915.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/4b7e0a8bb9dee07acc5822ad0caa72f0e5fae26e956b981aa707f2dba9bab915.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/82ef0fa6d7c834016fe52e93f6cd4185a044e0a900c02906f146998c09c2e22e.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/82ef0fa6d7c834016fe52e93f6cd4185a044e0a900c02906f146998c09c2e22e.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_linear/8d0fbe91fd547ad49d86acd6f31b339163f35cdfd183689367f6864d98d3328d.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_linear/8d0fbe91fd547ad49d86acd6f31b339163f35cdfd183689367f6864d98d3328d.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/96b820068578d6b778b0e1359d34e0dfa8c65417b6fbe3e3725fb1bc7a90b3c6.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/96b820068578d6b778b0e1359d34e0dfa8c65417b6fbe3e3725fb1bc7a90b3c6.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/bed78a06d90a74c03bd9b7d9dff94ea3c6436ab99bf182f92ac1e5c9b0977708.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/bed78a06d90a74c03bd9b7d9dff94ea3c6436ab99bf182f92ac1e5c9b0977708.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/c0de1f0a5e662a9392c06416df2e0124a75d8a97c497b19360f7bea1e3ab694b.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/c0de1f0a5e662a9392c06416df2e0124a75d8a97c497b19360f7bea1e3ab694b.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/e0a86032fae661b1de48828084ab32c3aee40b50871f0f8cd4b9c1b919991525.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/e0a86032fae661b1de48828084ab32c3aee40b50871f0f8cd4b9c1b919991525.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/db/mir_16_nearest-neighbour/f330f076443c96111fab1e6df633ac3c9e605ffec35b4a1a78bc952e6a5925b6.npz` & `earthkit_regrid-0.3.1/tests/data/local/db/mir_16_nearest-neighbour/f330f076443c96111fab1e6df633ac3c9e605ffec35b4a1a78bc952e6a5925b6.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/in_5x5.npz` & `earthkit_regrid-0.3.1/tests/data/local/in_5x5.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/in_H4_nested.npz` & `earthkit_regrid-0.3.1/tests/data/local/in_H4_nested.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/in_H4_ring.npz` & `earthkit_regrid-0.3.1/tests/data/local/in_H4_ring.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/in_N32.npz` & `earthkit_regrid-0.3.1/tests/data/local/in_N32.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/in_O32.npz` & `earthkit_regrid-0.3.1/tests/data/local/in_O32.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_5x5_10x10_linear.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_5x5_10x10_linear.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_5x5_10x10_nearest-neighbour.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_5x5_10x10_nearest-neighbour.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_H4_nested_10x10_linear.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_H4_nested_10x10_linear.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_H4_nested_10x10_nearest-neighbour.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_H4_nested_10x10_nearest-neighbour.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_H4_ring_10x10_linear.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_H4_ring_10x10_linear.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_H4_ring_10x10_nearest-neighbour.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_H4_ring_10x10_nearest-neighbour.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_N32_10x10_linear.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_N32_10x10_linear.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_N32_10x10_nearest-neighbour.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_N32_10x10_nearest-neighbour.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_O32_10x10_linear.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_O32_10x10_linear.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/data/local/out_O32_10x10_nearest-neighbour.npz` & `earthkit_regrid-0.3.1/tests/data/local/out_O32_10x10_nearest-neighbour.npz`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/test_gridspec.py` & `earthkit_regrid-0.3.1/tests/test_gridspec.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,23 +49,36 @@
         ({"grid": "O32"}, {"grid": [2, 2]}),
         ({"grid": "O32"}, {"grid": [2.5, 2.5]}),
         ({"grid": "O32"}, {"grid": [5, 5]}),
         ({"grid": "O32"}, {"grid": [10, 10]}),
         ({"grid": "O32", "shape": [5248]}, {"grid": [10, 10]}),
         ({"grid": "O32", "area": [90, 0, -90, 360]}, {"grid": [10, 10]}),
         ({"grid": "O32", "area": [87.8638, 0, -87.8638, 357.5]}, {"grid": [10, 10]}),
+        (
+            {"grid": "O32", "area": [87.8638, 0.01, -87.8638, 357.5]},
+            {"grid": [10, 10]},
+        ),
+        (
+            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.6]},
+            {"grid": [10, 10]},
+        ),
         ({"grid": "O32", "global": 1}, {"grid": [10, 10]}),
         (
             {"grid": "O32", "global": 1, "area": [87.8638, 0, -87.8638, 357.5]},
             {"grid": [10, 10]},
         ),
         ({"grid": "N32"}, {"grid": [10, 10]}),
         ({"grid": "N32", "shape": [6114]}, {"grid": [10, 10]}),
         ({"grid": "N32", "area": [90, 0, -90, 360]}, {"grid": [10, 10]}),
         ({"grid": "N32", "area": [87.8638, 0, -87.8638, 357.188]}, {"grid": [10, 10]}),
+        ({"grid": "N32", "area": [87.8638, 0, -87.8638, 357.189]}, {"grid": [10, 10]}),
+        (
+            {"grid": "N32", "area": [87.8638, 0.01, -87.8638, 357.188]},
+            {"grid": [10, 10]},
+        ),
         ({"grid": "N32", "global": 1}, {"grid": [10, 10]}),
         (
             {"grid": "N32", "global": 1, "area": [87.8638, 0, -87.8638, 357.188]},
             {"grid": [10, 10]},
         ),
         ({"grid": "H128"}, {"grid": [1, 1]}),
         ({"grid": "H128", "ordering": "ring"}, {"grid": [1, 1]}),
@@ -87,36 +100,26 @@
         ({"grid": [5, 5], "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": [5, 5], "area": [90, 10, -90, 370]}, {"grid": [10, 10]}, None),
         ({"grid": "G1280", "shape": 6599680}, {"grid": [10, 10]}, ValueError),
         ({"grid": "O32", "shape": 6599680}, {"grid": [10, 10]}, None),
         ({"grid": "O32", "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": "O32", "area": [90, -0.1, -90, 360]}, {"grid": [10, 10]}, None),
         (
-            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.6]},
+            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.7]},
             {"grid": [10, 10]},
             None,
         ),
         (
-            {"grid": "O32", "area": [87.8638, 0.01, -87.8638, 357.5]},
+            {"grid": "O32", "area": [87.8638, 0.2, -87.8638, 357.5]},
             {"grid": [10, 10]},
             None,
         ),
         ({"grid": "N32", "shape": 6599680}, {"grid": [10, 10]}, None),
         ({"grid": "N32", "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": "N32", "area": [90, -0.1, -90, 360]}, {"grid": [10, 10]}, None),
-        (
-            {"grid": "N32", "area": [87.8638, 0, -87.8638, 357.189]},
-            {"grid": [10, 10]},
-            None,
-        ),
-        (
-            {"grid": "N32", "area": [87.8638, 0.01, -87.8638, 357.188]},
-            {"grid": [10, 10]},
-            None,
-        ),
     ],
 )
 def test_gridspec_bad(gs_in, gs_out, err):
     if err:
         with pytest.raises(err):
             r = SYS_DB.find_entry(gs_in, gs_out, "linear")
     else:
```

### Comparing `earthkit-regrid-0.3.0/tests/test_interpolate.py` & `earthkit_regrid-0.3.1/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tests/test_local.py` & `earthkit_regrid-0.3.1/tests/test_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,23 +138,33 @@
         ({"grid": [5, 5], "shape": [37, 72]}, {"grid": [10, 10], "shape": [19, 36]}),
         ({"grid": [5, 5], "shape": [37, 72]}, {"grid": [10, 10]}),
         ({"grid": [5, 5]}, {"grid": [10, 10], "shape": [19, 36]}),
         ({"grid": "O32"}, {"grid": [10, 10]}),
         ({"grid": "O32", "shape": [5248]}, {"grid": [10, 10]}),
         ({"grid": "O32", "area": [90, 0, -90, 360]}, {"grid": [10, 10]}),
         ({"grid": "O32", "area": [87.8638, 0, -87.8638, 357.5]}, {"grid": [10, 10]}),
+        ({"grid": "O32", "area": [87.8638, 0.01, -87.8638, 357.5]}, {"grid": [10, 10]}),
         ({"grid": "O32", "global": 1}, {"grid": [10, 10]}),
         (
             {"grid": "O32", "global": 1, "area": [87.8638, 0, -87.8638, 357.5]},
             {"grid": [10, 10]},
         ),
         ({"grid": "N32"}, {"grid": [10, 10]}),
         ({"grid": "N32", "shape": [6114]}, {"grid": [10, 10]}),
         ({"grid": "N32", "area": [90, 0, -90, 360]}, {"grid": [10, 10]}),
         ({"grid": "N32", "area": [87.8638, 0, -87.8638, 357.188]}, {"grid": [10, 10]}),
+        ({"grid": "N32", "area": [87.8638, 0, -87.8638, 357.189]}, {"grid": [10, 10]}),
+        (
+            {"grid": "N32", "area": [87.8638, 0.01, -87.8638, 357.188]},
+            {"grid": [10, 10]},
+        ),
+        (
+            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.6]},
+            {"grid": [10, 10]},
+        ),
         ({"grid": "N32", "global": 1}, {"grid": [10, 10]}),
         (
             {"grid": "N32", "global": 1, "area": [87.8638, 0, -87.8638, 357.188]},
             {"grid": [10, 10]},
         ),
         ({"grid": "H4"}, {"grid": [10, 10]}),
         ({"grid": "H4", "ordering": "ring"}, {"grid": [10, 10]}),
@@ -177,36 +187,26 @@
         ({"grid": [5, 5], "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": [5, 5], "area": [90, 10, -90, 370]}, {"grid": [10, 10]}, None),
         ({"grid": "G1280", "shape": 6599680}, {"grid": [10, 10]}, ValueError),
         ({"grid": "O32", "shape": 6599680}, {"grid": [10, 10]}, None),
         ({"grid": "O32", "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": "O32", "area": [90, -0.1, -90, 360]}, {"grid": [10, 10]}, None),
         (
-            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.6]},
+            {"grid": "O32", "area": [87.8638, 0, -87.8638, 357.7]},
             {"grid": [10, 10]},
             None,
         ),
         (
-            {"grid": "O32", "area": [87.8638, 0.01, -87.8638, 357.5]},
+            {"grid": "O32", "area": [87.8638, 0.2, -87.8638, 357.5]},
             {"grid": [10, 10]},
             None,
         ),
         ({"grid": "N32", "shape": 6599680}, {"grid": [10, 10]}, None),
         ({"grid": "N32", "area": [90, 0, -90, 359.999]}, {"grid": [10, 10]}, None),
         ({"grid": "N32", "area": [90, -0.1, -90, 360]}, {"grid": [10, 10]}, None),
-        (
-            {"grid": "N32", "area": [87.8638, 0, -87.8638, 357.189]},
-            {"grid": [10, 10]},
-            None,
-        ),
-        (
-            {"grid": "N32", "area": [87.8638, 0.01, -87.8638, 357.188]},
-            {"grid": [10, 10]},
-            None,
-        ),
         ({"grid": "H4", "ordering": "any"}, {"grid": [10, 10]}, ValueError),
     ],
 )
 def test_local_gridspec_bad(gs_in, gs_out, err):
     DB = add_matrix_source(DB_PATH)
     if err:
         with pytest.raises(err):
```

### Comparing `earthkit-regrid-0.3.0/tests/test_version.py` & `earthkit_regrid-0.3.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/make-matrix.sh` & `earthkit_regrid-0.3.1/tools/make-matrix.sh`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/manage/build_db.py` & `earthkit_regrid-0.3.1/tools/manage/build_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/manage/build_local_test_db.py` & `earthkit_regrid-0.3.1/tools/manage/build_local_test_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/manage/merge_index.py` & `earthkit_regrid-0.3.1/tools/manage/merge_index.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/subset/eccharts_subset_db_conf.yaml` & `earthkit_regrid-0.3.1/tools/subset/eccharts_subset_db_conf.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/subset/subset_db_conf.yaml` & `earthkit_regrid-0.3.1/tools/subset/subset_db_conf.yaml`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/subset/subset_remote_db.py` & `earthkit_regrid-0.3.1/tools/subset/subset_remote_db.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/utils/grid.py` & `earthkit_regrid-0.3.1/tools/utils/grid.py`

 * *Files identical despite different names*

### Comparing `earthkit-regrid-0.3.0/tools/utils/matrix.py` & `earthkit_regrid-0.3.1/tools/utils/matrix.py`

 * *Files identical despite different names*

