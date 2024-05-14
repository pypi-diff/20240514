# Comparing `tmp/auglib-1.0.2.tar.gz` & `tmp/auglib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auglib-1.0.2.tar", last modified: Tue Jan 30 07:07:04 2024, max compression
+gzip compressed data, was "auglib-1.0.3.tar", last modified: Tue May 14 07:03:05 2024, max compression
```

## Comparing `auglib-1.0.2.tar` & `auglib-1.0.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.114083 auglib-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.090083 auglib-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.094083 auglib-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-01-30 07:06:46.000000 auglib-1.0.2/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-30 07:06:46.000000 auglib-1.0.2/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-01-30 07:06:46.000000 auglib-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-30 07:06:46.000000 auglib-1.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-30 07:06:46.000000 auglib-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-30 07:06:46.000000 auglib-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14383 2024-01-30 07:06:46.000000 auglib-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-01-30 07:06:46.000000 auglib-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-30 07:06:46.000000 auglib-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-30 07:07:04.114083 auglib-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-30 07:06:46.000000 auglib-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.094083 auglib-1.0.2/auglib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.098083 auglib-1.0.2/auglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.102083 auglib-1.0.2/auglib/core/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)   469680 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/bin/libSoundTouch.so.1
--rwxr-xr-x   0 runner    (1001) docker     (127)   267080 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/bin/libcauglib.so
--rwxr-xr-x   0 runner    (1001) docker     (127)  1144656 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/bin/libopencore-amrnb.so.0
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/observe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/time.py
--rw-r--r--   0 runner    (1001) docker     (127)   151637 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.102083 auglib-1.0.2/auglib/observe/
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/observe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.102083 auglib-1.0.2/auglib/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.102083 auglib-1.0.2/auglib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-30 07:06:46.000000 auglib-1.0.2/auglib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.114083 auglib-1.0.2/auglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-30 07:07:04.000000 auglib-1.0.2/auglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-01-30 07:07:04.000000 auglib-1.0.2/auglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 07:07:04.000000 auglib-1.0.2/auglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-30 07:07:04.000000 auglib-1.0.2/auglib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 07:07:04.000000 auglib-1.0.2/auglib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.106083 auglib-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.106083 auglib-1.0.2/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/api-src/auglib.observe.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/api-src/auglib.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/api-src/auglib.transform.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/api-src/auglib.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/external.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-01-30 07:06:46.000000 auglib-1.0.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-01-30 07:06:46.000000 auglib-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-30 07:06:46.000000 auglib-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 07:07:04.114083 auglib-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.110083 auglib-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 07:07:04.114083 auglib-1.0.2/tests/test-assets/
--rw-r--r--   0 runner    (1001) docker     (127)    21230 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate10200_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate12200_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate4750_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate5150_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate5900_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate6700_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate7400_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate7950_ffmpeg.wav
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_cache_root.py
--rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_observe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_amrnb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_append.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_append_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_babble_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_bandstop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_clip_by_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_compose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_compress_dynamic_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_fade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_fft_convolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_gain_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_highpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_lowpass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_mix.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_normalize_by_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_pink_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_prepend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_prepend_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_resample.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_tone.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_trim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_white_noise_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_transform_white_noise_uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-30 07:06:46.000000 auglib-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.904780 auglib-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.884780 auglib-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.888780 auglib-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-14 07:02:54.000000 auglib-1.0.3/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 07:02:54.000000 auglib-1.0.3/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-14 07:02:54.000000 auglib-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-14 07:02:54.000000 auglib-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-14 07:02:54.000000 auglib-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 07:02:54.000000 auglib-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14653 2024-05-14 07:02:54.000000 auglib-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-14 07:02:54.000000 auglib-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-14 07:02:54.000000 auglib-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 07:03:05.904780 auglib-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-14 07:02:54.000000 auglib-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.888780 auglib-1.0.3/auglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.888780 auglib-1.0.3/auglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.892780 auglib-1.0.3/auglib/core/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   469680 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/bin/libSoundTouch.so.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)   267080 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/bin/libcauglib.so
+-rwxr-xr-x   0 runner    (1001) docker     (127)  1144656 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/bin/libopencore-amrnb.so.0
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/observe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151637 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.892780 auglib-1.0.3/auglib/observe/
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/observe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.892780 auglib-1.0.3/auglib/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.892780 auglib-1.0.3/auglib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-14 07:02:54.000000 auglib-1.0.3/auglib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.904780 auglib-1.0.3/auglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-05-14 07:03:05.000000 auglib-1.0.3/auglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-14 07:03:05.000000 auglib-1.0.3/auglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 07:03:05.000000 auglib-1.0.3/auglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 07:03:05.000000 auglib-1.0.3/auglib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 07:03:05.000000 auglib-1.0.3/auglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.896780 auglib-1.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.896780 auglib-1.0.3/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/api-src/auglib.observe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/api-src/auglib.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/api-src/auglib.transform.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/api-src/auglib.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/external.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-14 07:02:54.000000 auglib-1.0.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2024-05-14 07:02:54.000000 auglib-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 07:02:54.000000 auglib-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 07:03:05.904780 auglib-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.900780 auglib-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 07:03:05.900780 auglib-1.0.3/tests/test-assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    21230 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate10200_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate12200_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate4750_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate5150_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate5900_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate6700_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate7400_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate7950_ffmpeg.wav
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_cache_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30011 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_observe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_amrnb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_append.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_append_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_babble_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_bandstop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_clip_by_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_compose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_compress_dynamic_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_fade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_fft_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_gain_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_highpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_lowpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_normalize_by_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_pink_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_prepend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_prepend_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_resample.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_tone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_trim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_white_noise_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_transform_white_noise_uniform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-14 07:02:54.000000 auglib-1.0.3/tests/test_utils.py
```

### Comparing `auglib-1.0.2/.github/workflows/doc.yml` & `auglib-1.0.3/.github/workflows/doc.yml`

 * *Files 10% similar despite different names*

```diff
@@ -12,48 +12,48 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ '3.10' ]
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Cache air
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/air/1.4.2
         key: air-1.4.2
 
     - name: Cache cough-speech-sneeze
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/cough-speech-sneeze/2.0.1
         key: cough-speech-sneeze-2.0.1
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/emodb/1.4.1
         key: emodb-1.4.1
 
     - name: Cache micirp
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/micirp/1.0.0
         key: micirp-1.0.0
 
     - name: Cache musan
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/musan/1.0.0
         key: musan-1.0.0
 
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Ubuntu - install libsndfile
       run: |
         sudo apt-get update
         sudo apt-get install --no-install-recommends --yes libsndfile1 ffmpeg sox libavcodec-extra
