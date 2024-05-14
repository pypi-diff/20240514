# Comparing `tmp/diffsims-0.5.2.tar.gz` & `tmp/diffsims-0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diffsims-0.5.2.tar", last modified: Tue May 23 14:38:43 2023, max compression
+gzip compressed data, was "diffsims-0.6rc1.tar", last modified: Tue May 14 21:22:47 2024, max compression
```

## Comparing `diffsims-0.5.2.tar` & `diffsims-0.6rc1.tar`

### file list

```diff
@@ -1,115 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-23 14:38:32.000000 diffsims-0.5.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-23 14:38:32.000000 diffsims-0.5.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-23 14:38:32.000000 diffsims-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 14:38:32.000000 diffsims-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 14:38:43.351786 diffsims-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-23 14:38:32.000000 diffsims-0.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/crystallography/
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17118 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20944 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/diffraction_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10958 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/library_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/rotation_list_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    18108 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/sphere_mesh_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/generators/zap_map_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims/libraries/
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/diffraction_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/structure_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/libraries/vector_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/pattern/detector_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/sims/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/sims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18084 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/sims/diffraction_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/structure_factor/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10471 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/structure_factor/structure_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/crystallography/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    24750 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_diffraction_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_library_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_rotation_list_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_sphere_mesh_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/generators/test_zap_map_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_diffraction_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_structure_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/library/test_vector_library.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/patterns/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/patterns/test_detector_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/sims/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/sims/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/sims/test_diffraction_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.347785 diffsims-0.5.2/diffsims/tests/structure_factor/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_factor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/structure_factor/test_structure_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/diffsims/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_discretise_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_kinematic_simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_probe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_ring_pattern_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_sim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/tests/utils/test_vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/diffsims/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/atomic_diffraction_generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24489 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/atomic_scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)    54440 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/discretise_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24183 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/fourier_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/kinematic_simulation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38198 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/lobato_scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/mask_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/probe_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/ring_pattern_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43469 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/scattering_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/shape_factor_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    23768 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/sim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-23 14:38:32.000000 diffsims-0.5.2/diffsims/utils/vector_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.343785 diffsims-0.5.2/diffsims.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 14:38:43.000000 diffsims-0.5.2/diffsims.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:38:43.351786 diffsims-0.5.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/related_projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 14:38:32.000000 diffsims-0.5.2/doc/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 14:38:32.000000 diffsims-0.5.2/readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 14:38:43.355785 diffsims-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-23 14:38:32.000000 diffsims-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.126854 diffsims-0.6rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-14 21:22:42.000000 diffsims-0.6rc1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-14 21:22:42.000000 diffsims-0.6rc1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-05-14 21:22:42.000000 diffsims-0.6rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 21:22:42.000000 diffsims-0.6rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-14 21:22:47.126854 diffsims-0.6rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-14 21:22:42.000000 diffsims-0.6rc1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.106854 diffsims-0.6rc1/diffsims/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.106854 diffsims-0.6rc1/diffsims/crystallography/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/crystallography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/crystallography/_diffracting_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/crystallography/get_hkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52456 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/crystallography/reciprocal_lattice_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.106854 diffsims-0.6rc1/diffsims/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21013 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/diffraction_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/library_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9722 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/rotation_list_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16125 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/simulation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18297 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/sphere_mesh_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/generators/zap_map_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/libraries/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/libraries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/libraries/diffraction_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/libraries/structure_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/libraries/vector_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6935 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/pattern/detector_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/sims/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/sims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18151 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/sims/diffraction_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/simulations/
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/simulations/simulation1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27726 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/simulations/simulation2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/structure_factor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/structure_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/structure_factor/atomic_scattering_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/structure_factor/atomic_scattering_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/structure_factor/structure_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.110854 diffsims-0.6rc1/diffsims/tests/crystallography/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/crystallography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/crystallography/test_diffracting_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/crystallography/test_get_hkl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25242 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   131200 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/old_simulation.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    11105 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_diffraction_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_library_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_rotation_list_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_simulation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_sphere_mesh_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/generators/test_zap_map_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/library/test_diffraction_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/library/test_structure_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/library/test_vector_library.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/patterns/test_detector_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/sims/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/sims/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11024 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/sims/test_diffraction_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/simulations/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/simulations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/simulations/test_simulations1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/simulations/test_simulations2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.114854 diffsims-0.6rc1/diffsims/tests/structure_factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/structure_factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/structure_factor/test_atomic_scattering_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/structure_factor/test_structure_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.118854 diffsims-0.6rc1/diffsims/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4348 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_discretise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_kinematic_simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_probe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3068 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_ring_pattern_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10952 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_sim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/tests/utils/test_vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/diffsims/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/atomic_diffraction_generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24489 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/atomic_scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54535 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/discretise_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24404 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/fourier_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/kinematic_simulation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38198 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/lobato_scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/mask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10040 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/probe_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/ring_pattern_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43469 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/scattering_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8770 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/shape_factor_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24459 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/sim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-05-14 21:22:42.000000 diffsims-0.6rc1/diffsims/utils/vector_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.126854 diffsims-0.6rc1/diffsims.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-14 21:22:47.000000 diffsims-0.6rc1/diffsims.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-05-14 21:22:47.000000 diffsims-0.6rc1/diffsims.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 21:22:47.000000 diffsims-0.6rc1/diffsims.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-14 21:22:47.000000 diffsims-0.6rc1/diffsims.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-14 21:22:47.000000 diffsims-0.6rc1/diffsims.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_static/pyxem_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/custom-attribute-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/custom-class-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/custom-function-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/custom-method-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/_templates/custom-module-template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/doc/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/user/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-14 21:22:42.000000 diffsims-0.6rc1/doc/user/related_projects.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.122854 diffsims-0.6rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-14 21:22:42.000000 diffsims-0.6rc1/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 21:22:47.126854 diffsims-0.6rc1/examples/creating_a_simulation_library/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-14 21:22:42.000000 diffsims-0.6rc1/examples/creating_a_simulation_library/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-14 21:22:42.000000 diffsims-0.6rc1/examples/creating_a_simulation_library/migration_guide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-14 21:22:42.000000 diffsims-0.6rc1/examples/creating_a_simulation_library/simulating_diffraction_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-14 21:22:42.000000 diffsims-0.6rc1/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-14 21:22:47.126854 diffsims-0.6rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-14 21:22:42.000000 diffsims-0.6rc1/setup.py
```

### Comparing `diffsims-0.5.2/CHANGELOG.rst` & `diffsims-0.6rc1/CHANGELOG.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,46 @@
 =========
 Changelog
 =========
 
 All notable changes to this project will be documented in this file.
+The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0>`_, and
+this project tries its best to adhere to
+`Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
-The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0>`_,
-and this project adheres to `Semantic Versioning
-<https://semver.org/spec/v2.0.0.html>`_.
+2024-05-12 - version 0.6.0
+==========================
+
+Added
+-----
+- Explicit support for Python 3.11.
+- Added Pre-Commit for code formatting.
+- Added deprecation tools for deprecating functions, parameters, methods, and
+  properties.
+
+Changed
+-------
+- Documentation theme from Furo to the PyData-Sphinx-Theme.
+- Ran ``black`` formatting to update the code style.
+
+Deprecated
+----------
+- ``get_hkl()``, ``get_highest_hkl()``, and ``get_equivalent_hkl()`` methods in the
+  crystallography module. Please use the following corresponding methods in the
+  ``ReciprocalLatticeVector`` class instead: ``from_highest_hkl()``,
+  ``from_min_dspacing()``, and ``symmetrise()``.
+
+Removed
+-------
+- Removed support for Python 3.6 and Python 3.7, leaving 3.8 as the oldest supported
+  version.
+- ``ReciprocalLatticePoint`` class; Use the ``ReciprocalLatticeVector`` class instead,
+  which is an improved replacement.
+- ``StructureLibrary.from_crystal_systems()`` class method, which previously raised a
+  ``NotImplementedError``, but now will throw an ``AttributeError`` instead.
 
 2023-05-22 - version 0.5.2
 ==========================
 
 Fixed
 -----
 - Always use no-python mode to silence Numba deprecation warnings.
```

### Comparing `diffsims-0.5.2/CONTRIBUTING.rst` & `diffsims-0.6rc1/CONTRIBUTING.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-=================
-Contributor Guide
-=================
+============
+Contributing
+============
 
 This guide is intended to get new developers started with contributing to diffsims.
 
 Many potential contributors will be scientists with much expert knowledge but
 potentially little experience with open-source code development. This guide is primarily
 aimed at this audience, helping to reduce the barrier to contribution.
 
 We have a `Code of Conduct
 <https://github.com/pyxem/diffsims/blob/master/.github/CODE_OF_CONDUCT.md>`_ that must
 be honoured by contributors.
 
+
 Start using diffsims
 ====================
 
 The best way to start understanding how diffsims works is to use it.
 
 For developing the code the home of diffsims is on GitHub and you'll see that a lot of
 this guide boils down to using that platform well. so visit the following link and poke
@@ -38,28 +39,30 @@
 Note: You cannot mess up the main diffsims project. So when you're starting out be
 confident to play, get it wrong, and if it all goes wrong you can always get a fresh
 install of diffsims!
 
 PS: If you choose to develop in Windows/Mac you may find the `Github Desktop
 <https://desktop.github.com>`_ useful.
 
+
 Questions?
 ==========
 
 Open source projects are all about community - we put in much effort to make good tools
 available to all and most people are happy to help others start out. Everyone had to
 start at some point and the philosophy of these projects centers around the fact that we
 can do better by working together.
 
 Much of the conversation happens in 'public' using the 'issues' pages on
 `GitHub <https://github.com/pyxem/diffsims/issues>`_ -- doing things in public can be
 scary but it ensures that issues are identified and logged until dealt with. This is
 also a good place to make a proposal for some new feature or tool that you want to work
 on.
 
+
 Good coding practice
 ====================
 
 The most important aspects of good coding practice are: (1) to work in manageable
 branches, (2) develop a good code style, (3) write tests for new functions, and (4)
 document what the code does. Tips on these points are provided below.
 
@@ -82,14 +85,17 @@
 consistency that you can read all about in the `Python Style Guide
 <https://peps.python.org/pep-0008/>`_.
 
 Please run the latest version of
 `black <https://black.readthedocs.io/en/stable/the_black_code_style/index.html>`_ on
 your newly added and modified files prior to each PR.
 
+If this doesn't work for you, you can also use the Pre-commit CI to reformat your code
+on github by commenting "pre-commit autofix" on your PR.
+
 Run and write tests
 -------------------
 
 All functionality in diffsims is tested via the `pytest
 <https://docs.pytest.org/en/stable/>`_ framework. The tests reside in the
 ``diffsims.tests`` module. Tests are short functions that call functions in diffsims and
 compare resulting output values with known answers. Good tests should depend on as few
@@ -120,14 +126,38 @@
 - When comparing integers, it's fine to use ``==``. When comparing floats use something
   like assert ``np.allclose(shifts, shifts_expected, atol=0.2)``.
 - ``@pytest.mark.parametrize()`` is a convenient decorator to test several parameters of
   the same function without having to write to much repetitive code, which is often
   error-prone. See `pytest documentation for more details
   <https://doc.pytest.org/en/latest/how-to/parametrize.html>`_.
 
+Deprecations
+------------
+We attempt to adhere to semantic versioning as best we can. This means that as little,
+ideally no, functionality should break between minor releases. Deprecation warnings
+are raised whenever possible and feasible for functions/methods/properties/arguments,
+so that users get a heads-up one (minor) release before something is removed or changes,
+with a possible alternative to be used.
+
+
+A deprecation decorator should be placed right above the object signature to be deprecated::
+
+    from diffsims.utils._deprecated import deprecated
+
+    @deprecated(since=0.8, removal=0.9, alternative="bar")
+    def foo(self, n): ...
+
+    @property
+    @deprecated(
+        since="0.9",
+        removal="0.10",
+        alternative="another",
+        alternative_is_function=True
+    ): ...
+
 Build and write documentation
 -----------------------------
 
 Docstrings -- written at the start of a function -- give essential information about how
 it should be used, such as which arguments can be passed to it and what the syntax
 should be. The docstrings mostly follow the `numpydoc
 <https://numpydoc.readthedocs.io/en/latest/format.html>`_ standard.
@@ -144,19 +174,21 @@
 
 The documentation's HTML pages are built in the ``doc/build/html`` directory from files
 in the `reStructuredText (reST)
 <https://www.sphinx-doc.org/en/master/usage/restructuredtext/basics.html>`_
 plaintext markup language. They should be accessible in the browser by typing
 ``file:///your-absolute/path/to/diffsims/doc/build/html/index.html`` in the address bar.
 
+
 Continuous integration (CI)
 ===========================
 
 We use `GitHub Actions <https://github.com/pyxem/diffsims/actions>`_ to ensure that
 diffsims can be installed on Windows, macOS and Linux. After a successful installation,
 the CI server runs the tests. After the tests return no errors, code coverage is
 reported to `Coveralls <https://coveralls.io/github/pyxem/diffsims?branch=master>`_.
 
+
 Learn more
 ==========
 
 1. The Python programming language, `for beginners <https://www.python.org/about/gettingstarted/>`__.
```

### Comparing `diffsims-0.5.2/LICENSE` & `diffsims-0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `diffsims-0.5.2/diffsims/__init__.py` & `diffsims-0.6rc1/diffsims/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/conftest.py` & `diffsims-0.6rc1/diffsims/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,24 +13,29 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 from diffpy.structure import Atom, Lattice, Structure
+import matplotlib.pyplot as plt
 from orix.crystal_map import Phase
 import pytest
 
 from diffsims.crystallography import ReciprocalLatticeVector
 from diffsims.generators.diffraction_generator import DiffractionGenerator
 
 
+def pytest_sessionstart(session):
+    plt.rcParams["backend"] = "agg"
+
+
 @pytest.fixture
 def default_structure():
-    """An atomic structure represented using diffpy"""
+    """An atomic structure represented using diffpy."""
     latt = Lattice(3, 3, 5, 90, 90, 120)
     atom = Atom(atype="Ni", xyz=[0, 0, 0], lattice=latt)
     hexagonal_structure = Structure(atoms=[atom], lattice=latt)
     return hexagonal_structure
 
 
 @pytest.fixture
@@ -105,7 +110,14 @@
         structure=Structure(
             lattice=Lattice(4.04, 4.04, 4.04, 90, 90, 90),
             atoms=[Atom("Al", [0, 0, 1])],
         ),
     )
     rlv = ReciprocalLatticeVector(phase, hkl=[[1, 1, 1], [2, 0, 0]])
     doctest_namespace["rlv"] = rlv
+
+
+@pytest.fixture(params=[("file_01")])
+def pickle_temp_file(tmpdir, request):
+    name = request.param
+    fname = tmpdir.join(name + ".pickle")
+    yield fname
```

### Comparing `diffsims-0.5.2/diffsims/crystallography/__init__.py` & `diffsims-0.6rc1/diffsims/sims/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,26 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Generation of reciprocal lattice vectors (crystal plane, reflector,
-g, hkl) for a crystal structure.
-"""
+"""Diffraction simulations."""
 
-from diffsims.crystallography.reciprocal_lattice_point import (
-    ReciprocalLatticePoint,
-    get_equivalent_hkl,
-    get_highest_hkl,
-    get_hkl,
+from diffsims.sims import (
+    diffraction_simulation,
 )
-from diffsims.crystallography.reciprocal_lattice_vector import ReciprocalLatticeVector
 
 __all__ = [
-    "get_equivalent_hkl",
-    "get_highest_hkl",
-    "get_hkl",
-    "ReciprocalLatticePoint",
-    "ReciprocalLatticeVector",
+    "diffraction_simulation",
 ]
```

### Comparing `diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_point.py` & `diffsims-0.6rc1/diffsims/generators/sphere_mesh_generators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,474 +12,516 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-from collections import defaultdict
+import numpy as np
+from scipy.spatial import cKDTree
 from itertools import product
-from warnings import warn
 
-import numpy as np
-from orix.vector import Vector3d
+from diffsims.utils.vector_utils import vectorised_spherical_polars_to_cartesians
 
-from diffsims.structure_factor.structure_factor import (
-    get_kinematical_structure_factor,
-    get_doyleturner_structure_factor,
-    get_refraction_corrected_wavelength,
-)
 
+__all__ = [
+    "beam_directions_grid_to_euler",
+    "get_cube_mesh_vertices",
+    "get_icosahedral_mesh_vertices",
+    "get_random_sphere_vertices",
+    "get_uv_sphere_mesh_vertices",
+]
 
-_FLOAT_EPS = np.finfo(float).eps  # Used to round values below 1e-16 to zero
 
+def _normalize_vectors(vectors):
+    """
+    Helper function which returns a list of vectors normalized to length 1 from
+    a 2D array representing a list of 3D vectors
+    """
+    return (vectors.T / np.linalg.norm(vectors, axis=1)).T
 
-class ReciprocalLatticePoint:
-    """*[Deprecated]* Reciprocal lattice point (or crystal plane,
-    reflector, g, etc.) with Miller indices, length of the reciprocal
-    lattice vectors and other relevant structure_factor parameters.
 
