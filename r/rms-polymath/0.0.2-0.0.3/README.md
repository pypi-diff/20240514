# Comparing `tmp/rms-polymath-0.0.2.tar.gz` & `tmp/rms_polymath-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rms-polymath-0.0.2.tar", last modified: Wed Jan 24 23:33:27 2024, max compression
+gzip compressed data, was "rms_polymath-0.0.3.tar", last modified: Tue May 14 19:18:32 2024, max compression
```

## Comparing `rms-polymath-0.0.2.tar` & `rms_polymath-0.0.3.tar`

### file list

```diff
@@ -1,142 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.166053 rms-polymath-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.142053 rms-polymath-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.146053 rms-polymath-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/.github/workflows/publish_to_test_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-24 23:33:27.166053 rms-polymath-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.150053 rms-polymath-0.0.2/polymath/
--rwxr-xr-x   0 runner    (1001) docker     (127)      841 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/polymath/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7680 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/boolean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.150053 rms-polymath-0.0.2/polymath/extensions/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4291 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21831 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/item_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/mask_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/math_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    41774 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/pickler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/shaper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/shrinker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/extensions/tvl.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22527 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27278 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/matrix3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8998 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/pair.py
--rw-r--r--   0 runner    (1001) docker     (127)    17622 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/polynomial.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31459 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)   177349 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/qube.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    61094 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/scalar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29830 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/units.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39900 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/vector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12195 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/polymath/vector3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.166053 rms-polymath-0.0.2/rms_polymath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/rms_polymath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/rms_polymath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/rms_polymath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/rms_polymath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-24 23:33:27.000000 rms-polymath-0.0.2/rms_polymath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-24 23:33:27.166053 rms-polymath-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.150053 rms-polymath-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 23:33:27.166053 rms-polymath-0.0.2/tests/unit_tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)      196 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24135 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_boolean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27878 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_indices.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix3_euler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2009 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix3_quaternion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4161 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix3_twovec.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4707 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_column_vectors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6836 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_inverse.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1925 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_is_diagonal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2670 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14971 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4583 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_row_vectors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1441 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_matrix_unitary.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2990 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_pair_as_pair.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_pair_clip2d.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11606 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_pair_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3924 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_pair_swapxy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1622 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_polynomial.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7473 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_quaternion.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1936 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_quaternion_euler.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3879 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_quaternion_matrix3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1925 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_quaternion_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3453 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_quaternion_parts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5610 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5538 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_any.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8159 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_as_this_type.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_derivs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19019 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_getitem.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_getstate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2635 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_identity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15431 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_items.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2350 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_iterate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7523 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_masking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5723 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_power.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2709 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_readonly.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20503 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_reshaping.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31817 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_setitem.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12816 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_shrink.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7380 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_stack.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9755 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_types.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3801 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_units.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3994 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_qube_zero.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4335 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_arccos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4317 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_arcsin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3476 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_arctan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6215 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_arctan2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_as_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2331 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_as_scalar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4037 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_cos.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4362 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_exp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3741 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_frac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4006 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_int.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3827 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4674 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_max.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1961 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_maximum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5000 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_mean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_median.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4555 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_minimum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14361 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    58946 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5859 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_quadratic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4526 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_reciprocal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3034 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_sign.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4037 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_sin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3567 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_sqrt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4593 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_sum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3854 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_scalar_tan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4170 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_units.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7136 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10914 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector3_misc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3270 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector3_spin.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2898 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_as_column.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3806 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_as_diagonal.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2883 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_as_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2919 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_as_row.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4461 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_as_vector.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7166 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_cross_2x2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8604 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_cross_3x3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4721 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_dot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10350 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_element_div.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9214 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_element_mul.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4144 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_masking.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6908 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_mean_sum.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3712 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_norm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3755 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_norm_sq.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34247 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_ops.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5059 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_outer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9294 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_perp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8961 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_proj.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6777 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_scalars.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_sep.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4894 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_ucross.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4226 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unit_tests/test_vector_unit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-01-24 23:32:51.000000 rms-polymath-0.0.2/tests/unittester.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.337633 rms_polymath-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.313633 rms_polymath-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.313633 rms_polymath-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/.github/workflows/publish_to_test_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-14 19:18:32.337633 rms_polymath-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.317633 rms_polymath-0.0.3/polymath/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/polymath/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7680 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/boolean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.317633 rms_polymath-0.0.3/polymath/extensions/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4291 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21831 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14982 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/item_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/mask_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23319 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/math_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41774 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/shaper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/shrinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/extensions/tvl.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22527 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27278 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/matrix3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8998 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/pair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17622 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/polynomial.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31459 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)   177349 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/qube.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    61094 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/scalar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29830 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/units.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    39900 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/vector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12195 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/polymath/vector3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.337633 rms_polymath-0.0.3/rms_polymath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/rms_polymath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/rms_polymath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/rms_polymath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/rms_polymath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 19:18:32.000000 rms_polymath-0.0.3/rms_polymath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-14 19:18:32.341633 rms_polymath-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.321633 rms_polymath-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:18:32.337633 rms_polymath-0.0.3/tests/unit_tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      196 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24135 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_boolean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27878 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_indices.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1473 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix3_euler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2009 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix3_quaternion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4161 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix3_twovec.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4707 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_column_vectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6836 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_inverse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1925 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_is_diagonal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2670 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14971 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4583 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_row_vectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1441 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_matrix_unitary.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2990 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_pair_as_pair.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1268 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_pair_clip2d.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11606 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_pair_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3924 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_pair_swapxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1622 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_polynomial.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7473 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_quaternion.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1936 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_quaternion_euler.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3879 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_quaternion_matrix3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1925 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_quaternion_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3453 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_quaternion_parts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5610 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5538 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_any.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8159 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_as_this_type.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_derivs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19019 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_getitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_getstate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2635 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_identity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15431 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_items.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2350 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_iterate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7523 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5723 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_power.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2709 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_readonly.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20503 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_reshaping.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31817 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_setitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12816 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_shrink.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7380 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_stack.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9755 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3801 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_units.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3994 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_qube_zero.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4335 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_arccos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4317 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_arcsin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3476 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_arctan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6215 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_arctan2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1213 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_as_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2331 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_as_scalar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4037 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_cos.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4362 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_exp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3741 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_frac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4006 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_int.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3827 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4674 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_max.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1961 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_maximum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5000 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_mean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4937 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_median.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4555 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_minimum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14361 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58946 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5859 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_quadratic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4526 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_reciprocal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3034 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_sign.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4037 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_sin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3567 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_sqrt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4593 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_sum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3854 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_scalar_tan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4170 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_units.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7136 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10914 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector3_misc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3270 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector3_spin.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2898 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_as_column.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3806 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_as_diagonal.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2883 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_as_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2919 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_as_row.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4461 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_as_vector.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7166 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_cross_2x2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8604 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_cross_3x3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4721 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_dot.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10350 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_element_div.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9214 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_element_mul.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4144 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_masking.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6908 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_mean_sum.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3712 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_norm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3755 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_norm_sq.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34247 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_ops.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5059 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_outer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9294 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_perp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8961 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_proj.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6777 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_scalars.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5497 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_sep.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4894 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_ucross.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4226 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unit_tests/test_vector_unit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5672 2024-05-14 19:18:00.000000 rms_polymath-0.0.3/tests/unittester.py
```

### Comparing `rms-polymath-0.0.2/.github/workflows/publish_to_pypi.yml` & `rms_polymath-0.0.3/.github/workflows/publish_to_pypi.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Publish to PyPI
-run-name: Publish to PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   release:
     types: [published]
 
 jobs:
   upload_pypi:
