# Comparing `tmp/astromodels-2.4.1.dev2.tar.gz` & `tmp/astromodels-2.4.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromodels-2.4.1.dev2.tar", last modified: Wed Nov  1 23:21:56 2023, max compression
+gzip compressed data, was "astromodels-2.4.2.dev1.tar", last modified: Mon May 13 23:01:18 2024, max compression
```

## Comparing `astromodels-2.4.1.dev2.tar` & `astromodels-2.4.2.dev1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      329 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.181140 astromodels-2.4.1.dev2/astromodels/
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-11-01 23:21:56.181140 astromodels-2.4.1.dev2/astromodels/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.157138 astromodels-2.4.1.dev2/astromodels/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/cpickle_compatibility_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/memoization.py
--rw-r--r--   0 runner    (1001) docker     (127)    42436 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    35019 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/model_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/my_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/node_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    45628 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/parameter_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/polarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/property.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8396 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/sky_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/spectral_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/thread_safe_unit_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/core/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.157138 astromodels-2.4.1.dev2/astromodels/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.161139 astromodels-2.4.1.dev2/astromodels/data/dark_matter/
--rw-r--r--   0 runner    (1001) docker     (127)  1200080 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/dark_matter/dmSpecTab.npy
--rw-r--r--   0 runner    (1001) docker     (127)   936288 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/dark_matter/gammamc_dif.dat
--rw-r--r--   0 runner    (1001) docker     (127)      517 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/log_theme.ini
--rw-r--r--   0 runner    (1001) docker     (127)   115904 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/past_1D_values.h5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.165139 astromodels-2.4.1.dev2/astromodels/data/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/tests/black_hole.yaml
--rw-r--r--   0 runner    (1001) docker     (127)  1835540 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/tests/old_table.h5
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/tests/simple_source.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34560 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/tests/test_xspec_table_model.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.165139 astromodels-2.4.1.dev2/astromodels/data/xsect/
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_phabs_angr.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_phabs_aspl.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_angr.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_aspl.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_wilm.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_wabs_angr.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.169139 astromodels-2.4.1.dev2/astromodels/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.169139 astromodels-2.4.1.dev2/astromodels/functions/dark_matter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/dark_matter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11801 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/dark_matter/dm_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    83913 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.169139 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/absorption.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/apec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/extinction.py
--rw-r--r--   0 runner    (1001) docker     (127)    20249 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/polynomials.py
--rw-r--r--   0 runner    (1001) docker     (127)    31837 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_1D/powerlaws.py
--rw-r--r--   0 runner    (1001) docker     (127)    29807 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/functions_3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     5563 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/numba_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21508 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/priors.py
--rw-r--r--   0 runner    (1001) docker     (127)    32506 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/functions/template_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.169139 astromodels-2.4.1.dev2/astromodels/sources/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11332 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/sources/extended_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/sources/particle_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/sources/point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/sources/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.173139 astromodels-2.4.1.dev2/astromodels/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_1D_function_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9369 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_extended_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    23948 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_load_xspec_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_memoizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    24934 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19209 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10171 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_polarization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6741 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_template_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/tests/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.173139 astromodels-2.4.1.dev2/astromodels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/angular_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/config_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/data_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/disk_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5648 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/long_path_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/pretty_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/table.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/valid_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/utils/vincenty.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/astromodels/xspec/
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/README
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.153138 astromodels-2.4.1.dev2/astromodels/xspec/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/array.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/astro/
--rw-r--r--   0 runner    (1001) docker     (127)    40695 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/astro/xspec_extension.hh
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/constants.hh
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/extension.hh
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/fcmp.hh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/astromodels/xspec/src/
--rw-r--r--   0 runner    (1001) docker     (127)    33813 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/src/_xspec.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/astromodels/xspec/xspec_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 23:21:56.157138 astromodels-2.4.1.dev2/astromodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4429 2023-11-01 23:21:56.000000 astromodels-2.4.1.dev2/astromodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-11-01 23:21:56.000000 astromodels-2.4.1.dev2/astromodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 23:21:56.000000 astromodels-2.4.1.dev2/astromodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-11-01 23:21:56.000000 astromodels-2.4.1.dev2/astromodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-11-01 23:21:56.000000 astromodels-2.4.1.dev2/astromodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2023-11-01 23:21:56.177140 astromodels-2.4.1.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12756 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    69019 2023-11-01 23:21:49.000000 astromodels-2.4.1.dev2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.517198 astromodels-2.4.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-13 23:01:18.517198 astromodels-2.4.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.517198 astromodels-2.4.2.dev1/astromodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 23:01:18.517198 astromodels-2.4.2.dev1/astromodels/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.497198 astromodels-2.4.2.dev1/astromodels/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/cpickle_compatibility_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/memoization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42436 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35019 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/model_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/my_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/node_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45628 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/parameter_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/polarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8396 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/sky_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/spectral_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/thread_safe_unit_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/core/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.497198 astromodels-2.4.2.dev1/astromodels/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.497198 astromodels-2.4.2.dev1/astromodels/data/dark_matter/
+-rw-r--r--   0 runner    (1001) docker     (127)  1200080 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/dark_matter/dmSpecTab.npy
+-rw-r--r--   0 runner    (1001) docker     (127)   936288 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/dark_matter/gammamc_dif.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/log_theme.ini
+-rw-r--r--   0 runner    (1001) docker     (127)   115904 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/past_1D_values.h5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.501198 astromodels-2.4.2.dev1/astromodels/data/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/tests/black_hole.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)  1835540 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/tests/old_table.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/tests/simple_source.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34560 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/tests/test_xspec_table_model.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.505198 astromodels-2.4.2.dev1/astromodels/data/xsect/
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_phabs_angr.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_phabs_aspl.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_angr.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_aspl.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_wilm.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_wabs_angr.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.505198 astromodels-2.4.2.dev1/astromodels/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.505198 astromodels-2.4.2.dev1/astromodels/functions/dark_matter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/dark_matter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/dark_matter/dm_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83913 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.509198 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/apec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/extinction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20249 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/polynomials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31837 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_1D/powerlaws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29807 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/functions_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/numba_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21508 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32506 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/functions/template_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.509198 astromodels-2.4.2.dev1/astromodels/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11332 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/sources/extended_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/sources/particle_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/sources/point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/sources/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.509198 astromodels-2.4.2.dev1/astromodels/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_1D_function_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9369 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_extended_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23948 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_load_xspec_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_memoizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24934 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19209 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10171 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_polarization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6741 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_template_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/angular_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/config_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/data_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/disk_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/long_path_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/pretty_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/valid_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/utils/vincenty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels/xspec/
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/README
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.489198 astromodels-2.4.2.dev1/astromodels/xspec/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/array.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/astro/
+-rw-r--r--   0 runner    (1001) docker     (127)    40695 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/astro/xspec_extension.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/constants.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/extension.hh
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/fcmp.hh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels/xspec/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    33813 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/src/_xspec.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-13 23:01:13.000000 astromodels-2.4.2.dev1/astromodels/xspec/xspec_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 23:01:18.513198 astromodels-2.4.2.dev1/astromodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-13 23:01:18.000000 astromodels-2.4.2.dev1/astromodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-13 23:01:18.000000 astromodels-2.4.2.dev1/astromodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 23:01:18.000000 astromodels-2.4.2.dev1/astromodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-13 23:01:18.000000 astromodels-2.4.2.dev1/astromodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 23:01:18.000000 astromodels-2.4.2.dev1/astromodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-13 23:01:18.517198 astromodels-2.4.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12946 2024-05-13 23:01:14.000000 astromodels-2.4.2.dev1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69019 2024-05-13 23:01:14.000000 astromodels-2.4.2.dev1/versioneer.py
```

### Comparing `astromodels-2.4.1.dev2/LICENSE` & `astromodels-2.4.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/PKG-INFO` & `astromodels-2.4.2.dev1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: astromodels
-Version: 2.4.1.dev2
+Version: 2.4.2.dev1
 Summary: Astromodels contains models to be used in likelihood or Bayesian analysis in astronomy
 Home-page: https://github.com/threeml/astromodels
 Download-URL: https://github.com/threeml/astromodels/archive/v0.1
 Author: Giacomo Vianello
 Author-email: giacomo.vianello@gmail.com
 Project-URL: Documentation, https://astromodels.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/threeML/astromodels/issues
 Project-URL: Source Code, https://github.com/threeML/astromodels
 Keywords: Likelihood,Models,fit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.6
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: scipy>=0.14
 Requires-Dist: astropy>=1.2
 Requires-Dist: dill
 Requires-Dist: future
 Requires-Dist: interpolation>=2.2.3