-    Notes
-    -----
-    Deprecated since version 0.5: Class ``ReciprocalLatticePoint`` is
-    deprecated and will be removed in version 0.6. Use
-    :class:`~diffsims.crystallography.ReciprocalLatticeVector` instead.
-    """
-
-    def __init__(self, phase, hkl):
-        """A container for Miller indices, structure factors and related
-        parameters for crystal planes (reciprocal lattice points,
-        reflectors, g, etc.).
-
-        Parameters
-        ----------
-        phase : orix.crystal_map.phase_list.Phase
-            A phase container with a crystal structure and a space and
-            point group describing the allowed symmetry operations.
-        hkl : orix.vector.Vector3d, np.ndarray, list, or tuple
-            Miller indices.
-
-        """
-
-        warn(
-            message=(
-                "Class `ReciprocalLatticePoint` is deprecated and will be removed in "
-                "version 0.6. Use `ReciprocalLatticeVector` instead."
-            ),
-            category=np.VisibleDeprecationWarning,
-        )
+def get_uv_sphere_mesh_vertices(resolution):
+    """Return the vertices of a UV (spherical coordinate) mesh on a unit
+    sphere [Cajaravelli2015]_. The mesh vertices are defined by the
+    parametrization:
+
+    .. math::
+        x = sin(u)cos(v)\n
+        y = sin(u)sin(v)\n
+        z = cos(u)
 
-        self.phase = phase
-        self._raise_if_no_point_group()
-        self._hkl = Vector3d(hkl)
-        self._structure_factor = [None] * self.size
-        self._theta = [None] * self.size
-
-    def __repr__(self):
-        return (
-            f"{self.__class__.__name__} {self.hkl.shape}\n"
-            f"Phase: {self.phase.name} ({self.phase.point_group.name})\n"
-            f"{np.array_str(self.hkl.data, precision=4, suppress_small=True)}"
-        )
+    Parameters
+    ----------
+    resolution : float
+        An angle in degrees. The maximum angle between nearest neighbor
+        grid points. In this mesh this occurs on the equator of the
+        sphere. All elevation grid lines are separated by at most
+        resolution. The step size of u and v are rounded up to get an
+        integer number of elevation and azimuthal grid lines with equal
+        spacing.
 
-    def __getitem__(self, key):
-        new_rlp = self.__class__(self.phase, self.hkl[key])
-        if self.structure_factor[0] is None:
-            new_rlp._structure_factor = [None] * new_rlp.size
-        else:
-            new_rlp._structure_factor = self.structure_factor[key]
-        if self.theta[0] is None:
-            new_rlp._theta = [None] * new_rlp.size
-        else:
-            new_rlp._theta = self.theta[key]
-        return new_rlp
+    Returns
+    -------
+    points_in_cartesian : numpy.ndarray (N,3)
+        Rows are x, y, z where z is the 001 pole direction
+    """
+    steps_theta = int(np.ceil(180 / resolution)) + 1  # elevation
+    steps_psi = int(np.ceil(360 / resolution))  # azimuthal
 
-    @property
-    def hkl(self):
-        """Return :class:`~orix.vector.Vector3d` of Miller indices."""
-        return Vector3d(self._hkl.data.astype(int))
-
-    @property
-    def h(self):
-        """Return :class:`np.ndarray` of Miller index h."""
-        return self.hkl.data[..., 0]
-
-    @property
-    def k(self):
-        """Return :class:`np.ndarray` of Miller index k."""
-        return self.hkl.data[..., 1]
-
-    @property
-    def l(self):
-        """Return :class:`np.ndarray` of Miller index l."""
-        return self.hkl.data[..., 2]
-
-    @property
-    def size(self):
-        """Return `int`."""
-        return self.hkl.size
-
-    @property
-    def shape(self):
-        """Return `tuple`."""
-        return self.hkl.data.shape
-
-    @property
-    def multiplicity(self):
-        """Return either `int` or :class:`np.ndarray` of `int`."""
-        return self.symmetrise(antipodal=True, return_multiplicity=True)[1]
-
-    @property
-    def gspacing(self):
-        """Return :class:`np.ndarray` of reciprocal lattice point
-        spacings.
-        """
-        return self.phase.structure.lattice.rnorm(self.hkl.data)
-
-    @property
-    def dspacing(self):
-        """Return :class:`np.ndarray` of direct lattice interplanar
-        spacings.
-        """
-        return 1 / self.gspacing
-
-    @property
-    def scattering_parameter(self):
-        """Return :class:`np.ndarray` of scattering parameters s."""
-        return 0.5 * self.gspacing
-
-    @property
-    def structure_factor(self):
-        """Return :class:`np.ndarray` of structure factors F or None."""
-        return self._structure_factor
-
-    @property
-    def allowed(self):
-        """Return whether planes diffract according to structure_factor
-        selection rules assuming kinematical scattering theory.
-        """
-        self._raise_if_no_space_group()
-
-        # Translational symmetry
-        centering = self.phase.space_group.short_name[0]
-
-        if centering == "P":  # Primitive
-            if self.phase.space_group.crystal_system == "HEXAGONAL":
-                # TODO: See rules in e.g.
-                #  https://mcl1.ncifcrf.gov/dauter_pubs/284.pdf, Table 4
-                #  http://xrayweb.chem.ou.edu/notes/symmetry.html, Systematic Absences
-                raise NotImplementedError
-            else:  # Any hkl
-                return np.ones(self.size, dtype=bool)
-        elif centering == "F":  # Face-centred, hkl all odd/even
-            selection = np.sum(np.mod(self.hkl.data, 2), axis=1)
-            return np.array([i not in [1, 2] for i in selection], dtype=bool)
-        elif centering == "I":  # Body-centred, h + k + l = 2n (even)
-            return np.mod(np.sum(self.hkl.data, axis=1), 2) == 0
-        elif centering == "A":  # Centred on A faces only
-            return np.mod(self.k + self.l, 2) == 0
-        elif centering == "B":  # Centred on B faces only
-            return np.mod(self.h + self.l, 2) == 0
-        elif centering == "C":  # Centred on C faces only
-            return np.mod(self.h + self.k, 2) == 0
-        elif centering in ["R", "H"]:  # Rhombohedral
-            return np.mod(-self.h + self.k + self.l, 3) == 0
-
-    @property
-    def theta(self):
-        """Return :class:`np.ndarray` of twice the Bragg angle."""
-        return self._theta
-
-    @classmethod
-    def from_min_dspacing(cls, phase, min_dspacing=0.5):
-        """Create a CrystalPlane object populated by unique Miller indices
-        with a direct space interplanar spacing greater than a lower
-        threshold.
-
-        Parameters
-        ----------
-        phase : orix.crystal_map.phase_list.Phase
-            A phase container with a crystal structure and a space and
-            point group describing the allowed symmetry operations.
-        min_dspacing : float, optional
-            Smallest interplanar spacing to consider. Default is 0.5 Å.
-        """
-        highest_hkl = get_highest_hkl(
-            lattice=phase.structure.lattice, min_dspacing=min_dspacing
+    psi = np.linspace(0, 2 * np.pi, num=steps_psi, endpoint=False)
+    theta = np.linspace(0, np.pi, num=steps_theta, endpoint=True)
+
+    psi_theta = np.asarray(list(product(psi, theta)))
+    r = np.ones((psi_theta.shape[0], 1))
+    points_in_spherical_polars = np.hstack((r, psi_theta))
+    # keep only one theta ==0 point, specifically the psi ==0 one
+    points_in_spherical_polars = points_in_spherical_polars[
+        np.logical_or(
+            np.abs(points_in_spherical_polars[:, 2]) > 0,
+            points_in_spherical_polars[:, 1] == 0,
+        )
+    ]
+    # keep only one theta ==180 point, specifically the psi ==0 one
+    points_in_spherical_polars = points_in_spherical_polars[
+        np.logical_or(
+            np.abs(points_in_spherical_polars[:, 2]) < np.deg2rad(180),
+            points_in_spherical_polars[:, 1] == 0,
         )
-        hkl = get_hkl(highest_hkl=highest_hkl)
-        return cls(phase=phase, hkl=hkl).unique()
+    ]
+    points_in_cartesians = vectorised_spherical_polars_to_cartesians(
+        points_in_spherical_polars
+    )
+    return points_in_cartesians
 
-    @classmethod
-    def from_highest_hkl(cls, phase, highest_hkl):
-        """Create a CrystalPlane object populated by unique Miller indices
-        below, but including, a set of higher indices.
-
-        Parameters
-        ----------
-        phase : orix.crystal_map.phase_list.Phase
-            A phase container with a crystal structure and a space and
-            point group describing the allowed symmetry operations.
-        highest_hkl : np.ndarray, list, or tuple of int
-            Highest Miller indices to consider (including).
-        """
-        hkl = get_hkl(highest_hkl=highest_hkl)
-        return cls(phase=phase, hkl=hkl).unique()
-
-    def unique(self, use_symmetry=True):
-        """Return planes with unique Miller indices.
-
-        Parameters
-        ----------
-        use_symmetry : bool, optional
-            Whether to use symmetry to remove the planes with indices
-            symmetrically equivalent to another set of indices.
-
-        Returns
-        -------
-        ReciprocalLatticePoint
-        """
-        if use_symmetry:
-            all_hkl = self.hkl.data
-            # Remove [0, 0, 0] points
-            all_hkl = all_hkl[~np.all(np.isclose(all_hkl, 0), axis=1)]
-
-            families = defaultdict(list)
-            for this_hkl in all_hkl.tolist():
-                for that_hkl in families.keys():
-                    if _is_equivalent(this_hkl, that_hkl):
-                        families[tuple(that_hkl)].append(this_hkl)
-                        break
-                else:
-                    families[tuple(this_hkl)].append(this_hkl)
-
-            n_families = len(families)
-            unique_hkl = np.zeros((n_families, 3))
-            for i, all_hkl_in_family in enumerate(families.values()):
-                unique_hkl[i] = sorted(all_hkl_in_family)[-1]
-        else:
-            unique_hkl = self.hkl.unique()
-        # TODO: Enable inheriting classes pass on their properties in this new object
-        return self.__class__(phase=self.phase, hkl=unique_hkl)
-
-    def symmetrise(
-        self,
-        antipodal=True,
-        unique=True,
-        return_multiplicity=False,
-    ):
-        """Return planes with symmetrically equivalent Miller indices.
-
-        Parameters
-        ----------
-        antipodal : bool, optional
-            Whether to include antipodal symmetry operations. Default is
-            True.
-        unique : bool, optional
-            Whether to return only distinct indices. Default is True.
-            If True, zero-entries, which are assumed to be degenerate, are
-            removed.
-        return_multiplicity : bool, optional
-            Whether to return the multiplicity of indices. This option is
-            only available if `unique` is True. Default is False.
-
-        Returns
-        -------
-        ReciprocalLatticePoint
-            Planes with Miller indices symmetrically equivalent to the
-            original planes.
-        multiplicity : np.ndarray
-            Multiplicity of the original Miller indices. Only returned if
-            `return_multiplicity` is True.
-
-        Notes
-        -----
-        Should be the same as EMsoft's CalcFamily in their symmetry.f90
-        module, although not entirely sure. Use with care.
-        """
-        # Get symmetry operations
-        pg = self.phase.point_group
-        operations = pg if antipodal else pg[~pg.improper]
-
-        out = get_equivalent_hkl(
-            hkl=self.hkl,
-            operations=operations,
-            unique=unique,
-            return_multiplicity=return_multiplicity,
+
+def get_cube_mesh_vertices(resolution, grid_type="spherified_corner"):
+    """Return the (x, y, z) coordinates of the vertices of a cube mesh
+    on a sphere. To generate the mesh, a cube is made to surround the
+    sphere. The surfaces of the cube are subdivided into a grid. The
+    vectors from the origin to these grid points are normalized to unit
+    length. The grid on the cube can be generated in three ways, see
+    `grid_type` and reference [Cajaravelli2015]_.
+
+    Parameters
+    ----------
+    resolution : float
+        The maximum angle in degrees between first nearest neighbor grid
+        points.
+    grid_type : str
+        The type of cube grid, can be either `normalized` or `spherified_edge`
+        or `spherified_corner` (default). For details see notes.
+
+    Returns
+    -------
+    points_in_cartesian : numpy.ndarray (N,3)
+        Rows are x, y, z where z is the 001 pole direction
+
+    Notes
+    -----
+    The resolution determines the maximum angle between first nearest
+    neighbor grid points, but to get an integer number of points between the
+    cube face center and the edges, the number of grid points is rounded up.
+    In practice this means that resolution is always an upper limit.
+    Additionally, where on the grid this maximum angle will be will depend
+    on the type of grid chosen. Resolution says something about the maximum
+    angle but nothing about the distribution of nearest neighbor angles or
+    the minimum angle - also this is fixed by the chosen grid.
+
+    In the normalized grid, the grid on the surface of the cube is linear.
+    The maximum angle between nearest neighbors is found between the <001>
+    directions and the first grid point towards the <011> directions. Points
+    approaching the edges and corners of the cube will have a smaller angular
+    deviation, so orientation space will be oversampled there compared to the
+    cube faces <001>.
+
+    In the spherified_edge grid, the grid is constructed so that there
+    are still two sets of perpendicular grid lines parallel to the {100}
+    directions on each cube face, but the spacing of the grid lines is
+    chosen so that the angles between the grid points on the line
+    connecting the face centers (<001>) to the edges (<011>) are equal.
+    The maximum angle is also between the <001> directions and the first
+    grid point towards the <011> edges. This grid slightly oversamples the
+    directions between <011> and <111>
+
+    The spherified_corner case is similar to the spherified_edge case, but
+    the spacing of the grid lines is chosen so that the angles between
+    the grid points on the line connecting the face centers to the cube
+    corners (<111>) is equal. The maximum angle in this grid is from the
+    corners to the first grid point towards the cube face centers.
+
+    References
+    ----------
+    .. [Cajaravelli2015] O. S. Cajaravelli, "Four Ways to Create a Mesh for a Sphere,"
+        https://medium.com/@oscarsc/four-ways-to-create-a-mesh-for-a-sphere-d7956b825db4.
+    """
+    # the angle between 001 and 011
+    max_angle = np.deg2rad(45)
+    # the distance on the cube face from 001 to 011 grid point
+    max_dist = 1
+    if grid_type == "normalized":
+        grid_len = np.tan(np.deg2rad(resolution))
+        steps = np.ceil(max_dist / grid_len)
+        i = np.arange(-steps, steps) / steps
+    elif grid_type == "spherified_edge":
+        steps = np.ceil(np.rad2deg(max_angle) / resolution)
+        k = np.arange(-steps, steps)
+        theta = np.arctan(max_dist) / steps
+        i = np.tan(k * theta)
+    elif grid_type == "spherified_corner":
+        # the angle from 001 to 111
+        max_angle_111 = np.arccos(1 / np.sqrt(3))
+        res_111 = np.deg2rad(resolution)
+        steps = np.ceil(max_angle_111 / res_111)
+        k = np.arange(-steps, steps)
+        theta = np.arctan(np.sqrt(2)) / steps
+        i = np.tan(k * theta) / np.sqrt(2)
+    else:
+        raise ValueError(
+            f"grid type {grid_type} not a valid grid type. "
+            f"Valid options: normalized, spherified_edge, "
+            f"spherified_corner."
         )
+    x, y = np.meshgrid(i, i)
+    x, y = x.ravel(), y.ravel()
+    z = np.ones(x.shape[0])
+    # the grid on all faces of the cube, avoiding overlap of points on edges
+    bottom = np.vstack([-x, -y, -z]).T
+    top = np.vstack([x, y, z]).T
+    east = np.vstack([z, x, -y]).T
+    west = np.vstack([-z, -x, y]).T
+    south = np.vstack([x, -z, y]).T
+    north = np.vstack([-x, z, -y]).T
+    # two corners are missing with this procedure
+    m_c = np.array([[-1, 1, 1], [1, -1, -1]])
+    # combine
+    all_vecs = np.vstack([bottom, top, east, west, south, north, m_c])
+    return _normalize_vectors(all_vecs)
 
-        # TODO: Enable inheriting classes pass on their properties in this new object
-        # Format output and return
-        if unique and return_multiplicity:
-            multiplicity = out[1]
-            if multiplicity.size == 1:
-                multiplicity = multiplicity[0]
-            return self.__class__(phase=self.phase, hkl=out[0]), multiplicity
-        else:
-            return self.__class__(phase=self.phase, hkl=out)
 
-    def calculate_structure_factor(self, method=None, voltage=None):
-        """Populate `self.structure_factor` with the structure factor F
-        for each plane.
-
-        Parameters
-        ----------
-        method : str, optional
-            Either "kinematical" for kinematical X-ray structure factors
-            or "doyleturner" for structure factors using Doyle-Turner
-            atomic scattering factors. If None (default), kinematical
-            structure factors are calculated.
-        voltage : float, optional
-            Beam energy in V used when `method=doyleturner`.
-        """
-        if method is None:
-            method = "kinematical"
-        methods = ["kinematical", "doyleturner"]
-        if method not in methods:
-            raise ValueError(f"method={method} must be among {methods}")
-        elif method == "doyleturner" and voltage is None:
-            raise ValueError(
-                "'voltage' parameter must be set when method='doyleturner'"
-            )
+def _compose_from_faces(corners, faces, n):
+    """
+    Helper function to refine a grid starting from a platonic solid,
+    adapted from meshzoo
 