@@ -65,9 +65,9 @@
 
     - name: Install docs requirements
       run: pip install -r docs/requirements.txt
 
     - name: Test building documentation
       run: python -m sphinx docs/ docs/_build/ -b html -W
 
-    #- name: Check links in documentation
-    #  run: python -m sphinx docs/ docs/_build/ -b linkcheck -W
+    - name: Check links in documentation
+      run: python -m sphinx docs/ docs/_build/ -b linkcheck -W
```

### Comparing `auglib-1.0.2/.github/workflows/publish.yml` & `auglib-1.0.3/.github/workflows/publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -17,45 +17,45 @@
 
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 2
 
     - name: Cache air
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/air/1.4.2
         key: air-1.4.2
 
     - name: Cache cough-speech-sneeze
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/cough-speech-sneeze/2.0.1
         key: cough-speech-sneeze-2.0.1
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/emodb/1.4.1
         key: emodb-1.4.1
 
     - name: Cache micirp
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/micirp/1.0.0
         key: micirp-1.0.0
 
     - name: Cache musan
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/musan/1.0.0
         key: musan-1.0.0
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build virtualenv
@@ -81,15 +81,15 @@
         pip install -r docs/requirements.txt
 
     - name: Build documentation
       run: |
         python -m sphinx docs/ build/html -b html
 
     - name: Deploy documentation to Github pages
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: ./build/html
 
     # Github release
     - name: Read CHANGELOG
       id: changelog
@@ -103,14 +103,14 @@
           echo 'body<<EOF'
           echo "$CHANGELOG"
           echo EOF
         } >> "$GITHUB_OUTPUT"
 
     - name: Create release on Github
       id: create_release
-      uses: softprops/action-gh-release@v1
+      uses: softprops/action-gh-release@v2
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
       with:
         tag_name: ${{ github.ref }}
         name: Release ${{ github.ref_name }}
         body: ${{ steps.changelog.outputs.body }}
