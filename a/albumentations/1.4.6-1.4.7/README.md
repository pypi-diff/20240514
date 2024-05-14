# Comparing `tmp/albumentations-1.4.6.tar.gz` & `tmp/albumentations-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "albumentations-1.4.6.tar", last modified: Sat May  4 05:33:59 2024, max compression
+gzip compressed data, was "albumentations-1.4.7.tar", last modified: Tue May 14 00:43:18 2024, max compression
```

## Comparing `albumentations-1.4.6.tar` & `albumentations-1.4.7.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.691548 albumentations-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-04 05:33:46.000000 albumentations-1.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-04 05:33:46.000000 albumentations-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-04 05:33:59.691548 albumentations-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    35779 2024-05-04 05:33:46.000000 albumentations-1.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.675548 albumentations-1.4.6/albumentations/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/blur/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/blur/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.679548 albumentations-1.4.6/albumentations/augmentations/crops/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/crops/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/domain_adaptation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/domain_adaptation_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/channel_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/grid_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/mask_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/dropout/xy_masking.py
--rw-r--r--   0 runner    (1001) docker     (127)    51656 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/geometric/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43682 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/resize.py
--rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/rotate.py
--rw-r--r--   0 runner    (1001) docker     (127)    79877 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/geometric/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/augmentations/mixing/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/mixing/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)   125204 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/augmentations/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.683548 albumentations-1.4.6/albumentations/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22401 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/bbox_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23980 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/keypoints_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    14159 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/transforms_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/core/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/albumentations/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/pytorch/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-04 05:33:46.000000 albumentations-1.4.6/albumentations/random_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/albumentations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-04 05:33:59.000000 albumentations-1.4.6/albumentations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-04 05:33:46.000000 albumentations-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 05:33:59.691548 albumentations-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-04 05:33:46.000000 albumentations-1.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 05:33:59.687548 albumentations-1.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    40223 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (127)    12940 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)    20751 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    54144 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional_cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_functional_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)    38359 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    57647 2024-05-04 05:33:46.000000 albumentations-1.4.6/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-14 00:43:09.000000 albumentations-1.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 00:43:09.000000 albumentations-1.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-14 00:43:18.726340 albumentations-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    35779 2024-05-14 00:43:09.000000 albumentations-1.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.714340 albumentations-1.4.7/albumentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/blur/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22830 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/blur/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.718340 albumentations-1.4.7/albumentations/augmentations/crops/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10272 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50508 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/crops/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15076 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/domain_adaptation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/domain_adaptation_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/channel_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/grid_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/mask_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/dropout/xy_masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51636 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/geometric/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43397 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10186 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14104 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/rotate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80815 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/geometric/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/augmentations/mixing/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/mixing/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126628 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/augmentations/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/check_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/bbox_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9107 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/keypoints_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/transforms_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/core/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.722340 albumentations-1.4.7/albumentations/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/pytorch/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-14 00:43:09.000000 albumentations-1.4.7/albumentations/random_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/albumentations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    37567 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 00:43:18.000000 albumentations-1.4.7/albumentations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-05-14 00:43:09.000000 albumentations-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 00:43:18.726340 albumentations-1.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-14 00:43:09.000000 albumentations-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 00:43:18.726340 albumentations-1.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40331 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21637 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52457 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional_cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_functional_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12432 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9303 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7753 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38359 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59111 2024-05-14 00:43:09.000000 albumentations-1.4.7/tests/test_transforms.py
```

### Comparing `albumentations-1.4.6/LICENSE` & `albumentations-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/PKG-INFO` & `albumentations-1.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.6
+Version: 1.4.7
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `albumentations-1.4.6/README.md` & `albumentations-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/__init__.py` & `albumentations-1.4.7/albumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/blur/functional.py` & `albumentations-1.4.7/albumentations/augmentations/blur/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/blur/transforms.py` & `albumentations-1.4.7/albumentations/augmentations/blur/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/crops/functional.py` & `albumentations-1.4.7/albumentations/augmentations/crops/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/crops/transforms.py` & `albumentations-1.4.7/albumentations/augmentations/crops/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/domain_adaptation.py` & `albumentations-1.4.7/albumentations/augmentations/domain_adaptation.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/domain_adaptation_functional.py` & `albumentations-1.4.7/albumentations/augmentations/domain_adaptation_functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/channel_dropout.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/channel_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/coarse_dropout.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/functional.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/functional.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/grid_dropout.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/grid_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/mask_dropout.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/mask_dropout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/dropout/xy_masking.py` & `albumentations-1.4.7/albumentations/augmentations/dropout/xy_masking.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/functional.py` & `albumentations-1.4.7/albumentations/augmentations/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -547,16 +547,16 @@
 @preserve_channel_dim
 def convolve(img: np.ndarray, kernel: np.ndarray) -> np.ndarray:
     conv_fn = _maybe_process_in_chunks(cv2.filter2D, ddepth=-1, kernel=kernel)
     return conv_fn(img)
 
 
 @preserve_channel_dim
-def image_compression(img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp", ".jpeg"]) -> np.ndarray:
-    if image_type in {".jpeg", ".jpg"}:
+def image_compression(img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp"]) -> np.ndarray:
+    if image_type == ".jpg":
         quality_flag = cv2.IMWRITE_JPEG_QUALITY
     elif image_type == ".webp":
         quality_flag = cv2.IMWRITE_WEBP_QUALITY
     else:
         NotImplementedError("Only '.jpg' and '.webp' compression transforms are implemented. ")
 
     input_dtype = img.dtype
```

### Comparing `albumentations-1.4.6/albumentations/augmentations/geometric/functional.py` & `albumentations-1.4.7/albumentations/augmentations/geometric/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 from albumentations.augmentations.utils import (
     _maybe_process_in_chunks,
     angle_2pi_range,
     clipped,
     preserve_channel_dim,
 )
 from albumentations.core.bbox_utils import denormalize_bbox, normalize_bbox
-from albumentations.core.types import BoxInternalType, ColorType, D4Type, KeypointInternalType
+from albumentations.core.types import (
+    NUM_MULTI_CHANNEL_DIMENSIONS,
+    BoxInternalType,
+    ColorType,
+    D4Type,
+    KeypointInternalType,
+)
 
 __all__ = [
     "optical_distortion",
     "elastic_transform_approx",
     "grid_distortion",
     "pad",
     "pad_with_params",
@@ -66,15 +72,14 @@
     "vflip",
     "d4",
     "bbox_d4",
     "keypoint_d4",
 ]
 
 TWO = 2
-THREE = 3
 
 ROT90_180_FACTOR = 2
 ROT90_270_FACTOR = 3
 
 
 def bbox_rot90(bbox: BoxInternalType, factor: int, rows: int, cols: int) -> BoxInternalType:
     """Rotates a bounding box by 90 degrees CCW (see np.rot90)
@@ -235,16 +240,16 @@
     raise ValueError(f"Invalid group member: {group_member}")
 
 
 @preserve_channel_dim
 def rotate(
     img: np.ndarray,
     angle: float,
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
+    interpolation: int,
+    border_mode: int,
     value: Optional[ColorType] = None,
 ) -> np.ndarray:
     height, width = img.shape[:2]
     # for images we use additional shifts of (0.5, 0.5) as otherwise
     # we get an ugly black border for 90deg rotations
     matrix = cv2.getRotationMatrix2D((width / 2 - 0.5, height / 2 - 0.5), angle, 1.0)
 
@@ -268,15 +273,15 @@
         method: Rotation method used. Should be one of: "largest_box", "ellipse". Default: "largest_box".
         rows: Image rows.
         cols: Image cols.
 
     Returns:
         A bounding box `(x_min, y_min, x_max, y_max)`.
 
-    References:
+    Reference:
         https://arxiv.org/abs/2109.13488
 
     """
     x_min, y_min, x_max, y_max = bbox[:4]
     scale = cols / float(rows)
     if method == "largest_box":
         x = np.array([x_min, x_max, x_max, x_min]) - 0.5
@@ -330,16 +335,16 @@
 
 @preserve_channel_dim
 def elastic_transform(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
+    interpolation: int,
+    border_mode: int,
     value: Optional[ColorType] = None,
     random_state: Optional[np.random.RandomState] = None,
     approximate: bool = False,
     same_dxdy: bool = False,
 ) -> np.ndarray:
     """Elastic deformation of images as described in [Simard2003]_ (with modifications).
     Based on https://gist.github.com/ernestum/601cdf56d2b424757de5
@@ -419,24 +424,24 @@
         borderMode=border_mode,
         borderValue=value,
     )
     return remap_fn(img)
 
 
 @preserve_channel_dim
-def resize(img: np.ndarray, height: int, width: int, interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
+def resize(img: np.ndarray, height: int, width: int, interpolation: int) -> np.ndarray:
     img_height, img_width = img.shape[:2]
     if (height, width) == img.shape[:2]:
         return img
     resize_fn = _maybe_process_in_chunks(cv2.resize, dsize=(width, height), interpolation=interpolation)
     return resize_fn(img)
 
 
 @preserve_channel_dim
-def scale(img: np.ndarray, scale: float, interpolation: int = cv2.INTER_LINEAR) -> np.ndarray:
+def scale(img: np.ndarray, scale: float, interpolation: int) -> np.ndarray:
     height, width = img.shape[:2]
     new_height, new_width = int(height * scale), int(width * scale)
     return resize(img, new_height, new_width, interpolation)
 
 
 def keypoint_scale(keypoint: KeypointInternalType, scale_x: float, scale_y: float) -> KeypointInternalType:
     """Scales a keypoint by scale_x and scale_y.
@@ -527,15 +532,15 @@
 
     return cast(
         BoxInternalType,
         normalize_bbox((x1, y1, x2, y2), height if keep_size else max_height, width if keep_size else max_width),
     )
 
 
-def rotation2d_matrix_to_euler_angles(matrix: np.ndarray, y_up: bool = False) -> float:
+def rotation2d_matrix_to_euler_angles(matrix: np.ndarray, y_up: bool) -> float:
     """Args:
     matrix (np.ndarray): Rotation matrix
     y_up (bool): is Y axis looks up or down
 
     """
     if y_up:
         return np.arctan2(matrix[1, 0], matrix[0, 0])