@@ -11,15 +11,15 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-polymath-0.0.2/.github/workflows/publish_to_test_pypi.yml` & `rms_polymath-0.0.3/.github/workflows/publish_to_test_pypi.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 name: Publish to Test PyPI
-run-name: Publish to Test PyPI triggered by ${{ github.ref_type }} ${{ github.ref_name }}
+run-name: "Publish to Test PyPI: ${{ github.ref_type }} ${{ github.ref_name }}"
 
 on:
   workflow_dispatch:
 
 jobs:
   upload_pypi:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python 3.12
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.12
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
```

### Comparing `rms-polymath-0.0.2/.github/workflows/run-tests.yml` & `rms_polymath-0.0.3/.github/workflows/run-tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Run Tests
-run-name: Run Tests triggered by ${{ github.ref_type }} ${{ github.ref_name }} or ${{ github.triggering_actor }}
+run-name: "Run Tests: ${{ github.ref_type }} ${{ github.ref_name }} by ${{ github.triggering_actor }}"
 
 on:
   workflow_dispatch:
   pull_request:
     branches: [ main ]
   push:
     branches: [ main ]
@@ -22,25 +22,29 @@
     steps:
       - name: Checkout
         uses: actions/checkout@v4
         with:
           ref: ${{ github.event.pull_request.head.sha }}
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install -r requirements.txt
 
       - name: Test with coverage
         run: |
           coverage run -m pytest
 
