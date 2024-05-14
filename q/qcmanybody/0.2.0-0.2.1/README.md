# Comparing `tmp/qcmanybody-0.2.0.tar.gz` & `tmp/qcmanybody-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcmanybody-0.2.0.tar", last modified: Mon May 13 18:07:04 2024, max compression
+gzip compressed data, was "qcmanybody-0.2.1.tar", last modified: Tue May 14 21:39:50 2024, max compression
```

## Comparing `qcmanybody-0.2.0.tar` & `qcmanybody-0.2.1.tar`

### file list

```diff
@@ -1,114 +1,110 @@
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.058955 qcmanybody-0.2.0/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.030955 qcmanybody-0.2.0/.github/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.035955 qcmanybody-0.2.0/.github/workflows/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5302 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/.github/workflows/ci.yml
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3113 2024-04-27 06:11:03.000000 qcmanybody-0.2.0/.gitignore
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.035955 qcmanybody-0.2.0/.vscode/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       56 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/.vscode/settings.json
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1546 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/LICENSE
--rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-13 18:07:04.057955 qcmanybody-0.2.0/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1688 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/README.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      445 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/codecov.yml
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.039955 qcmanybody-0.2.0/docs/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       35 2024-03-28 22:10:11.000000 qcmanybody-0.2.0/docs/api.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2150 2024-05-13 18:03:09.000000 qcmanybody-0.2.0/docs/changelog.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4341 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/core-interface.md
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.031955 qcmanybody-0.2.0/docs/extensions/
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.040955 qcmanybody-0.2.0/docs/extensions/mdantic_v1/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      241 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/extensions/mdantic_v1/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5334 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/extensions/mdantic_v1/mdantic.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       25 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/docs/high-level-interface.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-03-17 22:44:27.000000 qcmanybody-0.2.0/docs/how-to-guides.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1737 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/index.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4583 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/keywords.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    19797 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/docs/logo.png
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2573 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/docs/qcschema.md
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      304 2024-04-27 06:14:49.000000 qcmanybody-0.2.0/docs/results.md
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.040955 qcmanybody-0.2.0/docs/stylesheets/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      133 2024-03-28 22:10:11.000000 qcmanybody-0.2.0/docs/stylesheets/extra.css
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1877 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/mkdocs.yml
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1505 2024-04-27 06:14:44.000000 qcmanybody-0.2.0/pyproject.toml
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.041955 qcmanybody-0.2.0/qcmanybody/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      218 2024-05-03 01:04:53.000000 qcmanybody-0.2.0/qcmanybody/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7273 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/builder.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.043955 qcmanybody-0.2.0/qcmanybody/hide/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5871 2024-04-24 14:42:51.000000 qcmanybody-0.2.0/qcmanybody/hide/asdf.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1158 2024-04-16 23:10:20.000000 qcmanybody-0.2.0/qcmanybody/hide/hold_test_mbe_keywords.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      658 2024-03-15 16:39:58.000000 qcmanybody-0.2.0/qcmanybody/hide/tsts.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25486 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/manybody.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.044955 qcmanybody-0.2.0/qcmanybody/models/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      266 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/qcmanybody/models/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1330 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/generalized_optimization.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11042 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/manybody_input_pydv1.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15581 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/models/manybody_output_pydv1.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26556 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/qcng_computer.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.048955 qcmanybody-0.2.0/qcmanybody/tests/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/__init__.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2111 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/addons.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3511 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/common.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.051955 qcmanybody-0.2.0/qcmanybody/tests/component_data/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      561 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      386 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7612 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4480 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)   112168 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    61149 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      480 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      176 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5776 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1139 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    77120 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9708 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      335 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      316 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_energy_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4448 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4142 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    65348 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    59491 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3936 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/generate_component_data.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.056955 qcmanybody-0.2.0/qcmanybody/tests/ref_data/
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      925 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      863 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    30651 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      908 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      729 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    22108 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      931 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      914 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      940 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      540 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26095 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      921 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      499 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9825 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      946 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      924 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      858 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6579 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18555 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      871 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5520 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    17643 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      856 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    86478 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    76866 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      869 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    69847 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    71086 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    45626 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_multilevel.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    39159 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_singlelevel.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15035 2024-04-27 18:05:01.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_het4_grad.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    12835 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/tests/test_mbe_keywords.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1425 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_multi.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1577 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_multi_ss.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1412 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_single.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11514 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/test_utils.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7774 2024-04-24 19:42:44.000000 qcmanybody-0.2.0/qcmanybody/tests/utils.py
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15683 2024-05-13 18:03:00.000000 qcmanybody-0.2.0/qcmanybody/utils.py
-drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-13 18:07:04.056955 qcmanybody-0.2.0/qcmanybody.egg-info/
--rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/PKG-INFO
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4352 2024-05-13 18:07:04.000000 qcmanybody-0.2.0/qcmanybody.egg-info/SOURCES.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/dependency_links.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      108 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/requires.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       11 2024-05-13 18:07:03.000000 qcmanybody-0.2.0/qcmanybody.egg-info/top_level.txt
--rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       38 2024-05-13 18:07:04.058955 qcmanybody-0.2.0/setup.cfg
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.696650 qcmanybody-0.2.1/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.675650 qcmanybody-0.2.1/.github/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.678650 qcmanybody-0.2.1/.github/workflows/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5302 2024-05-13 18:03:00.000000 qcmanybody-0.2.1/.github/workflows/ci.yml
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3113 2024-04-27 06:11:03.000000 qcmanybody-0.2.1/.gitignore
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.678650 qcmanybody-0.2.1/.vscode/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       56 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/.vscode/settings.json
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1546 2024-04-27 06:14:44.000000 qcmanybody-0.2.1/LICENSE
+-rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-14 21:39:50.695650 qcmanybody-0.2.1/PKG-INFO
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1688 2024-05-13 18:03:00.000000 qcmanybody-0.2.1/README.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      445 2024-04-27 06:14:44.000000 qcmanybody-0.2.1/codecov.yml
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.680650 qcmanybody-0.2.1/docs/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      234 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/docs/api.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2409 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/docs/changelog.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4341 2024-04-27 06:14:49.000000 qcmanybody-0.2.1/docs/core-interface.md
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.676650 qcmanybody-0.2.1/docs/extensions/
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.680650 qcmanybody-0.2.1/docs/extensions/mdantic_v1/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      241 2024-04-27 06:14:44.000000 qcmanybody-0.2.1/docs/extensions/mdantic_v1/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5406 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/docs/extensions/mdantic_v1/mdantic.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       25 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/docs/high-level-interface.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-03-17 22:44:27.000000 qcmanybody-0.2.1/docs/how-to-guides.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1970 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/docs/index.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4583 2024-04-27 06:14:49.000000 qcmanybody-0.2.1/docs/keywords.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    19797 2024-04-27 06:14:44.000000 qcmanybody-0.2.1/docs/logo.png
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2599 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/docs/qcschema.md
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      304 2024-04-27 06:14:49.000000 qcmanybody-0.2.1/docs/results.md
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.681650 qcmanybody-0.2.1/docs/stylesheets/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      133 2024-03-28 22:10:11.000000 qcmanybody-0.2.1/docs/stylesheets/extra.css
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1943 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/mkdocs.yml
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1505 2024-04-27 06:14:44.000000 qcmanybody-0.2.1/pyproject.toml
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.681650 qcmanybody-0.2.1/qcmanybody/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      218 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7273 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/builder.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26576 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/computer.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    25486 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/manybody.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.683650 qcmanybody-0.2.1/qcmanybody/models/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      266 2024-04-27 18:05:01.000000 qcmanybody-0.2.1/qcmanybody/models/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1330 2024-05-13 18:03:00.000000 qcmanybody-0.2.1/qcmanybody/models/generalized_optimization.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11069 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/models/manybody_input_pydv1.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15581 2024-05-13 18:03:00.000000 qcmanybody-0.2.1/qcmanybody/models/manybody_output_pydv1.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.685650 qcmanybody-0.2.1/qcmanybody/tests/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/__init__.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     2111 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/addons.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3511 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/common.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.689650 qcmanybody-0.2.1/qcmanybody/tests/component_data/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      561 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      386 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7612 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4480 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)   112168 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    61149 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      480 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      176 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5776 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1139 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    77120 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9708 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      335 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_energy_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      316 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_energy_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4448 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4142 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    65348 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    59491 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     3936 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/generate_component_data.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.694650 qcmanybody-0.2.1/qcmanybody/tests/ref_data/
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      925 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      863 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    30651 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      908 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      729 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    22108 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      931 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      914 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      940 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      540 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    26095 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      921 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      499 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     9825 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      946 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      924 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      858 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     6579 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    18555 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      871 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     5520 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    17643 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      856 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    86478 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    76866 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      869 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    69847 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    71086 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    45581 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/tests/test_mbe_he4_multilevel.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    39118 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/tests/test_mbe_he4_singlelevel.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15022 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/tests/test_mbe_het4_grad.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    12769 2024-05-14 21:27:38.000000 qcmanybody-0.2.1/qcmanybody/tests/test_mbe_keywords.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1425 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/test_multi.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1577 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/test_multi_ss.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     1412 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/test_single.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    11514 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/test_utils.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     7774 2024-04-24 19:42:44.000000 qcmanybody-0.2.1/qcmanybody/tests/utils.py
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)    15683 2024-05-13 18:03:00.000000 qcmanybody-0.2.1/qcmanybody/utils.py
+drwxrwxr-x   0 psilocaluser  (1000) psilocaluser  (1000)        0 2024-05-14 21:39:50.694650 qcmanybody-0.2.1/qcmanybody.egg-info/
+-rw-r--r--   0 psilocaluser  (1000) psilocaluser  (1000)     4394 2024-05-14 21:39:50.000000 qcmanybody-0.2.1/qcmanybody.egg-info/PKG-INFO
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)     4257 2024-05-14 21:39:50.000000 qcmanybody-0.2.1/qcmanybody.egg-info/SOURCES.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)        1 2024-05-14 21:39:50.000000 qcmanybody-0.2.1/qcmanybody.egg-info/dependency_links.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)      108 2024-05-14 21:39:50.000000 qcmanybody-0.2.1/qcmanybody.egg-info/requires.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       11 2024-05-14 21:39:50.000000 qcmanybody-0.2.1/qcmanybody.egg-info/top_level.txt
+-rw-rw-r--   0 psilocaluser  (1000) psilocaluser  (1000)       38 2024-05-14 21:39:50.696650 qcmanybody-0.2.1/setup.cfg
```

### Comparing `qcmanybody-0.2.0/.github/workflows/ci.yml` & `qcmanybody-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/.gitignore` & `qcmanybody-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/LICENSE` & `qcmanybody-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/PKG-INFO` & `qcmanybody-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcmanybody
-Version: 0.2.0
+Version: 0.2.1
 Summary: QCManyBody
 Author-email: Benjamin Pritchard <bpp4@vt.edu>, "Lori A. Burns" <lori.burns@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, The Molecular Sciences Software Institute
         All rights reserved.