@@ -606,15 +611,15 @@
     scale: Dict[str, Any],
 ) -> KeypointInternalType:
     if _is_identity_matrix(matrix):
         return keypoint
 
     x, y, a, s = keypoint[:4]
     x, y = cv2.transform(np.array([[[x, y]]]), matrix.params[:2]).squeeze()
-    a += rotation2d_matrix_to_euler_angles(matrix.params[:2])
+    a += rotation2d_matrix_to_euler_angles(matrix.params[:2], y_up=False)
     s *= np.max([scale["x"], scale["y"]])
     return x, y, a, s
 
 
 def bbox_affine(
     bbox: BoxInternalType,
     matrix: skimage.transform.ProjectiveTransform,
@@ -828,20 +833,20 @@
     return float(x), float(y)
 
 
 def from_distance_maps(
     distance_maps: np.ndarray,
     inverted: bool,
     if_not_found_coords: Optional[Union[Sequence[int], Dict[str, Any]]],
-    threshold: Optional[float] = None,
+    threshold: Optional[float],
 ) -> List[Tuple[float, float]]:
     """Convert outputs of `to_distance_maps` to `KeypointsOnImage`.
     This is the inverse of `to_distance_maps`.
     """
-    if distance_maps.ndim != THREE:
+    if distance_maps.ndim != NUM_MULTI_CHANNEL_DIMENSIONS:
         msg = f"Expected three-dimensional input, got {distance_maps.ndim} dimensions and shape {distance_maps.shape}."
         raise ValueError(msg)
     height, width, nb_keypoints = distance_maps.shape
 
     drop_if_not_found, if_not_found_x, if_not_found_y = validate_if_not_found_coords(if_not_found_coords)
 
     keypoints = []
@@ -1164,16 +1169,16 @@
 
 
 @preserve_channel_dim
 def pad(
     img: np.ndarray,
     min_height: int,
     min_width: int,
-    border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ColorType] = None,
+    border_mode: int,
+    value: Optional[ColorType],
 ) -> np.ndarray:
     height, width = img.shape[:2]
 
     if height < min_height:
         h_pad_top = int((min_height - height) / 2.0)
         h_pad_bottom = min_height - height - h_pad_top
     else:
@@ -1200,16 +1205,16 @@
 @preserve_channel_dim
 def pad_with_params(
     img: np.ndarray,
     h_pad_top: int,
     h_pad_bottom: int,
     w_pad_left: int,
     w_pad_right: int,
-    border_mode: int = cv2.BORDER_REFLECT_101,
-    value: Optional[ColorType] = None,
+    border_mode: int,
+    value: Optional[ColorType],
 ) -> np.ndarray:
     pad_fn = _maybe_process_in_chunks(
         cv2.copyMakeBorder,
         top=h_pad_top,
         bottom=h_pad_bottom,
         left=w_pad_left,
         right=w_pad_right,
@@ -1218,19 +1223,19 @@
     )
     return pad_fn(img)
 
 
 @preserve_channel_dim
 def optical_distortion(
     img: np.ndarray,
-    k: int = 0,
-    dx: int = 0,
-    dy: int = 0,
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
+    k: int,
+    dx: int,
+    dy: int,
+    interpolation: int,
+    border_mode: int,
     value: Optional[ColorType] = None,
 ) -> np.ndarray:
     """Barrel / pincushion distortion. Unconventional augment.
 
     Reference:
         |  https://stackoverflow.com/questions/6199636/formulas-for-barrel-pincushion-distortion
         |  https://stackoverflow.com/questions/10364201/image-transformation-in-opencv
@@ -1251,19 +1256,19 @@
     map1, map2 = cv2.initUndistortRectifyMap(camera_matrix, distortion, None, None, (width, height), cv2.CV_32FC1)
     return cv2.remap(img, map1, map2, interpolation=interpolation, borderMode=border_mode, borderValue=value)
 
 
 @preserve_channel_dim
 def grid_distortion(
     img: np.ndarray,
-    num_steps: int = 10,
-    xsteps: Tuple[()] = (),
-    ysteps: Tuple[()] = (),
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
+    num_steps: int,
+    xsteps: Tuple[()],
+    ysteps: Tuple[()],
+    interpolation: int,
+    border_mode: int,
     value: Optional[ColorType] = None,
 ) -> np.ndarray:
     height, width = img.shape[:2]
 
     x_step = width // num_steps
     xx = np.zeros(width, np.float32)
     prev = 0
@@ -1313,16 +1318,16 @@
 
 @preserve_channel_dim
 def elastic_transform_approx(
     img: np.ndarray,
     alpha: float,
     sigma: float,
     alpha_affine: float,
-    interpolation: int = cv2.INTER_LINEAR,
-    border_mode: int = cv2.BORDER_REFLECT_101,
+    interpolation: int,
+    border_mode: int,
     value: Optional[ColorType] = None,
     random_state: Optional[np.random.RandomState] = None,
 ) -> np.ndarray:
     """Elastic deformation of images as described in [Simard2003]_ (with modifications for speed).
     Based on https://gist.github.com/ernestum/601cdf56d2b424757de5
 
     .. [Simard2003] Simard, Steinkraus and Platt, "Best Practices for
```

### Comparing `albumentations-1.4.6/albumentations/augmentations/geometric/resize.py` & `albumentations-1.4.7/albumentations/augmentations/geometric/resize.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/geometric/rotate.py` & `albumentations-1.4.7/albumentations/augmentations/geometric/rotate.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/geometric/transforms.py` & `albumentations-1.4.7/albumentations/augmentations/geometric/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1184,30 +1184,34 @@
         matrix: skimage.transform.PiecewiseAffineTransform,
         **params: Any,
     ) -> KeypointInternalType:
         return F.keypoint_piecewise_affine(keypoint, matrix, rows, cols, self.keypoints_threshold)
 
 
 class PadIfNeeded(DualTransform):
-    """Pad side of the image / max if side is less than desired number.
+    """Pads the sides of an image if the image dimensions are less than the specified minimum dimensions.
+    If the `pad_height_divisor` or `pad_width_divisor` is specified, the function additionally ensures
+    that the image dimensions are divisible by these values.
 
     Args:
-        min_height (int): minimal result image height.
-        min_width (int): minimal result image width.
-        pad_height_divisor (int): if not None, ensures image height is dividable by value of this argument.
-        pad_width_divisor (int): if not None, ensures image width is dividable by value of this argument.
-        position (Union[str, PositionType]): Position of the image. should be PositionType.CENTER or
-            PositionType.TOP_LEFT or PositionType.TOP_RIGHT or PositionType.BOTTOM_LEFT or PositionType.BOTTOM_RIGHT.
-            or PositionType.RANDOM. Default: PositionType.CENTER.
-        border_mode (OpenCV flag): OpenCV border mode.
-        value (int, float, list of int, list of float): padding value if border_mode is cv2.BORDER_CONSTANT.
-        mask_value (int, float,
-                    list of int,
-                    list of float): padding value for mask if border_mode is cv2.BORDER_CONSTANT.
-        p (float): probability of applying the transform. Default: 1.0.
+        min_height (int): Minimum desired height of the image. Ensures image height is at least this value.
+        min_width (int): Minimum desired width of the image. Ensures image width is at least this value.
+        pad_height_divisor (int, optional): If set, pads the image height to make it divisible by this value.
+        pad_width_divisor (int, optional): If set, pads the image width to make it divisible by this value.
+        position (Union[str, PositionType]): Position where the image is to be placed after padding.
+            Can be one of 'center', 'top_left', 'top_right', 'bottom_left', 'bottom_right', or 'random'.
+            Default is 'center'.
+        border_mode (int): Specifies the border mode to use if padding is required.
+            The default is `cv2.BORDER_REFLECT_101`. If `value` is provided and `border_mode` is set to a mode
+            that does not use a constant value, it should be manually set to `cv2.BORDER_CONSTANT`.
+        value (Union[int, float, list[int], list[float]], optional): Value to fill the border pixels if
+            the border mode is `cv2.BORDER_CONSTANT`. Default is None.
+        mask_value (Union[int, float, list[int], list[float]], optional): Similar to `value` but used for padding masks.
+            Default is None.
+        p (float): Probability of applying the transform. Default is 1.0.
 
     Targets:
         image, mask, bboxes, keypoints
 
     Image types:
         uint8, float32
 
@@ -1265,14 +1269,22 @@
         def validate_divisibility(self) -> Self:
             if (self.min_height is None) == (self.pad_height_divisor is None):
                 msg = "Only one of 'min_height' and 'pad_height_divisor' parameters must be set"
                 raise ValueError(msg)
             if (self.min_width is None) == (self.pad_width_divisor is None):
                 msg = "Only one of 'min_width' and 'pad_width_divisor' parameters must be set"
                 raise ValueError(msg)