```

### Comparing `auglib-1.0.2/.github/workflows/test.yml` & `auglib-1.0.3/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -25,18 +25,18 @@
             python-version: '3.11'
             tasks: tests
           - os: ubuntu-latest
             python-version: '3.9'
             tasks: tests
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Cache emodb
-      uses: actions/cache@v3
+      uses: actions/cache@v4
       with:
         path: ~/audb/emodb/1.4.1
         key: emodb-1.4.1
 
     - name: Set up Python ${{ matrix.python-version }} with Micromamba
       uses: mamba-org/setup-micromamba@v1
       with:
@@ -75,12 +75,12 @@
     - name: Install tests requirements
       run: pip install -r tests/requirements.txt
 
     - name: Test with pytest
       run: python -m pytest
 
     - name: Upload coverage to Codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         token: ${{ secrets.CODECOV_TOKEN }}
         file: ./coverage.xml
       if: matrix.os == 'ubuntu-latest'
```

### Comparing `auglib-1.0.2/.pre-commit-config.yaml` & `auglib-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/CHANGELOG.rst` & `auglib-1.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,29 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.3 (2024-05-14)
+--------------------------
+
+* Fixed: broken links
+  on the landing page
+  of the documentation
+
+
+Version 1.0.2 (2024-01-30)
+--------------------------
+
+* Fixed: ``auglib.transform.PinkNoise``
+  when applied to signals with odd sample length
+
+
 Version 1.0.1 (2024-01-26)
 --------------------------
 
 * Fixed: missing audio examples in documentation
 * Fixed: add missing entries to the changelog of 1.0.0
```

### Comparing `auglib-1.0.2/CONTRIBUTING.rst` & `auglib-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/LICENSE` & `auglib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/PKG-INFO` & `auglib-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auglib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Audio augmentations
 Author: Johannes Wagner, Andrea Crespi, Andreas Triantafyllopoulos, BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Anna Derington <aderington@audeering.com>
 License: MIT License
         
         Copyright (c) 2019- audEERING GmbH and Contributors
         
@@ -80,23 +80,23 @@
 It can be easily extended
 with external_ or `user defined`_ augmentations.
 
 Have a look at the installation_ instructions
 and listen to examples_.
 
 
-.. _datasets: https://audeering.github.io/usage.html#augment-a-database-to-disk
-.. _examples: https://audeering.github.io/examples.html
-.. _external: https://audeering.github.io/external.html
-.. _files: https://audeering.github.io/usage.html#augment-files-in-memory
-.. _installation: https://audeering.github.io/install.html
-.. _signals: https://audeering.github.io/usage.html#augment-a-signal
-.. _transforms: https://audeering.github.io/api/auglib.transform.html
-.. _usage: https://audeering.github.io/usage.html
-.. _user defined: https://audeering.github.io/api/auglib.transform.Function.html
+.. _datasets: https://audeering.github.io/auglib/usage.html#augment-a-dataset-to-disk
+.. _examples: https://audeering.github.io/auglib/examples.html
+.. _external: https://audeering.github.io/auglib/external.html
+.. _files: https://audeering.github.io/auglib/usage.html#augment-files-in-memory
+.. _installation: https://audeering.github.io/auglib/install.html
+.. _signals: https://audeering.github.io/auglib/usage.html#augment-a-signal
+.. _transforms: https://audeering.github.io/auglib/api/auglib.transform.html
+.. _usage: https://audeering.github.io/auglib/usage.html
+.. _user defined: https://audeering.github.io/auglib/api/auglib.transform.Function.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/auglib/workflows/Test/badge.svg
     :target: https://github.com/audeering/auglib/actions?query=workflow%3ATest
     :alt: Test status
 .. |coverage| image:: https://codecov.io/gh/audeering/auglib/branch/main/graph/badge.svg?token=3J0sF7GQhA
```

### Comparing `auglib-1.0.2/README.rst` & `auglib-1.0.3/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 It can be easily extended
 with external_ or `user defined`_ augmentations.
 
 Have a look at the installation_ instructions
 and listen to examples_.
 
 