-        # TODO: Find a better way to call different methods in the loop
-        structure_factors = np.zeros(self.size)
-        for i, (hkl, s) in enumerate(zip(self.hkl.data, self.scattering_parameter)):
-            if method == "kinematical":
-                structure_factors[i] = get_kinematical_structure_factor(
-                    phase=self.phase,
-                    hkl=hkl,
-                    scattering_parameter=s,
+    Parameters
+    ----------
+    corners: numpy.ndarray (N, 3)
+        Coordinates of vertices for starting shape
+    faces : list of 3-tuples of int elements
+        Each tuple in the list corresponds to the vertex indices making
+        up the face of the mesh
+    n : int
+        number of times the mesh is refined
+
+    Returns
+    -------
+    vertices: numpy.ndarray (N, 3)
+        The coordinates of the refined mesh vertices.
+
+    See also
+    --------
+    :func:`get_icosahedral_mesh_vertices`
+    """
+    # create corner nodes
+    vertices = [corners]
+    vertex_count = len(corners)
+    corner_nodes = np.arange(len(corners))
+    # create edges
+    edges = set()
+    for face in faces:
+        edges.add(tuple(sorted([face[0], face[1]])))
+        edges.add(tuple(sorted([face[1], face[2]])))
+        edges.add(tuple(sorted([face[2], face[0]])))
+    edges = list(edges)
+    # create edge nodes:
+    edge_nodes = {}
+    t = np.linspace(1 / n, 1.0, n - 1, endpoint=False)
+    corners = vertices[0]
+    k = corners.shape[0]
+    for edge in edges:
+        i0, i1 = edge
+        new_vertices = np.outer(1 - t, corners[i0]) + np.outer(t, corners[i1])
+        vertices.append(new_vertices)
+        vertex_count += len(vertices[-1])
+        edge_nodes[edge] = np.arange(k, k + len(t))
+        k += len(t)
+    triangle_cells = []
+    k = 0
+    for i in range(n):
+        j = np.arange(n - i)
+        triangle_cells.append(np.column_stack([k + j, k + j + 1, k + n - i + j + 1]))
+        j = j[:-1]
+        triangle_cells.append(
+            np.column_stack([k + j + 1, k + n - i + j + 2, k + n - i + j + 1])
+        )
+        k += n - i + 1
+    triangle_cells = np.vstack(triangle_cells)
+    for face in faces:
+        corners = face
+        edges = [(face[0], face[1]), (face[1], face[2]), (face[2], face[0])]
+        is_edge_reverted = [False, False, False]
+        for k, edge in enumerate(edges):
+            if edge[0] > edge[1]:
+                edges[k] = (edge[1], edge[0])
+                is_edge_reverted[k] = True
+        # First create the interior points in barycentric coordinates
+        if n == 1:
+            num_new_vertices = 0
+        else:
+            bary = (
+                np.hstack(
+                    [[np.full(n - i - 1, i), np.arange(1, n - i)] for i in range(1, n)]
                 )
+                / n
+            )
+            bary = np.array([1.0 - bary[0] - bary[1], bary[1], bary[0]])
+            corner_verts = np.array([vertices[0][i] for i in corners])
+            vertices_cart = np.dot(corner_verts.T, bary).T
+
+            vertices.append(vertices_cart)
+            num_new_vertices = len(vertices[-1])
+        # translation table
+        num_nodes_per_triangle = (n + 1) * (n + 2) // 2
+        tt = np.empty(num_nodes_per_triangle, dtype=int)
+        # first the corners
+        tt[0] = corner_nodes[corners[0]]
+        tt[n] = corner_nodes[corners[1]]
+        tt[num_nodes_per_triangle - 1] = corner_nodes[corners[2]]
+        # then the edges.
+        # edge 0
+        tt[1:n] = edge_nodes[edges[0]]
+        if is_edge_reverted[0]:
+            tt[1:n] = tt[1:n][::-1]
+        #
+        # edge 1
+        idx = 2 * n
+        for k in range(n - 1):
+            if is_edge_reverted[1]:
+                tt[idx] = edge_nodes[edges[1]][n - 2 - k]
             else:
-                structure_factors[i] = get_doyleturner_structure_factor(
-                    phase=self.phase,
-                    hkl=hkl,
-                    scattering_parameter=s,
-                    voltage=voltage,
-                )
-        self._structure_factor = np.where(
-            structure_factors < _FLOAT_EPS, 0, structure_factors
-        )
+                tt[idx] = edge_nodes[edges[1]][k]
+            idx += n - k - 1
+        #
+        # edge 2
+        idx = n + 1
+        for k in range(n - 1):
+            if is_edge_reverted[2]:
+                tt[idx] = edge_nodes[edges[2]][k]
+            else:
+                tt[idx] = edge_nodes[edges[2]][n - 2 - k]
+            idx += n - k
+        # now the remaining interior nodes
+        idx = n + 2
+        j = vertex_count
+        for k in range(n - 2):
+            for _ in range(n - k - 2):
+                tt[idx] = j
+                j += 1
+                idx += 1
+            idx += 2
+        vertex_count += num_new_vertices
+    vertices = np.concatenate(vertices)
+    return vertices
 
-    def calculate_theta(self, voltage):
-        """Populate `self.theta` with the Bragg angle :math:`theta_B` for
-        each plane.
-
-        Parameters
-        ----------
-        voltage : float
-            Beam energy in V.
-        """
-        wavelength = get_refraction_corrected_wavelength(self.phase, voltage)
-        self._theta = np.arcsin(0.5 * wavelength * self.gspacing)
-
-    def _raise_if_no_point_group(self):
-        """Raise ValueError if the phase attribute has no point group
-        set.
-        """
-        if self.phase.point_group is None:
-            raise ValueError(f"The phase {self.phase} must have a point group set")
-
-    def _raise_if_no_space_group(self):
-        """Raise ValueError if the phase attribute has no space group
-        set.
-        """
-        if self.phase.space_group is None:
-            raise ValueError(f"The phase {self.phase} must have a space group set")
-
-
-def get_highest_hkl(lattice, min_dspacing=0.5):
-    """Return the highest Miller indices hkl of the plane with a direct
-    space interplanar spacing greater than but closest to a lower
-    threshold.
+
+def _get_first_nearest_neighbors(points, leaf_size=50):
+    """
+    Helper function to get an array of first nearest neighbor points
+    for all points in a point cloud
 
     Parameters
     ----------
-    lattice : diffpy.structure.Lattice
-        Crystal lattice.
-    min_dspacing : float, optional
-        Smallest interplanar spacing to consider. Default is 0.5 Å.
+    points : numpy.ndarray (N, D)
+        Point cloud with N points in D dimensions
+    leaf_size : int
+        The NN search is performed using a cKDTree object. The way
+        this tree is constructed depends on leaf_size, so this parameter
+        will influence speed of tree construction and search.
 
     Returns
     -------
-    highest_hkl : np.ndarray
-        Highest Miller indices.
+    nn1_vec : numpy.ndarray (N,D)
+        Point cloud with N points in D dimensions, representing the nearest
+        neighbor point of each point in "points"
+    """
+    tree = cKDTree(points, leaf_size)
+    # get the indexes of the first nearest neighbor of each vertex
+    nn1 = tree.query(points, k=2)[1][:, 1]
+    nn1_vec = points[nn1]
+    return nn1_vec
+
+
+def _get_angles_between_nn_gridpoints(vertices, leaf_size=50):
+    """
+    Helper function to get the angles between all nearest neighbor grid
+    points on a grid of a sphere.
+    """
+    # normalize the vertex vectors
+    vertices = _normalize_vectors(vertices)
+    nn1_vec = _get_first_nearest_neighbors(vertices, leaf_size)
+    # the dot product between each point and its nearest neighbor
+    nn_dot = np.sum(vertices * nn1_vec, axis=1)
+    # angles
+    angles = np.rad2deg(np.arccos(nn_dot))
+    return angles
+
+
+def _get_max_grid_angle(vertices, leaf_size=50):
+    """
+    Helper function to get the maximum angle between nearest neighbor grid
+    points on a grid.
     """
-    highest_hkl = np.ones(3, dtype=int)
-    for i in range(3):
-        hkl = np.zeros(3)
-        d = min_dspacing + 1
-        while d > min_dspacing:
-            hkl[i] += 1
-            d = 1 / lattice.rnorm(hkl)
-        highest_hkl[i] = hkl[i]
-    return highest_hkl
+    return np.max(_get_angles_between_nn_gridpoints(vertices, leaf_size))
 
 
-def get_hkl(highest_hkl):
-    """Return a list of planes from a set of highest Miller indices.
+def get_icosahedral_mesh_vertices(resolution):
+    """
+    Return the (x, y, z) coordinates of the vertices of an icosahedral
+    mesh of a cube, see [Cajaravelli2015]_. Method was adapted from
+    meshzoo [Meshzoo]_.
 
     Parameters
     ----------
-    highest_hkl : orix.vector.Vector3d, np.ndarray, list, or tuple of int
-        Highest Miller indices to consider.
+    resolution : float
+        The maximum angle in degrees between neighboring grid points.
+        Since the mesh is generated iteratively, the actual maximum angle
+        in the mesh can be slightly smaller.
 
     Returns
     -------
-    hkl : np.ndarray
-        An array of Miller indices.
+    points_in_cartesian : numpy.ndarray (N,3)
+        Rows are x, y, z where z is the 001 pole direction
+
+    References
+    ----------
+    .. [Meshzoo] The `meshzoo.sphere` module.
     """
-    index_ranges = [np.arange(-i, i + 1) for i in highest_hkl]
-    return np.asarray(list(product(*index_ranges)))
+    t = (1.0 + np.sqrt(5.0)) / 2.0
+    corners = np.array(
+        [
+            [-1, +t, +0],
+            [+1, +t, +0],
+            [-1, -t, +0],
+            [+1, -t, +0],
+            #
+            [+0, -1, +t],
+            [+0, +1, +t],
+            [+0, -1, -t],
+            [+0, +1, -t],
+            #
+            [+t, +0, -1],
+            [+t, +0, +1],
+            [-t, +0, -1],
+            [-t, +0, +1],
+        ]
+    )
+    faces = [
+        (0, 11, 5),
+        (0, 5, 1),
+        (0, 1, 7),
+        (0, 7, 10),
+        (0, 10, 11),
+        (1, 5, 9),
+        (5, 11, 4),
+        (11, 10, 2),
+        (10, 7, 6),
+        (7, 1, 8),
+        (3, 9, 4),
+        (3, 4, 2),
+        (3, 2, 6),
+        (3, 6, 8),
+        (3, 8, 9),
+        (4, 9, 5),
+        (2, 4, 11),
+        (6, 2, 10),
+        (8, 6, 7),
+        (9, 8, 1),
+    ]
+    n = 1
+    angle = _get_max_grid_angle(corners)
+    # maybe not the most efficient approach, but the least work
+    while angle > resolution:
+        vertices = _compose_from_faces(corners, faces, n)
+        angle = _get_max_grid_angle(vertices)
+        n = n + 1
+    # push all nodes to the sphere
+    norms = np.sqrt(np.einsum("ij,ij->i", vertices, vertices))
+    vertices = (vertices.T / norms.T).T
+    return vertices
 
 
-def get_equivalent_hkl(hkl, operations, unique=False, return_multiplicity=False):
-    """Return symmetrically equivalent Miller indices.
+def get_random_sphere_vertices(resolution, seed=None):
+    """
+    Create a mesh that randomly samples the surface of a sphere
 
     Parameters
     ----------
-    hkl : orix.vector.Vector3d, np.ndarray, list or tuple of int
-        Miller indices.
-    operations : orix.quaternion.symmetry.Symmetry
-        Point group describing allowed symmetry operations.
-    unique : bool, optional
-        Whether to return only unique Miller indices. Default is False.
-    return_multiplicity : bool, optional
-        Whether to return the multiplicity of the input indices. Default
-        is False.
+    resolution : float
+        The expected mean angle between nearest neighbor
+        grid points in degrees.
+    seed : int, optional
+        passed to np.random.default_rng(), defaults to None which
+        will give a "new" random result each time
 
     Returns
     -------
-    new_hkl : orix.vector.Vector3d
-        The symmetrically equivalent Miller indices.
-    multiplicity : np.ndarray
-        Number of symmetrically equivalent indices. Only returned if
-        `return_multiplicity` is True.
-    """
-    new_hkl = operations.outer(Vector3d(hkl))
-    new_hkl = new_hkl.flatten().reshape(*new_hkl.shape[::-1])
-
-    multiplicity = None
-    if unique:
-        n_families = new_hkl.shape[0]
-        multiplicity = np.zeros(n_families, dtype=int)
-        temp_hkl = new_hkl[0].unique().data
-        multiplicity[0] = temp_hkl.shape[0]
-        if n_families > 1:
-            for i, hkl in enumerate(new_hkl[1:]):
-                temp_hkl2 = hkl.unique()
-                multiplicity[i + 1] = temp_hkl2.size
-                temp_hkl = np.append(temp_hkl, temp_hkl2.data, axis=0)
-        new_hkl = Vector3d(temp_hkl[: multiplicity.sum()])
-
-    # Remove 1-dimensions
-    new_hkl = new_hkl.squeeze()
+    points_in_cartesian : numpy.ndarray (N,3)
+        Rows are x, y, z where z is the 001 pole direction
 
-    if unique and return_multiplicity:
-        return new_hkl, multiplicity
+    References
+    ----------
+    https://mathworld.wolfram.com/SpherePointPicking.html
+    """
+    # convert resolution in degrees to number of points
+    number = int(1 / (4 * np.pi) * (360 / resolution) ** 2)
+    if seed is not None:
+        rng = np.random.default_rng(seed=seed)
     else:
-        return new_hkl
+        rng = np.random.default_rng()
+
+    xyz = rng.normal(size=(number, 3))
+    xyz = (xyz.T / np.linalg.norm(xyz, axis=1)).T
+    return xyz
 
 
-def _is_equivalent(this_hkl: list, that_hkl: list) -> bool:
-    return sorted(np.abs(this_hkl)) == sorted(np.abs(that_hkl))
+def beam_directions_grid_to_euler(vectors):
+    """
+    Convert list of vectors representing zones to a list of Euler angles
+    in the bunge convention with the constraint that phi1=0.
+
+    Parameters
+    ----------
+    vectors: numpy.ndarray (N, 3)
+        N 3-dimensional vectors to convert to Euler angles
+
+    Returns
+    -------
+    grid: numpy.ndarray (N, 3)
+        Euler angles in bunge convention corresponding to each vector in
+        degrees.
+
+    Notes
+    -----
+    The Euler angles represent the orientation of the crystal if that
+    particular vector were parallel to the beam direction [001]. The
+    additional constraint of phi1=0 means that this orientation is uniquely
+    defined for most vectors. phi1 represents the rotation of the crystal
+    around the beam direction and can be interpreted as the rotation of
+    a particular diffraction pattern.
+    """
+    norm = np.linalg.norm(vectors, axis=1)
+    z_comp = vectors[:, 2]
+    # second euler angle: around x' = angle between z and z''
+    Phi = np.arccos(z_comp / norm)
+    # first euler angle: around z = angle between x and x'
+    x_comp = vectors[:, 0]
+    y_comp = vectors[:, 1]
+    norm_proj = np.linalg.norm(vectors[:, :2], axis=1)
+    sign = np.sign(y_comp)
+    # correct for where we have y=0
+    sign[y_comp == 0] = np.sign(x_comp[y_comp == 0])
+    phi2 = sign * np.nan_to_num(np.arccos(x_comp / norm_proj))
+    # phi1 is just 0, rotation around z''
+    phi1 = np.zeros(phi2.shape[0])
+    grid = np.rad2deg(np.vstack([phi1, Phi, np.pi / 2 - phi2]).T)
+    return grid
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `diffsims-0.5.2/diffsims/crystallography/reciprocal_lattice_vector.py` & `diffsims-0.6rc1/diffsims/crystallography/reciprocal_lattice_vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -115,15 +115,14 @@
             self._coordinate_format = "hkil"
             xyz = _transform_space(hkl, "r", "c", phase.structure.lattice)
         else:
             hkl = np.asarray(hkl)
             self._coordinate_format = "hkl"
             xyz = _transform_space(hkl, "r", "c", phase.structure.lattice)
         super().__init__(xyz)
-
         self._theta = np.full(self.shape, np.nan)
         self._structure_factor = np.full(self.shape, np.nan, dtype="complex128")
 
     def __getitem__(self, key):
         miller_new = self.to_miller().__getitem__(key)
         rlv_new = self.from_miller(miller_new)
 
@@ -1019,24 +1018,26 @@
             new_out += (idx,)
         if len(new_out) == 1:
             return new_out[0]
         else:
             return new_out
 
     @classmethod
-    def from_highest_hkl(cls, phase, hkl):
+    def from_highest_hkl(cls, phase, hkl, include_zero_vector=False):
         """Create a set of unique reciprocal lattice vectors from three
         highest indices.
 
         Parameters
         ----------
         phase : orix.crystal_map.Phase
             A phase with a crystal lattice and symmetry.
         hkl : numpy.ndarray, list, or tuple
             Three highest reciprocal lattice vector indices.
+        include_zero_vector : bool
+            If ``True``, include the zero vector (000) in the set of vectors.
 
         Examples
         --------
         >>> from diffpy.structure import Atom, Lattice, Structure
         >>> from orix.crystal_map import Phase
         >>> from diffsims.crystallography import ReciprocalLatticeVector
         >>> phase = Phase(
@@ -1063,30 +1064,36 @@
 
         >>> rlv.allowed.all()
         False
 
         """
 
         idx = _get_indices_from_highest(highest_indices=hkl)
-        return cls(phase, hkl=idx).unique()
+        new = cls(phase, hkl=idx).unique()
+        if include_zero_vector:
+            new_data = np.vstack((new.hkl, np.zeros(3, dtype=int)))
+            new = ReciprocalLatticeVector(phase, hkl=new_data)
+        return new
 
     @classmethod
-    def from_min_dspacing(cls, phase, min_dspacing=0.7):
+    def from_min_dspacing(cls, phase, min_dspacing=0.7, include_zero_vector=False):
         """Create a set of unique reciprocal lattice vectors with a
         a direct space interplanar spacing greater than a lower
         threshold.
 
         Parameters
         ----------
         phase : orix.crystal_map.Phase
             A phase with a crystal lattice and symmetry.
         min_dspacing : float, optional
             Smallest interplanar spacing to consider. Default is 0.7,
             in the unit used to define the lattice parameters in
             ``phase``, which is assumed to be Ångström.
+        include_zero_vector: bool
+            If ``True``, include the zero vector (000) in the set of vectors.
 
         Examples
         --------
         >>> from diffpy.structure import Atom, Lattice, Structure
         >>> from orix.crystal_map import Phase
         >>> from diffsims.crystallography import ReciprocalLatticeVector
         >>> phase = Phase(
@@ -1124,15 +1131,19 @@
         highest_hkl = _get_highest_hkl(
             lattice=phase.structure.lattice, min_dspacing=min_dspacing
         )
         hkl = _get_indices_from_highest(highest_indices=highest_hkl)
         dspacing = 1 / phase.structure.lattice.rnorm(hkl)
         idx = dspacing >= min_dspacing
         hkl = hkl[idx]
-        return cls(phase, hkl=hkl).unique()
+        new = cls(phase, hkl=hkl).unique()
+        if include_zero_vector:
+            new_data = np.vstack((new.hkl, np.zeros(3, dtype=int)))
+            new = cls(phase, hkl=new_data)
+        return new
 
     @classmethod
     def from_miller(cls, miller):
         r"""Create a new instance from a ``Miller`` instance.
 
         Parameters
         ----------
```

### Comparing `diffsims-0.5.2/diffsims/generators/__init__.py` & `diffsims-0.6rc1/diffsims/generators/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -22,16 +22,18 @@
 
 from diffsims.generators import (
     diffraction_generator,
     library_generator,
     rotation_list_generators,
     sphere_mesh_generators,
     zap_map_generator,
+    simulation_generator,
 )
 
 __all__ = [
     "diffraction_generator",
     "library_generator",
     "rotation_list_generators",
     "sphere_mesh_generators",
+    "simulation_generator",
     "zap_map_generator",
 ]
```

### Comparing `diffsims-0.5.2/diffsims/generators/diffraction_generator.py` & `diffsims-0.6rc1/diffsims/generators/diffraction_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -38,14 +38,19 @@
     lorentzian,
     sinc,
     sin2c,
     lorentzian_precession,
 )
 
 
+__all__ = [
+    "AtomicDiffractionGenerator",
+    "DiffractionGenerator",
+]
+
 _shape_factor_model_mapping = {
     "linear": linear,
     "atanc": atanc,
     "sinc": sinc,
     "sin2c": sin2c,
     "lorentzian": lorentzian,
 }
@@ -249,28 +254,28 @@
         cartesian_coordinates = np.matmul(R, cartesian_coordinates.T).T
 
         # Identify the excitation errors of candidate points
         r_sphere = 1 / wavelength
         r_spot = np.sqrt(np.sum(np.square(cartesian_coordinates[:, :2]), axis=1))
         z_spot = cartesian_coordinates[:, 2]
 
-        z_sphere = -np.sqrt(r_sphere ** 2 - r_spot ** 2) + r_sphere
+        z_sphere = -np.sqrt(r_sphere**2 - r_spot**2) + r_sphere
         excitation_error = z_sphere - z_spot
 
         # determine the pre-selection reflections
         if self.precession_angle == 0:
             intersection = np.abs(excitation_error) < max_excitation_error
         else:
             # only consider points that intersect the ewald sphere at some point
             # the center point of the sphere
             P_z = r_sphere * np.cos(np.deg2rad(self.precession_angle))
             P_t = r_sphere * np.sin(np.deg2rad(self.precession_angle))
             # the extremes of the ewald sphere
-            z_surf_up = P_z - np.sqrt(r_sphere ** 2 - (r_spot + P_t) ** 2)
-            z_surf_do = P_z - np.sqrt(r_sphere ** 2 - (r_spot - P_t) ** 2)
+            z_surf_up = P_z - np.sqrt(r_sphere**2 - (r_spot + P_t) ** 2)
+            z_surf_do = P_z - np.sqrt(r_sphere**2 - (r_spot - P_t) ** 2)
             intersection = (z_spot - max_excitation_error <= z_surf_up) & (
                 z_spot + max_excitation_error >= z_surf_do
             )
 
         # select these reflections
         intersection_coordinates = cartesian_coordinates[intersection]
         excitation_error = excitation_error[intersection]
```

### Comparing `diffsims-0.5.2/diffsims/generators/library_generator.py` & `diffsims-0.6rc1/diffsims/generators/library_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -25,14 +25,20 @@
 from diffsims.libraries.diffraction_library import DiffractionLibrary
 from diffsims.libraries.vector_library import DiffractionVectorLibrary
 
 from diffsims.utils.sim_utils import get_points_in_sphere
 from diffsims.utils.vector_utils import get_angle_cartesian_vec
 
 
+__all__ = [
+    "DiffractionLibraryGenerator",
+    "VectorLibraryGenerator",
+]
+
+
 class DiffractionLibraryGenerator:
     """Computes a library of electron diffraction patterns for specified atomic
     structures and orientations.
     """
 
     def __init__(self, electron_diffraction_calculator):
         """Initialises the generator with a diffraction calculator.
```

### Comparing `diffsims-0.5.2/diffsims/generators/rotation_list_generators.py` & `diffsims-0.6rc1/diffsims/generators/rotation_list_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,34 +12,39 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-"""
-Provides users with a range of gridding functions
-"""
+"""Provides users with a range of gridding functions."""
 
 import numpy as np
 
 from orix.sampling.sample_generators import get_sample_fundamental, get_sample_local
 from orix.quaternion.rotation import Rotation
-from orix.vector.neo_euler import AxAngle
 
 from diffsims.utils.sim_utils import uvtw_to_uvw
 from diffsims.generators.sphere_mesh_generators import (
     get_uv_sphere_mesh_vertices,
     get_cube_mesh_vertices,
     get_icosahedral_mesh_vertices,
     get_random_sphere_vertices,
     beam_directions_grid_to_euler,
 )
 
 
+__all__ = [
+    "get_beam_directions_grid",
+    "get_fundamental_zone_grid",
+    "get_grid_around_beam_direction",
+    "get_list_from_orix",
+    "get_local_grid",
+]
+
 # Corners determined by requiring a complete coverage of the pole figure. The pole
 # figures are plotted with MTEX without implying any crystal symmetry. The plotted
 # orientations are obtained by converting vectors returned by get_beam_directions_grid()
 # into Euler angles using the procedure by GitHub user @din14970 described here:
 # https://github.com/pyxem/orix/issues/125#issuecomment-698956290.
 crystal_system_dictionary = {
     "cubic": [(0, 0, 1), (1, 1, 1), (1, 0, 1)],
@@ -48,16 +53,15 @@
     "tetragonal": [(0, 0, 1), (1, 0, 0), (1, 1, 0)],
     "orthorhombic": [(0, 0, 1), (-1, 0, 0), (0, 1, 0)],
     "monoclinic": [(0, -1, 0), (0, 0, 1), (0, 1, 0)],
 }
 
 
 def get_list_from_orix(grid, rounding=2):
-    """
-    Converts an orix sample to a rotation list
+    """Converts an orix sample to a rotation list.
 
     Parameters
     ----------
     grid : orix.quaternion.rotation.Rotation
         A grid of rotations
     rounding : int, optional
         The number of decimal places to retain, defaults to 2
@@ -159,15 +163,15 @@
     z = np.deg2rad(np.asarray(beam_rotation))
     beam_rotation = Rotation.from_euler(z)
 
     angles = np.deg2rad(
         np.arange(start=angular_range[0], stop=angular_range[1], step=resolution)
     )
     axes = np.repeat([[0, 0, 1]], angles.shape[0], axis=0)
-    in_plane_rotation = Rotation.from_neo_euler(AxAngle.from_axes_angles(axes, angles))
+    in_plane_rotation = Rotation.from_axes_angles(axes, angles)
 
     orix_grid = beam_rotation * in_plane_rotation
     rotation_list = get_list_from_orix(orix_grid, rounding=2)
     return rotation_list
 
 
 def get_beam_directions_grid(crystal_system, resolution, mesh="spherified_cube_edge"):
```

### Comparing `diffsims-0.5.2/diffsims/generators/zap_map_generator.py` & `diffsims-0.6rc1/diffsims/generators/zap_map_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,14 +16,22 @@
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 from transforms3d.euler import axangle2euler
 
 
+__all__ = [
+    "corners_to_centroid_and_edge_centers",
+    "generate_directional_simulations",
+    "generate_zap_map",
+    "get_rotation_from_z_to_direction",
+]
+
+
 def get_rotation_from_z_to_direction(structure, direction):
     """
     Finds the rotation that takes [001] to a given zone axis.
 
     Parameters
     ----------
     structure : diffpy.structure.structure.Structure
```

### Comparing `diffsims-0.5.2/diffsims/libraries/__init__.py` & `diffsims-0.6rc1/diffsims/libraries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/libraries/diffraction_library.py` & `diffsims-0.6rc1/diffsims/libraries/diffraction_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -17,14 +17,20 @@
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 
 import numpy as np
 
 
+__all__ = [
+    "DiffractionLibrary",
+    "load_DiffractionLibrary",
+]
+
+
 def load_DiffractionLibrary(filename, safety=False):
     """Loads a previously saved diffraction library.
 
     Parameters
     ----------
     filename : str
         The location of the file to be loaded.
@@ -162,12 +168,12 @@
         Parameters
         ----------
         filename : str
             The location in which to save the file
 
         See Also
         --------
-        load_DiffractionLibrary()
+        load_DiffractionLibrary
 
         """
         with open(filename, "wb") as handle:
             pickle.dump(self, handle, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `diffsims-0.5.2/diffsims/libraries/structure_library.py` & `diffsims-0.6rc1/diffsims/libraries/structure_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,14 +12,18 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
+__all__ = [
+    "StructureLibrary",
+]
+
 
 class StructureLibrary:
     """
     A dictionary containing all the structures and their associated rotations
     in the .struct_lib attribute.
 
     Attributes
@@ -73,44 +77,14 @@
             convention and in degrees.
         Returns
         -------
         StructureLibrary
         """
         return cls(identifiers, structures, orientations)
 
-    @classmethod
-    def from_crystal_systems(
-        cls, identifiers, structures, systems, resolution, equal="angle"
-    ):
-        """
-        Creates a structure library from crystal system derived orientation lists
-
-        Parameters
-        ----------
-        identifiers : list of strings/ints
-            A list of phase identifiers referring to different atomic structures.
-        structures : list of diffpy.structure.Structure objects.
-            A list of diffpy.structure.Structure objects describing the atomic
-            structure associated with each phase in the library.
-        systems : list
-            A list over indentifiers of crystal systems
-        resolution : float
-            resolution in degrees
-        equal : str
-            Default is 'angle'
-
-        Raises
-        ------
-        NotImplementedError:
-            "This function has been removed in version 0.3.0, in favour of creation from orientation lists"
-        """
-        raise NotImplementedError(
-            "This function has been removed in version 0.3.0, in favour of creation from orientation lists"
-        )
-
     def get_library_size(self, to_print=False):
         """
         Returns the the total number of orientations in the
         current StructureLibrary object. Will also print the number of orientations
         for each identifier in the library if the to_print==True
 
         Parameters
```

### Comparing `diffsims-0.5.2/diffsims/libraries/vector_library.py` & `diffsims-0.6rc1/diffsims/libraries/vector_library.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -15,14 +15,20 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import pickle
 
 
+__all__ = [
+    "DiffractionVectorLibrary",
+    "load_VectorLibrary",
+]
+
+
 def load_VectorLibrary(filename, safety=False):
     """Loads a previously saved vectorlibrary.
 
     Parameters
     ----------
     filename : str
         The location of the file to be loaded
@@ -32,15 +38,15 @@
     Returns
     -------
     VectorLibrary
         Previously saved Library
 
     See Also
     --------
-    VectorLibrary.pickle_library()
+    VectorLibrary.pickle_library
     """
     if safety:
         with open(filename, "rb") as handle:
             return pickle.load(handle)
     else:
         raise RuntimeError(
             "Unpickling is risky, turn safety to True if \
@@ -82,12 +88,12 @@
         Parameters
         ----------
         filename : str
             The location in which to save the file
 
         See Also
         --------
-            load_VectorLibrary()
+        load_VectorLibrary
 
         """
         with open(filename, "wb") as handle:
             pickle.dump(self, handle, protocol=pickle.HIGHEST_PROTOCOL)
```

### Comparing `diffsims-0.5.2/diffsims/pattern/__init__.py` & `diffsims-0.6rc1/diffsims/tests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,11 +11,7 @@
 # diffsims is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
-
-from diffsims.pattern import detector_functions
-
-__all__ = ["detector_functions"]
```

### Comparing `diffsims-0.5.2/diffsims/pattern/detector_functions.py` & `diffsims-0.6rc1/diffsims/pattern/detector_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -18,14 +18,26 @@
 
 import numpy as np
 
 from numpy.random import default_rng
 from scipy import ndimage as ndi
 
 
+__all__ = [
+    "add_dead_pixels",
+    "add_detector_offset",
+    "add_gaussian_noise",
+    "add_gaussian_point_spread",
+    "add_linear_detector_gain",
+    "add_shot_noise",
+    "add_shot_and_point_spread",
+    "constrain_to_dynamic_range",
+]
+
+
 def constrain_to_dynamic_range(pattern, detector_max=None):
     """Force the values within pattern to lie between [0,detector_max]
 
     Parameters
     ----------
     pattern : numpy.ndarray
         The diffraction pattern at the detector after corruption
```

### Comparing `diffsims-0.5.2/diffsims/release_info.py` & `diffsims-0.6rc1/diffsims/release_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 name = "diffsims"
-version = "0.5.2"
+version = "0.6rc1"
 author = "Duncan Johnstone, Phillip Crout"
-copyright = "Copyright 2017-2023, The diffsims developers"
+copyright = "Copyright 2017-2024, The diffsims developers"
 # Initial committer first, then listed by line additions
 credits = [
     "Duncan Johnstone",
     "Phillip Crout",
     "Håkon Wiik Ånes",
+    "Carter Francis",
     "Eric Prestat",
     "Rob Tovey",
     "Simon Høgås",
     "Ben Martineau",
     "Niels Cautaerts",
     "Joonatan Laulainen",
     "Isabel Wood",
@@ -21,10 +22,10 @@
     "Jedrzej Morzy",
     "Endre Jacobsen",
     "Tina Bergh",
     "Tomas Ostasevicius",
     "Eirik Opheim",
 ]
 license = "GPLv3+"
-maintainer = "Duncan Johnstone, Phillip Crout, Håkon Wiik Ånes"
+maintainer = "Duncan Johnstone, Phillip Crout, Håkon Wiik Ånes, Carter Francis"
 email = "pyxem.team@gmail.com"
 status = "Development"
```

### Comparing `diffsims-0.5.2/diffsims/sims/__init__.py` & `diffsims-0.6rc1/diffsims/simulations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,16 +12,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Diffraction simulations."""
+"""Kinematic Diffraction Simulation Results."""
 
-from diffsims.sims import (
-    diffraction_simulation,
-)
+from diffsims.simulations.simulation2d import Simulation2D
+from diffsims.simulations.simulation1d import Simulation1D
 
 __all__ = [
-    "diffraction_simulation",
+    "Simulation1D",
+    "Simulation2D",
 ]
```

### Comparing `diffsims-0.5.2/diffsims/sims/diffraction_simulation.py` & `diffsims-0.6rc1/diffsims/sims/diffraction_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -11,20 +11,27 @@
 # diffsims is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
+import copy
 
 import matplotlib.pyplot as plt
 import numpy as np
+
 from diffsims.pattern.detector_functions import add_shot_and_point_spread
 from diffsims.utils import mask_utils
-import copy
+
+
+__all__ = [
+    "DiffractionSimulation",
+    "ProfileSimulation",
+]
 
 
 class DiffractionSimulation:
     """Holds the result of a kinematic diffraction pattern simulation.
 
     Parameters
     ----------
@@ -199,15 +206,15 @@
         else:
             coords_transformed = self.calibrated_coordinates.copy()
         cx, cy = center
         x = coords_transformed[:, 0]
         y = coords_transformed[:, 1]
         mirrored_factor = -1 if mirrored else 1
         theta = mirrored_factor * np.arctan2(y, x) + np.deg2rad(angle)
-        rd = np.sqrt(x ** 2 + y ** 2)
+        rd = np.sqrt(x**2 + y**2)
         coords_transformed[:, 0] = rd * np.cos(theta) + cx
         coords_transformed[:, 1] = rd * np.sin(theta) + cy
         return coords_transformed
 
     def rotate_shift_coordinates(self, angle, center=(0, 0), mirrored=False):
         """
         Rotate, flip or shift patterns in-plane
```

### Comparing `diffsims-0.5.2/diffsims/structure_factor/__init__.py` & `diffsims-0.6rc1/diffsims/structure_factor/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_factor.py` & `diffsims-0.6rc1/diffsims/structure_factor/atomic_scattering_factor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/structure_factor/atomic_scattering_parameters.py` & `diffsims-0.6rc1/diffsims/structure_factor/atomic_scattering_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/structure_factor/structure_factor.py` & `diffsims-0.6rc1/diffsims/structure_factor/structure_factor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/__init__.py` & `diffsims-0.6rc1/diffsims/tests/crystallography/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/crystallography/__init__.py` & `diffsims-0.6rc1/diffsims/tests/generators/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py` & `diffsims-0.6rc1/diffsims/tests/crystallography/test_reciprocal_lattice_vector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,14 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 from diffpy.structure import Atom, Lattice, Structure
 import numpy as np
 from orix.crystal_map import Phase
 from orix.vector import Miller, Vector3d
+
 import pytest
 
 from diffsims.crystallography import ReciprocalLatticeVector
 from diffsims.crystallography.reciprocal_lattice_vector import _get_set_per_hkl
 
 
 class TestReciprocalLatticeVector:
@@ -68,20 +69,28 @@
         is passed.
         """
         with pytest.raises(ValueError, match="Exactly one of "):
             _ = ReciprocalLatticeVector(nickel_phase, hkl=[1, 1, 1], hkil=[1, 1, -2, 1])
         with pytest.raises(ValueError, match="Exactly one of "):
             _ = ReciprocalLatticeVector(nickel_phase)
 
+    @pytest.mark.parametrize("include_zero_vector", [True, False])
     @pytest.mark.parametrize("d, desired_size", [(2, 18), (1, 92), (0.5, 750)])
-    def test_init_from_min_dspacing(self, ferrite_phase, d, desired_size):
+    def test_init_from_min_dspacing(
+        self, ferrite_phase, d, desired_size, include_zero_vector
+    ):
         """Class method gives desired number of vectors."""
-        rlv = ReciprocalLatticeVector.from_min_dspacing(ferrite_phase, d)
+        rlv = ReciprocalLatticeVector.from_min_dspacing(
+            ferrite_phase, d, include_zero_vector=include_zero_vector
+        )
+        if include_zero_vector:
+            desired_size += 1
         assert rlv.size == desired_size
 
+    @pytest.mark.parametrize("include_zero_vector", [True, False])
     @pytest.mark.parametrize(
         "hkl, desired_highest_hkl, desired_lowest_hkl, desired_size",
         [
             ([3, 3, 3], [3, 3, 3], [-3, -3, -3], 342),
             ([3, 4, 0], [3, 4, 0], [-3, -4, 0], 62),
             ([4, 3, 0], [4, 3, 0], [-4, -3, 0], 62),
         ],
@@ -89,17 +98,23 @@
     def test_init_from_highest_hkl(
         self,
         silicon_carbide_phase,
         hkl,
         desired_highest_hkl,
         desired_lowest_hkl,
         desired_size,
+        include_zero_vector,
     ):
         """Class method gives desired number of vectors and indices."""
-        rlv = ReciprocalLatticeVector.from_highest_hkl(silicon_carbide_phase, hkl)
+        rlv = ReciprocalLatticeVector.from_highest_hkl(
+            silicon_carbide_phase, hkl, include_zero_vector=include_zero_vector
+        )
+        if include_zero_vector:
+            desired_size += 1
+            desired_lowest_hkl = [0, 0, 0]
         assert np.allclose(rlv[0].hkl, desired_highest_hkl)
         assert np.allclose(rlv[-1].hkl, desired_lowest_hkl)
         assert rlv.size == desired_size
 
     def test_repr(self, ferrite_phase):
         """String representation gives desired (start of) string."""
         rlv = ReciprocalLatticeVector.from_min_dspacing(ferrite_phase, 2)
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/__init__.py` & `diffsims-0.6rc1/diffsims/tests/library/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/test_diffraction_generator.py` & `diffsims-0.6rc1/diffsims/tests/generators/test_diffraction_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -97,29 +97,29 @@
     if hasattr(x, "shape"):
         return (abs(x[..., 0]) < 6) * (abs(x[..., 1]) < 6)
     else:
         v = abs(x[0].reshape(-1, 1, 1)) < 6
         v = v * abs(x[1].reshape(1, -1, 1)) < 6
         return v + 0 * x[2].reshape(1, 1, -1)
 
+
 @pytest.mark.parametrize("model", [binary, linear, atanc, sin2c, lorentzian])
 def test_shape_factor_precession(model):
     excitation = np.array([-0.1, 0.1])
     r = np.array([1, 5])
     _ = _shape_factor_precession(excitation, r, 0.5, model, 0.1)
 
 
 def test_linear_shape_factor():
     excitation = np.array([-2, -1, -0.5, 0, 0.5, 1, 2])
     totest = linear(excitation, 1)
-    np.testing.assert_allclose(totest, np.array([0,0,0.5,1,0.5,0,0]))
+    np.testing.assert_allclose(totest, np.array([0, 0, 0.5, 1, 0.5, 0, 0]))
     np.testing.assert_allclose(linear(0.5, 1), 0.5)
 
 
-
 @pytest.mark.parametrize(
     "model, expected",
     [("linear", linear), ("lorentzian", lorentzian), (binary, binary)],
 )
 def test_diffraction_generator_init(model, expected):
     generator = DiffractionGenerator(300, shape_factor_model=model)
     assert generator.shape_factor_model == expected
@@ -198,15 +198,14 @@
         )
         assert np.all(smaller)
 
     def test_shape_factor_strings(self, diffraction_calculator, local_structure):
         _ = diffraction_calculator.calculate_ed_data(local_structure, 2)
 
     def test_shape_factor_custom(self, diffraction_calculator, local_structure):
-
         t1 = diffraction_calculator.calculate_ed_data(
             local_structure, 2, max_excitation_error=0.02
         )
         t2 = diffraction_calculator.calculate_ed_data(
             local_structure, 2, max_excitation_error=0.4
         )
 
@@ -245,40 +244,40 @@
         diffraction1 = dca.calculate_ed_data(local_structure, probe, 1)
         diffraction2 = dca.calculate_ed_data(
             local_structure, probe, 1, [0, 0], 200, False
         )
 
         np.testing.assert_allclose(diffraction1, diffraction2, 1e-6, 1e-6)
 
-    @pytest.mark.xfail(raises=NotImplementedError)
     def test_mode(self, diffraction_calculator_atomic, local_structure):
-        diffraction = diffraction_calculator_atomic.calculate_ed_data(
-            local_structure, probe, 1, mode="other"
-        )
+        with pytest.raises(NotImplementedError):
+            _ = diffraction_calculator_atomic.calculate_ed_data(
+                local_structure, probe, 1, mode="other"
+            )
 
-    @pytest.mark.xfail(raises=ValueError, strict=True)
     def test_bad_ZERO(self, diffraction_calculator_atomic, local_structure):
-        _ = diffraction_calculator_atomic.calculate_ed_data(
-            local_structure, probe, 1, ZERO=-1
-        )
+        with pytest.raises(ValueError):
+            _ = diffraction_calculator_atomic.calculate_ed_data(
+                local_structure, probe, 1, ZERO=-1
+            )
 
 
 @pytest.mark.parametrize("scattering_param", ["lobato", "xtables"])
 def test_param_check(scattering_param):
     generator = DiffractionGenerator(300, scattering_params=scattering_param)
 
 
-@pytest.mark.xfail(raises=NotImplementedError)
 def test_invalid_scattering_params():
     scattering_param = "_empty"
-    generator = DiffractionGenerator(300, scattering_params=scattering_param)
+    with pytest.raises(NotImplementedError):
+        _ = DiffractionGenerator(300, scattering_params=scattering_param)
 
 
-@pytest.mark.xfail(faises=NotImplementedError)
 def test_invalid_shape_model():
-    generator = DiffractionGenerator(300, shape_factor_model="dracula")
+    with pytest.raises(NotImplementedError):
+        _ = DiffractionGenerator(300, shape_factor_model="dracula")
 
 
 @pytest.mark.parametrize("shape", [(10, 20), (20, 10)])
 def test_param_check_atomic(shape):
     detector = [np.linspace(-1, 1, s) for s in shape]
-    generator = AtomicDiffractionGenerator(300, detector, True)
+    _ = AtomicDiffractionGenerator(300, detector, True)
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/test_library_generator.py` & `diffsims-0.6rc1/diffsims/tests/generators/test_library_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/test_rotation_list_generator.py` & `diffsims-0.6rc1/diffsims/tests/generators/test_rotation_list_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -83,17 +83,17 @@
         ("cubic", 300),
         ("hexagonal", 1050),
         ("trigonal", 1657),
         ("tetragonal", 852),
         ("orthorhombic", 1657),
         ("monoclinic", 6441),
         ("triclinic", 12698),
-    ]
+    ],
 )
 def test_get_beam_directions_grid_size(crystal_system, desired_size):
     grid = get_beam_directions_grid(crystal_system, 2)
     assert grid.shape[0] == desired_size
 
 
-@pytest.mark.xfail()
 def test_invalid_mesh_beam_directions():
-    _ = get_beam_directions_grid("cubic", 10, mesh="invalid")
+    with pytest.raises(NotImplementedError):
+        _ = get_beam_directions_grid("cubic", 10, mesh="invalid")
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/test_sphere_mesh_generators.py` & `diffsims-0.6rc1/diffsims/tests/generators/test_sphere_mesh_generators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/generators/test_zap_map_generator.py` & `diffsims-0.6rc1/diffsims/tests/generators/test_zap_map_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -47,15 +47,15 @@
         assert np.allclose(r_to_x, (90, 90, -90))
 
     def test_rotation_to_static_y_axis(self, sample_system):
         r_to_y = get_rotation_from_z_to_direction(sample_system, [0, 1, 0])
         assert np.allclose(r_to_y, (180, 90, -180))
 
     def test_rotations_to_static_yz(self, sample_system):
-        """ We rotate from z towards y, and compare the results to geometry"""
+        """We rotate from z towards y, and compare the results to geometry"""
         r_to_yz = get_rotation_from_z_to_direction(sample_system, [0, 1, 1])
         tan_angle = np.tan(np.deg2rad(r_to_yz[1]))
         tan_lattice = sample_system.lattice.b / sample_system.lattice.c
         assert np.allclose(tan_angle, tan_lattice, atol=1e-5)
 
 
 @pytest.mark.parametrize(
@@ -66,15 +66,15 @@
     z_dict = generate_zap_map(default_structure, default_simulator, system=system)
     assert (0, 0, 1) in z_dict.keys()
     assert (0, 0, 0) not in z_dict.keys()
 
 
 @pytest.mark.parametrize("density", ["3", "7"])
 def test_zap_map_density_changes(default_structure, default_simulator, density):
-    """ Checks density arguments are passed correctly """
+    """Checks density arguments are passed correctly"""
     z_dict = generate_zap_map(default_structure, default_simulator, density=density)
     if density == "3":
         assert str(len(z_dict.keys())) == "3"
     elif density == "7":
         assert len(z_dict.keys()) > 5  # monoclinic case gives 6 rather than 7
```

### Comparing `diffsims-0.5.2/diffsims/tests/library/__init__.py` & `diffsims-0.6rc1/diffsims/tests/patterns/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/library/test_diffraction_library.py` & `diffsims-0.6rc1/diffsims/tests/library/test_diffraction_library.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,16 +12,14 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-import os
-
 import numpy as np
 import pytest
 
 from diffsims.generators.diffraction_generator import DiffractionGenerator
 from diffsims.generators.library_generator import DiffractionLibraryGenerator
 from diffsims.libraries.diffraction_library import load_DiffractionLibrary
 from diffsims.libraries.structure_library import StructureLibrary
@@ -54,18 +52,17 @@
     alpha = get_library.get_library_entry(phase="Phase", angle=(0, 0, 0))["intensities"]
     beta = get_library.get_library_entry(phase="Phase", angle=(1e-8, 0, 0))[
         "intensities"
     ]
     assert np.allclose(alpha, beta)
 
 
-def test_library_io(get_library):
-    get_library.pickle_library("file_01.pickle")
-    loaded_library = load_DiffractionLibrary("file_01.pickle", safety=True)
-    os.remove("file_01.pickle")
+def test_library_io(get_library, pickle_temp_file):
+    get_library.pickle_library(pickle_temp_file)
+    loaded_library = load_DiffractionLibrary(pickle_temp_file, safety=True)
     # We can't check that the entire libraries are the same as the memory
     # location of the 'Sim' changes
     for i in range(len(get_library["Phase"]["orientations"])):
         np.testing.assert_allclose(
             get_library["Phase"]["orientations"][i],
             loaded_library["Phase"]["orientations"][i],
         )
@@ -92,11 +89,11 @@
     with pytest.raises(ValueError, match="It appears that no library entry lies"):
         assert isinstance(
             get_library.get_library_entry(phase="Phase", angle=(1e-1, 0, 0))["Sim"],
             DiffractionSimulation,
         )
 
 
-def test_unsafe_loading(get_library):
+def test_unsafe_loading(get_library, pickle_temp_file):
     with pytest.raises(RuntimeError, match="Unpickling is risky, turn safety to True "):
-        get_library.pickle_library("file_01.pickle")
-        _ = load_DiffractionLibrary("file_01.pickle")
+        get_library.pickle_library(pickle_temp_file)
+        _ = load_DiffractionLibrary(pickle_temp_file)
```

### Comparing `diffsims-0.5.2/diffsims/tests/library/test_structure_library.py` & `diffsims-0.6rc1/diffsims/tests/library/test_structure_library.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -40,27 +40,17 @@
     np.testing.assert_equal(library.identifiers, identifiers)
     np.testing.assert_equal(library.structures, structures)
     np.testing.assert_equal(library.orientations, orientations)
     np.testing.assert_equal(library.struct_lib["a"], (1, 3))
     np.testing.assert_equal(library.struct_lib["b"], (2, 4))
 
 
-@pytest.mark.xfail(reason="Functionality removed")
-def test_from_systems_methods():
-    identifiers = ["a", "b"]
-    structures = [1, 2]
-    systems = ["cubic", "hexagonal"]
-    library = StructureLibrary.from_crystal_systems(
-        identifiers, structures, systems, resolution=2
-    )
-
-
 @pytest.mark.parametrize(
     "identifiers, structures, orientations",
     [
         (["a"], [1, 2], [3, 4]),
         (["a"], [1], [3, 4]),
     ],
 )
-@pytest.mark.xfail(raises=ValueError)
 def test_constructor_parameter_validation_errors(identifiers, structures, orientations):
-    StructureLibrary(identifiers, structures, orientations)
+    with pytest.raises(ValueError):
+        _ = StructureLibrary(identifiers, structures, orientations)
```

### Comparing `diffsims-0.5.2/diffsims/tests/library/test_vector_library.py` & `diffsims-0.6rc1/diffsims/tests/library/test_vector_library.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -13,15 +13,14 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import pytest
-import os
 import numpy as np
 
 from diffsims.generators.library_generator import (
     VectorLibraryGenerator,
     _generate_lookup_table,
 )
 
@@ -34,31 +33,30 @@
     structure_library = StructureLibrary(
         ["Phase"], [default_structure], [[(0, 0, 0), (0, 0.2, 0)]]
     )
     vlg = VectorLibraryGenerator(structure_library)
     return vlg.get_vector_library(0.5)
 
 
-def test_library_io(get_library):
-    get_library.pickle_library("file_01.pickle")
-    loaded_library = load_VectorLibrary("file_01.pickle", safety=True)
-    os.remove("file_01.pickle")
+def test_library_io(get_library, pickle_temp_file):
+    get_library.pickle_library(pickle_temp_file)
+    loaded_library = load_VectorLibrary(pickle_temp_file, safety=True)
     # we can't check that the entire libraries are the same as the memory
     # location of the 'Sim' changes
     np.testing.assert_allclose(
         get_library["Phase"]["measurements"], loaded_library["Phase"]["measurements"]
     )
     np.testing.assert_allclose(
         get_library["Phase"]["indices"], loaded_library["Phase"]["indices"]
     )
 
 
-@pytest.mark.xfail(raises=RuntimeError)
-def test_unsafe_loading(get_library):
-    get_library.pickle_library("file_01.pickle")
-    loaded_library = load_VectorLibrary("file_01.pickle")
+def test_unsafe_loading(get_library, pickle_temp_file):
+    get_library.pickle_library(pickle_temp_file)
+    with pytest.raises(RuntimeError):
+        _ = load_VectorLibrary(pickle_temp_file)
 
 
 def test_generate_lookup_table(default_structure):
     lattice = default_structure.lattice.reciprocal()
-    table = _generate_lookup_table(lattice, 0.5, unique=True)
-    table = _generate_lookup_table(lattice, 0.5, unique=False)
+    _ = _generate_lookup_table(lattice, 0.5, unique=True)
+    _ = _generate_lookup_table(lattice, 0.5, unique=False)
```

### Comparing `diffsims-0.5.2/diffsims/tests/patterns/__init__.py` & `diffsims-0.6rc1/diffsims/tests/sims/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/patterns/test_detector_functions.py` & `diffsims-0.6rc1/diffsims/tests/patterns/test_detector_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -41,18 +41,18 @@
     dmax = int(max / 3)
     z = constrain_to_dynamic_range(pattern, detector_max=dmax)
     assert np.max(z) == dmax
     assert not np.may_share_memory(pattern, z)
 
 
 class TestReturnsareCopies:
-    """ We want pattern to remain untouched by the noise addition """
+    """We want pattern to remain untouched by the noise addition"""
 
     def test_copy_shot_and_point_spread(self, pattern):
-        """ Also covers shot/point independantly """
+        """Also covers shot/point independantly"""
         z = add_shot_and_point_spread(pattern, 2, shot_noise=True)
         assert not np.may_share_memory(pattern, z)
 
     def test_copy_gaussian(self, pattern):
         z = add_gaussian_noise(pattern, 2)
         assert not np.may_share_memory(pattern, z)
 
@@ -78,79 +78,79 @@
         z2 = add_shot_and_point_spread(pattern, 2, shot_noise=True, seed=8)
         assert np.allclose(z1a, z1b)
         assert not np.allclose(z1a, z2)
 
 
 class TestShotNoise:
     def test_seed_duplicates(self, pattern):
-        """ Same seed should imply same result """
+        """Same seed should imply same result"""
         z1 = add_shot_noise(pattern, seed=7)
         z2 = add_shot_noise(pattern, seed=7)
         assert np.allclose(z1, z2)
 
     def test_seed_unduplicates(self, pattern):
-        """ Different seeds should (almost always) give different results"""
+        """Different seeds should (almost always) give different results"""
         z1 = add_shot_noise(pattern, seed=7)
         z2 = add_shot_noise(pattern, seed=312)
         z3 = add_shot_noise(pattern, seed=None)
         assert not np.allclose(z1, z2)
         assert not np.allclose(z1, z3)
 
 
 class TestGaussianNoise:
     def test_seed_duplicates(self, pattern):
-        """ Same seed should imply same result """
+        """Same seed should imply same result"""
         z1 = add_gaussian_noise(pattern, sigma=3, seed=7)
         z2 = add_gaussian_noise(pattern, sigma=3, seed=7)
         assert np.allclose(z1, z2)
 
 
 class TestDeadPixel:
     def test_seed_duplicates(self, pattern):
-        """ Same seed should imply same result """
+        """Same seed should imply same result"""
         pattern = pattern + 1  # so that we can detect dead pixels
         z1 = add_dead_pixels(pattern, n=6, seed=7)
         z2 = add_dead_pixels(pattern, n=6, seed=7)
         assert np.allclose(z1, z2)
         assert np.sum(z1 == 0) == 6  # we should have 6 dead pixels!
 
     def test_frac_kwarg(self, pattern):
         pattern = pattern + 1  # so that we can detect dead pixels
         pattern_size = pattern.shape[0] * pattern.shape[1]
         fraction = 6 / pattern_size
         z1 = add_dead_pixels(pattern, fraction=fraction)
         assert np.sum(z1 == 0) == 6  # we should have 6 dead pixels!
 
-    @pytest.mark.xfail(strict=True)
     def test_bad_kwarg_choices_a(self, pattern):
-        _ = add_dead_pixels(pattern, n=None, fraction=None)
+        with pytest.raises(ValueError):
+            _ = add_dead_pixels(pattern, n=None, fraction=None)
 
-    @pytest.mark.xfail(strict=True)
     def test_bad_kwarg_choices_b(self, pattern):
-        _ = add_dead_pixels(pattern, n=6, fraction=0.2)
+        with pytest.raises(ValueError):
+            _ = add_dead_pixels(pattern, n=6, fraction=0.2)
 
 
 class TestDetectorGainOffset:
     def test_gain_scalar(self, pattern):
-        """ Tests scalar gains are invertible """
+        """Tests scalar gains are invertible"""
         g1 = add_linear_detector_gain(pattern, 1.1)
         g2 = add_linear_detector_gain(g1, 1 / 1.1)
         assert np.allclose(pattern, g2)
 
     def test_gain_array(self, pattern):
-        """ Test array gain are invertible """
+        """Test array gain are invertible"""
         pattern = pattern + 1  # avoids problems inverting zeroes
         g1 = add_linear_detector_gain(pattern, pattern)
         g2 = add_linear_detector_gain(g1, np.divide(1, pattern))
         assert np.allclose(pattern, g2)
 
     def test_offset_scalar(self, pattern):
-        """ Test postive scalar offsets are invertible """
+        """Test postive scalar offsets are invertible"""
         g1 = add_detector_offset(pattern, 3)
         g2 = add_detector_offset(g1, -3)
         assert np.allclose(pattern, g2)
 
     def test_offset_array(self, pattern):
-        """ Test postive array offsets are invertible """
+        """Test postive array offsets are invertible"""
         g1 = add_detector_offset(pattern, pattern)
         g2 = add_detector_offset(g1, -pattern)
         assert np.allclose(pattern, g2)
```

### Comparing `diffsims-0.5.2/diffsims/tests/sims/__init__.py` & `diffsims-0.6rc1/diffsims/tests/simulations/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/sims/test_diffraction_simulation.py` & `diffsims-0.6rc1/diffsims/tests/sims/test_diffraction_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,19 +12,21 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
+import matplotlib.pyplot as plt
 import numpy as np
 import pytest
 
 from diffsims.sims.diffraction_simulation import (
-    DiffractionSimulation, ProfileSimulation
+    DiffractionSimulation,
+    ProfileSimulation,
 )
 
 
 def test_wrong_calibration_setting():
     with pytest.raises(ValueError, match="must be a float"):
         DiffractionSimulation(
             coordinates=np.asarray([[0.3, 1.2, 0]]),
@@ -81,14 +83,15 @@
             (4, 4, 4),
         ],
     )
 
 
 def test_plot_profile_simulation(profile_simulation):
     profile_simulation.get_plot()
+    plt.close()
 
 
 class TestDiffractionSimulation:
     @pytest.fixture
     def diffraction_simulation(self):
         return DiffractionSimulation(
             np.array([[0, 0, 0], [1, 2, 3], [3, 4, 5]], dtype=float)
@@ -100,15 +103,15 @@
             np.array([[0, 0, 0], [1, 2, 3], [3, 4, 5]], dtype=float), calibration=0.5
         )
 
     def test_failed_initialization(self):
         with pytest.raises(ValueError, match="Coordinate"):
             DiffractionSimulation(
                 np.array([[0, 0, 0], [1, 2, 3], [3, 4, 5]], dtype=float),
-                indices=np.array([1, 2, 3])
+                indices=np.array([1, 2, 3]),
             )
 
     def test_init(self, diffraction_simulation):
         assert np.allclose(
             diffraction_simulation.coordinates, np.array([[1, 2, 3], [3, 4, 5]])
         )
         assert np.isnan(diffraction_simulation.indices).all()
@@ -315,8 +318,10 @@
                     [2.1, 3.4, 0],
                 ]
             ),
             indices=np.array([[-2, 3, 4], [2, -6, 1], [0, 0, 0]]),
             intensities=np.array([3.0, 5.0, 2.0]),
             calibration=[1, 2],
         )