+
+            if self.value is not None and self.border_mode in {cv2.BORDER_REFLECT_101, cv2.BORDER_REFLECT101}:
+                self.border_mode = cv2.BORDER_CONSTANT
+
+            if self.border_mode == cv2.BORDER_CONSTANT and self.value is None:
+                msg = "If 'border_mode' is set to 'BORDER_CONSTANT', 'value' must be provided."
+                raise ValueError(msg)
+
             return self
 
     def __init__(
         self,
         min_height: Optional[int] = 1024,
         min_width: Optional[int] = 1024,
         pad_height_divisor: Optional[int] = None,
```

### Comparing `albumentations-1.4.6/albumentations/augmentations/mixing/transforms.py` & `albumentations-1.4.7/albumentations/augmentations/mixing/transforms.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/augmentations/transforms.py` & `albumentations-1.4.7/albumentations/augmentations/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,79 +316,105 @@
         return ("mean", "std", "max_pixel_value", "normalization")
 
 
 class ImageCompression(ImageOnlyTransform):
     """Decreases image quality by Jpeg, WebP compression of an image.
 
     Args:
-        quality_lower: lower bound on the image quality. Should be in [0, 100] range for jpeg and [1, 100] for webp.
-        quality_upper: upper bound on the image quality. Should be in [0, 100] range for jpeg and [1, 100] for webp.
+        quality_range: tuple of bounds on the image quality i.e. (quality_lower, quality_upper).
+            Both values should be in [1, 100] range.
         compression_type (ImageCompressionType): should be ImageCompressionType.JPEG or ImageCompressionType.WEBP.
             Default: ImageCompressionType.JPEG
 
     Targets:
         image
 
     Image types:
         uint8, float32
 
     """
 
     class InitSchema(BaseTransformInitSchema):
-        quality_lower: int = Field(default=99, description="Lower bound on the image quality", ge=1, le=100)
-        quality_upper: int = Field(default=100, description="Upper bound on the image quality", ge=1, le=100)
+        quality_range: OnePlusIntNonDecreasingRangeType = Field(
+            default=(99, 100),
+            description="lower and upper bound on the image quality as tuple (lower_bound, upper_bound)",
+        )
+        quality_lower: Optional[int] = Field(
+            default=99,
+            description="Lower bound on the image quality",
+            ge=1,
+            le=100,
+            deprecated="`quality_lower` and `quality_upper` are deprecated. "
+            "Use `quality_range` as tuple (quality_lower, quality_upper) instead.",
+        )
+        quality_upper: Optional[int] = Field(
+            default=100,
+            description="Upper bound on the image quality",
+            ge=1,
+            le=100,
+            deprecated="`quality_lower` and `quality_upper` are deprecated. "
+            "Use `quality_range` as tuple (quality_lower, quality_upper) instead.",
+        )
         compression_type: ImageCompressionType = Field(
             default=ImageCompressionType.JPEG,
             description="Image compression format",
         )
 
         @model_validator(mode="after")
-        def validate_quality(self) -> Self:
-            if self.quality_lower >= self.quality_upper:
-                msg = "quality_lower must be less than quality_upper"
-                raise ValueError(msg)
+        def validate_ranges(self) -> Self:
+            # Update the quality_range based on the non-None values of quality_lower and quality_upper
+            if self.quality_lower is not None or self.quality_upper is not None:
+                lower = self.quality_lower if self.quality_lower is not None else self.quality_range[0]
+                upper = self.quality_upper if self.quality_upper is not None else self.quality_range[1]
+                self.quality_range = (lower, upper)
+                # Clear the deprecated individual quality settings
+                self.quality_lower = None
+                self.quality_upper = None
+
+            # Validate the quality_range
+            if not (1 <= self.quality_range[0] <= MAX_JPEG_QUALITY and 1 <= self.quality_range[1] <= MAX_JPEG_QUALITY):
+                raise ValueError(f"Quality range values should be within [1, {MAX_JPEG_QUALITY}] range.")
+
             return self
 
     def __init__(
         self,
-        quality_lower: int = 99,
-        quality_upper: int = 100,
+        quality_lower: Optional[int] = None,
+        quality_upper: Optional[int] = None,
         compression_type: ImageCompressionType = ImageCompressionType.JPEG,
+        quality_range: Tuple[int, int] = (99, 100),
         always_apply: bool = False,
         p: float = 0.5,
     ):
         super().__init__(always_apply, p)
-
-        self.quality_lower = quality_lower
-        self.quality_upper = quality_upper
+        self.quality_range = quality_range
         self.compression_type = compression_type
 
-    def apply(
-        self, img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp", ".jpeg"], **params: Any
-    ) -> np.ndarray:
+    def apply(self, img: np.ndarray, quality: int, image_type: Literal[".jpg", ".webp"], **params: Any) -> np.ndarray:
         if img.ndim != MONO_CHANNEL_DIMENSIONS and img.shape[-1] not in (1, 3, 4):
             msg = "ImageCompression transformation expects 1, 3 or 4 channel images."
             raise TypeError(msg)
         return F.image_compression(img, quality, image_type)
 
     def get_params(self) -> Dict[str, Any]:
-        image_type = ".jpg"
-
-        if self.compression_type == ImageCompressionType.WEBP:
+        if self.compression_type == ImageCompressionType.JPEG:
+            image_type = ".jpg"
+        elif self.compression_type == ImageCompressionType.WEBP:
             image_type = ".webp"
+        else:
+            raise ValueError(f"Unknown image compression type: {self.compression_type}")
 
         return {
-            "quality": random_utils.randint(self.quality_lower, self.quality_upper + 1),
+            "quality": random_utils.randint(self.quality_range[0], self.quality_range[1] + 1),
             "image_type": image_type,
         }
 
     def get_transform_init_args(self) -> Dict[str, Any]:
         return {
-            "quality_lower": self.quality_lower,
-            "quality_upper": self.quality_upper,
+            "quality_range": self.quality_range,
             "compression_type": self.compression_type.value,
         }
 
 
 class RandomSnow(ImageOnlyTransform):
     """Bleach out some pixel values simulating snow.
```

### Comparing `albumentations-1.4.6/albumentations/augmentations/utils.py` & `albumentations-1.4.7/albumentations/augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/bbox_utils.py` & `albumentations-1.4.7/albumentations/core/bbox_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,18 +488,34 @@
         cols (int): The number of columns (width) in the image.
 
     Returns:
         BoxInternalType: The clipped bounding box, normalized to the image dimensions.
     """
     x_min, y_min, x_max, y_max = denormalize_bbox(bbox, rows, cols)[:4]
 
-    x_min = np.clip(x_min, 0, cols - 1)
-    x_max = np.clip(x_max, 0, cols - 1)
-    y_min = np.clip(y_min, 0, rows - 1)
-    y_max = np.clip(y_max, 0, rows - 1)
+    ## Note:
+    # It could be tempting to use cols - 1 and rows - 1 as the upper bounds for the clipping
+
+    # But this would cause the bounding box to be clipped to the image dimensions - 1 which is not what we want.
+    # Bounding box lives not in the middle of pixels but between them.
+
+    # Example: for image with height 100, width 100, the pixel values are in the range [0, 99]
+    # but if we want bounding box to be 1 pixel width and height and lie on the boundary of the image
+    # it will be described as [99, 99, 100, 100] => clip by image_size - 1 will lead to [99, 99, 99, 99]
+    # which is incorrect
+
+    # It could be also tempting to clip `x_min`` to `cols - 1`` and `y_min` to `rows - 1`, but this also leads
+    # to another error. If image fully lies outside of the visible area and min_area is set to 0, then
+    # the bounding box will be clipped to the image size - 1 and will be 1 pixel in size and fully visible,
+    # but it should be completely removed.
+
+    x_min = np.clip(x_min, 0, cols)
+    x_max = np.clip(x_max, 0, cols)
+    y_min = np.clip(y_min, 0, rows)
+    y_max = np.clip(y_max, 0, rows)
     return cast(BoxType, normalize_bbox((x_min, y_min, x_max, y_max), rows, cols) + tuple(bbox[4:]))
 
 
 def filter_bboxes(
     bboxes: Sequence[BoxType],
     rows: int,
     cols: int,
```

### Comparing `albumentations-1.4.6/albumentations/core/composition.py` & `albumentations-1.4.7/albumentations/core/composition.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import warnings
 from collections import defaultdict
-from typing import Any, Dict, Iterator, List, Optional, Sequence, Union, cast
+from typing import Any, Dict, Iterator, List, Optional, Sequence, Set, Union, cast
 
 import cv2
 import numpy as np
 
 from albumentations import random_utils
 
 from .bbox_utils import BboxParams, BboxProcessor
@@ -61,15 +61,17 @@
 
         self.transforms = transforms
         self.p = p
 
         self.replay_mode = False
         self.applied_in_replay = False
         self._additional_targets: Dict[str, str] = {}
+        self._available_keys: Set[str] = set()
         self.processors: Dict[str, Union[BboxProcessor, KeypointsProcessor]] = {}
+        self._set_keys()
 
     def __iter__(self) -> Iterator[TransformType]:
         return iter(self.transforms)
 
     def __len__(self) -> int:
         return len(self.transforms)
 
@@ -82,14 +84,18 @@
     def __repr__(self) -> str:
         return self.indented_repr()
 
     @property
     def additional_targets(self) -> Dict[str, str]:
         return self._additional_targets
 
+    @property
+    def available_keys(self) -> Set[str]:
+        return self._available_keys
+
     def indented_repr(self, indent: int = REPR_INDENT_STEP) -> str:
         args = {k: v for k, v in self.to_dict_private().items() if not (k.startswith("__") or k == "transforms")}
         repr_string = self.__class__.__name__ + "(["
         for t in self.transforms:
             repr_string += "\n"
             t_repr = t.indented_repr(indent + REPR_INDENT_STEP) if hasattr(t, "indented_repr") else repr(t)
             repr_string += " " * indent + t_repr + ","
@@ -123,19 +129,33 @@
         if additional_targets:
             for k, v in additional_targets.items():
                 if k in self._additional_targets and v != self._additional_targets[k]:
                     raise ValueError(
                         f"Trying to overwrite existed additional targets. "
                         f"Key={k} Exists={self._additional_targets[k]} New value: {v}",
                     )
-                self._additional_targets.update(additional_targets)
+            self._additional_targets.update(additional_targets)
             for t in self.transforms:
                 t.add_targets(additional_targets)
             for proc in self.processors.values():
                 proc.add_targets(additional_targets)
+        self._set_keys()
+
+    def _set_keys(self) -> None:
+        """Set _available_keys"""
+        for t in self.transforms:
+            self._available_keys.update(t.available_keys)
+        if self.processors:
+            self._available_keys.update(["labels"])
+            for proc in self.processors.values():
+                if proc.default_data_name not in self._available_keys:  # if no transform to process this data
+                    warnings.warn(f"Got processor for {proc.default_data_name}, but no transform to process it.")
+                self._available_keys.update(proc.data_fields)
+                if proc.params.label_fields:
+                    self._available_keys.update(proc.params.label_fields)
 
     def set_deterministic(self, flag: bool, save_key: str = "replay") -> None:
         for t in self.transforms:
             t.set_deterministic(flag, save_key)
 
 
 class Compose(BaseCompose):
@@ -188,14 +208,15 @@
 
         self.add_targets(additional_targets)
 
         self.is_check_args = True
         self._disable_check_args_for_transforms(self.transforms)
 
         self.is_check_shapes = is_check_shapes
+        self._always_apply = get_always_apply(self.transforms)  # transforms list that always apply
         self._check_each_transform = tuple(  # processors that checks after each transform
             proc for proc in self.processors.values() if getattr(proc.params, "check_each_transform", False)
         )
 
     @staticmethod
     def _disable_check_args_for_transforms(transforms: TransformsSeqType) -> None:
         for transform in transforms:
@@ -207,26 +228,30 @@
     def disable_check_args_private(self) -> None:
         self.is_check_args = False
 
     def __call__(self, *args: Any, force_apply: bool = False, **data: Any) -> Dict[str, Any]:
         if args:
             msg = "You have to pass data to augmentations as named arguments, for example: aug(image=image)"
             raise KeyError(msg)
-        if self.is_check_args:
-            self._check_args(**data)
 
         if not isinstance(force_apply, (bool, int)):
             msg = "force_apply must have bool or int type"
             raise TypeError(msg)
 
         need_to_run = force_apply or random.random() < self.p
+        if not need_to_run and not self._always_apply:
+            return data
+
+        transforms = self.transforms if need_to_run else self._always_apply
+
+        if self.is_check_args:
+            self._check_args(**data)
 
         for p in self.processors.values():
             p.ensure_data_valid(data)
-        transforms = self.transforms if need_to_run else get_always_apply(self.transforms)
 
         for p in self.processors.values():
             p.preprocess(data)
 
         for t in transforms:
             data = t(**data)
 
@@ -282,14 +307,17 @@
     def _check_args(self, **kwargs: Any) -> None:
         checked_single = ["image", "mask"]
         checked_multi = ["masks"]
         check_bbox_param = ["bboxes"]
         check_keypoints_param = ["keypoints"]
         shapes = []
         for data_name, data in kwargs.items():
+            if data_name not in self._available_keys and data_name not in ["mask", "masks"]:
+                msg = f"Key {data_name} is not in available keys."
+                raise ValueError(msg)
             internal_data_name = self._additional_targets.get(data_name, data_name)
             if internal_data_name in checked_single:
                 if not isinstance(data, np.ndarray):
                     raise TypeError(f"{data_name} must be numpy array type")
                 shapes.append(data.shape[:2])
             if internal_data_name in checked_multi and data is not None and len(data):
                 if not isinstance(data[0], np.ndarray):
@@ -489,14 +517,15 @@
         p: float = 1.0,
         is_check_shapes: bool = True,
         save_key: str = "replay",
     ):
         super().__init__(transforms, bbox_params, keypoint_params, additional_targets, p, is_check_shapes)
         self.set_deterministic(True, save_key=save_key)
         self.save_key = save_key
+        self._available_keys.add(save_key)
 
     def __call__(self, *args: Any, force_apply: bool = False, **kwargs: Any) -> Dict[str, Any]:
         kwargs[self.save_key] = defaultdict(dict)
         result = super().__call__(force_apply=force_apply, **kwargs)
         serialized = self.get_dict_with_id()
         self.fill_with_params(serialized, result[self.save_key])
         self.fill_applied(serialized)
```

### Comparing `albumentations-1.4.6/albumentations/core/keypoints_utils.py` & `albumentations-1.4.7/albumentations/core/keypoints_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/pydantic.py` & `albumentations-1.4.7/albumentations/core/pydantic.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/serialization.py` & `albumentations-1.4.7/albumentations/core/serialization.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/transforms_interface.py` & `albumentations-1.4.7/albumentations/core/transforms_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import random
 from copy import deepcopy
-from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Tuple, Union, cast
 from warnings import warn
 
 import cv2
 import numpy as np
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
@@ -39,16 +39,20 @@
 
 
 class CombinedMeta(SerializableMeta, ValidatedTransformMeta):
     pass
 
 
 class BasicTransform(Serializable, metaclass=CombinedMeta):
-    # `_targets` defines the types of targets (e.g., image, mask) that the transform can be applied to.
-    _targets: Union[Tuple[Targets, ...], Targets]
+    _targets: Union[Tuple[Targets, ...], Targets]  # targets that this transform can work on
+    _available_keys: Set[str]  # targets that this transform, as string, lower-cased
+    _key2func: Dict[
+        str,
+        Callable[..., Any],
+    ]  # mapping for targets (plus additional targets) and methods for which they depend
     call_backup = None
     interpolation: int
     fill_value: ColorType
     mask_fill_value: Optional[ColorType]
     # replay mode params
     deterministic: bool = False
     save_key = "replay"
@@ -60,14 +64,16 @@
 
     def __init__(self, always_apply: bool = False, p: float = 0.5):
         self.p = p
         self.always_apply = always_apply
         self._additional_targets: Dict[str, str] = {}
         # replay mode params
         self.params: Dict[Any, Any] = {}
+        self._key2func = {}
+        self._set_keys()
 
     def __call__(self, *args: Any, force_apply: bool = False, **kwargs: Any) -> Any:
         if args:
             msg = "You have to pass data to augmentations as named arguments, for example: aug(image=image)"
             raise KeyError(msg)
         if self.replay_mode:
             if self.applied_in_replay:
@@ -93,20 +99,19 @@
         return kwargs
 
     def apply_with_params(self, params: Dict[str, Any], *args: Any, **kwargs: Any) -> Dict[str, Any]:
         """Apply transforms with parameters."""
         params = self.update_params(params, **kwargs)
         res = {}
         for key, arg in kwargs.items():
-            if arg is not None:
-                target_function = self._get_target_function(key)
-                target_dependencies = {k: kwargs[k] for k in self.target_dependence.get(key, [])}
-                res[key] = target_function(arg, **dict(params, **target_dependencies))
+            if key in self._key2func and arg is not None:
+                target_function = self._key2func[key]
+                res[key] = target_function(arg, **params)
             else:
-                res[key] = None
+                res[key] = arg
         return res
 
     def set_deterministic(self, flag: bool, save_key: str = "replay") -> "BasicTransform":
         """Set transform to be deterministic."""
         if save_key == "params":
             msg = "params save_key is reserved"
             raise KeyError(msg)
@@ -121,22 +126,14 @@
         return self
 
     def __repr__(self) -> str:
         state = self.get_base_init_args()
         state.update(self.get_transform_init_args())
         return f"{self.__class__.__name__}({format_args(state)})"
 
-    def _get_target_function(self, key: str) -> Callable[..., Any]:
-        """Returns function to process target"""
-        transform_key = key
-        if key in self._additional_targets:
-            transform_key = self._additional_targets.get(key, key)
-
-        return self.targets.get(transform_key, lambda x, **p: x)
-
     def apply(self, img: np.ndarray, *args: Any, **params: Any) -> np.ndarray:
         """Apply transform on image."""
         raise NotImplementedError
 
     def get_params(self) -> Dict[str, Any]:
         """Returns parameters independent of input"""
         return {}
@@ -145,40 +142,62 @@
     def targets(self) -> Dict[str, Callable[..., Any]]:
         # mapping for targets and methods for which they depend
         # for example:
         # >>  {"image": self.apply}
         # >>  {"masks": self.apply_to_masks}
         raise NotImplementedError
 
+    def _set_keys(self) -> None:
+        """Set _available_keys"""
+        if not hasattr(self, "_targets"):
+            self._available_keys = set()
+        else:
+            self._available_keys = {
+                target.value.lower()
+                for target in (self._targets if isinstance(self._targets, tuple) else [self._targets])
+            }
+        self._available_keys.update(self.targets.keys())
+        self._key2func = {key: self.targets[key] for key in self._available_keys if key in self.targets}
+
+    @property
+    def available_keys(self) -> Set[str]:
+        """Returns set of available keys"""
+        return self._available_keys
+
     def update_params(self, params: Dict[str, Any], **kwargs: Any) -> Dict[str, Any]:
         """Update parameters with transform specific params"""
         if hasattr(self, "interpolation"):
             params["interpolation"] = self.interpolation
         if hasattr(self, "fill_value"):
             params["fill_value"] = self.fill_value
         if hasattr(self, "mask_fill_value"):
             params["mask_fill_value"] = self.mask_fill_value
         params.update({"cols": kwargs["image"].shape[1], "rows": kwargs["image"].shape[0]})
         return params
 
-    @property
-    def target_dependence(self) -> Dict[str, Any]:
-        return {}
-
     def add_targets(self, additional_targets: Dict[str, str]) -> None:
         """Add targets to transform them the same way as one of existing targets
         ex: {'target_image': 'image'}
         ex: {'obj1_mask': 'mask', 'obj2_mask': 'mask'}
         by the way you must have at least one object with key 'image'
 
         Args:
             additional_targets (dict): keys - new target name, values - old target name. ex: {'image2': 'image'}
 
         """
-        self._additional_targets = {**self._additional_targets, **additional_targets}
+        for k, v in additional_targets.items():
+            if k in self._additional_targets and v != self._additional_targets[k]:
+                raise ValueError(
+                    f"Trying to overwrite existed additional targets. "
+                    f"Key={k} Exists={self._additional_targets[k]} New value: {v}",
+                )
+            if v in self._available_keys:
+                self._additional_targets[k] = v
+                self._key2func[k] = self.targets[v]
+                self._available_keys.add(k)
 
     @property
     def targets_as_params(self) -> List[str]:
         """Targets used to get params"""
         return []
 
     def get_params_dependent_on_targets(self, params: Dict[str, Any]) -> Dict[str, Any]:
```

### Comparing `albumentations-1.4.6/albumentations/core/types.py` & `albumentations-1.4.7/albumentations/core/types.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/utils.py` & `albumentations-1.4.7/albumentations/core/utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/core/validation.py` & `albumentations-1.4.7/albumentations/core/validation.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations/pytorch/transforms.py` & `albumentations-1.4.7/albumentations/pytorch/transforms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Dict, List, Tuple
 
 import numpy as np
 import torch
 
 from albumentations.core.transforms_interface import BasicTransform
+from albumentations.core.types import Targets
 
 __all__ = ["ToTensorV2"]
 
 TWO = 2
 THREE = 3
 
 
@@ -19,14 +20,16 @@
         transpose_mask (bool): If True, transposes 3D input mask dimensions from `[height, width, num_channels]` to
             `[num_channels, height, width]`.
         always_apply (bool): Indicates if this transformation should be always applied. Default: True.
         p (float): Probability of applying the transform. Default: 1.0.
 
     """
 
+    _targets = (Targets.IMAGE, Targets.MASK)
+
     def __init__(self, transpose_mask: bool = False, always_apply: bool = True, p: float = 1.0):
         super().__init__(always_apply=always_apply, p=p)
         self.transpose_mask = transpose_mask
 
     @property
     def targets(self) -> Dict[str, Any]:
         return {"image": self.apply, "mask": self.apply_to_mask, "masks": self.apply_to_masks}
@@ -47,10 +50,7 @@
         return torch.from_numpy(mask)
 
     def apply_to_masks(self, masks: List[np.ndarray], **params: Any) -> List[torch.Tensor]:
         return [self.apply_to_mask(mask, **params) for mask in masks]
 
     def get_transform_init_args_names(self) -> Tuple[str, ...]:
         return ("transpose_mask",)
-
-    def get_params_dependent_on_targets(self, params: Any) -> Dict[str, Any]:
-        return {}
```

### Comparing `albumentations-1.4.6/albumentations/random_utils.py` & `albumentations-1.4.7/albumentations/random_utils.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/albumentations.egg-info/PKG-INFO` & `albumentations-1.4.7/albumentations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: albumentations
-Version: 1.4.6
+Version: 1.4.7
 Summary: An efficient library for image augmentation, providing extensive transformations to support machine learning and computer vision tasks.
 Home-page: https://albumentations.ai
 Author: Vladimir I. Iglovikov, Mikhail Druzhinin, Alex Parinov, Alexander Buslaev, Eugene Khvedchenya
 License: MIT
 Keywords: image augmentation,data augmentation,computer vision,deep learning,machine learning,image processing,artificial intelligence,augmentation library,image transformation,vision augmentation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `albumentations-1.4.6/albumentations.egg-info/SOURCES.txt` & `albumentations-1.4.7/albumentations.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 albumentations/__init__.py
+albumentations/check_version.py
 albumentations/random_utils.py
 albumentations.egg-info/PKG-INFO
 albumentations.egg-info/SOURCES.txt
 albumentations.egg-info/dependency_links.txt
 albumentations.egg-info/requires.txt
 albumentations.egg-info/top_level.txt
 albumentations/augmentations/__init__.py
```

### Comparing `albumentations-1.4.6/pyproject.toml` & `albumentations-1.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     "D205",
     "D105",
     "D417",
     "D106",
     "EM101",
     "COM812",
     "B008",
+    "G004",
 ]
 
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
 unfixable = []
 
 # Allow unused variables when underscore-prefixed.
```

### Comparing `albumentations-1.4.6/setup.py` & `albumentations-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_augmentations.py` & `albumentations-1.4.7/tests/test_augmentations.py`

 * *Files 1% similar despite different names*

```diff
@@ -849,20 +849,20 @@
         assert image_padded.shape[0] >= image.shape[0]
         assert image_padded.shape[0] - image.shape[0] <= pad.pad_height_divisor
 
 
 @pytest.mark.parametrize(
     ["params", "image_shape"],
     [
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "center"}, (5, 6)],
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "top_left"}, (5, 6)],
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "top_right"}, (5, 6)],
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "bottom_left"}, (5, 6)],
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "bottom_right"}, (5, 6)],
-        [{"min_height": 10, "min_width": 12, "border_mode": 0, "value": 1, "position": "random"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "center"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "top_left"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "top_right"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "bottom_left"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "bottom_right"}, (5, 6)],
+        [{"min_height": 10, "min_width": 12, "border_mode": cv2.BORDER_CONSTANT, "value": 1, "position": "random"}, (5, 6)],
     ],
 )
 def test_pad_if_needed_position(params, image_shape):
     set_seed(42)
 
     image = np.zeros(image_shape)
     pad = A.PadIfNeeded(**params)
```

### Comparing `albumentations-1.4.6/tests/test_bbox.py` & `albumentations-1.4.7/tests/test_bbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from albumentations.core.bbox_utils import (
     calculate_bbox_area,
     convert_bbox_from_albumentations,
     convert_bbox_to_albumentations,
     convert_bboxes_to_albumentations,
     denormalize_bbox,
     denormalize_bboxes,
+    filter_bboxes,
     normalize_bbox,
     normalize_bboxes,
 )
 from albumentations.core.composition import BboxParams, Compose, ReplayCompose
 from albumentations.core.transforms_interface import NoOp
 import albumentations as A
+from .utils import set_seed
 
 @pytest.mark.parametrize(
     ["bbox", "expected"],
     [((15, 25, 100, 200), (0.0375, 0.125, 0.25, 1.0)), ((15, 25, 100, 200, 99), (0.0375, 0.125, 0.25, 1.0, 99))],
 )
 def test_normalize_bbox(bbox, expected):
     normalized_bbox = normalize_bbox(bbox, 200, 400)
@@ -296,15 +298,143 @@
     labels = [1]
 
     # Test should raise an error since bbox is out of image bounds and clipping is not enabled
     with pytest.raises(ValueError):
         transform(image=np.zeros((100, 100, 3), dtype=np.uint8), bboxes=[bbox], labels=labels)
 
 @pytest.mark.parametrize("image_size, bbox, expected_bbox", [
-    ((100, 100), (-10, -10, 110, 110), (0, 0, 99, 99)),
-    ((200, 200), (-20, -20, 220, 220), (0, 0, 199, 199)),
-    ((50, 50), (-5, -5, 55, 55), (0, 0, 49, 49))
+    ((100, 100), (-10, -10, 110, 110), (0, 0, 100, 100)),
+    ((200, 200), (-20, -20, 220, 220), (0, 0, 200, 200)),
+    ((50, 50), (-5, -5, 55, 55), (0, 0, 50, 50))
 ])
 def test_bounding_box_outside_clip(image_size, bbox, expected_bbox):
     transform = Compose([A.NoOp()], bbox_params={'format': 'pascal_voc', 'label_fields': ['labels'], 'clip': True})
     transformed = transform(image=np.zeros((*image_size, 3), dtype=np.uint8), bboxes=[bbox], labels=[1])
     assert transformed['bboxes'][0] == expected_bbox
+
+@pytest.mark.parametrize("bbox, expected_bbox", [
+    ((1, 1, 1, 1), (2, 1, 1, 1)),
+    ((0, 1, 1, 1), (3, 1, 1, 1)),
+    ((1, 0, 1, 1), (2, 0, 1, 1)),
+    ((0, 0, 1, 1), (3, 0, 1, 1))
+    ])
+def test_bounding_box_hflip(bbox, expected_bbox):
+    image = np.zeros((4, 4, 3), dtype=np.uint8)
+
+    transform = A.Compose(
+        [A.HorizontalFlip(p=1.0)],
+        bbox_params=A.BboxParams(format="coco", label_fields=[]),
+    )
+
+    transformed = transform(image=image, bboxes=[bbox])
+
+    assert transformed["bboxes"][0] == expected_bbox
+
+
+@pytest.mark.parametrize("bbox, expected_bbox", [
+    ((1, 1, 1, 1), (1, 2, 1, 1)),
+    ((0, 1, 1, 1), (0, 2, 1, 1)),
+    ((1, 0, 1, 1), (1, 3, 1, 1)),
+    ((0, 0, 1, 1), (0, 3, 1, 1))
+    ])
+def test_bounding_box_hflip(bbox, expected_bbox):
+    image = np.zeros((4, 4, 3), dtype=np.uint8)
+
+    transform = A.Compose(
+        [A.VerticalFlip(p=1.0)],
+        bbox_params=A.BboxParams(format="coco", label_fields=[]),
+    )
+
+    transformed = transform(image=image, bboxes=[bbox])
+
+    assert transformed["bboxes"][0] == expected_bbox
+
+
+
+@pytest.mark.parametrize(
+    ["bboxes", "min_area", "min_visibility", "target"],
+    [
+        (
+            [(0.1, 0.5, 1.1, 0.9), (-0.1, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
+            0,
+            0,
+            [(0.1, 0.5, 1, 0.9), (0.0, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
+        ),
+        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.5, 0.5, 0.6)], 150, 0, [(0.1, 0.5, 0.8, 0.9)]),
+        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.9, 0.5, 1.6)], 0, 0.75, [(0.1, 0.5, 0.8, 0.9)]),
+        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1.1)], 0, 0.7, [(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1)]),
+    ],
+)
+def test_filter_bboxes(bboxes, min_area, min_visibility, target):
+    filtered_bboxes = filter_bboxes(bboxes, min_area=min_area, min_visibility=min_visibility, rows=100, cols=100)
+    assert filtered_bboxes == target
+
+
+@pytest.mark.parametrize(
+    ["bboxes", "img_width", "img_height", "min_width", "min_height", "target"],
+    [
+        [
+            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
+            100,
+            100,
+            20,
+            20,
+            [(0.1, 0.1, 0.9, 0.9)],
+        ],
+        [
+            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
+            100,
+            100,
+            20,
+            0,
+            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.9, 0.2)],
+        ],
+        [
+            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
+            100,
+            100,
+            0,
+            20,
+            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9)],
+        ],
+    ],
+)
+def test_filter_bboxes_by_min_width_height(bboxes, img_width, img_height, min_width, min_height, target):
+    filtered_bboxes = filter_bboxes(bboxes, cols=img_width, rows=img_height, min_width=min_width, min_height=min_height)
+    assert filtered_bboxes == target
+
+@pytest.mark.parametrize(
+    "get_transform",
+    [
+        lambda sign: A.Affine(translate_px=sign * 2),
+        lambda sign: A.ShiftScaleRotate(shift_limit=(sign * 0.02, sign * 0.02), scale_limit=0, rotate_limit=0),
+    ],
+)
+@pytest.mark.parametrize(
+    ["bboxes", "expected", "min_visibility", "sign"],
+    [
+        [[(0, 0, 10, 10, 1)], [], 0.9, -1],
+        [[(0, 0, 10, 10, 1)], [(0, 0, 8, 8, 1)], 0.6, -1],
+        [[(90, 90, 100, 100, 1)], [], 0.9, 1],
+        [[(90, 90, 100, 100, 1)], [(92, 92, 100, 100, 1)], 0.49, 1],
+    ],
+)
+def test_bbox_clipping(get_transform, bboxes, expected, min_visibility: float, sign: int):
+    image = np.zeros([100, 100, 3], dtype=np.uint8)
+    transform = get_transform(sign)
+    transform.p = 1
+    transform = A.Compose([transform], bbox_params=A.BboxParams(format="pascal_voc", min_visibility=min_visibility))
+
+    res = transform(image=image, bboxes=bboxes)["bboxes"]
+    assert res == expected
+
+
+def test_bbox_clipping_perspective():
+    set_seed(0)
+    transform = A.Compose(
+        [A.Perspective(scale=(0.05, 0.05), p=1)], bbox_params=A.BboxParams(format="pascal_voc", min_visibility=0.6)
+    )
+
+    image = np.empty([1000, 1000, 3], dtype=np.uint8)
+    bboxes = np.array([[0, 0, 100, 100, 1]])
+    res = transform(image=image, bboxes=bboxes)["bboxes"]
+    assert len(res) == 0
```

### Comparing `albumentations-1.4.6/tests/test_blur.py` & `albumentations-1.4.7/tests/test_blur.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_core.py` & `albumentations-1.4.7/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,16 @@
     augmentation = OneOrOther(first, second, p=1)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert first.called != second.called
 
 
 def test_compose():
-    first = MagicMock()
-    second = MagicMock()
+    first = MagicMock(available_keys={"image"})
+    second = MagicMock(available_keys={"image"})
     augmentation = Compose([first, second], p=1)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert first.called
     assert second.called
 
 
@@ -66,45 +66,45 @@
     aug = Compose([HorizontalFlip(p=1), Rotate(p=1), OneOf([Blur(p=1), MedianBlur(p=1)], p=1)], p=1)
     image = np.ones((8, 8))
     data = aug(image=image)
     assert data
 
 
 def test_always_apply():
-    first = MagicMock(always_apply=True)
-    second = MagicMock(always_apply=False)
+    first = MagicMock(always_apply=True, available_keys={"image"})
+    second = MagicMock(always_apply=False, available_keys={"image"})
     augmentation = Compose([first, second], p=0)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert first.called
     assert not second.called
 
 
 def test_one_of():
-    transforms = [Mock(p=1) for _ in range(10)]
+    transforms = [Mock(p=1, available_keys={"image"}) for _ in range(10)]
     augmentation = OneOf(transforms, p=1)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert len([transform for transform in transforms if transform.called]) == 1
 
 
 @pytest.mark.parametrize("N", [1, 2, 5, 10])
 @pytest.mark.parametrize("replace", [True, False])
 def test_n_of(N, replace):
-    transforms = [Mock(p=1, side_effect=lambda **kw: {"image": kw["image"]}) for _ in range(10)]
+    transforms = [Mock(p=1, side_effect=lambda **kw: {"image": kw["image"]}, available_keys={"image"}) for _ in range(10)]
     augmentation = SomeOf(transforms, N, p=1, replace=replace)
     image = np.ones((8, 8))
     augmentation(image=image)
     if not replace:
         assert len([transform for transform in transforms if transform.called]) == N
     assert sum([transform.call_count for transform in transforms]) == N
 
 
 def test_sequential():
-    transforms = [Mock(side_effect=lambda **kw: kw) for _ in range(10)]
+    transforms = [Mock(side_effect=lambda **kw: kw, available_keys={"image"}) for _ in range(10)]
     augmentation = Sequential(transforms, p=1)
     image = np.ones((8, 8))
     augmentation(image=image)
     assert len([transform for transform in transforms if transform.called]) == len(transforms)
 
 
 @pytest.mark.parametrize("input,kwargs,expected", [
@@ -250,21 +250,21 @@
             {"image": np.empty([100, 100, 3], np.uint8), "mask1": None},
             {"mask1": "mask"},
             "mask1 must be numpy array type",
         ],
     ],
 )
 def test_targets_type_check(targets, additional_targets, err_message):
-    aug = Compose([], additional_targets=additional_targets)
+    aug = Compose([A.NoOp()], additional_targets=additional_targets)
 
     with pytest.raises(TypeError) as exc_info:
         aug(**targets)
     assert str(exc_info.value) == err_message
 
-    aug = Compose([])
+    aug = Compose([A.NoOp()])
     aug.add_targets(additional_targets)
     with pytest.raises(TypeError) as exc_info:
         aug(**targets)
     assert str(exc_info.value) == err_message
 
 
 @pytest.mark.parametrize(
@@ -288,24 +288,24 @@
             None,
             {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 95, 95, 0], [85, 85, 95, 95, 0]]},
         ],
         [
             {"bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]]},
             BboxParams("pascal_voc", check_each_transform=True),
             None,
-            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]]},
+            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]]},
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=True),
             KeypointParams("xy", check_each_transform=True),
-            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]], "keypoints": np.array([[10, 10]]) + 25},
+            {"bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]], "keypoints": np.array([[10, 10]]) + 25},
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=False),
@@ -319,15 +319,15 @@
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
             },
             BboxParams("pascal_voc", check_each_transform=True),
             KeypointParams("xy", check_each_transform=False),
             {
-                "bboxes": [[25, 25, 35, 35, 0], [30, 30, 74, 74, 0]],
+                "bboxes": [[25, 25, 35, 35, 0], [30, 30, 75, 75, 0]],
                 "keypoints": np.array([[10, 10], [70, 70], [10, 70], [70, 10]]) + 25,
             },
         ],
         [
             {
                 "bboxes": [[0, 0, 10, 10, 0], [5, 5, 70, 70, 0], [60, 60, 70, 70, 0]],
                 "keypoints": [[10, 10], [70, 70], [10, 70], [70, 10]],
@@ -349,15 +349,15 @@
     res = augs(image=image, **targets)
 
     for key, item in expected.items():
         assert np.all(np.array(item) == np.array(res[key]))
 
 @pytest.mark.parametrize("image", IMAGES)
 def test_bbox_params_is_not_set(image, bboxes):
-    t = Compose([])
+    t = Compose([A.NoOp(p=1.0)])
     with pytest.raises(ValueError) as exc_info:
         t(image=image, bboxes=bboxes)
     assert str(exc_info.value) == "bbox_params must be specified for bbox transformations"
 
 
 @pytest.mark.parametrize(
     "compose_transform", get_filtered_transforms((BaseCompose,), custom_arguments={SomeOf: {"n": 1}})
@@ -390,15 +390,15 @@
     transforms(image=image)
 
 
 @pytest.mark.parametrize(
     "transforms",
     [
         Compose([ChannelShuffle(p=1)], p=1),
-        Compose([ChannelShuffle(p=0)], p=0),
+        # Compose([ChannelShuffle(p=0)], p=0),  # p=0, never calls, no process for data
     ],
 )
 def test_contiguous_output(transforms):
     image = np.empty([3, 24, 24], dtype=np.uint8).transpose(1, 2, 0)
     mask = np.empty([3, 24, 24], dtype=np.uint8).transpose(1, 2, 0)
 
     # check preconditions
@@ -417,26 +417,26 @@
     "targets",
     [
         {"image": np.ones((20, 20, 3), dtype=np.uint8), "mask": np.ones((30, 20))},
         {"image": np.ones((20, 20, 3), dtype=np.uint8), "masks": [np.ones((30, 20))]},
     ],
 )
 def test_compose_image_mask_equal_size(targets):
-    transforms = Compose([])
+    transforms = Compose([A.NoOp()])
 
     with pytest.raises(ValueError) as exc_info:
         transforms(**targets)
 
     assert str(exc_info.value).startswith(
         "Height and Width of image, mask or masks should be equal. "
         "You can disable shapes check by setting a parameter is_check_shapes=False "
         "of Compose class (do it only if you are sure about your data consistency)."
     )
     # test after disabling shapes check
-    transforms = Compose([], is_check_shapes=False)
+    transforms = Compose([A.NoOp()], is_check_shapes=False)
     transforms(**targets)
 
 
 def test_additional_targets():
     """Check add_target rises error if trying add existing target."""
     transforms = Compose([], additional_targets={"image2": "image"})
     # add same name, same target, OK
@@ -499,24 +499,24 @@
         [  # image only
             A.Blur(p=1),
             A.MedianBlur(p=1),
             A.ToGray(p=1),
             A.CLAHE(p=1),
             A.RandomBrightnessContrast(p=1),
             A.RandomGamma(p=1),
-            A.ImageCompression(quality_lower=75, p=1),
+            A.ImageCompression(quality_range=(75, 100), p=1),
         ],
         [  # with dual
             A.Blur(p=1),
             A.MedianBlur(p=1),
             A.ToGray(p=1),
             A.CLAHE(p=1),
             A.RandomBrightnessContrast(p=1),
             A.RandomGamma(p=1),
-            A.ImageCompression(quality_lower=75, p=1),
+            A.ImageCompression(quality_range=(75, 100), p=1),
             A.Crop(x_max=50, y_max=50),
         ]
     ]
 )
 @pytest.mark.parametrize(
     ["compose_args", "args"],
     [
@@ -574,7 +574,23 @@
     # Just check that everything is fine - no errors
 
     pipeline = A.Compose(transforms, **compose_args)
 
     res = pipeline(**args)
     for k in args.keys():
         assert k in res
+
+
+def test_compose_non_available_keys() -> None:
+    """Check that non available keys raises error, except `mask` and `masks`"""
+    transform = A.Compose(
+        [MagicMock(available_keys={"image"}),],
+    )
+    image = np.empty([10, 10, 3], dtype=np.uint8)
+    mask = np.empty([10, 10], dtype=np.uint8)
+    _res = transform(image=image, mask=mask)
+    _res = transform(image=image, masks=[mask])
+    with pytest.raises(ValueError) as exc_info:
+        _res = transform(image=image, image_2=mask)
+
+    expected_msg = "Key image_2 is not in available keys."
+    assert str(exc_info.value) == expected_msg
```

### Comparing `albumentations-1.4.6/tests/test_functional.py` & `albumentations-1.4.7/tests/test_functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from numpy.testing import assert_array_almost_equal_nulp, assert_almost_equal
 import skimage
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
 from albumentations.augmentations.utils import get_opencv_dtype_from_numpy, is_multispectral_image, MAX_VALUES_BY_DTYPE
-from albumentations.core.bbox_utils import filter_bboxes
+
 from albumentations.core.types import d4_group_elements
 from tests.conftest import IMAGES, RECTANGULAR_IMAGES
 from tests.utils import convert_2d_to_target_format, set_seed
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_vflip(target):
@@ -182,15 +182,15 @@
 
 @pytest.mark.parametrize("image", IMAGES)
 def test_compare_rotate_and_affine(image):
     # Generate the rotation matrix for a 60-degree rotation around the image center
     rotation_matrix = generate_rotation_matrix(image, 60)
 
     # Apply rotation using FGeometric.rotate
-    rotated_img_1 = FGeometric.rotate(image, angle=60, border_mode = cv2.BORDER_CONSTANT, value = 0)
+    rotated_img_1 = FGeometric.rotate(image, angle=60, border_mode = cv2.BORDER_CONSTANT, value = 0, interpolation=cv2.INTER_LINEAR)
 
     # Convert 2x3 cv2 matrix to 3x3 for skimage's ProjectiveTransform
     full_matrix = np.vstack([rotation_matrix, [0, 0, 1]])
     projective_transform = skimage.transform.ProjectiveTransform(matrix=full_matrix)
 
     # Apply rotation using warp_affine
     rotated_img_2 = FGeometric.warp_affine(
@@ -285,26 +285,26 @@
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_pad(target):
     img = np.array([[1, 2], [3, 4]], dtype=np.uint8)
     expected = np.array([[4, 3, 4, 3], [2, 1, 2, 1], [4, 3, 4, 3], [2, 1, 2, 1]], dtype=np.uint8)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
-    padded = FGeometric.pad(img, min_height=4, min_width=4)
+    padded = FGeometric.pad(img, min_height=4, min_width=4, border_mode=cv2.BORDER_REFLECT_101, value=None)
     assert np.array_equal(padded, expected)
 
 
 @pytest.mark.parametrize("target", ["image", "image_4_channels"])
 def test_pad_float(target):
     img = np.array([[0.1, 0.2], [0.3, 0.4]], dtype=np.float32)
     expected = np.array(
         [[0.4, 0.3, 0.4, 0.3], [0.2, 0.1, 0.2, 0.1], [0.4, 0.3, 0.4, 0.3], [0.2, 0.1, 0.2, 0.1]], dtype=np.float32
     )
     img, expected = convert_2d_to_target_format([img, expected], target=target)
-    padded_img = FGeometric.pad(img, min_height=4, min_width=4)
+    padded_img = FGeometric.pad(img, min_height=4, min_width=4, value=None, border_mode=cv2.BORDER_REFLECT_101)
     assert_array_almost_equal_nulp(padded_img, expected)
 
 
 @pytest.mark.parametrize(
     ["shift_params", "expected"], [[(-10, 0, 10), (117, 127, 137)], [(-200, 0, 200), (0, 127, 255)]]
 )
 def test_shift_rgb(shift_params, expected):
@@ -538,19 +538,19 @@
     actual_message = str(exc_info.value)
     assert (
         expected_message in actual_message or actual_message in expected_message
     ), f"Expected part of the error message to be: '{expected_message}', got: '{actual_message}'"
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
-def test_resize_default_interpolation(target):
+def test_resize_linear_interpolation(target):
     img = np.array([[1, 1, 1, 1], [2, 2, 2, 2], [3, 3, 3, 3], [4, 4, 4, 4]], dtype=np.uint8)
     expected = np.array([[2, 2], [4, 4]], dtype=np.uint8)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
-    resized_img = FGeometric.resize(img, 2, 2)
+    resized_img = FGeometric.resize(img, 2, 2, interpolation=cv2.INTER_LINEAR)
     height, width = resized_img.shape[:2]
     assert height == 2
     assert width == 2
     assert np.array_equal(resized_img, expected)
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
@@ -565,15 +565,15 @@
     assert np.array_equal(resized_img, expected)
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_resize_different_height_and_width(target):
     img = np.ones((100, 100), dtype=np.uint8)
     img = convert_2d_to_target_format([img], target=target)
-    resized_img = FGeometric.resize(img, height=20, width=30)
+    resized_img = FGeometric.resize(img, height=20, width=30, interpolation=cv2.INTER_LINEAR)
     height, width = resized_img.shape[:2]
     assert height == 20
     assert width == 30
     if target == "image":
         num_channels = resized_img.shape[2]
         assert num_channels == 3
 
@@ -581,15 +581,15 @@
 @pytest.mark.parametrize("target", ["image", "mask"])
 def test_resize_default_interpolation_float(target):
     img = np.array(
         [[0.1, 0.1, 0.1, 0.1], [0.2, 0.2, 0.2, 0.2], [0.3, 0.3, 0.3, 0.3], [0.4, 0.4, 0.4, 0.4]], dtype=np.float32
     )
     expected = np.array([[0.15, 0.15], [0.35, 0.35]], dtype=np.float32)
     img, expected = convert_2d_to_target_format([img, expected], target=target)
-    resized_img = FGeometric.resize(img, 2, 2)
+    resized_img = FGeometric.resize(img, 2, 2, interpolation=cv2.INTER_LINEAR)
     height, width = resized_img.shape[:2]
     assert height == 2
     assert width == 2
     assert_array_almost_equal_nulp(resized_img, expected)
 
 
 @pytest.mark.parametrize("target", ["image", "mask"])
@@ -681,68 +681,14 @@
 
 def test_bbox_transpose():
     assert np.allclose(FGeometric.bbox_transpose((0.7, 0.1, 0.8, 0.4), 100, 200), (0.1, 0.7, 0.4, 0.8))
     rot90 = FGeometric.bbox_rot90((0.7, 0.1, 0.8, 0.4), 2, 100, 200)
     reflected_anti_diagonal = FGeometric.bbox_transpose(rot90, 100, 200)
     assert np.allclose(reflected_anti_diagonal, (0.6, 0.2, 0.9, 0.3))
 
-
-@pytest.mark.parametrize(
-    ["bboxes", "min_area", "min_visibility", "target"],
-    [
-        (
-            [(0.1, 0.5, 1.1, 0.9), (-0.1, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
-            0,
-            0,
-            [(0.1, 0.5, 0.99, 0.9), (0.0, 0.5, 0.8, 0.9), (0.1, 0.5, 0.8, 0.9)],
-        ),
-        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.5, 0.5, 0.6)], 150, 0, [(0.1, 0.5, 0.8, 0.9)]),
-        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.9, 0.5, 1.6)], 0, 0.75, [(0.1, 0.5, 0.8, 0.9)]),
-        ([(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 1.1)], 0, 0.7, [(0.1, 0.5, 0.8, 0.9), (0.4, 0.7, 0.5, 0.99)]),
-    ],
-)
-def test_filter_bboxes(bboxes, min_area, min_visibility, target):
-    filtered_bboxes = filter_bboxes(bboxes, min_area=min_area, min_visibility=min_visibility, rows=100, cols=100)
-    assert filtered_bboxes == target
-
-
-@pytest.mark.parametrize(
-    ["bboxes", "img_width", "img_height", "min_width", "min_height", "target"],
-    [
-        [
-            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
-            100,
-            100,
-            20,
-            20,
-            [(0.1, 0.1, 0.9, 0.9)],
-        ],
-        [
-            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
-            100,
-            100,
-            20,
-            0,
-            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.9, 0.2)],
-        ],
-        [
-            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9), (0.1, 0.1, 0.9, 0.2), (0.1, 0.1, 0.2, 0.2)],
-            100,
-            100,
-            0,
-            20,
-            [(0.1, 0.1, 0.9, 0.9), (0.1, 0.1, 0.2, 0.9)],
-        ],
-    ],
-)
-def test_filter_bboxes_by_min_width_height(bboxes, img_width, img_height, min_width, min_height, target):
-    filtered_bboxes = filter_bboxes(bboxes, cols=img_width, rows=img_height, min_width=min_width, min_height=min_height)
-    assert filtered_bboxes == target
-
-
 def test_fun_max_size():
     target_width = 256
 
     img = np.empty((330, 49), dtype=np.uint8)
     out = FGeometric.smallest_max_size(img, target_width, interpolation=cv2.INTER_LINEAR)
 
     assert out.shape == (1724, target_width)
@@ -1022,15 +968,15 @@
 
 
 def test_maybe_process_in_chunks():
     image = np.random.randint(0, 256, (100, 100, 6), np.uint8)
 
     for i in range(1, image.shape[-1] + 1):
         before = image[:, :, :i]
-        after = FGeometric.rotate(before, angle=1)
+        after = FGeometric.rotate(before, angle=1, interpolation=cv2.INTER_LINEAR, border_mode=cv2.BORDER_REFLECT_101)
         assert before.shape == after.shape
 
 
 def test_multiply_uint8_optimized():
     image = np.random.randint(0, 256, [256, 320], np.uint8)
     m = 1.5
```

### Comparing `albumentations-1.4.6/tests/test_functional_cutout.py` & `albumentations-1.4.7/tests/test_functional_cutout.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_functional_mixing.py` & `albumentations-1.4.7/tests/test_functional_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_keypoint.py` & `albumentations-1.4.7/tests/test_keypoint.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_mixing.py` & `albumentations-1.4.7/tests/test_mixing.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_pydantic.py` & `albumentations-1.4.7/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_pytorch.py` & `albumentations-1.4.7/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_random.py` & `albumentations-1.4.7/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_serialization.py` & `albumentations-1.4.7/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_targets.py` & `albumentations-1.4.7/tests/test_targets.py`

 * *Files identical despite different names*

### Comparing `albumentations-1.4.6/tests/test_transforms.py` & `albumentations-1.4.7/tests/test_transforms.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import pytest
 import warnings
 from torchvision import transforms as torch_transforms
 
 import albumentations as A
 import albumentations.augmentations.functional as F
 import albumentations.augmentations.geometric.functional as FGeometric
-from albumentations.augmentations.blur.functional import gaussian_blur
+from albumentations.augmentations.transforms import ImageCompression
+from albumentations.core.types import ImageCompressionType
 from albumentations.random_utils import get_random_seed
 from tests.conftest import IMAGES, SQUARE_MULTI_UINT8_IMAGE, SQUARE_UINT8_IMAGE
 
 from .utils import get_dual_transforms, get_image_only_transforms, get_transforms, set_seed
 
 
 
@@ -1001,16 +1002,16 @@
                     [199, 99, 20, 20],
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
                     [15.65896994771262, 0.2946228229078849, 21.047137067150473, 4.617219579173327, 0],
-                    [194.29851584295034, 25.564320319214918, 199, 29.88691707548036, 0],
-                    [178.9528629328495, 95.38278042082668, 184.34103005228735, 99, 0],
+                    [194.29851584295034, 25.564320319214918, 199.68668296238818, 29.88691707548036, 0],
+                    [178.9528629328495, 95.38278042082668, 184.34103005228735, 99.70537717709212, 0],
                     [0.47485022613917677, 70.11308292451965, 5.701484157049652, 73.70074852182076, 0],
                 ],
                 "keypoints": [
                     [16.466635890349504, 0.2946228229078849, 147.04220486917677, 0.0],
                     [198.770582727028, 26.08267308836993, 157.04220486917674, 9.30232558139535],
                     [182.77879706281766, 98.84085782583904, 167.04220486917674, 18.6046511627907],
                     [0.4748502261391767, 73.05280756037699, 177.04220486917674, 27.90697674418604],
@@ -1033,15 +1034,15 @@
                     [0, 99, 30, 30],
                 ],
             },
             {
                 "bboxes": [
                     [0.3133170376117963, 25.564320319214918, 5.701484157049649, 29.88691707548036, 0],
                     [178.9528629328495, 0.2946228229078862, 184.34103005228735, 4.617219579173327, 0],
-                    [194.29851584295034, 70.11308292451965, 199, 74.43567968078509, 0],
+                    [194.29851584295034, 70.11308292451965, 199.68668296238818, 74.43567968078509, 0],
                     [15.658969947712617, 95.38278042082668, 20.88560387862309, 98.97044601812779, 0],
                 ],
                 "keypoints": [
                     [0.3133170376117963, 26.212261280658684, 212.95779513082323, 0.0],
                     [182.6172638742903, 0.42421101519664006, 222.95779513082323, 9.30232558139535],
                     [198.60904953850064, 73.18239575266574, 232.9577951308232, 18.6046511627907],
                     [16.305102701822126, 98.97044601812779, 242.9577951308232, 27.906976744186046],
@@ -1116,52 +1117,14 @@
     assert np.allclose(res_a["image"], res_b["image"])
     res_a = np.array(res_a["keypoints"])
     res_b = np.array(res_b["keypoints"])
     diff = np.round(np.abs(res_a - res_b))
     assert diff[:, :2].max() <= 2
     assert (diff[:, -1] % 360).max() <= 1
 
-@pytest.mark.parametrize(
-    "get_transform",
-    [
-        lambda sign: A.Affine(translate_px=sign * 2),
-        lambda sign: A.ShiftScaleRotate(shift_limit=(sign * 0.02, sign * 0.02), scale_limit=0, rotate_limit=0),
-    ],
-)
-@pytest.mark.parametrize(
-    ["bboxes", "expected", "min_visibility", "sign"],
-    [
-        [[(0, 0, 10, 10, 1)], [], 0.9, -1],
-        [[(0, 0, 10, 10, 1)], [(0, 0, 8, 8, 1)], 0.6, -1],
-        [[(90, 90, 100, 100, 1)], [], 0.9, 1],
-        [[(90, 90, 100, 100, 1)], [(92, 92, 99, 99, 1)], 0.49, 1],
-    ],
-)
-def test_bbox_clipping(get_transform, bboxes, expected, min_visibility: float, sign: int):
-    image = np.zeros([100, 100, 3], dtype=np.uint8)
-    transform = get_transform(sign)
-    transform.p = 1
-    transform = A.Compose([transform], bbox_params=A.BboxParams(format="pascal_voc", min_visibility=min_visibility))
-
-    res = transform(image=image, bboxes=bboxes)["bboxes"]
-    assert res == expected
-
-
-def test_bbox_clipping_perspective():
-    set_seed(0)
-    transform = A.Compose(
-        [A.Perspective(scale=(0.05, 0.05), p=1)], bbox_params=A.BboxParams(format="pascal_voc", min_visibility=0.6)
-    )
-
-    image = np.empty([1000, 1000, 3], dtype=np.uint8)
-    bboxes = np.array([[0, 0, 100, 100, 1]])
-    res = transform(image=image, bboxes=bboxes)["bboxes"]
-    assert len(res) == 0
-
-
 @pytest.mark.parametrize("seed", list(range(10)))
 def test_motion_blur_allow_shifted(seed):
     set_seed(seed)
 
     transform = A.MotionBlur(allow_shifted=False)
     kernel = transform.get_params()["kernel"]
 
@@ -1327,14 +1290,38 @@
                                              p=1)],
                     bbox_params=A.BboxParams("pascal_voc"),
                     keypoint_params=A.KeypointParams("xy"))
 
     assert aug(image=image, mask=image, bboxes=bboxes, keypoints=keypoints)
 
 @pytest.mark.parametrize("params, expected", [
+    # Test default initialization values
+    ({}, {"quality_range": (99, 100), "compression_type": ImageCompressionType.JPEG}),
+    # Test custom quality range and compression type
+    ({"quality_range": (10, 90), "compression_type": ImageCompressionType.WEBP},
+     {"quality_range": (10, 90), "compression_type": ImageCompressionType.WEBP}),
+    # Deprecated quality values handling
+    ({"quality_lower": 75}, {"quality_range": (75, 100)}),
+])
+def test_image_compression_initialization(params, expected):
+    img_comp = ImageCompression(**params)
+    for key, value in expected.items():
+        assert getattr(img_comp, key) == value, f"Failed on {key} with value {value}"
+
+@pytest.mark.parametrize("params", [
+    ({"quality_range": (101, 105)}),  # Invalid quality range
+    ({"quality_range": (0, 0)}),  # Invalid range for JPEG
+    ({"compression_type": "unknown"})  # Invalid compression type
+])
+def test_image_compression_invalid_input(params):
+    with pytest.raises(Exception):
+        ImageCompression(**params)
+
+
+@pytest.mark.parametrize("params, expected", [
     # Default values
     ({}, {"num_holes_range": (1, 1), "hole_height_range": (8, 8), "hole_width_range": (8, 8)}),
     # Boundary values
     ({"num_holes_range": (2, 3)}, {"num_holes_range": (2, 3)}),
     ({"hole_height_range": (0.1, 0.1)}, {"hole_height_range": (0.1, 0.1)}),
     ({"hole_width_range": (0.1, 0.1)}, {"hole_width_range": (0.1, 0.1)}),
     # Random fill value
@@ -1506,8 +1493,34 @@
 @pytest.mark.parametrize("params", [
     ({"scale_range": (0.9, 0.1)}),  # Invalid range, max < min
     ({"scale_range": (1.1, 1.2)}),  # Values outside valid scale range (0, 1)
     ({"interpolation_pair": {"downscale": 9999, "upscale": 9999}}),  # Invalid interpolation method
 ])
 def test_downscale_invalid_input(params):
     with pytest.raises(Exception):
-        aug = A.Downscale(**params, p=1)
+        A.Downscale(**params, p=1)
+
+
+@pytest.mark.parametrize("params, expected", [
+    # Default values
+    ({}, {"min_height": 1024, "min_width": 1024, "position": A.PadIfNeeded.PositionType.CENTER, "border_mode": cv2.BORDER_REFLECT_101}),
+    # Boundary values
+    ({"min_height": 800, "min_width": 800}, {"min_height": 800, "min_width": 800}),
+    ({"pad_height_divisor": 10, "min_height": None, "pad_width_divisor": 10, "min_width": None},
+     {"pad_height_divisor": 10, "min_height": None, "pad_width_divisor": 10, "min_width": None}),
+    ({"position": "top_left"}, {"position": A.PadIfNeeded.PositionType.TOP_LEFT}),
+    # Value handling when border_mode is BORDER_CONSTANT
+    ({"border_mode": cv2.BORDER_CONSTANT, "value": 255}, {"border_mode": cv2.BORDER_CONSTANT, "value": 255}),
+    ({"border_mode": cv2.BORDER_REFLECT_101, "value": 255}, {"border_mode": cv2.BORDER_CONSTANT, "value": 255}),
+    ({"border_mode": cv2.BORDER_CONSTANT, "value": [0, 0, 0]}, {"border_mode": cv2.BORDER_CONSTANT, "value": [0, 0, 0]}),
+    # Mask value handling
+    ({"border_mode": cv2.BORDER_CONSTANT, "value": [0, 0, 0], "mask_value": 128}, {"border_mode": cv2.BORDER_CONSTANT, "mask_value": 128, "value": [0, 0, 0]}),
+])
+def test_pad_if_needed_functionality(params, expected):
+    # Setup the augmentation with the provided parameters
+    aug = A.PadIfNeeded(**params, p=1)
+    # Get the initialization arguments to check against expected
+    aug_dict = {key: getattr(aug, key) for key in expected.keys()}
+
+    # Assert each expected key/value pair
+    for key, value in expected.items():
+        assert aug_dict[key] == value, f"Failed on {key} with value {value}"
```