-.. _datasets: https://audeering.github.io/usage.html#augment-a-database-to-disk
-.. _examples: https://audeering.github.io/examples.html
-.. _external: https://audeering.github.io/external.html
-.. _files: https://audeering.github.io/usage.html#augment-files-in-memory
-.. _installation: https://audeering.github.io/install.html
-.. _signals: https://audeering.github.io/usage.html#augment-a-signal
-.. _transforms: https://audeering.github.io/api/auglib.transform.html
-.. _usage: https://audeering.github.io/usage.html
-.. _user defined: https://audeering.github.io/api/auglib.transform.Function.html
+.. _datasets: https://audeering.github.io/auglib/usage.html#augment-a-dataset-to-disk
+.. _examples: https://audeering.github.io/auglib/examples.html
+.. _external: https://audeering.github.io/auglib/external.html
+.. _files: https://audeering.github.io/auglib/usage.html#augment-files-in-memory
+.. _installation: https://audeering.github.io/auglib/install.html
+.. _signals: https://audeering.github.io/auglib/usage.html#augment-a-signal
+.. _transforms: https://audeering.github.io/auglib/api/auglib.transform.html
+.. _usage: https://audeering.github.io/auglib/usage.html
+.. _user defined: https://audeering.github.io/auglib/api/auglib.transform.Function.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/auglib/workflows/Test/badge.svg
     :target: https://github.com/audeering/auglib/actions?query=workflow%3ATest
     :alt: Test status
 .. |coverage| image:: https://codecov.io/gh/audeering/auglib/branch/main/graph/badge.svg?token=3J0sF7GQhA
```

### Comparing `auglib-1.0.2/auglib/__init__.py` & `auglib-1.0.3/auglib/__init__.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/bin/libSoundTouch.so.1` & `auglib-1.0.3/auglib/core/bin/libSoundTouch.so.1`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/bin/libcauglib.so` & `auglib-1.0.3/auglib/core/bin/libcauglib.so`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/bin/libopencore-amrnb.so.0` & `auglib-1.0.3/auglib/core/bin/libopencore-amrnb.so.0`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/cache.py` & `auglib-1.0.3/auglib/core/cache.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/interface.py` & `auglib-1.0.3/auglib/core/interface.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/observe.py` & `auglib-1.0.3/auglib/core/observe.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/resolver.py` & `auglib-1.0.3/auglib/core/resolver.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/time.py` & `auglib-1.0.3/auglib/core/time.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/transform.py` & `auglib-1.0.3/auglib/core/transform.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/core/utils.py` & `auglib-1.0.3/auglib/core/utils.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/observe/__init__.py` & `auglib-1.0.3/auglib/observe/__init__.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib/transform/__init__.py` & `auglib-1.0.3/auglib/transform/__init__.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/auglib.egg-info/PKG-INFO` & `auglib-1.0.3/auglib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auglib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Audio augmentations
 Author: Johannes Wagner, Andrea Crespi, Andreas Triantafyllopoulos, BahaEddine Abrougui
 Author-email: Hagen Wierstorf <hwierstorf@audeering.com>, Anna Derington <aderington@audeering.com>
 License: MIT License
         
         Copyright (c) 2019- audEERING GmbH and Contributors
         
@@ -80,23 +80,23 @@
 It can be easily extended
 with external_ or `user defined`_ augmentations.
 
 Have a look at the installation_ instructions
 and listen to examples_.
 
 
-.. _datasets: https://audeering.github.io/usage.html#augment-a-database-to-disk
-.. _examples: https://audeering.github.io/examples.html
-.. _external: https://audeering.github.io/external.html
-.. _files: https://audeering.github.io/usage.html#augment-files-in-memory
-.. _installation: https://audeering.github.io/install.html
-.. _signals: https://audeering.github.io/usage.html#augment-a-signal
-.. _transforms: https://audeering.github.io/api/auglib.transform.html
-.. _usage: https://audeering.github.io/usage.html
-.. _user defined: https://audeering.github.io/api/auglib.transform.Function.html
+.. _datasets: https://audeering.github.io/auglib/usage.html#augment-a-dataset-to-disk
+.. _examples: https://audeering.github.io/auglib/examples.html
+.. _external: https://audeering.github.io/auglib/external.html
+.. _files: https://audeering.github.io/auglib/usage.html#augment-files-in-memory
+.. _installation: https://audeering.github.io/auglib/install.html
+.. _signals: https://audeering.github.io/auglib/usage.html#augment-a-signal
+.. _transforms: https://audeering.github.io/auglib/api/auglib.transform.html
+.. _usage: https://audeering.github.io/auglib/usage.html
+.. _user defined: https://audeering.github.io/auglib/api/auglib.transform.Function.html
 
 
 .. badges images and links:
 .. |tests| image:: https://github.com/audeering/auglib/workflows/Test/badge.svg
     :target: https://github.com/audeering/auglib/actions?query=workflow%3ATest
     :alt: Test status
 .. |coverage| image:: https://codecov.io/gh/audeering/auglib/branch/main/graph/badge.svg?token=3J0sF7GQhA
```