-Requires-Dist: numba>0.52
+Requires-Dist: numba
 Requires-Dist: h5py
 Requires-Dist: pandas
 Requires-Dist: tables
 Requires-Dist: colorama
 Requires-Dist: omegaconf
 Requires-Dist: rich
 Requires-Dist: joblib
```

### Comparing `astromodels-2.4.1.dev2/README.md` & `astromodels-2.4.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/__init__.py` & `astromodels-2.4.2.dev1/astromodels/__init__.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/memoization.py` & `astromodels-2.4.2.dev1/astromodels/core/memoization.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/model.py` & `astromodels-2.4.2.dev1/astromodels/core/model.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/model_parser.py` & `astromodels-2.4.2.dev1/astromodels/core/model_parser.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/my_yaml.py` & `astromodels-2.4.2.dev1/astromodels/core/my_yaml.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/node_type.py` & `astromodels-2.4.2.dev1/astromodels/core/node_type.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/parameter.py` & `astromodels-2.4.2.dev1/astromodels/core/parameter.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/parameter_transformation.py` & `astromodels-2.4.2.dev1/astromodels/core/parameter_transformation.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/polarization.py` & `astromodels-2.4.2.dev1/astromodels/core/polarization.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/property.py` & `astromodels-2.4.2.dev1/astromodels/core/property.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/serialization.py` & `astromodels-2.4.2.dev1/astromodels/core/serialization.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/sky_direction.py` & `astromodels-2.4.2.dev1/astromodels/core/sky_direction.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/spectral_component.py` & `astromodels-2.4.2.dev1/astromodels/core/spectral_component.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/thread_safe_unit_format.py` & `astromodels-2.4.2.dev1/astromodels/core/thread_safe_unit_format.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/tree.py` & `astromodels-2.4.2.dev1/astromodels/core/tree.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/core/units.py` & `astromodels-2.4.2.dev1/astromodels/core/units.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/dark_matter/dmSpecTab.npy` & `astromodels-2.4.2.dev1/astromodels/data/dark_matter/dmSpecTab.npy`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/dark_matter/gammamc_dif.dat` & `astromodels-2.4.2.dev1/astromodels/data/dark_matter/gammamc_dif.dat`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/log_theme.ini` & `astromodels-2.4.2.dev1/astromodels/data/log_theme.ini`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/past_1D_values.h5` & `astromodels-2.4.2.dev1/astromodels/data/past_1D_values.h5`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/tests/black_hole.yaml` & `astromodels-2.4.2.dev1/astromodels/data/tests/black_hole.yaml`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/tests/old_table.h5` & `astromodels-2.4.2.dev1/astromodels/data/tests/old_table.h5`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/tests/simple_source.yaml` & `astromodels-2.4.2.dev1/astromodels/data/tests/simple_source.yaml`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/tests/test.yaml` & `astromodels-2.4.2.dev1/astromodels/data/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/tests/test_xspec_table_model.fits` & `astromodels-2.4.2.dev1/astromodels/data/tests/test_xspec_table_model.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_phabs_angr.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_phabs_angr.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_phabs_aspl.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_phabs_aspl.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_angr.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_angr.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_aspl.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_aspl.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_tbabs_wilm.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_tbabs_wilm.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/data/xsect/xsect_wabs_angr.fits` & `astromodels-2.4.2.dev1/astromodels/data/xsect/xsect_wabs_angr.fits`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/__init__.py` & `astromodels-2.4.2.dev1/astromodels/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/dark_matter/dm_models.py` & `astromodels-2.4.2.dev1/astromodels/functions/dark_matter/dm_models.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/function.py` & `astromodels-2.4.2.dev1/astromodels/functions/function.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/__init__.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/__init__.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/absorption.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/absorption.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/apec.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/apec.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/blackbody.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/blackbody.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/extinction.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/extinction.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/functions.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/functions.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/polynomials.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/polynomials.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_1D/powerlaws.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_1D/powerlaws.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_2D.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_2D.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/functions_3D.py` & `astromodels-2.4.2.dev1/astromodels/functions/functions_3D.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/numba_functions.py` & `astromodels-2.4.2.dev1/astromodels/functions/numba_functions.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/priors.py` & `astromodels-2.4.2.dev1/astromodels/functions/priors.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/functions/template_model.py` & `astromodels-2.4.2.dev1/astromodels/functions/template_model.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/sources/extended_source.py` & `astromodels-2.4.2.dev1/astromodels/sources/extended_source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/sources/particle_source.py` & `astromodels-2.4.2.dev1/astromodels/sources/particle_source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/sources/point_source.py` & `astromodels-2.4.2.dev1/astromodels/sources/point_source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/sources/source.py` & `astromodels-2.4.2.dev1/astromodels/sources/source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_1D_function_values.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_1D_function_values.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_extended_source.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_extended_source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_functions.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_load_xspec_models.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_load_xspec_models.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_model.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_parameter.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_point_source.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_point_source.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_polarization.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_polarization.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_template_model.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_template_model.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/tests/test_tree.py` & `astromodels-2.4.2.dev1/astromodels/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/angular_distance.py` & `astromodels-2.4.2.dev1/astromodels/utils/angular_distance.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/config_structure.py` & `astromodels-2.4.2.dev1/astromodels/utils/config_structure.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/configuration.py` & `astromodels-2.4.2.dev1/astromodels/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/data_files.py` & `astromodels-2.4.2.dev1/astromodels/utils/data_files.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/disk_usage.py` & `astromodels-2.4.2.dev1/astromodels/utils/disk_usage.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/file_utils.py` & `astromodels-2.4.2.dev1/astromodels/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/io.py` & `astromodels-2.4.2.dev1/astromodels/utils/io.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/logging.py` & `astromodels-2.4.2.dev1/astromodels/utils/logging.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/long_path_formatter.py` & `astromodels-2.4.2.dev1/astromodels/utils/long_path_formatter.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/pretty_list.py` & `astromodels-2.4.2.dev1/astromodels/utils/pretty_list.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/table.py` & `astromodels-2.4.2.dev1/astromodels/utils/table.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/utils/vincenty.py` & `astromodels-2.4.2.dev1/astromodels/utils/vincenty.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/LICENSE` & `astromodels-2.4.2.dev1/astromodels/xspec/LICENSE`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/factory.py` & `astromodels-2.4.2.dev1/astromodels/xspec/factory.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/array.hh` & `astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/array.hh`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/astro/xspec_extension.hh` & `astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/astro/xspec_extension.hh`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/constants.hh` & `astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/constants.hh`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/extension.hh` & `astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/extension.hh`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/include/sherpa/fcmp.hh` & `astromodels-2.4.2.dev1/astromodels/xspec/include/sherpa/fcmp.hh`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/src/_xspec.cc` & `astromodels-2.4.2.dev1/astromodels/xspec/src/_xspec.cc`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels/xspec/xspec_settings.py` & `astromodels-2.4.2.dev1/astromodels/xspec/xspec_settings.py`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/astromodels.egg-info/PKG-INFO` & `astromodels-2.4.2.dev1/astromodels.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: astromodels
-Version: 2.4.1.dev2
+Version: 2.4.2.dev1
 Summary: Astromodels contains models to be used in likelihood or Bayesian analysis in astronomy
 Home-page: https://github.com/threeml/astromodels
 Download-URL: https://github.com/threeml/astromodels/archive/v0.1
 Author: Giacomo Vianello
 Author-email: giacomo.vianello@gmail.com
 Project-URL: Documentation, https://astromodels.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/threeML/astromodels/issues
 Project-URL: Source Code, https://github.com/threeML/astromodels
 Keywords: Likelihood,Models,fit
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Environment :: Console
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.6
 Requires-Dist: PyYAML>=5.1
 Requires-Dist: scipy>=0.14
 Requires-Dist: astropy>=1.2
 Requires-Dist: dill
 Requires-Dist: future
 Requires-Dist: interpolation>=2.2.3