+      - name: Print coverage report
+        run: |
+          coverage report -m
+
       - name: Upload coverage report to codecov
-        uses: codecov/codecov-action@v3
-        env:
-          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: codecov/codecov-action@v4
+        if: matrix.os == 'ubuntu-latest' && matrix.python-version == '3.12'
         with:
+          token: ${{ secrets.CODECOV_TOKEN }}
           verbose: true
```

### Comparing `rms-polymath-0.0.2/.gitignore` & `rms_polymath-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/LICENSE` & `rms_polymath-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/__init__.py` & `rms_polymath-0.0.3/polymath/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 from polymath.units      import Units
 from polymath.vector     import Vector
 from polymath.vector3    import Vector3
 
 import polymath.extensions
 
 try:
-    from _version import __version__
+    from ._version import __version__
 except ImportError as err:
     __version__ = 'Version unspecified'
 
 ################################################################################
```

### Comparing `rms-polymath-0.0.2/polymath/boolean.py` & `rms_polymath-0.0.3/polymath/boolean.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/__init__.py` & `rms_polymath-0.0.3/polymath/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/indexer.py` & `rms_polymath-0.0.3/polymath/extensions/indexer.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/item_ops.py` & `rms_polymath-0.0.3/polymath/extensions/item_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/iterator.py` & `rms_polymath-0.0.3/polymath/extensions/iterator.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/mask_ops.py` & `rms_polymath-0.0.3/polymath/extensions/mask_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/math_ops.py` & `rms_polymath-0.0.3/polymath/extensions/math_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/pickler.py` & `rms_polymath-0.0.3/polymath/extensions/pickler.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/shaper.py` & `rms_polymath-0.0.3/polymath/extensions/shaper.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/shrinker.py` & `rms_polymath-0.0.3/polymath/extensions/shrinker.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/extensions/tvl.py` & `rms_polymath-0.0.3/polymath/extensions/tvl.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/matrix.py` & `rms_polymath-0.0.3/polymath/matrix.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/matrix3.py` & `rms_polymath-0.0.3/polymath/matrix3.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/pair.py` & `rms_polymath-0.0.3/polymath/pair.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/polynomial.py` & `rms_polymath-0.0.3/polymath/polynomial.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/quaternion.py` & `rms_polymath-0.0.3/polymath/quaternion.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/qube.py` & `rms_polymath-0.0.3/polymath/qube.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/scalar.py` & `rms_polymath-0.0.3/polymath/scalar.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/units.py` & `rms_polymath-0.0.3/polymath/units.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/vector.py` & `rms_polymath-0.0.3/polymath/vector.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/polymath/vector3.py` & `rms_polymath-0.0.3/polymath/vector3.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/pyproject.toml` & `rms_polymath-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/rms_polymath.egg-info/SOURCES.txt` & `rms_polymath-0.0.3/rms_polymath.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 .coveragerc
 .gitignore
+CODE_OF_CONDUCT.md
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 .github/workflows/publish_to_pypi.yml
 .github/workflows/publish_to_test_pypi.yml