### Comparing `auglib-1.0.2/auglib.egg-info/SOURCES.txt` & `auglib-1.0.3/auglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/api-src/auglib.transform.rst` & `auglib-1.0.3/docs/api-src/auglib.transform.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/conf.py` & `auglib-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/examples.rst` & `auglib-1.0.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/external.rst` & `auglib-1.0.3/docs/external.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/index.rst` & `auglib-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/install.rst` & `auglib-1.0.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/docs/usage.rst` & `auglib-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/pyproject.toml` & `auglib-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile.wav` & `auglib-1.0.3/tests/test-assets/opensmile.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate10200_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate10200_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate12200_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate12200_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate4750_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate4750_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate5150_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate5150_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate5900_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate5900_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate6700_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate6700_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate7400_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate7400_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test-assets/opensmile_amrnb_rate7950_ffmpeg.wav` & `auglib-1.0.3/tests/test-assets/opensmile_amrnb_rate7950_ffmpeg.wav`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_cache_root.py` & `auglib-1.0.3/tests/test_cache_root.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_interface.py` & `auglib-1.0.3/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_observe.py` & `auglib-1.0.3/tests/test_observe.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_time.py` & `auglib-1.0.3/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_amrnb.py` & `auglib-1.0.3/tests/test_transform_amrnb.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_append.py` & `auglib-1.0.3/tests/test_transform_append.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_append_value.py` & `auglib-1.0.3/tests/test_transform_append_value.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_babble_noise.py` & `auglib-1.0.3/tests/test_transform_babble_noise.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_bandpass.py` & `auglib-1.0.3/tests/test_transform_bandpass.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_bandstop.py` & `auglib-1.0.3/tests/test_transform_bandstop.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_base.py` & `auglib-1.0.3/tests/test_transform_base.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_clip.py` & `auglib-1.0.3/tests/test_transform_clip.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_clip_by_ratio.py` & `auglib-1.0.3/tests/test_transform_clip_by_ratio.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_compose.py` & `auglib-1.0.3/tests/test_transform_compose.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_compress_dynamic_range.py` & `auglib-1.0.3/tests/test_transform_compress_dynamic_range.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_fade.py` & `auglib-1.0.3/tests/test_transform_fade.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_fft_convolve.py` & `auglib-1.0.3/tests/test_transform_fft_convolve.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_function.py` & `auglib-1.0.3/tests/test_transform_function.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_gain_stage.py` & `auglib-1.0.3/tests/test_transform_gain_stage.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_highpass.py` & `auglib-1.0.3/tests/test_transform_highpass.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_lowpass.py` & `auglib-1.0.3/tests/test_transform_lowpass.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_mask.py` & `auglib-1.0.3/tests/test_transform_mask.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_mix.py` & `auglib-1.0.3/tests/test_transform_mix.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_normalize_by_peak.py` & `auglib-1.0.3/tests/test_transform_normalize_by_peak.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_pink_noise.py` & `auglib-1.0.3/tests/test_transform_pink_noise.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_prepend.py` & `auglib-1.0.3/tests/test_transform_prepend.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_prepend_value.py` & `auglib-1.0.3/tests/test_transform_prepend_value.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_resample.py` & `auglib-1.0.3/tests/test_transform_resample.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_select.py` & `auglib-1.0.3/tests/test_transform_select.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_shift.py` & `auglib-1.0.3/tests/test_transform_shift.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_tone.py` & `auglib-1.0.3/tests/test_transform_tone.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_trim.py` & `auglib-1.0.3/tests/test_transform_trim.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_white_noise_gaussian.py` & `auglib-1.0.3/tests/test_transform_white_noise_gaussian.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_transform_white_noise_uniform.py` & `auglib-1.0.3/tests/test_transform_white_noise_uniform.py`

 * *Files identical despite different names*

### Comparing `auglib-1.0.2/tests/test_utils.py` & `auglib-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