-        ax, sp = short_sim.plot(units=units_in, show_labels=True)
+        _ = short_sim.plot(units=units_in, show_labels=True)
+
+        plt.close()
```

### Comparing `diffsims-0.5.2/diffsims/tests/structure_factor/__init__.py` & `diffsims-0.6rc1/diffsims/tests/structure_factor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_factor.py` & `diffsims-0.6rc1/diffsims/tests/structure_factor/test_atomic_scattering_factor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py` & `diffsims-0.6rc1/diffsims/tests/structure_factor/test_atomic_scattering_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/structure_factor/test_structure_factor.py` & `diffsims-0.6rc1/diffsims/tests/structure_factor/test_structure_factor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/__init__.py` & `diffsims-0.6rc1/diffsims/tests/utils/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_atomic_diffraction_generator_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -123,15 +123,15 @@
         ((10, 20, 1), 1e10),
     ],
 )
 def test_grid2sphere(shape, rad):
     x = [np.linspace(-1, 1, s) if s > 1 else np.array([0]) for s in shape]
     X = to_mesh(x)
     Y = to_mesh((x[0], x[1], np.array([0]))).reshape(-1, 3)
-    w = 1 / (1 + (Y ** 2).sum(-1) / rad ** 2)
+    w = 1 / (1 + (Y**2).sum(-1) / rad**2)
     Y *= w[..., None]
     Y[:, 2] = rad * (1 - w)
     Y = Y.reshape(shape[0], shape[1], 3)
 
     for i in range(3):
         np.testing.assert_allclose(
             Y[..., i], grid2sphere(X[..., i], x, None, rad), 1e-4, 1e-4
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_discretise_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_discretise_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -58,41 +58,31 @@
         assert f.min() >= 0
     else:
         assert a.min() >= 0 or Z == 19
         assert b.min() >= 0
         assert len(a) == len(b)
 
 
-@pytest.mark.xfail(raises=ValueError)
-def test_2_atoms_getA():
-    get_atoms(np.array([0, 1]))
-
-
-@pytest.mark.xfail(raises=ValueError)
-def test_max_atom_getA():
-    get_atoms("Es")
+@pytest.mark.parametrize("atoms", [np.array([0, 1]), "Es"])
+def tests_get_atoms_raises(atoms):
+    with pytest.raises(ValueError):
+        get_atoms(atoms)
 
 
 @pytest.mark.parametrize(
     "r",
     [
         0.5,
         pytest.param(0.1, marks=pytest.mark.xfail),
         pytest.param(0.1, marks=pytest.mark.xfail),
     ],
 )
 def test_rebin(r):
     x = [np.linspace(0, 1, 10), np.linspace(0, 1, 21), np.linspace(0, 1, 32)]
-    loc = np.concatenate(
-        [
-            0 * np.linspace(0, 1, 500)[:, None],
-        ]
-        * 3,
-        axis=1,
-    )
+    loc = np.concatenate([0 * np.linspace(0, 1, 500)[:, None]] * 3, axis=1)
     k = 1
     mem = 1e5
     rebin(x, loc, r, k, mem)
 
 
 @pytest.mark.parametrize(
     "n, shape",
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_fourier_transform.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_fourier_transform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -202,17 +202,17 @@
 
     for FT in (ft, ft1, ft2):
         np.testing.assert_allclose(g, FT(f, axes=axes), 1e-5, 1e-5)
     for IFT in (ift, ift1, ift2):
         np.testing.assert_allclose(f, IFT(g, axes=axes), 1e-5, 1e-5)
 
 
-@pytest.mark.xfail(raises=ValueError)
 def test_fail_DFT():
-    get_DFT()
+    with pytest.raises(ValueError):
+        get_DFT()
 
 
 @pytest.mark.parametrize(
     "shape1, shape2, n1, n2, dx",
     [
         ([10], [10], 1, 5, None),
         ([10, 1], [10, 10], 2, 6, 1),
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_generic_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_generic_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_kinematic_simulation_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_kinematic_simulation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -123,15 +123,15 @@
         ((10, 20, 1), 1e10),
     ],
 )
 def test_grid2sphere(shape, rad):
     x = [np.linspace(-1, 1, s) if s > 1 else np.array([0]) for s in shape]
     X = to_mesh(x)
     Y = to_mesh((x[0], x[1], np.array([0]))).reshape(-1, 3)
-    w = 1 / (1 + (Y ** 2).sum(-1) / rad ** 2)
+    w = 1 / (1 + (Y**2).sum(-1) / rad**2)
     Y *= w[..., None]
     Y[:, 2] = rad * (1 - w)
     Y = Y.reshape(shape[0], shape[1], 3)
 
     for i in range(3):
         np.testing.assert_allclose(
             Y[..., i], grid2sphere(X[..., i], x, None, rad), 1e-4, 1e-4
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_mask_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_mask_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -24,30 +24,30 @@
     mask = mu.create_mask((20, 10))
     assert mask.shape[0] == 20
     assert mask.shape[1] == 10
 
 
 def test_invert_mask():
     mask = mu.create_mask((20, 10))
-    initial = mask[0,0]
+    initial = mask[0, 0]
     mu.invert_mask(mask)
-    assert initial != mask[0,0]
+    assert initial != mask[0, 0]
 
 
 def test_add_polygon():
     mask = mu.create_mask((20, 10))
-    coords = np.array([[5, 5],[15, 5],[10,10]])
+    coords = np.array([[5, 5], [15, 5], [10, 10]])
     mu.add_polygon_to_mask(mask, coords)
 
 
 def test_add_circles_to_mask():
     mask = mu.create_mask((20, 10))
-    coords = np.array([[5, 5],[15, 5],[10,10]])
+    coords = np.array([[5, 5], [15, 5], [10, 10]])
     mu.add_circles_to_mask(mask, coords, 3)
-    
+
 
 def test_add_circle_to_mask():
     mask = mu.create_mask((20, 10))
     mu.add_circle_to_mask(mask, 5, 5, 5)
 
 
 def test_add_annulus_to_mask():
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_probe_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_probe_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -81,18 +81,18 @@
     ]
     primes = np.array(primes, dtype=int)[::3]
     for i, j in enumerate(primes[n:]):
         x[::j] += i * (-1) ** j
     return x.reshape(shape)
 
 
-@pytest.mark.xfail(raises=NotImplementedError)
 def test_null_probe():
     p = ProbeFunction()
-    p(1)
+    with pytest.raises(NotImplementedError):
+        p(1)
 
 
 @pytest.fixture(params=[(10, 11, 12)])
 def simple_mesh(request):
     return [np.linspace(-1, 1, n) for n in request.param]
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_ring_pattern_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_ring_pattern_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_sim_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_sim_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -110,33 +110,33 @@
         300.0,
         simulation_size=32,
         illumination="gaussian_probe",
         scattering_params="xtables",
     )
 
 
-@pytest.mark.xfail(raises=NotImplementedError)
 def test_kinematic_simulator_invalid_scattering_params():
     atomic_coordinates = np.asarray([[0, 0, 0]])  # structure.cart_coords
-    sim = simulate_kinematic_scattering(
-        atomic_coordinates,
-        "Si",
-        300.0,
-        simulation_size=32,
-        illumination="gaussian_probe",
-        scattering_params="_empty",
-    )
+    with pytest.raises(NotImplementedError):
+        simulate_kinematic_scattering(
+            atomic_coordinates,
+            "Si",
+            300.0,
+            simulation_size=32,
+            illumination="gaussian_probe",
+            scattering_params="_empty",
+        )
 
 
-@pytest.mark.xfail(raises=ValueError)
 def test_kinematic_simulator_invalid_illumination():
     atomic_coordinates = np.asarray([[0, 0, 0]])  # structure.cart_coords
-    sim = simulate_kinematic_scattering(
-        atomic_coordinates, "Si", 300.0, simulation_size=32, illumination="gaussian"
-    )
+    with pytest.raises(ValueError):
+        simulate_kinematic_scattering(
+            atomic_coordinates, "Si", 300.0, simulation_size=32, illumination="gaussian"
+        )
 
 
 @pytest.mark.parametrize(
     "uvtw, uvw",
     [
         ((0, 0, 0, 1), (0, 0, 1)),
         ((1, 0, 0, 1), (2, 1, 1)),
@@ -147,15 +147,15 @@
     val = uvtw_to_uvw(uvtw)
     np.testing.assert_almost_equal(val, uvw)
 
 
 class TestHolzCalibration:
     def test_get_holz_angle(self):
         wavelength = 2.51 / 1000
-        lattice_parameter = 0.3905 * 2 ** 0.5
+        lattice_parameter = 0.3905 * 2**0.5
         angle = get_holz_angle(wavelength, lattice_parameter)
         assert np.isclose(angle, 0.095378, rtol=1e-4)
 
     def test_scattering_angle_to_lattice_parameter(self):
         wavelength = 2.51 / 1000
         angle = 95.37805 / 1000
         lattice_size = scattering_angle_to_lattice_parameter(wavelength, angle)
```

### Comparing `diffsims-0.5.2/diffsims/tests/utils/test_vector_utils.py` & `diffsims-0.6rc1/diffsims/tests/utils/test_vector_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -15,16 +15,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 import pytest
 
-from diffsims.utils.vector_utils import get_angle_cartesian
-from diffsims.utils.vector_utils import get_angle_cartesian_vec
+from diffsims.utils.vector_utils import get_angle_cartesian, get_angle_cartesian_vec
 
 
 @pytest.mark.parametrize(
     "vec_a, vec_b, expected_angle",
     [([0, 0, 1], [0, 1, 0], np.deg2rad(90)), ([0, 0, 0], [0, 0, 1], 0)],
 )
 def test_get_angle_cartesian(vec_a, vec_b, expected_angle):
@@ -43,10 +42,10 @@
     ],
 )
 def test_get_angle_cartesian_vec(a, b, expected_angles):
     angles = get_angle_cartesian_vec(a, b)
     np.testing.assert_allclose(angles, expected_angles)
 
 
-@pytest.mark.xfail(raises=ValueError)
 def test_get_angle_cartesian_vec_input_validation():
-    get_angle_cartesian_vec(np.empty((2, 3)), np.empty((5, 3)))
+    with pytest.raises(ValueError):
+        get_angle_cartesian_vec(np.empty((2, 3)), np.empty((5, 3)))
```

### Comparing `diffsims-0.5.2/diffsims/utils/__init__.py` & `diffsims-0.6rc1/diffsims/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/utils/atomic_diffraction_generator_utils.py` & `diffsims-0.6rc1/diffsims/utils/atomic_diffraction_generator_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,31 +12,38 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-"""
-Back end for computing diffraction patterns with a kinematic model.
+"""Back-end for computing diffraction patterns with a kinematic model.
 """
 
-from diffsims.utils.discretise_utils import get_discretisation
 from numpy import array, pi, sin, cos, empty
 from scipy.interpolate import interpn
+
+from diffsims.utils.discretise_utils import get_discretisation
 from diffsims.utils.fourier_transform import (
     get_DFT,
     to_recip,
     fftshift_phase,
     plan_fft,
     fast_abs,
 )
 from diffsims.utils.generic_utils import to_mesh
 
 
+__all__ = [
+    "get_diffraction_image",
+    "grid2sphere",
+    "precess_mat",
+]
+
+
 def normalise(arr):
     return arr / arr.max()
 
 
 def get_diffraction_image(
     coordinates,
     species,
@@ -198,15 +205,15 @@
             return arr
         elif arr.shape[2] == 1:
             return arr[:, :, 0]
 
     y = to_mesh((x[0], x[1], array([0])), dx).reshape(-1, 3)
 
     if C is not None:  # project on line to centre
-        w = 1 / (1 + (y ** 2).sum(-1) / C ** 2)
+        w = 1 / (1 + (y**2).sum(-1) / C**2)
         y *= w[:, None]
         if dx is None:
             y[:, 2] = C * (1 - w)
         else:
             y += C * (1 - w)[:, None] * dx[2]
 
     out = interpn(x, arr, y, method="linear", bounds_error=False, fill_value=0)
```

### Comparing `diffsims-0.5.2/diffsims/utils/atomic_scattering_params.py` & `diffsims-0.6rc1/diffsims/utils/atomic_scattering_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/utils/discretise_utils.py` & `diffsims-0.6rc1/diffsims/utils/discretise_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,17 +12,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Utils for converting lists of atoms to a discretised volume
+"""Utils for converting lists of atoms to a discretised volume."""
 
-"""
+from math import (
+    sqrt as c_sqrt,
+    exp as c_exp,
+    erf as c_erf,
+    ceil,
+    cos as c_cos,
+    sin as c_sin,
+    floor,
+)
 
 from numpy import (
     unique,
     require,
     array,
     arange,
     ones,
@@ -32,30 +40,28 @@
     ascontiguousarray,
     sqrt,
     random,
     isscalar,
     exp,
     prod,
 )
-from diffsims.utils.generic_utils import get_grid
 from psutil import virtual_memory
 import numba
-from .generic_utils import _CUDA, cuda
 
-c_abs = abs
-from math import (
-    sqrt as c_sqrt,
-    exp as c_exp,
-    erf as c_erf,
-    ceil,
-    cos as c_cos,
-    sin as c_sin,
-    floor,
-)
+from diffsims.utils.generic_utils import get_grid, _CUDA, cuda
+
+__all__ = [
+    "do_binning",
+    "get_atoms",
+    "get_discretisation",
+    "rebin",
+    "ATOMIC_SCATTERING_PARAMS_PENG",
+]
 
+c_abs = abs
 FTYPE, CTYPE = "f8", "c16"
 c_FTYPE = numba.float64 if FTYPE[1] == "8" else numba.float32
 
 
 ##########
 # Look-up table of atoms
 ##########
@@ -86,15 +92,15 @@
     """
     if isscalar(Z):
         Z = array([Z])
     if Z.dtype.char not in "US":
         Z = Z.astype(int)
     Z = unique(Z)
     if Z.size > 1:
-        raise ValueError("Only 1 atom can generated at once")
+        raise ValueError("Only 1 atom can be generated at once")
     else:
         Z = Z[0]
     if Z == 0:
         # Mimics a Dirac spike
         a = array([1] * 5 + [0.1] * 5).reshape(2, -1).T
     elif Z.dtype.char not in "US":
         a = array(ATOMIC_SCATTERING_PARAMS_PENG[keys[Z]])
@@ -504,15 +510,14 @@
 
 
 # Coverage: Cuda code is not tested by travis
 if _CUDA:  # pragma: no cover
 
     @cuda.jit
     def __density3D_pw_gpu(x0, x1, x2, xmin, loc, sublist, r, a, d, B, precomp, h, out):
-
         i0, i1, i2 = cuda.grid(3)
         if i0 >= x0.size or i1 >= x1.size or i2 >= x2.size:
             return
         X0, X1, X2 = x0[i0], x1[i1], x2[i2]
         Y0, Y1, Y2 = 0, 0, 0
 
         bin0 = int((X0 - xmin[0]) / r[0])
@@ -534,15 +539,14 @@
             Y1 = loc[j0, 1] - X1
             Y2 = loc[j0, 2] - X2
             Sum += __atom_pw_gpu(Y0, Y1, Y2, precomp, h)
         out[i0, i1, i2] = Sum
 
     @cuda.jit
     def __density3D_av_gpu(x0, x1, x2, xmin, loc, sublist, r, a, d, B, precomp, h, out):
-
         i0, i1, i2 = cuda.grid(3)
         if i0 >= x0.size or i1 >= x1.size or i2 >= x2.size:
             return
         X0, X1, X2 = x0[i0], x1[i1], x2[i2]
         Y0, Y1, Y2 = 0, 0, 0
 
         bin0 = int((X0 - xmin[0]) / r[0])
@@ -631,36 +635,36 @@
         The cut-off radius for this atom
 
     """
 
     if pw:
         n_zeros = sum(1 for D in d if D == 0)
         f = lambda x: sum(
-            a[i] * c_exp(-b[i] * x ** 2) * (pi / b[i]) ** (n_zeros / 2)
+            a[i] * c_exp(-b[i] * x**2) * (pi / b[i]) ** (n_zeros / 2)
             for i in range(a.size)
         )
         Rmax = 0.1
         while f(Rmax) >= ZERO * f(0):
             Rmax *= 1.1
         h = max(Rmax / 500, max(d) / 10)
-        pms = array([Rmax ** 2, 1 / h], dtype=dtype)
+        pms = array([Rmax**2, 1 / h], dtype=dtype)
         precomp = array([f(x) for x in arange(0, Rmax + 2 * h, h)], dtype=dtype)
 
     else:
 
         def f(i, j, x):
             A = a[i] ** (1 / 3)  # factor spread evenly over 3 dimensions
             B = b[i] ** 0.5
             if d[j] == 0:
                 return A * 2 / B
             return (
                 A
                 * (c_erf(B * (x + d[j] / 2)) - c_erf(B * (x - d[j] / 2)))
                 / (2 * d[j] * B)
-                * pi ** 0.5
+                * pi**0.5
             )
 
         h = [D / 10 for D in d]
         Rmax = ones([a.size, 3], dtype=dtype) / 10
         L = 1
         for i in range(a.size):
             for j in range(3):
```

### Comparing `diffsims-0.5.2/diffsims/utils/fourier_transform.py` & `diffsims-0.6rc1/diffsims/utils/fourier_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -24,14 +24,31 @@
 @author: Rob Tovey
 """
 
 from numpy import array, pi, inf, ceil, exp, isscalar, prod, require, empty
 from numpy.fft import fftfreq
 import numba
 
+
+__all__ = [
+    "convolve",
+    "fast_abs",
+    "fast_fft_len",
+    "fftn",
+    "fftshift_phase",
+    "from_recip",
+    "get_DFT",
+    "get_recip_points",
+    "ifftn",
+    "plan_fft",
+    "plan_ifft",
+    "to_recip",
+]
+
+
 # This section produces 6 utilities:
 #    fftn, ifftn, ifftshift, fftshift, plan_fft, plan_ifft
 # By default, uses the pyfftw implementations. If a lot of identical ffts are
 # needed then use the planning functions.
 # Coverage: pyfftw is not tested by travis
 try:  # pragma: no cover
     import pyfftw
@@ -195,15 +212,14 @@
             auto_align_input,
             auto_contiguous,
             avoid_copy,
             norm,
         )
         return plan, plan.input_array
 
-
 except ImportError:
     # Only scipy has a next_fast_len, usually numpy is a little faster
     # (note they are not identical)
     from scipy.fftpack import fftn, ifftn, ifftshift, fftshift, next_fast_len
     from numpy.fft import fftn, ifftn, ifftshift, fftshift
 
     _fftn, _ifftn = fftn, ifftn
```

### Comparing `diffsims-0.5.2/diffsims/utils/generic_utils.py` & `diffsims-0.6rc1/diffsims/utils/generic_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -22,15 +22,23 @@
 Generic tools for all areas of code.
 
 @author: Rob Tovey
 """
 from numpy import isscalar, zeros, array
 import numba
 
-# Coverage: Cuda code is not tested by travis
+
+__all__ = [
+    "GLOBAL_BOOL",
+    "get_grid",
+    "to_mesh",
+]
+
+
+# Coverage: Cuda code is not tested
 try:  # pragma: no cover
     from numba import cuda
 
     __CUDA = cuda.is_available()
 except Exception:  # pragma: no cover
     cuda = None
     __CUDA = False
```

### Comparing `diffsims-0.5.2/diffsims/utils/kinematic_simulation_utils.py` & `diffsims-0.6rc1/diffsims/utils/kinematic_simulation_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -19,27 +19,36 @@
 """
 Created on 1 Nov 2019
 
 Back end for computing diffraction patterns with a kinematic model.
 
 @author: Rob Tovey
 """
-from diffsims.utils.discretise_utils import get_discretisation
 from numpy import array, pi, sin, cos, empty
 from scipy.interpolate import interpn
+
+from diffsims.utils.discretise_utils import get_discretisation
 from diffsims.utils.fourier_transform import (
     get_DFT,
     to_recip,
     fftshift_phase,
     plan_fft,
     fast_abs,
 )
 from diffsims.utils.generic_utils import to_mesh
 
 
+__all__ = [
+    "get_diffraction_image",
+    "grid2sphere",
+    "normalise",
+    "precess_mat",
+]
+
+
 def normalise(arr):
     return arr / arr.max()
 
 
 def get_diffraction_image(
     coordinates,
     species,
@@ -201,15 +210,15 @@
             return arr
         elif arr.shape[2] == 1:
             return arr[:, :, 0]
 
     y = to_mesh((x[0], x[1], array([0])), dx).reshape(-1, 3)
 
     if C is not None:  # project on line to centre
-        w = 1 / (1 + (y ** 2).sum(-1) / C ** 2)
+        w = 1 / (1 + (y**2).sum(-1) / C**2)
         y *= w[:, None]
         if dx is None:
             y[:, 2] = C * (1 - w)
         else:
             y += C * (1 - w)[:, None] * dx[2]
 
     out = interpn(x, arr, y, method="linear", bounds_error=False, fill_value=0)
```

### Comparing `diffsims-0.5.2/diffsims/utils/lobato_scattering_params.py` & `diffsims-0.6rc1/diffsims/utils/lobato_scattering_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/utils/mask_utils.py` & `diffsims-0.6rc1/diffsims/utils/mask_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -50,15 +50,15 @@
 
     Returns
     -------
     None:
         the mask is adjusted inplace
     """
     coords = np.array(coords)
-    coords = np.ravel(coords, order='C').tolist()
+    coords = np.ravel(coords, order="C").tolist()
     tempmask = Image.fromarray(mask)
     draw = ImageDraw.Draw(tempmask)
     draw.polygon(coords, fill=fill)
     mask[:] = np.array(tempmask).astype(bool)
 
 
 def add_circles_to_mask(mask, coords, r, fill=False):
@@ -78,15 +78,15 @@
 
     Returns
     -------
     None:
         the mask is adjusted inplace
     """
     coords = np.array(coords)
-    r = r*np.ones(coords.shape[0])
+    r = r * np.ones(coords.shape[0])
     for i, j in zip(coords, r):
         add_circle_to_mask(mask, i[0], i[1], j, fill=fill)
 
 
 def add_circle_to_mask(mask, x, y, r, fill=False):
     """
     Add a single circle to the mask
@@ -108,15 +108,15 @@
     -------
     None:
         the mask is adjusted inplace
     """
     xx = np.arange(mask.shape[1])
     yy = np.arange(mask.shape[0])
     X, Y = np.meshgrid(xx, yy)
-    condition = ((X - x)**2 + (Y - y)**2 < r**2)
+    condition = (X - x) ** 2 + (Y - y) ** 2 < r**2
     mask[condition] = fill
 
 
 def add_annulus_to_mask(mask, r1, r2, x=None, y=None, fill=False):
     """
     Add an annular feature on the mask
 
@@ -143,15 +143,17 @@
     if x is None:
         x = mask.shape[1] / 2
     if y is None:
         y = mask.shape[0] / 2
     xx = np.arange(mask.shape[1])
     yy = np.arange(mask.shape[0])
     X, Y = np.meshgrid(xx, yy)
-    condition = ((X - x)**2 + (Y - y)**2 > r1**2) & ((X - x)**2 + (Y - y)**2 < r2**2)
+    condition = ((X - x) ** 2 + (Y - y) ** 2 > r1**2) & (
+        (X - x) ** 2 + (Y - y) ** 2 < r2**2
+    )
     mask[condition] = fill
 
 
 def add_band_to_mask(mask, x, y, theta, width, fill=False):
     """
     Add a straight band to a mask
 
@@ -177,14 +179,14 @@
     None:
         the mask is adjusted inplace
     """
     # see distance from point to line formula https://en.wikipedia.org/wiki/Distance_from_a_point_to_a_line
     theta_r = np.deg2rad(theta)
     a = np.sin(theta_r)
     b = -np.cos(theta_r)
-    c = -(a*x+b*y)
+    c = -(a * x + b * y)
     denom = np.sqrt(a**2 + b**2)
     xx = np.arange(mask.shape[1])
     yy = np.arange(mask.shape[0])
     X, Y = np.meshgrid(xx, yy)
-    condition = np.abs(a*X+b*Y+c)/denom < width/2
+    condition = np.abs(a * X + b * Y + c) / denom < width / 2
     mask[condition] = fill
```

### Comparing `diffsims-0.5.2/diffsims/utils/probe_utils.py` & `diffsims-0.6rc1/diffsims/utils/probe_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -17,21 +17,27 @@
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 Created on 5 Nov 2019
 
 @author: Rob Tovey
 """
-from diffsims.utils.fourier_transform import get_DFT, from_recip
-from diffsims.utils.generic_utils import to_mesh
 import numba
 from math import sqrt as c_sqrt
 from numpy import empty, maximum, sqrt, arange, pi, linspace, ones
 from scipy.special import jv
 
+from diffsims.utils.fourier_transform import get_DFT, from_recip
+from diffsims.utils.generic_utils import to_mesh
+
+__all__ = [
+    "BesselProbe",
+    "ProbeFunction",
+]
+
 
 class ProbeFunction:
     """Object representing a probe function.
 
     Parameters
     ----------
     func : function
@@ -167,15 +173,15 @@
         scale = ones(1, dtype=x.dtype) if scale is None else scale
         if out is None:
             out = empty(x.shape[:-1], dtype=scale.dtype)
         if x.shape[-1] == 1 or x.ndim == 1:
             x = maximum(1e-16, abs(x)).reshape(-1)
             out[...] = jv(1, x) / x * scale
         elif x.shape[-1] == 2:
-            x = maximum(1e-16, sqrt(abs(x * x).sum(-1) / self._r ** 2))
+            x = maximum(1e-16, sqrt(abs(x * x).sum(-1) / self._r**2))
             out[...] = jv(1, x) / x * scale
         else:
             d = abs(x[1, 1, 0, :2] - x[0, 0, 0, :2])
             h = d.min() / 10
             s = ((d[0] * x.shape[0]) ** 2 + (d[1] * x.shape[1]) ** 2) ** 0.5
 
             fine_grid = arange(h / 2, s / self._r + h, h)
@@ -233,23 +239,21 @@
                     dy2.append(
                         abs(y[tmp] - y[..., 2].item(0)) if y.shape[-1] == 3 else 1
                     )
                 eps = max(1e-16, max(dy2) * 0.5)
                 if out is None:
                     out = empty(y.shape[:3], dtype=y.dtype)
 
-                _bessFT(
-                    y.reshape(-1, 3), 1 / r ** 2, 2 * pi * r ** 2, eps, out.reshape(-1)
-                )
+                _bessFT(y.reshape(-1, 3), 1 / r**2, 2 * pi * r**2, eps, out.reshape(-1))
 
             else:
                 if out is None:
-                    out = (2 * pi * r ** 2) * (abs(y * y).sum(-1) <= 1 / r ** 2)
+                    out = (2 * pi * r**2) * (abs(y * y).sum(-1) <= 1 / r**2)
                 else:
-                    out[...] = (2 * pi * r ** 2) * (abs(y * y).sum(-1) <= 1 / r ** 2)
+                    out[...] = (2 * pi * r**2) * (abs(y * y).sum(-1) <= 1 / r**2)
         return out
 
 
 # Coverage: Numba code does not register when code is run
 @numba.njit(parallel=True, fastmath=True)
 def _bess(X, R, H, J, scale, out):  # pragma: no cover
     if scale.size == 1:
```

### Comparing `diffsims-0.5.2/diffsims/utils/ring_pattern_utils.py` & `diffsims-0.6rc1/diffsims/utils/ring_pattern_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -16,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
 import numpy as np
 
 
 def calc_radius_with_distortion(x, y, xc, yc, asym, rot):
-    """ calculate the distance of each 2D point from the center (xc, yc) """
+    """calculate the distance of each 2D point from the center (xc, yc)"""
     xp = x * np.cos(rot) - y * np.sin(rot)
     yp = x * np.sin(rot) + y * np.cos(rot)
     xcp = xc * np.cos(rot) - yc * np.sin(rot)
     ycp = xc * np.sin(rot) + yc * np.cos(rot)
 
     return np.sqrt((xp - xcp) ** 2 + asym * (yp - ycp) ** 2)
 
@@ -94,16 +94,16 @@
         amps = [1, 0.44, 0.19, 0.16, 0.04, 0.014, 0.038, 0.036]
 
         x = pts[: round(np.size(pts, 0) / 2)]
         y = pts[round(np.size(pts, 0) / 2) :]
         Ri = calc_radius_with_distortion(x, y, xcenter, ycenter, asymmetry, rotation)
 
         v = []
-        denom = 2 * spread ** 2
-        v.append(direct_beam_amplitude * Ri ** -2)  # np.exp((-1*(Ri)*(Ri))/d0)
+        denom = 2 * spread**2
+        v.append(direct_beam_amplitude * Ri**-2)  # np.exp((-1*(Ri)*(Ri))/d0)
         for i in [0, 1, 2, 3, 4, 5, 6, 7]:
             v.append(amps[i] * np.exp((-1 * (Ri - rings[i]) * (Ri - rings[i])) / denom))
 
         return (
             amplitude
             * (v[0] + v[1] + v[2] + v[3] + v[4] + v[5] + v[6] + v[7] + v[8]).ravel()
         )
```

### Comparing `diffsims-0.5.2/diffsims/utils/scattering_params.py` & `diffsims-0.6rc1/diffsims/utils/scattering_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
```

### Comparing `diffsims-0.5.2/diffsims/utils/sim_utils.py` & `diffsims-0.6rc1/diffsims/utils/sim_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -23,14 +23,40 @@
 import numpy as np
 from scipy.constants import h, m_e, e, c, pi, mu_0
 
 from diffsims.utils.atomic_scattering_params import ATOMIC_SCATTERING_PARAMS
 from diffsims.utils.lobato_scattering_params import ATOMIC_SCATTERING_PARAMS_LOBATO
 
 
+__all__ = [
+    "acceleration_voltage_to_relativistic_mass",
+    "acceleration_voltage_to_velocity",
+    "acceleration_voltage_to_wavelength",
+    "beta_to_bst",
+    "bst_to_beta",
+    "diffraction_scattering_angle",
+    "et_to_beta",
+    "get_atomic_scattering_factors",
+    "get_electron_wavelength",
+    "get_holz_angle",
+    "get_intensities_params",
+    "get_interaction_constant",
+    "get_kinematical_intensities",
+    "get_points_in_sphere",
+    "get_scattering_params_dict",
+    "get_unique_families",
+    "get_vectorized_list_for_atomic_scattering_factors",
+    "is_lattice_hexagonal",
+    "scattering_angle_to_lattice_parameter",
+    "simulate_kinematic_scattering",
+    "tesla_to_am",
+    "uvtw_to_uvw",
+]
+
+
 def get_electron_wavelength(accelerating_voltage):
     """Calculates the (relativistic) electron wavelength in Angstroms
     for a given accelerating voltage in kV.
 
     Parameters
     ----------
     accelerating_voltage : float or 'inf'
@@ -237,15 +263,15 @@
         dwfactors,
     ) = get_vectorized_list_for_atomic_scattering_factors(
         structure=structure,
         debye_waller_factors=debye_waller_factors,
         scattering_params=scattering_params,
     )
 
-    gspacing_squared = g_hkls_array ** 2
+    gspacing_squared = g_hkls_array**2
 
     if scattering_params is not None:
         atomic_scattering_factor = get_atomic_scattering_factors(
             gspacing_squared, coeffs, scattering_params
         )
     else:
         # Set all atomic scattering factors to 1
@@ -365,15 +391,15 @@
     wavelength = get_electron_wavelength(accelerating_voltage)
 
     # Define a 2D array of k-vectors at which to evaluate scattering.
     l = np.linspace(-max_k, max_k, simulation_size)
     kx, ky = np.meshgrid(l, l)
 
     # Convert 2D k-vectors into 3D k-vectors accounting for Ewald sphere.
-    k = np.array((kx, ky, (wavelength / 2) * (kx ** 2 + ky ** 2)))
+    k = np.array((kx, ky, (wavelength / 2) * (kx**2 + ky**2)))
 
     # Calculate scattering vector squared for each k-vector.
     gs_sq = np.linalg.norm(k, axis=0) ** 2
 
     # Get the scattering factors for this element.
     fs = get_atomic_scattering_factors(gs_sq, coeffs[np.newaxis, :], scattering_params)
 
@@ -381,15 +407,15 @@
     scattering = np.zeros_like(gs_sq)
     if illumination == "plane_wave":
         for r in atomic_coordinates:
             scattering = scattering + (fs * np.exp(np.dot(k.T, r) * np.pi * 2j))
     elif illumination == "gaussian_probe":
         for r in atomic_coordinates:
             probe = (1 / (np.sqrt(2 * np.pi) * sigma)) * np.exp(
-                (-np.abs(((r[0] ** 2) - (r[1] ** 2)))) / (4 * sigma ** 2)
+                (-np.abs(((r[0] ** 2) - (r[1] ** 2)))) / (4 * sigma**2)
             )
             scattering = scattering + (probe * fs * np.exp(np.dot(k.T, r) * np.pi * 2j))
     else:
         raise ValueError(
             "User specified illumination '{}' not defined.".format(illumination)
         )
 
@@ -473,15 +499,14 @@
     u, v, t, w = uvtw
     u, v, w = 2 * u + v, 2 * v + u, w
     common_factor = math.gcd(math.gcd(u, v), w)
     return tuple((int(x / common_factor)) for x in (u, v, w))
 
 
 def get_intensities_params(reciprocal_lattice, reciprocal_radius):
-
     """Calculates the variables needed for get_kinematical_intensities
 
     Parameters
     ----------
     reciprocal_lattice : diffpy.Structure.Lattice
         The reciprocal crystal lattice for the structure of interest.
     reciprocal_radius  : float
@@ -544,15 +569,15 @@
     >>> wavelength = 2.51/1000 # Electron wavelength for 200 kV
     >>> angle = sim_utils.get_holz_angle(wavelength, lattice_size)
 
     """
     k0 = 1.0 / electron_wavelength
     kz = 1.0 / lattice_parameter
     in_root = kz * ((2 * k0) - kz)
-    sin_angle = (in_root ** 0.5) / k0
+    sin_angle = (in_root**0.5) / k0
     angle = np.arcsin(sin_angle)
     return angle
 
 
 def scattering_angle_to_lattice_parameter(electron_wavelength, angle):
     """Convert scattering angle data to lattice parameter sizes.
 
@@ -686,15 +711,15 @@
     >>> import diffsims.utils.sim_utils as sim_utils
     >>> v = sim_utils.acceleration_voltage_to_velocity(200000) # 200 kV
     >>> round(v)
     208450035
 
     """
 
-    part1 = (1 + (acceleration_voltage * e) / (m_e * c ** 2)) ** 2
+    part1 = (1 + (acceleration_voltage * e) / (m_e * c**2)) ** 2
     v = c * (1 - (1 / part1)) ** 0.5
     return v
 
 
 def acceleration_voltage_to_relativistic_mass(acceleration_voltage):
     """Get relativistic mass of electron as function of acceleration voltage.
 
@@ -711,15 +736,15 @@
     Example
     -------
     >>> import diffsims.utils.sim_utils as sim_utils
     >>> mr = sim_utils.acceleration_voltage_to_relativistic_mass(200000) # 200 kV
 
     """
     v = acceleration_voltage_to_velocity(acceleration_voltage)
-    part1 = 1 - (v ** 2) / (c ** 2)
+    part1 = 1 - (v**2) / (c**2)
     mr = m_e / (part1) ** 0.5
     return mr
 
 
 def et_to_beta(et, acceleration_voltage):
     """Calculate beam deflection (beta) values from E * t.
 
@@ -743,15 +768,15 @@
     >>> acceleration_voltage = 200000  # 200 kV (in Volt)
     >>> beta = sim_utils.et_to_beta(data, acceleration_voltage)
 
     """
     wavelength = acceleration_voltage_to_wavelength(acceleration_voltage)
     m = acceleration_voltage_to_relativistic_mass(acceleration_voltage)
 
-    beta = e * (wavelength ** 2) * m * et / (h ** 2)
+    beta = e * (wavelength**2) * m * et / (h**2)
     return beta
 
 
 def acceleration_voltage_to_wavelength(acceleration_voltage):
     """Get electron wavelength from the acceleration voltage.
 
     Parameters
@@ -762,15 +787,15 @@
     Returns
     -------
     wavelength : float or array-like
         In meters
 
     """
     energy = acceleration_voltage * e
-    wavelength = h / (2 * m_e * energy * (1 + (energy / (2 * m_e * c ** 2)))) ** 0.5
+    wavelength = h / (2 * m_e * energy * (1 + (energy / (2 * m_e * c**2)))) ** 0.5
     return wavelength
 
 
 def diffraction_scattering_angle(acceleration_voltage, lattice_size, miller_index):
     """Get electron scattering angle from a crystal lattice.
 
     Returns the total scattering angle, as measured from the middle of the
@@ -795,10 +820,10 @@
     angle : float
         Scattering angle in radians.
 
     """
     wavelength = acceleration_voltage_to_wavelength(acceleration_voltage)
     h, k, l = miller_index
     a = lattice_size
-    d = a / (h ** 2 + k ** 2 + l ** 2) ** 0.5
+    d = a / (h**2 + k**2 + l**2) ** 0.5
     scattering_angle = 2 * np.arcsin(wavelength / (2 * d))
     return scattering_angle
```

### Comparing `diffsims-0.5.2/diffsims/utils/vector_utils.py` & `diffsims-0.6rc1/diffsims/utils/vector_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -12,17 +12,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with diffsims.  If not, see <http://www.gnu.org/licenses/>.
 
-import numpy as np
 import math
 
+import numpy as np
+
+
+__all__ = [
+    "get_angle_cartesian",
+    "get_angle_cartesian_vec",
+    "vectorised_spherical_polars_to_cartesians",
+]
+
 
 def get_angle_cartesian_vec(a, b):
     """Compute the angles between two lists of vectors in a cartesian
     coordinate system.
 
     Parameters
     ----------
```

### Comparing `diffsims-0.5.2/diffsims.egg-info/SOURCES.txt` & `diffsims-0.6rc1/diffsims.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -11,68 +11,81 @@
 diffsims/release_info.py
 diffsims.egg-info/PKG-INFO
 diffsims.egg-info/SOURCES.txt
 diffsims.egg-info/dependency_links.txt
 diffsims.egg-info/requires.txt
 diffsims.egg-info/top_level.txt
 diffsims/crystallography/__init__.py
-diffsims/crystallography/reciprocal_lattice_point.py
+diffsims/crystallography/_diffracting_vector.py
+diffsims/crystallography/get_hkl.py
 diffsims/crystallography/reciprocal_lattice_vector.py
 diffsims/generators/__init__.py
 diffsims/generators/diffraction_generator.py
 diffsims/generators/library_generator.py
 diffsims/generators/rotation_list_generators.py
+diffsims/generators/simulation_generator.py
 diffsims/generators/sphere_mesh_generators.py
 diffsims/generators/zap_map_generator.py
 diffsims/libraries/__init__.py
 diffsims/libraries/diffraction_library.py
 diffsims/libraries/structure_library.py
 diffsims/libraries/vector_library.py
 diffsims/pattern/__init__.py
 diffsims/pattern/detector_functions.py
 diffsims/sims/__init__.py
 diffsims/sims/diffraction_simulation.py
+diffsims/simulations/__init__.py
+diffsims/simulations/simulation1d.py
+diffsims/simulations/simulation2d.py
 diffsims/structure_factor/__init__.py
 diffsims/structure_factor/atomic_scattering_factor.py
 diffsims/structure_factor/atomic_scattering_parameters.py
 diffsims/structure_factor/structure_factor.py
 diffsims/tests/__init__.py
 diffsims/tests/crystallography/__init__.py
-diffsims/tests/crystallography/test_reciprocal_lattice_point.py
+diffsims/tests/crystallography/test_diffracting_vector.py
+diffsims/tests/crystallography/test_get_hkl.py
 diffsims/tests/crystallography/test_reciprocal_lattice_vector.py
 diffsims/tests/generators/__init__.py
+diffsims/tests/generators/old_simulation.npy
 diffsims/tests/generators/test_diffraction_generator.py
 diffsims/tests/generators/test_library_generator.py
 diffsims/tests/generators/test_rotation_list_generator.py
+diffsims/tests/generators/test_simulation_generator.py
 diffsims/tests/generators/test_sphere_mesh_generators.py
 diffsims/tests/generators/test_zap_map_generator.py
 diffsims/tests/library/__init__.py
 diffsims/tests/library/test_diffraction_library.py
 diffsims/tests/library/test_structure_library.py
 diffsims/tests/library/test_vector_library.py
 diffsims/tests/patterns/__init__.py
 diffsims/tests/patterns/test_detector_functions.py
 diffsims/tests/sims/__init__.py
 diffsims/tests/sims/test_diffraction_simulation.py
+diffsims/tests/simulations/__init__.py
+diffsims/tests/simulations/test_simulations1d.py
+diffsims/tests/simulations/test_simulations2d.py
 diffsims/tests/structure_factor/__init__.py
 diffsims/tests/structure_factor/test_atomic_scattering_factor.py
 diffsims/tests/structure_factor/test_atomic_scattering_parameters.py
 diffsims/tests/structure_factor/test_structure_factor.py
 diffsims/tests/utils/__init__.py
 diffsims/tests/utils/test_atomic_diffraction_generator_utils.py
+diffsims/tests/utils/test_deprecation.py
 diffsims/tests/utils/test_discretise_utils.py
 diffsims/tests/utils/test_fourier_transform.py
 diffsims/tests/utils/test_generic_utils.py
 diffsims/tests/utils/test_kinematic_simulation_utils.py
 diffsims/tests/utils/test_mask_utils.py
 diffsims/tests/utils/test_probe_utils.py
 diffsims/tests/utils/test_ring_pattern_utils.py
 diffsims/tests/utils/test_sim_utils.py
 diffsims/tests/utils/test_vector_utils.py
 diffsims/utils/__init__.py
+diffsims/utils/_deprecated.py
 diffsims/utils/atomic_diffraction_generator_utils.py
 diffsims/utils/atomic_scattering_params.py
 diffsims/utils/discretise_utils.py
 diffsims/utils/fourier_transform.py
 diffsims/utils/generic_utils.py
 diffsims/utils/kinematic_simulation_utils.py
 diffsims/utils/lobato_scattering_params.py
@@ -82,14 +95,25 @@
 diffsims/utils/scattering_params.py
 diffsims/utils/shape_factor_models.py
 diffsims/utils/sim_utils.py
 diffsims/utils/vector_utils.py
 doc/Makefile
 doc/changelog.rst
 doc/conf.py
-doc/contributing.rst
 doc/index.rst
-doc/installation.rst
 doc/make.bat
-doc/reference.rst
-doc/related_projects.rst
-doc/usage.rst
+doc/_static/pyxem_logo.png
+doc/_templates/custom-attribute-template.rst
+doc/_templates/custom-class-template.rst
+doc/_templates/custom-function-template.rst
+doc/_templates/custom-method-template.rst
+doc/_templates/custom-module-template.rst
+doc/_templates/autosummary/base.rst
+doc/dev/index.rst
+doc/reference/index.rst
+doc/user/index.rst
+doc/user/installation.rst
+doc/user/related_projects.rst
+examples/README.rst
+examples/creating_a_simulation_library/README.rst
+examples/creating_a_simulation_library/migration_guide.py
+examples/creating_a_simulation_library/simulating_diffraction_patterns.py
```

### Comparing `diffsims-0.5.2/doc/make.bat` & `diffsims-0.6rc1/doc/make.bat`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 REM Command file for Sphinx documentation
 
 if "%SPHINXBUILD%" == "" (
 	set SPHINXBUILD=sphinx-build
 )
 set SOURCEDIR=.
-set BUILDDIR=_build
+set BUILDDIR=build
 
 if "%1" == "" goto help
 
 %SPHINXBUILD% >NUL 2>NUL
 if errorlevel 9009 (
 	echo.
 	echo.The 'sphinx-build' command was not found. Make sure you have Sphinx
```

### Comparing `diffsims-0.5.2/doc/related_projects.rst` & `diffsims-0.6rc1/doc/user/related_projects.rst`

 * *Files 25% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 ================
 
 Related, open-source projects that users of diffsims might find useful:
 
 - `pyxem <https://pyxem.readthedocs.io/en/stable>`_: Python library for
   multi-dimensional diffraction microscopy. Uses diffsims.
 - `orix <https://orix.readthedocs.io/en/stable>`_: Python library for handling crystal
-  orientation mapping data. diffsims depends on orix.
+  orientation mapping data. diffsims uses on orix.
 - `kikuchipy <https://kikuchipy.org/en/stable>`_: Python library for processing,
   simulating and indexing of electron backscatter diffraction (EBSD) patterns. Uses
   diffsims.
```

### Comparing `diffsims-0.5.2/readthedocs.yaml` & `diffsims-0.6rc1/readthedocs.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Build documentation in the doc/ directory with Sphinx
 sphinx:
   configuration: doc/conf.py
 
 # Set the version of Python and other tools you might need
 build:
-  os: ubuntu-20.04
+  os: ubuntu-22.04
   tools:
-    python: "3.9"
+    python: "3.11"
 
 # Build doc in all formats (HTML, PDF and ePub)
 formats:
   - htmlzip
   - pdf
 
 # Python environment for building the docs
```

### Comparing `diffsims-0.5.2/setup.py` & `diffsims-0.6rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2017-2023 The diffsims developers
+# Copyright 2017-2024 The diffsims developers
 #
 # This file is part of diffsims.
 #
 # diffsims is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
@@ -23,68 +23,70 @@
 
 # Projects with optional features for building the documentation and running
 # tests. From setuptools:
 # https://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-extras-optional-features-with-their-own-dependencies
 # fmt: off
 extra_feature_requirements = {
     "doc": [
-        "furo",
-        "sphinx         >= 3.0.2"
+        "numpydoc",
+        "pydata-sphinx-theme",
+        "sphinx                 >= 3.0.2",
+        "sphinx-design",
+        "sphinx_gallery",
     ],
     "tests": [
-        "pytest         >= 5.4",
-        "pytest-cov     >= 2.8.1",
+        "coverage               >= 5.0",
+        "pytest                 >= 5.4",
+        "pytest-cov             >= 2.8.1",
         "pytest-xdist",
-        "coverage       >= 5.0"
     ],
 }
 extra_feature_requirements["dev"] = [
-    "black              >= 19.3b0",
+    "black                      >= 23.1",
     "manifix",
-    "pre-commit         >= 1.16"
+    "pre-commit                 >= 1.16"
 ] + list(chain(*list(extra_feature_requirements.values())))
 # fmt: on
 
 setup(
     name=name,
     version=version,
     description="Diffraction Simulations in Python",
     author=author,
     author_email=email,
     license=license,
     url="https://github.com/pyxem/diffsims",
     long_description=open("README.rst").read(),
     classifiers=[
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         (
             "License :: OSI Approved :: GNU General Public License v3 or later "
             "(GPLv3+)"
         ),
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Physics",
     ],
     packages=find_packages(),
     extras_require=extra_feature_requirements,
     install_requires=[
-        "diffpy.structure   >= 3.0.0",  # First Python 3 support
+        "diffpy.structure   >= 3.0.2",
         "matplotlib         >= 3.3",
         "numba",
-        "numpy              >= 1.17",
-        "orix               >= 0.9",
+        "numpy              >= 1.17.3",
+        "orix               >= 0.12.1",
         "psutil",
-        "scipy              >= 1.0",
+        "scipy              >= 1.8",
         "tqdm               >= 4.9",
         "transforms3d",
     ],
     python_requires=">=3.6",
     package_data={
         "": ["LICENSE", "README.rst", "readthedocs.yaml"],
         "diffsims": ["*.py"],
```