```

### Comparing `qcmanybody-0.2.0/README.md` & `qcmanybody-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/docs/changelog.md` & `qcmanybody-0.2.1/docs/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 
 #### MUST (Unmerged)
 
 #### WIP (Unmerged)
 -->
 
 
+## v0.2.1 / 2024-05-14
+
+#### Enhancements
+
+* [\#27](https://github.com/MolSSI/QCManyBody/pull/27) Intf -- move high-level interface from
+  `qcmb.qcng_computer.ManyBodyComputerQCNG` to `qcmb.computer.ManyBodyComputer`. Suppressed remaining printing. @loriab
+
+
 ## v0.2.0 / 2024-05-13
 
 #### New Features
 
 * [\#25](https://github.com/MolSSI/QCManyBody/pull/25) Schema -- added a new field `ManyBodyResults.component_results`
   to store subsystem `AtomicResult`s (or other Result if layered computation). By default this is not stored, but it can
   be with `ManyBodyInput.protocols.component_results = "all"`. @loriab
```

### Comparing `qcmanybody-0.2.0/docs/core-interface.md` & `qcmanybody-0.2.1/docs/core-interface.md`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/docs/extensions/mdantic_v1/mdantic.py` & `qcmanybody-0.2.1/docs/extensions/mdantic_v1/mdantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 import inspect
 import importlib
 from enum import Enum
 from collections import namedtuple
 from typing import List, Dict, Optional
 
 import tabulate
-from pydantic.v1 import BaseModel
+try:
+    from pydantic.v1 import BaseModel
+except ModuleNotFoundError:
+    from pydantic import BaseModel
 from markdown import Markdown
 from markdown.extensions import Extension
 from markdown.preprocessors import Preprocessor
 
 
 class Mdantic(Extension):
     def __init__(self, configs=None):
```

### Comparing `qcmanybody-0.2.0/docs/index.md` & `qcmanybody-0.2.1/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -40,8 +40,19 @@
 
 ## Table of Contents
 
 1. [Common Keywords and Options](keywords.md)
 2. [High-level Interface](high-level-interface.md)
 3. [Core Interface](core-interface.md)
 4. [Results](results.md)
-5. [How-To Guides](how-to-guides.md)
+5. [How-To Guides](how-to-guides.md)
+
+<!--
+
+PYTHONPATH=docs/extensions:. mkdocs serve
+
+python -m sphinx.ext.intersphinx 'https://molssi.github.io/QCManyBody/objects.inv'
+python -m sphinx.ext.intersphinx 'http://127.0.0.1:8000/QCManyBody/objects.inv'
+
+mkdocs build
+
+-->
```

### Comparing `qcmanybody-0.2.0/docs/keywords.md` & `qcmanybody-0.2.1/docs/keywords.md`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/docs/logo.png` & `qcmanybody-0.2.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/docs/qcschema.md` & `qcmanybody-0.2.1/docs/qcschema.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 <!-- ====  Inputs  ================================================================= -->
 
 ::: qcmanybody.models.BsseEnum
     options:
         show_root_heading: true
+        show_source: true
 
 
 ::: qcmanybody.models.ManyBodyKeywords
     options:
         show_root_heading: true
 
 $pydantic: qcmanybody.models.manybody_input_pydv1.ManyBodyKeywords
```

### Comparing `qcmanybody-0.2.0/mkdocs.yml` & `qcmanybody-0.2.1/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -30,30 +30,33 @@
       name: "Switch to light mode"
 
 extra_css:
   - stylesheets/extra.css
 
 plugins:
 - search
+- autorefs
 - mkdocstrings:
     default_handler: python
+    enable_inventory: true
     handlers:
       python:
         paths: [.]
         options:
           docstring_style: numpy
           allow_inspection: true
           members_order: source
           separate_signature: true
           filters: ["!^_"]
           docstring_options:
             ignore_init_summary: true
           merge_init_into_class: true
           show_signature_annotations: true
           signature_crossrefs: true
+          show_source: true
         import:
           - https://docs.python.org/3/objects.inv
           - https://numpy.org/doc/stable/objects.inv
           - https://docs.scipy.org/doc/scipy/objects.inv
           - https://matplotlib.org/stable/objects.inv
           - https://molssi.github.io/QCElemental/objects.inv
           - https://molssi.github.io/QCEngine/objects.inv
```

### Comparing `qcmanybody-0.2.0/pyproject.toml` & `qcmanybody-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/builder.py` & `qcmanybody-0.2.1/qcmanybody/builder.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/manybody.py` & `qcmanybody-0.2.1/qcmanybody/manybody.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/models/generalized_optimization.py` & `qcmanybody-0.2.1/qcmanybody/models/generalized_optimization.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/models/manybody_input_pydv1.py` & `qcmanybody-0.2.1/qcmanybody/models/manybody_input_pydv1.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,22 +167,22 @@
     )
     supersystem_ie_only: Optional[bool] = Field(
         False,
         validate_default=True,
         # definitive description
         description="Target the supersystem total/interaction energy (IE) data over the many-body expansion (MBE) "
             "analysis, thereby omitting intermediate-body calculations. When False (default), compute each n-body level "
-            "in the MBE up through ``max_nbody``. When True (only allowed for ``max_nbody = nfragments``), only compute "
+            "in the MBE up through ``max_nbody``. When True (only allowed for ``max_nbody = nfragments`` ), only compute "
             "enough for the overall interaction/total energy: max_nbody-body and 1-body. When True, properties "
-            "``INTERACTION {driver} THROUGH {max_nbody}-BODY`` will always be available; ``TOTAL {driver} THROUGH "
-            "{max_nbody}-BODY`` will be available depending on ``return_total_data``; and ``{max_nbody}-BODY "
-            "CONTRIBUTION TO {driver}`` won't be available (except for dimers). This keyword produces no savings for a "
-            "two-fragment molecule. But for the interaction energy of a three-fragment molecule, for example, 2-body "
-            "subsystems can be skipped with ``supersystem_ie_only=True`` Do not use with ``vmfc`` in ``bsse_type``"
-            "as it cannot produce savings."
+            "``INTERACTION {driver} THROUGH {max_nbody}-BODY`` will always be available; "
+            "``TOTAL {driver} THROUGH {max_nbody}-BODY`` will be available depending on ``return_total_data`` ; and "
+            "``{max_nbody}-BODY CONTRIBUTION TO {driver}`` won't be available (except for dimers). This keyword produces "
+            "no savings for a two-fragment molecule. But for the interaction energy of a three-fragment molecule, for "
+            "example, 2-body subsystems can be skipped with ``supersystem_ie_only=True``. Do not use with ``vmfc`` in "
+            "``bsse_type`` as it cannot produce savings.",
     )
 
     # v2: @field_validator("bsse_type", mode="before")
     @validator("bsse_type", pre=True)
     @classmethod
     def set_bsse_type(cls, v: Any) -> List[BsseEnum]:
         if not isinstance(v, list):
@@ -197,15 +197,15 @@
 
 class ManyBodySpecification(ProtoModel):
     """Combining the what (ManyBodyKeywords) with the how (AtomicSpecification)."""
 
     schema_name: Literal["qcschema_manybodyspecification"] = "qcschema_manybodyspecification"
     #provenance: Provenance = Field(Provenance(**provenance_stamp(__name__)), description=Provenance.__doc__)
     keywords: ManyBodyKeywords = Field(..., description=ManyBodyKeywords.__doc__)
-    #program: str = Field(..., description="The program for which the Specification is intended.")
+    #program: str = Field(..., description="The program for which the Specification is intended.")  # TODO is qcmanybody
     protocols: ManyBodyProtocols = Field(ManyBodyProtocols(), description=str(ManyBodyProtocols.__doc__))
     driver: DriverEnum = Field(
         ...,
         description="The computation driver; i.e., energy, gradient, hessian.",
     )
     #specification: Union[AtomicSpecification, Dict[str, AtomicSpecification]] = Field(
     specification: Dict[str, AtomicSpecification] = Field(
```

### Comparing `qcmanybody-0.2.0/qcmanybody/models/manybody_output_pydv1.py` & `qcmanybody-0.2.1/qcmanybody/models/manybody_output_pydv1.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/qcng_computer.py` & `qcmanybody-0.2.1/qcmanybody/computer.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     # v2: )
     class Config:
         extra = "allow"
         # v2: frozen = False
         allow_mutation = True
 
 
-class AtomicComputerQCNG(BaseComputerQCNG):
+class AtomicComputer(BaseComputerQCNG):
     """Computer for analytic single-geometry computations."""
 
     molecule: Molecule = Field(..., description="The molecule to use in the computation.")
     basis: str = Field(..., description="The quantum chemistry basis set to evaluate (e.g., 6-31g, cc-pVDZ, ...).")
     method: str = Field(..., description="The quantum chemistry method to evaluate (e.g., B3LYP, MP2, ...).")
     driver: DriverEnum = Field(..., description="The resulting type of computation: energy, gradient, hessian, properties."
         "Note for finite difference that this should be the target driver, not the means driver.")
@@ -126,15 +126,15 @@
 
         NOTE: client removed (compared to psi4.driver.AtomicComputer)
         """
         if self.result:
             return self.result
 
 
-class ManyBodyComputerQCNG(BaseComputerQCNG):
+class ManyBodyComputer(BaseComputerQCNG):
 
     input_data: ManyBodyInput = Field(
         ...,
         description="Input schema containing the relevant settings for performing the many body "
             "expansion. This is entirely redundant with the piecemeal assembly of this Computer class "
             "and is only stored to be available for error handling and exact reconstruction of ManyBodyResult.",
     )
@@ -217,63 +217,63 @@
         return list(dict.fromkeys([(BsseEnum[bt.lower()].value if bt.lower() in BsseEnum.__members__ else bt.lower()) for bt in v]))
 
     # v2: @field_validator("embedding_charges")
     @validator("embedding_charges", pre=True)
     @classmethod
     # v2: def set_embedding_charges(cls, v: Any, info: FieldValidationInfo) -> Dict[int, List[float]]:
     def set_embedding_charges(cls, v, values): # -> Dict[int, List[float]]:
-        print(f"hit embedding_charges validator with {v}", end="")
+        # print(f"hit embedding_charges validator with {v}", end="")
         nfr = len(values["molecule"].fragments)
         # v2: if len(v) != info.data["nfragments"]:
         if v and len(v) != nfr:
             raise ValueError(f"embedding_charges dict should have entries for each 1-indexed fragment ({nfr})")
 
-        print(f" ... setting embedding_charges={v}")
+        # print(f" ... setting embedding_charges={v}")
         return v
 
     # v2: @field_validator("return_total_data")
     @validator("return_total_data", always=True)
     @classmethod
     # v2: def set_return_total_data(cls, v: Optional[bool], info: FieldValidationInfo) -> bool:
     def set_return_total_data(cls, v: Optional[bool], values) -> bool:
-        print(f"hit return_total_data validator with {v}", end="")
+        # print(f"hit return_total_data validator with {v}", end="")
         if v is not None:
             rtd = v
         # v2: elif info.data["driver"] in ["gradient", "hessian"]:
         elif values["driver"] in ["gradient", "hessian"]:
             rtd = True
         else:
             rtd = False
 
         # v2: if info.data.get("embedding_charges", False) and rtd is False:
         if values.get("embedding_charges", False) and rtd is False:
             raise ValueError("Cannot return interaction data when using embedding scheme.")
 
-        print(f" ... setting rtd={rtd}")
+        # print(f" ... setting rtd={rtd}")
         return rtd
 
     # v2: @field_validator("levels")
     @validator("levels", always=True)
     @classmethod
     # v2: def set_levels(cls, v: Any, info: FieldValidationInfo) -> Dict[Union[int, Literal["supersystem"]], str]:
     def set_levels(cls, v: Any, values) -> Dict[Union[int, Literal["supersystem"]], str]:
-        print(f"hit levels validator with {v}", end="")
+        # print(f"hit levels validator with {v}", end="")
 
         if v is None:
             pass
             # TODO levels = {plan.max_nbody: method}
             #v = {info.data["nfragments"]: "???method???"}
             #v = {len(info.data["molecule"].fragments): "???method???"}
             # v2: v = {len(info.data["molecule"].fragments): "(auto)"}
             v = {len(values["molecule"].fragments): "(auto)"}
         else:
             # rearrange bodies in order with supersystem last lest body count fail in organization loop below
             v = dict(sorted(v.items(), key=lambda item: 1000 if item[0] == "supersystem" else item[0]))
 
-        print(f" ... setting levels={v}")
+        # print(f" ... setting levels={v}")
         return v
 
     # TODO @computed_field(
     # TODO     description="Distribution of active n-body levels among model chemistry levels. All bodies in range "
     # TODO         "[1, self.max_nbody] must be present exactly once. Number of items in outer list is how many different "
     # TODO         "modelchems. Each inner list specifies what n-bodies to be run at the corresponding modelchem (e.g., "
     # TODO         "`[[1, 2]]` has max_nbody=2 and 1-body and 2-body contributions computed at the same level of theory; "
@@ -281,15 +281,15 @@
     # TODO         "An entry 'supersystem' means all higher order n-body effects up to the number of fragments. The n-body "
     # TODO         "levels are effectively sorted in the outer list, and any 'supersystem' element is at the end.")
         #json_schema_extra={
         #    "shape": ["nmc", "<varies>"],
         #},
     @property
     def nbodies_per_mc_level(self) -> List[List[Union[int, Literal["supersystem"]]]]:
-        print(f"hit nbodies_per_mc_level", end="")
+        # print(f"hit nbodies_per_mc_level", end="")
 
         # Organize nbody calculations into modelchem levels
         # * expand keys of `levels` into full lists of nbodies covered. save to plan, resetting max_nbody accordingly
         # * below, process values of `levels`, which are modelchem strings, into kwargs specs
         nbodies_per_mc_level = []
         prev_body = 0
         for nb in self.levels:
@@ -300,28 +300,28 @@
                 for m in range(prev_body + 1, nb + 1):
                     nbodies.append(m)
             else:
                 nbodies.append(nb)
             nbodies_per_mc_level.append(nbodies)
             prev_body = nb  # formerly buggy `+= 1`
 
-        print(f" ... setting nbodies_per_mc_level={nbodies_per_mc_level}")
+        # print(f" ... setting nbodies_per_mc_level={nbodies_per_mc_level}")
         return nbodies_per_mc_level
 
     # v2: @field_validator("max_nbody")
     @validator("max_nbody", always=True)
     @classmethod
     # v2: def set_max_nbody(cls, v: Any, info: FieldValidationInfo) -> int:
     def set_max_nbody(cls, v: Any, values) -> int:
-        print(f"hit max_nbody validator with {v}", end="")
+        # print(f"hit max_nbody validator with {v}", end="")
         # v2: levels_max_nbody = max(nb for nb in info.data["levels"] if nb != "supersystem")
         # v2: nfr = len(info.data["molecule"].fragments)
         levels_max_nbody = max(nb for nb in values["levels"] if nb != "supersystem")
         nfr = len(values["molecule"].fragments)
-        print(f" {levels_max_nbody=} {nfr=}", end="")
+        # print(f" {levels_max_nbody=} {nfr=}", end="")
 
         #ALT if v == -1:
         if v is None:
             v = levels_max_nbody
         elif v < 0 or v > nfr:
             raise ValueError(f"max_nbody={v} should be between 1 and {nfr}.")
         elif v != levels_max_nbody:
@@ -329,15 +329,15 @@
             # TODO reconsider logic. move this from levels to here?
             # v2: info.data["levels"] = {v: "(auto)"}
             values["levels"] = {v: "(auto)"}
         else:
             pass
             # TODO once was           return min(v, nfragments)
 
-        print(f" ... setting max_nbody={v}")
+        # print(f" ... setting max_nbody={v}")
         return v
 
 #       levels          max_nbody           F-levels        F-max_nbody     result
 #
 #       {stuff}         None                {stuff}         set from stuff  all consistent; max_nbody from levels
 #       None            int                 {int: mtd}      int             all consistent; levels from max_nbody
 #       None            None                {nfr: mtd}      nfr             all consistent; any order
@@ -346,29 +346,29 @@
     # TODO also, perhaps change nbodies_per_mc_level into dict of lists so that pos'n/label indexing coincides
 
     # v2: @field_validator("supersystem_ie_only")
     @validator("supersystem_ie_only", always=True)
     @classmethod
     # v2: def set_supersystem_ie_only(cls, v: Optional[bool], info: FieldValidationInfo) -> bool:
     def set_supersystem_ie_only(cls, v: Optional[bool], values) -> bool:
-        print(f"hit supersystem_ie_only validator with {v}", end="")
+        # print(f"hit supersystem_ie_only validator with {v}", end="")
         sio = v
         # v2: _nfr = len(info.data["molecule"].fragments)
         _nfr = len(values["molecule"].fragments)
 
         # v2: _max_nbody = info.data["max_nbody"]
         # get(..., None) b/c in v1, all fields processed even if max_nbody previously failed
         _max_nbody = values.get("max_nbody", None)
         if (sio is True) and (_max_nbody != _nfr):
             raise ValueError(f"Cannot skip intermediate n-body jobs when max_nbody={_max_nbody} != nfragments={_nfr}.")
 
         if (sio is True) and ("vmfc" in values["bsse_type"]):
             raise ValueError(f"Cannot skip intermediate n-body jobs when VMFC in bsse_type={values['bsse_type']}. Use CP instead.")
 
-        print(f" ... setting {sio=}")
+        # print(f" ... setting {sio=}")
         return sio
 
     @classmethod
     def from_manybodyinput(cls, input_model: ManyBodyInput, build_tasks: bool = True):
 
         computer_model = cls(
             molecule=input_model.molecule,
@@ -428,15 +428,15 @@
                     raise RuntimeError(f"Don't know how to handle external charges in {specifications[chem]['program']}")
 
             _, real, bas = delabeler(label)
             result = qcng.compute(inp, specifications[chem]["program"])
             component_results[label] = result
 
             if not result.success:
-                print(result.error.error_message)
+                # print(result.error.error_message)
                 raise RuntimeError("Calculation did not succeed! Error:\n" + result.error.error_message)
 
             # pull out stuff
             props = {"energy", "gradient", "hessian"}
 
             component_properties[label] = {}
```

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/addons.py` & `qcmanybody-0.2.1/qcmanybody/tests/addons.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/common.py` & `qcmanybody-0.2.1/qcmanybody/tests/common.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_energy_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_multi_ss_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/component_data/h2o_trimer_single_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/generate_component_data.py` & `qcmanybody-0.2.1/qcmanybody/tests/generate_component_data.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_multi_ss_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_gradient_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_1.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.inp`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.json.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst` & `qcmanybody-0.2.1/qcmanybody/tests/ref_data/h2o_trimer_single_hessian_2.out.zst`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_multilevel.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_mbe_he4_multilevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 
 from qcelemental import constants
 from qcelemental.models import Molecule
 # v2: from qcelemental.models.procedures_manybody import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
 from qcelemental.testing import compare_values, compare_recursive
 
 from qcmanybody.models import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
-from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.computer import ManyBodyComputer, qcvars_to_manybodyproperties
 
-import qcengine as qcng
 from .addons import using
 from .test_mbe_he4_singlelevel import sumdict as sumdict_single
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
     return qcvars_to_manybodyproperties[qcvar]
 
@@ -722,15 +721,15 @@
 
     mbe_keywords = ManyBodyKeywords(levels=levels, **mbe_keywords)
     mbe_data_multilevel_631g["molecule"] = he_tetramer
     mbe_data_multilevel_631g["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_multilevel_631g)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = he4_refs_conv_multilevel_631g[pattern]
     ans = refs[anskey]
     ref_nmbe = calcinfo_nmbe[pattern]
     ref_bodykeys = bodykeys[pattern] if pattern in bodykeys else bodykeys
@@ -815,15 +814,15 @@
 
     mbe_keywords = ManyBodyKeywords(levels=levels, **mbe_keywords)
     mbe_data_multilevel_631g["molecule"] = he_tetramer
     mbe_data_multilevel_631g["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_multilevel_631g)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = he4_refs_conv_multilevel_631g[pattern]
     ans = refs[anskey]
     ref_nmbe = calcinfo_nmbe[pattern]
     ref_bodykeys = bodykeys[pattern] if pattern in bodykeys else bodykeys
@@ -892,15 +891,15 @@
        },
        id="3b_vmfc"),
 ])
 def test_count_he4_multi(mbe_keywords, ref_count, he_tetramer, request):
     atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": "mybas"}, program="myqc", driver="energy")
     mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy"}, molecule=he_tetramer)
 
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model, build_tasks=False)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model, build_tasks=False)
     ret = ret.qcmb_calculator
 
     text, dcount = ret.format_calc_plan()
     assert compare_recursive(ref_count["all"], dcount, atol=1.e-6)
     for sset in ["all", "cp", "nocp", "vmfc_compute"]:
         text, dcount = ret.format_calc_plan(sset)
         assert compare_recursive(ref_count[sset], dcount, atol=1.e-6)
```

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_he4_singlelevel.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_mbe_he4_singlelevel.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 
 from qcelemental import constants
 from qcelemental.models import Molecule
 # v2: from qcelemental.models.procedures_manybody import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
 from qcelemental.testing import compare_values, compare_recursive
 
 from qcmanybody.models import AtomicSpecification, ManyBodyKeywords, ManyBodyInput
-from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.computer import ManyBodyComputer, qcvars_to_manybodyproperties
 
-import qcengine as qcng
 from .addons import using
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
     return qcvars_to_manybodyproperties[qcvar]
 
 
@@ -621,15 +620,15 @@
     #   addressing 4-body formulas
     # e, wfn = energy('MP2/aug-cc-pVDZ', molecule=he_tetramer, ...)
 
     atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": basis}, program=program, driver="energy", keywords=keywords, protocols={"stdout": False})
     mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy", "protocols": {"component_results": "all"}}, molecule=he_tetramer)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model)
     print(f"SSSSSSS {request.node.name}")
     # v2: pprint.pprint(ret.model_dump(), width=200)
     pprint.pprint(ret.dict(), width=200)
 
     _inner = request.node.name.split("[")[1].split("]")[0]
     kwdsln, progln = _inner.split("-")
     refs = he4_refs_df if progln == "psi4_df" else he4_refs_conv
@@ -708,15 +707,15 @@
         },
         id="3b_vmfc"),
 ])
 def test_count_he4_single(mbe_keywords, ref_count, he_tetramer):
     atomic_spec = AtomicSpecification(model={"method": "mp2", "basis": "mybas"}, program="myqc", driver="energy")
     mbe_model = ManyBodyInput(specification={"specification": atomic_spec, "keywords": mbe_keywords, "driver": "energy"}, molecule=he_tetramer)
 
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model, build_tasks=False)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model, build_tasks=False)
     ret = ret.qcmb_calculator
 
     text, dcount = ret.format_calc_plan()
     assert compare_recursive(ref_count["all"], dcount, atol=1.e-6)
     for sset in ["all", "cp", "nocp", "vmfc_compute"]:
         text, dcount = ret.format_calc_plan(sset)
         assert compare_recursive(ref_count[sset], dcount, atol=1.e-6)
```

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_het4_grad.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_mbe_het4_grad.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import numpy as np
 
 from qcelemental.models import Molecule
 from qcelemental.testing import compare_values
 
 from qcmanybody.models import ManyBodyKeywords, ManyBodyInput
-from qcmanybody.qcng_computer import ManyBodyComputerQCNG, qcvars_to_manybodyproperties
+from qcmanybody.computer import ManyBodyComputer, qcvars_to_manybodyproperties
 
 from .addons import uusing
 
 def skprop(qcvar):
     # qcng: return qcng.procedures.manybody.qcvars_to_manybodyproperties[qcvar]
     return qcvars_to_manybodyproperties[qcvar]
 
@@ -254,15 +254,15 @@
     mbe_keywords = ManyBodyKeywords(**mbe_keywords)
     mbe_data_grad_dtz["molecule"] = het_tetramer
     mbe_data_grad_dtz["specification"]["driver"] = "gradient"
     mbe_data_grad_dtz["specification"]["keywords"] = mbe_keywords
     mbe_model = ManyBodyInput(**mbe_data_grad_dtz)
 
     # qcng: ret = qcng.compute_procedure(mbe_model, "manybody", raise_error=True)
-    ret = ManyBodyComputerQCNG.from_manybodyinput(mbe_model)
+    ret = ManyBodyComputer.from_manybodyinput(mbe_model)
     print(f"MMMMMMM {request.node.name}")
     pprint.pprint(ret.dict(), width=200)
 
     refs = het4_refs_conv_grad_dtz[kwdsln]
     ansE = refs[anskeyE]
     ansG = refs[anskeyG]
     ref_nmbe = calcinfo_nmbe
```

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_mbe_keywords.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_mbe_keywords.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 except ImportError:
     from pydantic import ValidationError
 
 import qcelemental
 from qcelemental.models import DriverEnum, Molecule
 from qcmanybody.models import BsseEnum, ManyBodyInput
 
-import qcengine as qcng
-
-# qcng: from qcengine.procedures.manybody import ManyBodyComputerQCNG
-from qcmanybody.qcng_computer import ManyBodyComputerQCNG
+# qcng: from qcengine.procedures.manybody import ManyBodyComputer
+from qcmanybody.computer import ManyBodyComputer
 from qcmanybody import ManyBodyCalculator
 
 
 @pytest.fixture(scope="function")
 def mbe_data():
     henehh = Molecule(symbols=["He", "Ne", "H", "H"], fragments=[[0], [1], [2, 3]], geometry=[0, 0, 0, 2, 0, 0, 0, 1, 0, 0, -1, 0])
     return {
@@ -99,15 +97,15 @@
     pytest.param("hessian", {"return_total_data": False}, False),
 ])
 def test_mbe_rtd(mbe_data, driver, kws, ans):
     mbe_data["specification"]["driver"] = driver
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+    comp_model = ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.driver == driver
     assert comp_model.return_total_data == ans
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, [3, {3: "(auto)"}, [[1, 2, 3]] ]),
@@ -146,15 +144,15 @@
 
     #pytest.param({}, [ , {}, [] ]),
 ])
 def test_mbe_level_bodies(mbe_data, kws, ans):
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+    comp_model = ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.nfragments == 3
     assert comp_model.max_nbody == ans[0]
     assert list(comp_model.levels.items()) == list(ans[1].items())  # compare as OrderedDict
     assert comp_model.nbodies_per_mc_level == ans[2]
 
 
@@ -174,15 +172,15 @@
 ])
 def test_mbe_level_5mer(mbe_data, kws, ans):
     he3ne2 = Molecule(symbols=["He", "He", "He", "Ne", "Ne"], fragments=[[0], [1], [2], [3], [4]], geometry=[0, 0, 0, 2, 0, 0, -2, 0, 0, 0, 2, 0, 0, -2, 0])
     mbe_data["molecule"] = he3ne2
     mbe_data["specification"]["keywords"] = kws
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+    comp_model = ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.nfragments == 5
     assert comp_model.max_nbody == ans[0]
     assert list(comp_model.levels.items()) == list(ans[1].items())  # compare as OrderedDict
     assert comp_model.nbodies_per_mc_level == ans[2]
 
 
@@ -196,15 +194,15 @@
 ])
 def test_mbe_level_fails(mbe_data, kws, errmsg):
     mbe_data["specification"]["keywords"] = kws
 
     # v2: with pytest.raises(Exception):
     with pytest.raises(ValidationError) as e:
         input_model = ManyBodyInput(**mbe_data)
-        ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+        ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert errmsg in str(e.value), e.value
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, [BsseEnum.cp]),
     pytest.param({"bsse_type": "CP"}, [BsseEnum.cp]),
@@ -226,15 +224,15 @@
         with pytest.raises(ValidationError) as e:
             input_model = ManyBodyInput(**mbe_data)
 
         assert "not a valid enumeration member; permitted: 'nocp', 'cp', 'vmfc'" in str(e.value)
         return
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+    comp_model = ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.bsse_type == ans, f"{comp_model=} != {ans}"
 
 
 @pytest.mark.parametrize("kws,ans", [
     pytest.param({}, False),
     pytest.param({"max_nbody": 3, "supersystem_ie_only": True}, True),
@@ -248,21 +246,21 @@
 ])
 def test_mbe_sie(mbe_data, kws, ans):
     mbe_data["specification"]["keywords"] = kws
 
     if isinstance(ans, str):
         input_model = ManyBodyInput(**mbe_data)
         with pytest.raises(ValidationError) as e:
-            ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+            ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
         assert ans in str(e.value)
         return
 
     input_model = ManyBodyInput(**mbe_data)
-    comp_model = ManyBodyComputerQCNG.from_manybodyinput(input_model, build_tasks=False)
+    comp_model = ManyBodyComputer.from_manybodyinput(input_model, build_tasks=False)
 
     assert comp_model.supersystem_ie_only == ans
 
 
 def test_noncontiguous_fragments_ordinary():
     with pytest.raises(qcelemental.exceptions.ValidationError) as e:
         Molecule(symbols=["H", "Ne", "Cl"], geometry=[0, 0, 0, 2, 0, 0, 0, 2, 0], fragments=[[0, 2], [1]])
```

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_multi.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_multi_ss.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_multi_ss.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_single.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_single.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/test_utils.py` & `qcmanybody-0.2.1/qcmanybody/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/tests/utils.py` & `qcmanybody-0.2.1/qcmanybody/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody/utils.py` & `qcmanybody-0.2.1/qcmanybody/utils.py`

 * *Files identical despite different names*

### Comparing `qcmanybody-0.2.0/qcmanybody.egg-info/PKG-INFO` & `qcmanybody-0.2.1/qcmanybody.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcmanybody
-Version: 0.2.0
+Version: 0.2.1
 Summary: QCManyBody
 Author-email: Benjamin Pritchard <bpp4@vt.edu>, "Lori A. Burns" <lori.burns@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023-2024, The Molecular Sciences Software Institute
         All rights reserved.
```

### Comparing `qcmanybody-0.2.0/qcmanybody.egg-info/SOURCES.txt` & `qcmanybody-0.2.1/qcmanybody.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,25 +17,22 @@
 docs/qcschema.md
 docs/results.md
 docs/extensions/mdantic_v1/__init__.py
 docs/extensions/mdantic_v1/mdantic.py
 docs/stylesheets/extra.css
 qcmanybody/__init__.py
 qcmanybody/builder.py
+qcmanybody/computer.py
 qcmanybody/manybody.py
-qcmanybody/qcng_computer.py
 qcmanybody/utils.py
 qcmanybody.egg-info/PKG-INFO
 qcmanybody.egg-info/SOURCES.txt
 qcmanybody.egg-info/dependency_links.txt
 qcmanybody.egg-info/requires.txt
 qcmanybody.egg-info/top_level.txt
-qcmanybody/hide/asdf.py
-qcmanybody/hide/hold_test_mbe_keywords.py
-qcmanybody/hide/tsts.py
 qcmanybody/models/__init__.py
 qcmanybody/models/generalized_optimization.py
 qcmanybody/models/manybody_input_pydv1.py
 qcmanybody/models/manybody_output_pydv1.py
 qcmanybody/tests/__init__.py
 qcmanybody/tests/addons.py
 qcmanybody/tests/common.py
```