-Requires-Dist: numba>0.52
+Requires-Dist: numba
 Requires-Dist: h5py
 Requires-Dist: pandas
 Requires-Dist: tables
 Requires-Dist: colorama
 Requires-Dist: omegaconf
 Requires-Dist: rich
 Requires-Dist: joblib
```

### Comparing `astromodels-2.4.1.dev2/astromodels.egg-info/SOURCES.txt` & `astromodels-2.4.2.dev1/astromodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astromodels-2.4.1.dev2/setup.cfg` & `astromodels-2.4.2.dev1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,38 @@
 name = astromodels
 description = Astromodels contains models to be used in likelihood or Bayesian analysis in astronomy
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/threeml/astromodels
 author_email = giacomo.vianello@gmail.com
 author = Giacomo Vianello
-requires_python = >=3.7.0
+requires_python = >=3.9.0
 project_urls = 
 	Documentation = https://astromodels.readthedocs.io
 	Bug Tracker = https://github.com/threeML/astromodels/issues
 	Source Code = https://github.com/threeML/astromodels
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Topic :: Scientific/Engineering :: Astronomy
 	Intended Audience :: Science/Research
 	Operating System :: POSIX
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Environment :: Console
 
 [options]
 include_package_data = True
 install_requires = 
 	numpy>=1.6
 	PyYAML>=5.1
 	scipy>=0.14
 	astropy>=1.2
 	dill
 	future
 	interpolation>=2.2.3
-	numba>0.52
+	numba
 	h5py
 	pandas
 	tables
 	colorama
 	omegaconf
 	rich
 	joblib
```

### Comparing `astromodels-2.4.1.dev2/setup.py` & `astromodels-2.4.2.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,18 +188,24 @@
             return sanitize_lib_name(library_name), library_dir
 
 
 
 
 def setup_xspec():
 
+    skip_xspec = os.environ.get("SKIP_XSPEC")
     headas_root = os.environ.get("HEADAS")
     conda_prefix = os.environ.get("CONDA_PREFIX")
     xspec_version = os.environ.get("ASTRO_XSPEC_VERSION")
 
+    if skip_xspec is not None:
+
+        print("The SKIP_XSPEC env variable was set. Xspec support will not be installed.")
+        return None
+
     # thanks to the sherpa team for this
     
     if xspec_version is None:
 
         print("WARN: You have not specified and XSPEC version with the ")
         print("WARN: environment variable ASTRO_XSPEC_VERSION")
         print(f"WARN: we will assume you have {_default_xspec_version}")
```

### Comparing `astromodels-2.4.1.dev2/versioneer.py` & `astromodels-2.4.2.dev1/versioneer.py`

 * *Files identical despite different names*