```

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_boolean.py` & `rms_polymath-0.0.3/tests/unit_tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_indices.py` & `rms_polymath-0.0.3/tests/unit_tests/test_indices.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix3_euler.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix3_euler.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix3_quaternion.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix3_quaternion.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix3_twovec.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix3_twovec.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_column_vectors.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_column_vectors.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_inverse.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_inverse.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_is_diagonal.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_is_diagonal.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_misc.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_misc.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_ops.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_row_vectors.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_row_vectors.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_matrix_unitary.py` & `rms_polymath-0.0.3/tests/unit_tests/test_matrix_unitary.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_pair_as_pair.py` & `rms_polymath-0.0.3/tests/unit_tests/test_pair_as_pair.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_pair_clip2d.py` & `rms_polymath-0.0.3/tests/unit_tests/test_pair_clip2d.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_pair_misc.py` & `rms_polymath-0.0.3/tests/unit_tests/test_pair_misc.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_pair_swapxy.py` & `rms_polymath-0.0.3/tests/unit_tests/test_pair_swapxy.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_polynomial.py` & `rms_polymath-0.0.3/tests/unit_tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_quaternion.py` & `rms_polymath-0.0.3/tests/unit_tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_quaternion_euler.py` & `rms_polymath-0.0.3/tests/unit_tests/test_quaternion_euler.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_quaternion_matrix3.py` & `rms_polymath-0.0.3/tests/unit_tests/test_quaternion_matrix3.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_quaternion_ops.py` & `rms_polymath-0.0.3/tests/unit_tests/test_quaternion_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_quaternion_parts.py` & `rms_polymath-0.0.3/tests/unit_tests/test_quaternion_parts.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_all.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_all.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_any.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_any.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_as_this_type.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_as_this_type.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_derivs.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_derivs.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_getitem.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_getitem.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_getstate.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_getstate.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_identity.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_identity.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_items.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_items.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_iterate.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_iterate.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_masking.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_masking.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_power.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_power.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_readonly.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_readonly.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_reshaping.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_reshaping.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_setitem.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_setitem.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_shrink.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_shrink.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_stack.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_stack.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_types.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_types.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_units.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_units.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_qube_zero.py` & `rms_polymath-0.0.3/tests/unit_tests/test_qube_zero.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_arccos.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_arccos.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_arcsin.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_arcsin.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_arctan.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_arctan.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_arctan2.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_arctan2.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_as_index.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_as_index.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_as_scalar.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_as_scalar.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_cos.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_cos.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_exp.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_exp.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_frac.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_frac.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_int.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_int.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_log.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_log.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_max.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_max.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_maximum.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_maximum.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_mean.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_mean.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_median.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_median.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_min.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_min.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_minimum.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_minimum.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_misc.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_misc.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_ops.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_quadratic.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_quadratic.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_reciprocal.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_reciprocal.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_sign.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_sign.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_sin.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_sin.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_sqrt.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_sqrt.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_sum.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_sum.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_scalar_tan.py` & `rms_polymath-0.0.3/tests/unit_tests/test_scalar_tan.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_units.py` & `rms_polymath-0.0.3/tests/unit_tests/test_units.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector3.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector3.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector3_misc.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector3_misc.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector3_spin.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector3_spin.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_as_column.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_as_column.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_as_diagonal.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_as_diagonal.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_as_index.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_as_index.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_as_row.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_as_row.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_as_vector.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_as_vector.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_cross_2x2.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_cross_2x2.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_cross_3x3.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_cross_3x3.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_dot.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_dot.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_element_div.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_element_div.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_element_mul.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_element_mul.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_masking.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_masking.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_mean_sum.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_mean_sum.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_norm.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_norm.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_norm_sq.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_norm_sq.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_ops.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_ops.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_outer.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_outer.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_perp.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_perp.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_proj.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_proj.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_scalars.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_scalars.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_sep.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_sep.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_ucross.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_ucross.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unit_tests/test_vector_unit.py` & `rms_polymath-0.0.3/tests/unit_tests/test_vector_unit.py`

 * *Files identical despite different names*

### Comparing `rms-polymath-0.0.2/tests/unittester.py` & `rms_polymath-0.0.3/tests/unittester.py`

 * *Files identical despite different names*

