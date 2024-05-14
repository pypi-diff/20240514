# Comparing `tmp/lensless-1.0.6.tar.gz` & `tmp/lensless-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensless-1.0.6.tar", last modified: Wed Feb 21 14:15:53 2024, max compression
+gzip compressed data, was "lensless-1.0.7.tar", last modified: Tue May 14 10:32:38 2024, max compression
```

## Comparing `lensless-1.0.6.tar` & `lensless-1.0.7.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.892867 lensless-1.0.6/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    35149 2023-10-04 12:52:03.000000 lensless-1.0.6/LICENSE
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      510 2024-02-21 14:15:53.892867 lensless-1.0.6/PKG-INFO
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7205 2024-02-19 14:51:10.000000 lensless-1.0.6/README.rst
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/docs/
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/docs/source/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2293 2023-11-20 14:55:27.000000 lensless-1.0.6/docs/source/conf.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/lensless/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1097 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/__init__.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/lensless/eval/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:11:31.000000 lensless-1.0.6/lensless/eval/__init__.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9663 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/eval/benchmark.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10356 2024-02-21 13:51:41.000000 lensless-1.0.6/lensless/eval/metric.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/lensless/hardware/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:11:31.000000 lensless-1.0.6/lensless/hardware/__init__.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    12657 2023-11-18 07:40:48.000000 lensless-1.0.6/lensless/hardware/aperture.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      554 2023-12-05 15:40:23.000000 lensless-1.0.6/lensless/hardware/constants.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    15511 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/hardware/mask.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10918 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/hardware/sensor.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10586 2023-11-18 07:40:48.000000 lensless-1.0.6/lensless/hardware/slm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10735 2024-02-09 13:51:25.000000 lensless-1.0.6/lensless/hardware/trainable_mask.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    11917 2023-12-05 15:40:23.000000 lensless-1.0.6/lensless/hardware/utils.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/lensless/recon/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:11:31.000000 lensless-1.0.6/lensless/recon/__init__.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    13764 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/admm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8929 2024-01-23 16:11:40.000000 lensless-1.0.6/lensless/recon/admm_pnp.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10422 2023-10-04 12:52:03.000000 lensless-1.0.6/lensless/recon/apgd.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/lensless/recon/drunet/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9912 2023-10-04 12:52:03.000000 lensless-1.0.6/lensless/recon/drunet/basicblock.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6412 2023-11-18 07:40:48.000000 lensless-1.0.6/lensless/recon/drunet/network_unet.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8305 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/gd.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1383 2023-10-04 12:52:03.000000 lensless-1.0.6/lensless/recon/mirflickr.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8372 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/model_dict.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    21990 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/recon.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6228 2023-10-04 12:52:03.000000 lensless-1.0.6/lensless/recon/rfft_convolve.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6371 2023-10-04 12:52:03.000000 lensless-1.0.6/lensless/recon/tikhonov.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1712 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/trainable_inversion.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    13451 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/trainable_recon.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8344 2023-12-18 12:26:16.000000 lensless-1.0.6/lensless/recon/unrolled_admm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     4199 2023-11-18 07:40:48.000000 lensless-1.0.6/lensless/recon/unrolled_fista.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    33149 2024-02-09 12:13:21.000000 lensless-1.0.6/lensless/recon/utils.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/lensless/utils/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:11:31.000000 lensless-1.0.6/lensless/utils/__init__.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    35692 2024-02-09 12:44:30.000000 lensless-1.0.6/lensless/utils/dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    13063 2023-12-05 15:40:23.000000 lensless-1.0.6/lensless/utils/image.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    17833 2024-02-09 12:44:37.000000 lensless-1.0.6/lensless/utils/io.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8253 2024-01-17 16:13:53.000000 lensless-1.0.6/lensless/utils/plot.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5754 2023-12-13 16:15:13.000000 lensless-1.0.6/lensless/utils/simulation.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)       22 2024-02-21 14:11:58.000000 lensless-1.0.6/lensless/version.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.880867 lensless-1.0.6/lensless.egg-info/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      510 2024-02-21 14:15:53.000000 lensless-1.0.6/lensless.egg-info/PKG-INFO
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2905 2024-02-21 14:15:53.000000 lensless-1.0.6/lensless.egg-info/SOURCES.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)        1 2024-02-21 14:15:53.000000 lensless-1.0.6/lensless.egg-info/dependency_links.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      122 2024-02-21 14:15:53.000000 lensless-1.0.6/lensless.egg-info/requires.txt
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      360 2024-02-21 14:15:53.000000 lensless-1.0.6/lensless.egg-info/top_level.txt
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/profile/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2659 2023-10-04 12:52:03.000000 lensless-1.0.6/profile/admm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8647 2023-10-04 12:52:03.000000 lensless-1.0.6/profile/diffusercam_admm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7637 2023-10-04 12:52:03.000000 lensless-1.0.6/profile/diffusercam_gd.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3602 2023-10-04 12:52:03.000000 lensless-1.0.6/profile/gradient_descent.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      113 2023-10-04 12:52:03.000000 lensless-1.0.6/pyproject.toml
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/scripts/
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/scripts/classify/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10356 2024-02-21 13:51:41.000000 lensless-1.0.6/scripts/classify/train_celeba_vit.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.884867 lensless-1.0.6/scripts/data/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1290 2024-02-08 10:03:23.000000 lensless-1.0.6/scripts/data/16bit_image.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/data/3d/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      627 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/data/3d/mat_to_npy.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      795 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/data/3d/mat_to_npz.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     4258 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/data/3d/npy_to_obj.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3462 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/data/3d/npy_to_tiff.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3969 2024-02-20 16:11:45.000000 lensless-1.0.6/scripts/data/download_diffusercam_huggingface.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3030 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/data/prepare_mirflickr_subset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5435 2024-02-20 10:57:47.000000 lensless-1.0.6/scripts/data/upload_diffusercam_huggingface.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/demo/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    32971 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/demo/telegram_bot.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7697 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/demo.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/eval/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    12342 2024-02-09 12:13:21.000000 lensless-1.0.6/scripts/eval/benchmark_recon.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2054 2023-11-18 07:40:48.000000 lensless-1.0.6/scripts/eval/compute_metrics_from_original.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3815 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/eval/mirflickr_admm.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/hardware/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3914 2023-11-18 07:40:48.000000 lensless-1.0.6/scripts/hardware/config_digicam.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1971 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/hardware/digicam_measure_psfs.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)      435 2023-11-18 07:40:48.000000 lensless-1.0.6/scripts/hardware/set_digicam_mask_distance.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/measure/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5639 2023-11-18 07:40:48.000000 lensless-1.0.6/scripts/measure/analyze_image.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2741 2023-11-18 07:40:48.000000 lensless-1.0.6/scripts/measure/analyze_measured_dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    10191 2023-12-05 15:40:23.000000 lensless-1.0.6/scripts/measure/collect_dataset_on_device.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5609 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/measure/collect_mnist.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7339 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/measure/collect_mnist_on_device.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2319 2023-11-18 07:41:26.000000 lensless-1.0.6/scripts/measure/compare_measured_original.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6015 2023-11-30 13:13:42.000000 lensless-1.0.6/scripts/measure/digicam_capture.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3001 2024-02-09 14:14:24.000000 lensless-1.0.6/scripts/measure/digicam_example.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9872 2023-12-05 15:40:23.000000 lensless-1.0.6/scripts/measure/on_device_capture.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3594 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/measure/prep_display_image.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9989 2023-12-05 15:40:23.000000 lensless-1.0.6/scripts/measure/remote_capture.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2356 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/measure/remote_display.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.888867 lensless-1.0.6/scripts/recon/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7497 2024-02-09 12:13:21.000000 lensless-1.0.6/scripts/recon/admm.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     4238 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/recon/admm_mirflickr.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2252 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/recon/apgd_pycsou.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6026 2024-02-21 13:51:41.000000 lensless-1.0.6/scripts/recon/dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7331 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/recon/demo.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2756 2024-02-09 12:13:21.000000 lensless-1.0.6/scripts/recon/diffusercam_mirflickr.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2600 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/recon/gradient_descent.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)    25612 2024-02-09 13:52:09.000000 lensless-1.0.6/scripts/recon/train_unrolled.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.892867 lensless-1.0.6/scripts/sim/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6253 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     6362 2024-01-12 15:26:49.000000 lensless-1.0.6/scripts/sim/digicam_psf.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     9507 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/mask_dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     8551 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/mask_single_file.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3457 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/single_file.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2573 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/torch_custom_dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2858 2023-10-04 12:52:03.000000 lensless-1.0.6/scripts/sim/torch_dataset.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)       38 2024-02-21 14:15:53.892867 lensless-1.0.6/setup.cfg
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1250 2024-02-21 14:11:31.000000 lensless-1.0.6/setup.py
-drwxr-xr-x   0 bezzam   (157676) LCAV-unit (11225)        0 2024-02-21 14:15:53.892867 lensless-1.0.6/test/
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     7896 2023-10-04 12:52:03.000000 lensless-1.0.6/test/test_algos.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     2120 2023-10-04 12:52:03.000000 lensless-1.0.6/test/test_convolver.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     1616 2023-10-04 12:52:03.000000 lensless-1.0.6/test/test_io.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     3064 2023-12-06 16:09:28.000000 lensless-1.0.6/test/test_masks.py
--rw-r--r--   0 bezzam   (157676) LCAV-unit (11225)     5877 2023-10-04 12:52:03.000000 lensless-1.0.6/test/test_sensor.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.412523 lensless-1.0.7/
+-rw-r--r--   0 eric       (501) staff       (20)    35149 2024-02-05 20:04:27.000000 lensless-1.0.7/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      752 2024-05-14 10:32:38.412332 lensless-1.0.7/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     9448 2024-05-01 14:15:23.000000 lensless-1.0.7/README.rst
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.392129 lensless-1.0.7/docs/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.394494 lensless-1.0.7/docs/source/
+-rw-r--r--   0 eric       (501) staff       (20)     2348 2024-04-25 16:01:38.000000 lensless-1.0.7/docs/source/conf.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.395074 lensless-1.0.7/lensless/
+-rw-r--r--   0 eric       (501) staff       (20)     1097 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.396000 lensless-1.0.7/lensless/eval/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/eval/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    11942 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/eval/benchmark.py
+-rw-r--r--   0 eric       (501) staff       (20)    10397 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/eval/metric.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.398223 lensless-1.0.7/lensless/hardware/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/hardware/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    12657 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/hardware/aperture.py
+-rw-r--r--   0 eric       (501) staff       (20)      554 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/hardware/constants.py
+-rw-r--r--   0 eric       (501) staff       (20)    18103 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/hardware/fabrication.py
+-rw-r--r--   0 eric       (501) staff       (20)    29392 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/hardware/mask.py
+-rw-r--r--   0 eric       (501) staff       (20)    10919 2024-04-23 07:53:35.000000 lensless-1.0.7/lensless/hardware/sensor.py
+-rw-r--r--   0 eric       (501) staff       (20)    11298 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/hardware/slm.py
+-rw-r--r--   0 eric       (501) staff       (20)    15369 2024-04-23 07:53:35.000000 lensless-1.0.7/lensless/hardware/trainable_mask.py
+-rw-r--r--   0 eric       (501) staff       (20)    11992 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/hardware/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.400493 lensless-1.0.7/lensless/recon/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/recon/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    14572 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/recon/admm.py
+-rw-r--r--   0 eric       (501) staff       (20)    10421 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/apgd.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.400836 lensless-1.0.7/lensless/recon/drunet/
+-rw-r--r--   0 eric       (501) staff       (20)     9912 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/recon/drunet/basicblock.py
+-rw-r--r--   0 eric       (501) staff       (20)     6412 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/recon/drunet/network_unet.py
+-rw-r--r--   0 eric       (501) staff       (20)     8913 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/recon/gd.py
+-rw-r--r--   0 eric       (501) staff       (20)     1383 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/recon/mirflickr.py
+-rw-r--r--   0 eric       (501) staff       (20)     9864 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/model_dict.py
+-rw-r--r--   0 eric       (501) staff       (20)    22244 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/recon.py
+-rw-r--r--   0 eric       (501) staff       (20)     6797 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/rfft_convolve.py
+-rw-r--r--   0 eric       (501) staff       (20)     6371 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/recon/tikhonov.py
+-rw-r--r--   0 eric       (501) staff       (20)     1854 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/trainable_inversion.py
+-rw-r--r--   0 eric       (501) staff       (20)    14217 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/trainable_recon.py
+-rw-r--r--   0 eric       (501) staff       (20)     8741 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/recon/unrolled_admm.py
+-rw-r--r--   0 eric       (501) staff       (20)     4199 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/recon/unrolled_fista.py
+-rw-r--r--   0 eric       (501) staff       (20)    39224 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/recon/utils.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.402016 lensless-1.0.7/lensless/utils/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2024-04-08 14:51:21.000000 lensless-1.0.7/lensless/utils/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)    60149 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/utils/dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)    13063 2024-05-02 14:48:54.000000 lensless-1.0.7/lensless/utils/image.py
+-rw-r--r--   0 eric       (501) staff       (20)    18630 2024-05-14 10:13:12.000000 lensless-1.0.7/lensless/utils/io.py
+-rw-r--r--   0 eric       (501) staff       (20)    10781 2024-04-25 16:01:38.000000 lensless-1.0.7/lensless/utils/plot.py
+-rw-r--r--   0 eric       (501) staff       (20)     5754 2024-02-05 20:04:27.000000 lensless-1.0.7/lensless/utils/simulation.py
+-rw-r--r--   0 eric       (501) staff       (20)       22 2024-05-14 10:14:45.000000 lensless-1.0.7/lensless/version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.395574 lensless-1.0.7/lensless.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      752 2024-05-14 10:32:38.000000 lensless-1.0.7/lensless.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2862 2024-05-14 10:32:38.000000 lensless-1.0.7/lensless.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2024-05-14 10:32:38.000000 lensless-1.0.7/lensless.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)      122 2024-05-14 10:32:38.000000 lensless-1.0.7/lensless.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)      127 2024-05-14 10:32:38.000000 lensless-1.0.7/lensless.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.402284 lensless-1.0.7/notebooks/
+-rw-r--r--   0 eric       (501) staff       (20)     1952 2024-04-17 15:03:28.000000 lensless-1.0.7/notebooks/test_kc_dataset.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.403293 lensless-1.0.7/profile/
+-rw-r--r--   0 eric       (501) staff       (20)     2667 2024-05-14 10:13:12.000000 lensless-1.0.7/profile/admm.py
+-rw-r--r--   0 eric       (501) staff       (20)     8647 2024-02-05 20:04:27.000000 lensless-1.0.7/profile/diffusercam_admm.py
+-rw-r--r--   0 eric       (501) staff       (20)     7637 2024-02-05 20:04:27.000000 lensless-1.0.7/profile/diffusercam_gd.py
+-rw-r--r--   0 eric       (501) staff       (20)     3610 2024-05-14 10:13:12.000000 lensless-1.0.7/profile/gradient_descent.py
+-rw-r--r--   0 eric       (501) staff       (20)      113 2024-02-05 20:04:27.000000 lensless-1.0.7/pyproject.toml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.403443 lensless-1.0.7/scripts/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.403675 lensless-1.0.7/scripts/classify/
+-rw-r--r--   0 eric       (501) staff       (20)    10438 2024-04-08 14:51:21.000000 lensless-1.0.7/scripts/classify/train_celeba_vit.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.404740 lensless-1.0.7/scripts/data/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.405293 lensless-1.0.7/scripts/data/3d/
+-rw-r--r--   0 eric       (501) staff       (20)      627 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/data/3d/mat_to_npy.py
+-rw-r--r--   0 eric       (501) staff       (20)      795 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/data/3d/mat_to_npz.py
+-rw-r--r--   0 eric       (501) staff       (20)     4258 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/data/3d/npy_to_obj.py
+-rw-r--r--   0 eric       (501) staff       (20)     3462 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/data/3d/npy_to_tiff.py
+-rw-r--r--   0 eric       (501) staff       (20)     7602 2024-05-01 14:15:23.000000 lensless-1.0.7/scripts/data/authenticate.py
+-rw-r--r--   0 eric       (501) staff       (20)     2565 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/data/authenticate_roc.py
+-rw-r--r--   0 eric       (501) staff       (20)     3030 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/data/prepare_mirflickr_subset.py
+-rw-r--r--   0 eric       (501) staff       (20)      817 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/data/rename_mirflickr25k.py
+-rw-r--r--   0 eric       (501) staff       (20)     9865 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/data/upload_dataset_huggingface.py
+-rw-r--r--   0 eric       (501) staff       (20)     5609 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/data/upload_diffusercam_huggingface.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.405437 lensless-1.0.7/scripts/demo/
+-rw-r--r--   0 eric       (501) staff       (20)    39282 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/demo/telegram_bot.py
+-rw-r--r--   0 eric       (501) staff       (20)     9171 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/demo.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.405764 lensless-1.0.7/scripts/eval/
+-rw-r--r--   0 eric       (501) staff       (20)    13484 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/eval/benchmark_recon.py
+-rw-r--r--   0 eric       (501) staff       (20)     2054 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/eval/compute_metrics_from_original.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.406416 lensless-1.0.7/scripts/hardware/
+-rw-r--r--   0 eric       (501) staff       (20)     3914 2024-04-26 21:50:54.000000 lensless-1.0.7/scripts/hardware/config_digicam.py
+-rw-r--r--   0 eric       (501) staff       (20)     1971 2024-04-26 21:50:54.000000 lensless-1.0.7/scripts/hardware/digicam_measure_psfs.py
+-rw-r--r--   0 eric       (501) staff       (20)      435 2024-04-26 21:50:54.000000 lensless-1.0.7/scripts/hardware/set_digicam_mask_distance.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.407673 lensless-1.0.7/scripts/measure/
+-rw-r--r--   0 eric       (501) staff       (20)     5699 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/measure/analyze_image.py
+-rw-r--r--   0 eric       (501) staff       (20)     2741 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/measure/analyze_measured_dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)    13083 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/measure/collect_dataset_on_device.py
+-rw-r--r--   0 eric       (501) staff       (20)     9872 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/measure/on_device_capture.py
+-rw-r--r--   0 eric       (501) staff       (20)     4067 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/measure/prep_display_image.py
+-rw-r--r--   0 eric       (501) staff       (20)    10005 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/measure/remote_capture.py
+-rw-r--r--   0 eric       (501) staff       (20)     2356 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/measure/remote_display.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.409823 lensless-1.0.7/scripts/recon/
+-rw-r--r--   0 eric       (501) staff       (20)     7501 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/recon/admm.py
+-rw-r--r--   0 eric       (501) staff       (20)     2252 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/recon/apgd_pycsou.py
+-rw-r--r--   0 eric       (501) staff       (20)     6305 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/recon/dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)     6977 2024-04-25 16:01:38.000000 lensless-1.0.7/scripts/recon/demo.py
+-rw-r--r--   0 eric       (501) staff       (20)     2756 2024-04-08 14:51:21.000000 lensless-1.0.7/scripts/recon/diffusercam_mirflickr.py
+-rw-r--r--   0 eric       (501) staff       (20)     3222 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/recon/digicam_mirflickr.py
+-rw-r--r--   0 eric       (501) staff       (20)     2604 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/recon/gradient_descent.py
+-rw-r--r--   0 eric       (501) staff       (20)     2322 2024-05-03 18:14:04.000000 lensless-1.0.7/scripts/recon/mirflickr_hugging_face.py
+-rw-r--r--   0 eric       (501) staff       (20)      813 2024-04-17 17:31:32.000000 lensless-1.0.7/scripts/recon/recon_miniset.py
+-rw-r--r--   0 eric       (501) staff       (20)    19294 2024-05-14 10:13:12.000000 lensless-1.0.7/scripts/recon/train_learning_based.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.411072 lensless-1.0.7/scripts/sim/
+-rw-r--r--   0 eric       (501) staff       (20)     6253 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)     6362 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/digicam_psf.py
+-rw-r--r--   0 eric       (501) staff       (20)     9507 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/mask_dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)     8551 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/mask_single_file.py
+-rw-r--r--   0 eric       (501) staff       (20)     3457 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/single_file.py
+-rw-r--r--   0 eric       (501) staff       (20)     2573 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/torch_custom_dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)     2858 2024-02-05 20:04:27.000000 lensless-1.0.7/scripts/sim/torch_dataset.py
+-rw-r--r--   0 eric       (501) staff       (20)       38 2024-05-14 10:32:38.412562 lensless-1.0.7/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)     1250 2024-05-14 10:28:18.000000 lensless-1.0.7/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2024-05-14 10:32:38.412056 lensless-1.0.7/test/
+-rw-r--r--   0 eric       (501) staff       (20)     7907 2024-05-14 10:13:12.000000 lensless-1.0.7/test/test_algos.py
+-rw-r--r--   0 eric       (501) staff       (20)     2120 2024-04-22 20:24:02.000000 lensless-1.0.7/test/test_convolver.py
+-rw-r--r--   0 eric       (501) staff       (20)     1620 2024-05-14 10:13:12.000000 lensless-1.0.7/test/test_io.py
+-rw-r--r--   0 eric       (501) staff       (20)     3098 2024-05-14 10:13:12.000000 lensless-1.0.7/test/test_masks.py
+-rw-r--r--   0 eric       (501) staff       (20)     5877 2024-02-05 20:04:27.000000 lensless-1.0.7/test/test_sensor.py
```

### Comparing `lensless-1.0.6/LICENSE` & `lensless-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/README.rst` & `lensless-1.0.7/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,32 +12,52 @@
       :alt: DOI
 
 .. image:: https://static.pepy.tech/badge/lensless
       :target: https://www.pepy.tech/projects/lensless
       :alt: Downloads
 
 
-*A Hardware and Software Toolkit for Lensless Computational Imaging with a Raspberry Pi*
------------------------------------------------------------------------------------------
+.. image:: https://colab.research.google.com/assets/colab-badge.svg
+      :target: https://lensless.readthedocs.io/en/latest/examples.html
+      :alt: notebooks
+
+.. image:: https://huggingface.co/datasets/huggingface/badges/resolve/main/powered-by-huggingface-dark.svg
+      :target: https://huggingface.co/bezzam
+      :alt: huggingface
+
+
+*A Hardware and Software Toolkit for Lensless Computational Imaging*
+--------------------------------------------------------------------
 
 .. image:: https://github.com/LCAV/LenslessPiCam/raw/main/scripts/recon/example.png
     :alt: Lensless imaging example
     :align: center
 
 
-This toolkit has everything you need to perform imaging with a lensless
-camera. We make use of a low-cost implementation of DiffuserCam [1]_, 
-where we use a piece of tape instead of the lens and the
-`Raspberry Pi HQ camera sensor <https://www.raspberrypi.com/products/raspberry-pi-high-quality-camera>`__
-(the `V2 sensor <https://www.raspberrypi.com/products/camera-module-v2/>`__
-is also supported). Similar principles and methods can be used for a
-different lensless encoder and a different sensor. 
+This toolkit has everything you need to perform imaging with a lensless camera.
+The sensor in most examples is the `Raspberry Pi HQ <https://www.raspberrypi.com/products/raspberry-pi-high-quality-camera>`__,
+camera sensor as it is low cost (around 50 USD) and has a high resolution (12 MP).
+The lensless encoder/mask used in most examples is either a piece of tape or a `low-cost LCD <https://www.adafruit.com/product/358>`__.
+As **modularity** is a key feature of this toolkit, we try to support different sensors and/or lensless encoders.
+
+The toolkit includes:
+
+* Camera assembly tutorials (`link <https://lensless.readthedocs.io/en/latest/building.html>`__).
+* Measurement scripts (`link <https://lensless.readthedocs.io/en/latest/measurement.html>`__).
+* Dataset preparation and loading tools, with `Hugging Face <https://huggingface.co/bezzam>`__ integration (`slides <https://docs.google.com/presentation/d/18h7jTcp20jeoiF8dJIEcc7wHgjpgFgVxZ_bJ04W55lg/edit?usp=sharing>`__ on uploading a dataset to Hugging Face with `this script <https://github.com/LCAV/LenslessPiCam/blob/main/scripts/data/upload_dataset_huggingface.py>`__).
+* `Reconstruction algorithms <https://lensless.readthedocs.io/en/latest/reconstruction.html>`__ (e.g. FISTA, ADMM, unrolled algorithms, trainable inversion, pre- and post-processors).
+* `Training script <https://github.com/LCAV/LenslessPiCam/blob/main/scripts/recon/train_learning_based.py>`__ for learning-based reconstruction.
+* `Pre-trained models <https://github.com/LCAV/LenslessPiCam/blob/main/lensless/recon/model_dict.py>`__ that can be loaded from `Hugging Face <https://huggingface.co/bezzam>`__, for example in `this script <https://github.com/LCAV/LenslessPiCam/blob/main/scripts/recon/diffusercam_mirflickr.py>`__.
+* Mask `design <https://lensless.readthedocs.io/en/latest/mask.html>`__ and `fabrication <https://lensless.readthedocs.io/en/latest/fabrication.html>`__ tools.
+* `Simulation tools <https://lensless.readthedocs.io/en/latest/simulation.html>`__.
+* `Evalutions tools <https://lensless.readthedocs.io/en/latest/evaluation.html>`__ (e.g. PSNR, LPIPS, SSIM, visualizations).
+* `Demo <https://lensless.readthedocs.io/en/latest/demo.html#telegram-demo>`__ that can be run on Telegram!
 
-*If you are interested in exploring reconstruction algorithms without building the camera, that is entirely possible!*
-The provided reconstruction algorithms can be used with the provided data or simulated data.
+Please refer to the `documentation <http://lensless.readthedocs.io>`__ for more details,
+while an overview of example notebooks can be found `here <https://lensless.readthedocs.io/en/latest/examples.html>`__.
 
 We've also written a few Medium articles to guide users through the process
 of building the camera, measuring data with it, and reconstruction.
 They are all laid out in `this post <https://medium.com/@bezzam/a-complete-lensless-imaging-tutorial-hardware-software-and-algorithms-8873fa81a660>`__.
 
 Setup 
 -----
@@ -142,31 +162,39 @@
 
    # install in virtual environment
    cd LenslessPiCam
    virtualenv --system-site-packages -p python3 lensless_env
    source lensless_env/bin/activate
    pip install --no-deps -e .
    pip install -r rpi_requirements.txt
+
+   # test on-device camera capture (after setting up the camera)
+   source lensless_env/bin/activate
+   python scripts/measure/on_device_capture.py
+
+You may still need to manually install ``numpy`` and/or ``scipy`` with ``pip`` in case libraries (e.g. ``libopenblas.so.0``) cannot be detected.
    
 
 Acknowledgements
 ----------------
 
 The idea of building a lensless camera from a Raspberry Pi and a piece of 
 tape comes from Prof. Laura Waller's group at UC Berkeley. So a huge kudos 
 to them for the idea and making tools/code/data available! Below is some of 
 the work that has inspired this toolkit:
 
 * `Build your own DiffuserCam tutorial <https://waller-lab.github.io/DiffuserCam/tutorial>`__.
-* `DiffuserCam Lensless MIR Flickr dataset <https://waller-lab.github.io/LenslessLearning/dataset.html>`__ [2]_. 
+* `DiffuserCam Lensless MIR Flickr dataset <https://waller-lab.github.io/LenslessLearning/dataset.html>`__ [1]_. 
 
 A few students at EPFL have also contributed to this project:
 
 * Julien Sahli: support and extension of algorithms for 3D.
 * Yohann Perron: unrolled algorithms for reconstruction.
+* Aaron Fargeon: mask designs.
+* Rein Bentdal: mask fabrication with 3D printing.
 
 Citing this work
 ----------------
 
 If you use these tools in your own research, please cite the following:
 
 ::
@@ -183,10 +211,8 @@
       title = {LenslessPiCam: A Hardware and Software Platform for Lensless Computational Imaging with a Raspberry Pi},
       journal = {Journal of Open Source Software}
    }
 
 References
 ----------
 
-.. [1] Antipa, N., Kuo, G., Heckel, R., Mildenhall, B., Bostan, E., Ng, R., & Waller, L. (2018). DiffuserCam: lensless single-exposure 3D imaging. Optica, 5(1), 1-9.
-
-.. [2] Monakhova, K., Yurtsever, J., Kuo, G., Antipa, N., Yanny, K., & Waller, L. (2019). Learned reconstructions for practical mask-based lensless imaging. Optics express, 27(20), 28075-28090.
+.. [1] Monakhova, K., Yurtsever, J., Kuo, G., Antipa, N., Yanny, K., & Waller, L. (2019). Learned reconstructions for practical mask-based lensless imaging. Optics express, 27(20), 28075-28090.
```

### Comparing `lensless-1.0.6/docs/source/conf.py` & `lensless-1.0.7/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     "paramiko.ssh_exception",
     "perlin_numpy",
     "hydra",
     "hydra.utils",
     "scipy.special",
     "matplotlib.cm",
     "pyffs",
+    "datasets",
+    "huggingface_hub",
+    "cadquery",
 ]
 for mod_name in MOCK_MODULES:
     sys.modules[mod_name] = mock.Mock()
 # -- Project information
 
 sys.path.insert(0, os.path.abspath(os.path.join("..", "..")))
 from lensless import __version__
```

### Comparing `lensless-1.0.6/lensless/__init__.py` & `lensless-1.0.7/lensless/__init__.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/eval/benchmark.py` & `lensless-1.0.7/lensless/eval/benchmark.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from lensless.utils.dataset import DiffuserCamTestDataset
 from lensless.utils.io import save_image
 from waveprop.noise import add_shot_noise
 from tqdm import tqdm
 import os
 import numpy as np
+import wandb
 
 try:
     import torch
     from torch.utils.data import DataLoader
     from torch.nn import MSELoss, L1Loss
     from torchmetrics import StructuralSimilarityIndexMeasure
     from torchmetrics.image import lpip, psnr
@@ -33,14 +34,17 @@
     metrics=None,
     crop=None,
     save_idx=None,
     output_dir=None,
     unrolled_output_factor=False,
     return_average=True,
     snr=None,
+    use_wandb=False,
+    label=None,
+    epoch=None,
     **kwargs,
 ):
     """
     Compute multiple metrics for a reconstruction algorithm.
 
     Parameters
     ----------
@@ -79,21 +83,21 @@
         output_dir = str(output_dir)
         if not os.path.exists(output_dir):
             os.mkdir(output_dir)
 
     if metrics is None:
         metrics = {
             "MSE": MSELoss().to(device),
-            "MAE": L1Loss().to(device),
+            # "MAE": L1Loss().to(device),
             "LPIPS_Vgg": lpip.LearnedPerceptualImagePatchSimilarity(
                 net_type="vgg", normalize=True
             ).to(device),
-            "LPIPS_Alex": lpip.LearnedPerceptualImagePatchSimilarity(
-                net_type="alex", normalize=True
-            ).to(device),
+            # "LPIPS_Alex": lpip.LearnedPerceptualImagePatchSimilarity(
+            #     net_type="alex", normalize=True
+            # ).to(device),
             "PSNR": psnr.PeakSignalNoiseRatio().to(device),
             "SSIM": StructuralSimilarityIndexMeasure().to(device),
             "ReconstructionError": None,
         }
 
     metrics_values = {key: [] for key in metrics}
     if unrolled_output_factor:
@@ -102,141 +106,182 @@
             if key != "ReconstructionError":
                 metrics_values[key + "_unrolled"] = []
 
     # loop over batches
     dataloader = DataLoader(dataset, batch_size=batchsize, pin_memory=(device != "cpu"))
     model.reset()
     idx = 0
-    for lensless, lensed in tqdm(dataloader):
-        lensless = lensless.to(device)
-        lensed = lensed.to(device)
-
-        # add shot noise
-        if snr is not None:
-            for i in range(lensless.shape[0]):
-                lensless[i] = add_shot_noise(lensless[i], float(snr))
+    with torch.no_grad():
+        for batch in tqdm(dataloader):
+            if hasattr(dataset, "multimask"):
+                if dataset.multimask:
+                    lensless, lensed, psfs = batch
+                    psfs = psfs.to(device)
+                else:
+                    lensless, lensed = batch
+                    psfs = None
+            else:
+                lensless, lensed = batch
+                psfs = None
+
+            lensless = lensless.to(device)
+            lensed = lensed.to(device)
+
+            # add shot noise
+            if snr is not None:
+                for i in range(lensless.shape[0]):
+                    lensless[i] = add_shot_noise(lensless[i], float(snr))
 
-        # compute predictions
-        with torch.no_grad():
+            # compute predictions
             if batchsize == 1:
+                if psfs is not None:
+                    model._set_psf(psfs[0])
                 model.set_data(lensless)
                 prediction = model.apply(
                     plot=False, save=False, output_intermediate=unrolled_output_factor, **kwargs
                 )
 
             else:
-                prediction = model.batch_call(lensless, **kwargs)
+                prediction = model.forward(lensless, psfs, **kwargs)
 
-        if unrolled_output_factor:
-            unrolled_out = prediction[-1]
-            prediction = prediction[0]
-
-        # Convert to [N*D, C, H, W] for torchmetrics
-        prediction = prediction.reshape(-1, *prediction.shape[-3:]).movedim(-1, -3)
-        lensed = lensed.reshape(-1, *lensed.shape[-3:]).movedim(-1, -3)
-
-        if crop is not None:
-            prediction = prediction[
-                ...,
-                crop["vertical"][0] : crop["vertical"][1],
-                crop["horizontal"][0] : crop["horizontal"][1],
-            ]
-            lensed = lensed[
-                ...,
-                crop["vertical"][0] : crop["vertical"][1],
-                crop["horizontal"][0] : crop["horizontal"][1],
-            ]
-
-        if save_idx is not None:
-            batch_idx = np.arange(idx, idx + batchsize)
-
-            for i, idx in enumerate(batch_idx):
-                if idx in save_idx:
-                    prediction_np = prediction.cpu().numpy()[i].squeeze()
-                    # switch to [H, W, C]
-                    prediction_np = np.moveaxis(prediction_np, 0, -1)
-                    save_image(prediction_np, fp=os.path.join(output_dir, f"{idx}.png"))
-
-        # normalization
-        prediction_max = torch.amax(prediction, dim=(-1, -2, -3), keepdim=True)
-        if torch.all(prediction_max != 0):
-            prediction = prediction / prediction_max
-        else:
-            print("Warning: prediction is zero")
-        lensed_max = torch.amax(lensed, dim=(1, 2, 3), keepdim=True)
-        lensed = lensed / lensed_max
-
-        # compute metrics
-        for metric in metrics:
-            if metric == "ReconstructionError":
-                metrics_values[metric].append(model.reconstruction_error().cpu().item())
-            else:
-                if "LPIPS" in metric:
-                    if prediction.shape[1] == 1:
-                        # LPIPS needs 3 channels
-                        metrics_values[metric].append(
-                            metrics[metric](
-                                prediction.repeat(1, 3, 1, 1), lensed.repeat(1, 3, 1, 1)
-                            )
-                            .cpu()
-                            .item()
-                        )
-                    else:
-                        metrics_values[metric].append(
-                            metrics[metric](prediction, lensed).cpu().item()
-                        )
+            if unrolled_output_factor:
+                unrolled_out = prediction[-1]
+                prediction = prediction[0]
+            prediction_original = prediction.clone()
+
+            # Convert to [N*D, C, H, W] for torchmetrics
+            prediction = prediction.reshape(-1, *prediction.shape[-3:]).movedim(-1, -3)
+            lensed = lensed.reshape(-1, *lensed.shape[-3:]).movedim(-1, -3)
+
+            if hasattr(dataset, "alignment"):
+                if dataset.alignment is not None:
+                    prediction = dataset.extract_roi(prediction, axis=(-2, -1))
                 else:
-                    metrics_values[metric].append(metrics[metric](prediction, lensed).cpu().item())
-
-        # compute metrics for unrolled output
-        if unrolled_output_factor:
-
-            # -- convert to CHW and remove depth
-            unrolled_out = unrolled_out.reshape(-1, *unrolled_out.shape[-3:]).movedim(-1, -3)
-
-            # -- extraction region of interest
-            if crop is not None:
-                unrolled_out = unrolled_out[
+                    prediction, lensed = dataset.extract_roi(
+                        prediction, axis=(-2, -1), lensed=lensed
+                    )
+                assert np.all(lensed.shape == prediction.shape)
+            elif crop is not None:
+                prediction = prediction[
+                    ...,
+                    crop["vertical"][0] : crop["vertical"][1],
+                    crop["horizontal"][0] : crop["horizontal"][1],
+                ]
+                lensed = lensed[
                     ...,
                     crop["vertical"][0] : crop["vertical"][1],
                     crop["horizontal"][0] : crop["horizontal"][1],
                 ]
 
-            # -- normalization
-            unrolled_out_max = torch.amax(unrolled_out, dim=(-1, -2, -3), keepdim=True)
-            if torch.all(unrolled_out_max != 0):
-                unrolled_out = unrolled_out / unrolled_out_max
+            if save_idx is not None:
+                batch_idx = np.arange(idx, idx + batchsize)
+
+                for i, _batch_idx in enumerate(batch_idx):
+                    if _batch_idx in save_idx:
+                        prediction_np = prediction.cpu().numpy()[i]
+                        # switch to [H, W, C] for saving
+                        prediction_np = np.moveaxis(prediction_np, 0, -1)
+                        fp = os.path.join(output_dir, f"{_batch_idx}.png")
+                        save_image(prediction_np, fp=fp)
+
+                        if use_wandb:
+                            assert epoch is not None, "epoch must be provided for wandb logging"
+                            log_key = (
+                                f"{_batch_idx}_{label}" if label is not None else f"{_batch_idx}"
+                            )
+                            wandb.log({log_key: wandb.Image(fp)}, step=epoch)
+
+            # normalization
+            prediction_max = torch.amax(prediction, dim=(-1, -2, -3), keepdim=True)
+            if torch.all(prediction_max != 0):
+                prediction = prediction / prediction_max
+            else:
+                print("Warning: prediction is zero")
+            lensed_max = torch.amax(lensed, dim=(1, 2, 3), keepdim=True)
+            lensed = lensed / lensed_max
 
-            # -- compute metrics
+            # compute metrics
             for metric in metrics:
                 if metric == "ReconstructionError":
-                    # only have this for final output
-                    continue
+                    metrics_values[metric].append(
+                        model.reconstruction_error(
+                            prediction=prediction_original, lensless=lensless
+                        )
+                        .cpu()
+                        .item()
+                    )
                 else:
-                    if "LPIPS" in metric:
-                        if unrolled_out.shape[1] == 1:
-                            # LPIPS needs 3 channels
-                            metrics_values[metric].append(
-                                metrics[metric](
-                                    unrolled_out.repeat(1, 3, 1, 1), lensed.repeat(1, 3, 1, 1)
+                    try:
+                        if "LPIPS" in metric:
+                            if prediction.shape[1] == 1:
+                                # LPIPS needs 3 channels
+                                metrics_values[metric].append(
+                                    metrics[metric](
+                                        prediction.repeat(1, 3, 1, 1), lensed.repeat(1, 3, 1, 1)
+                                    )
+                                    .cpu()
+                                    .item()
                                 )
-                                .cpu()
-                                .item()
+                            else:
+                                metrics_values[metric].append(
+                                    metrics[metric](prediction, lensed).cpu().item()
+                                )
+                        else:
+                            metrics_values[metric].append(
+                                metrics[metric](prediction, lensed).cpu().item()
                             )
+                    except Exception as e:
+                        print(f"Error in metric {metric}: {e}")
+
+            # compute metrics for unrolled output
+            if unrolled_output_factor:
+
+                # -- convert to CHW and remove depth
+                unrolled_out = unrolled_out.reshape(-1, *unrolled_out.shape[-3:]).movedim(-1, -3)
+
+                # -- extraction region of interest
+                if crop is not None:
+                    unrolled_out = unrolled_out[
+                        ...,
+                        crop["vertical"][0] : crop["vertical"][1],
+                        crop["horizontal"][0] : crop["horizontal"][1],
+                    ]
+
+                # -- normalization
+                unrolled_out_max = torch.amax(unrolled_out, dim=(-1, -2, -3), keepdim=True)
+                if torch.all(unrolled_out_max != 0):
+                    unrolled_out = unrolled_out / unrolled_out_max
+
+                # -- compute metrics
+                for metric in metrics:
+                    if metric == "ReconstructionError":
+                        # only have this for final output
+                        continue
+                    else:
+                        if "LPIPS" in metric:
+                            if unrolled_out.shape[1] == 1:
+                                # LPIPS needs 3 channels
+                                metrics_values[metric].append(
+                                    metrics[metric](
+                                        unrolled_out.repeat(1, 3, 1, 1), lensed.repeat(1, 3, 1, 1)
+                                    )
+                                    .cpu()
+                                    .item()
+                                )
+                            else:
+                                metrics_values[metric + "_unrolled"].append(
+                                    metrics[metric](unrolled_out, lensed).cpu().item()
+                                )
                         else:
                             metrics_values[metric + "_unrolled"].append(
                                 metrics[metric](unrolled_out, lensed).cpu().item()
                             )
-                    else:
-                        metrics_values[metric + "_unrolled"].append(
-                            metrics[metric](unrolled_out, lensed).cpu().item()
-                        )
 
-        model.reset()
-        idx += batchsize
+            model.reset()
+            idx += batchsize
 
     # average metrics
     if return_average:
         for metric in metrics:
             metrics_values[metric] = np.mean(metrics_values[metric])
 
     return metrics_values
```

### Comparing `lensless-1.0.6/lensless/eval/metric.py` & `lensless-1.0.7/lensless/eval/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,20 +294,21 @@
 
     if vertical_crop is None:
         vertical_crop = (0, estimate.shape[0])
     if horizontal_crop is None:
         horizontal_crop = (0, estimate.shape[1])
 
     # crop and rotate estimate image
-    estimate = rotate(
-        estimate[vertical_crop[0] : vertical_crop[1], horizontal_crop[0] : horizontal_crop[1]],
-        angle=rotation,
-        mode="nearest",
-        reshape=False,
-    )
+    if rotation:
+        estimate = rotate(
+            estimate[vertical_crop[0] : vertical_crop[1], horizontal_crop[0] : horizontal_crop[1]],
+            angle=rotation,
+            mode="nearest",
+            reshape=False,
+        )
     estimate /= estimate.max()
     estimate = np.clip(estimate, 0, 1)
     if verbose:
         print("estimate cropped: ")
         print(estimate.shape)
         print(estimate.dtype)
         print(estimate.max())
```

### Comparing `lensless-1.0.6/lensless/hardware/aperture.py` & `lensless-1.0.7/lensless/hardware/aperture.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/hardware/constants.py` & `lensless-1.0.7/lensless/hardware/constants.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/hardware/sensor.py` & `lensless-1.0.7/lensless/hardware/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
 
         Returns
         -------
         sensor : :py:class:`~lensless.sensor.VirtualSensor`
             Sensor.
 
         """
+
         if name not in SensorOptions.values():
             raise ValueError(f"Sensor {name} not supported.")
         sensor_specs = sensor_dict[name].copy()
         return cls(**sensor_specs, downsample=downsample)
 
     def capture(self, scene=None, bit_depth=None, bayer=False):
         """
```

### Comparing `lensless-1.0.6/lensless/hardware/slm.py` & `lensless-1.0.7/lensless/hardware/slm.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,45 @@
 
 
 import os
 import numpy as np
 from lensless.hardware.utils import check_username_hostname
 from lensless.utils.io import get_ctypes
 from slm_controller.hardware import SLMParam, slm_devices
-from waveprop.spherical import spherical_prop
-from waveprop.color import ColorSystem
-from waveprop.rs import angular_spectrum
-from waveprop.slm import get_centers
-from waveprop.devices import SLMParam as SLMParam_wp
 from scipy.ndimage import rotate as rotate_func
 
 
 try:
     import torch
     from torchvision import transforms
 
     torch_available = True
 except ImportError:
     torch_available = False
 
+try:
+    from waveprop.spherical import spherical_prop
+    from waveprop.color import ColorSystem
+    from waveprop.rs import angular_spectrum
+    from waveprop.slm import get_centers
+    from waveprop.devices import SLMParam as SLMParam_wp
+
+    waveprop_available = True
+except ImportError:
+    waveprop_available = False
+
 
 SUPPORTED_DEVICE = {
     "adafruit": "~/slm-controller/examples/adafruit_slm.py",
     "nokia": "~/slm-controller/examples/nokia_slm.py",
     "holoeye": "~/slm-controller/examples/holoeye_slm.py",
 }
 
 
-def set_programmable_mask(pattern, device, rpi_username, rpi_hostname, verbose=False):
+def set_programmable_mask(pattern, device, rpi_username=None, rpi_hostname=None, verbose=False):
     """
     Set LCD pattern on Raspberry Pi.
 
     This function assumes that `slm-controller <https://github.com/ebezzam/slm-controller>`_
     is installed on the Raspberry Pi.
 
     Parameters
@@ -51,15 +57,19 @@
     rpi_username : str
         Username of Raspberry Pi.
     rpi_hostname : str
         Hostname of Raspberry Pi.
 
     """
 
-    client = check_username_hostname(rpi_username, rpi_hostname)
+    if rpi_username is not None:
+        assert (
+            rpi_hostname is not None
+        ), "rpi_hostname must be specified if rpi_username is specified"
+        client = check_username_hostname(rpi_username, rpi_hostname)
 
     # get path to python executable on Raspberry Pi
     rpi_python = "~/slm-controller/slm_controller_env/bin/python"
     assert (
         device in SUPPORTED_DEVICE.keys()
     ), f"Device {device} not supported. Supported devices: {SUPPORTED_DEVICE.keys()}"
     script = SUPPORTED_DEVICE[device]
@@ -73,35 +83,45 @@
     ), f"Pattern shape {pattern.shape} does not match expected shape {expected_shape}"
 
     # save pattern
     pattern_fn = "tmp_pattern.npy"
     local_path = os.path.join(os.getcwd(), pattern_fn)
     np.save(local_path, pattern)
 
-    # copy pattern to Raspberry Pi
-    remote_path = f"~/{pattern_fn}"
-    if verbose:
-        print(f"PUTTING {local_path} to {remote_path}")
-
-    os.system(
-        'scp %s "%s@%s:%s" >/dev/null 2>&1' % (local_path, rpi_username, rpi_hostname, remote_path)
-    )
-    # # -- not sure why this doesn't work... permission denied
-    # sftp = client.open_sftp()
-    # sftp.put(local_path, remote_path, confirm=True)
-    # sftp.close()
-
-    # run script on Raspberry Pi to set mask pattern
-    command = f"{rpi_python} {script} --file_path {remote_path}"
-    if verbose:
-        print(f"COMMAND : {command}")
-    _stdin, _stdout, _stderr = client.exec_command(command)
-    if verbose:
-        print(_stdout.read().decode())
-    client.close()
+    if rpi_username is not None:
+
+        # copy pattern to Raspberry Pi
+        remote_path = f"~/{pattern_fn}"
+        if verbose:
+            print(f"PUTTING {local_path} to {remote_path}")
+        os.system(
+            'scp %s "%s@%s:%s" >/dev/null 2>&1'
+            % (local_path, rpi_username, rpi_hostname, remote_path)
+        )
+        # # -- not sure why this doesn't work... permission denied
+        # sftp = client.open_sftp()
+        # sftp.put(local_path, remote_path, confirm=True)
+        # sftp.close()
+
+        # run script on Raspberry Pi to set mask pattern
+        command = f"{rpi_python} {script} --file_path {remote_path}"
+        if verbose:
+            print(f"COMMAND : {command}")
+        _stdin, _stdout, _stderr = client.exec_command(command)
+        if verbose:
+            print(_stdout.read().decode())
+        client.close()
+
+    else:
+
+        # run script on Raspberry Pi to set mask pattern
+        command = f"{rpi_python} {script} --file_path {local_path} >/dev/null 2>&1"
+        if verbose:
+            print(f"COMMAND : {command}")
+        os.system(command)
 
     os.remove(local_path)
 
 
 def get_programmable_mask(
     vals,
     sensor,
@@ -127,14 +147,16 @@
     flipud : bool, optional
         Flip mask vertically.
     nbits : int, optional
         Number of bits/levels to quantize mask to.
 
     """
 
+    assert waveprop_available
+
     use_torch = False
     if torch_available:
         use_torch = isinstance(vals, torch.Tensor)
     dtype = vals.dtype
 
     # -- prepare SLM mask
     n_active_slm_pixels = vals.shape
@@ -214,19 +236,19 @@
     sub_shape = subpattern.shape
     controllable_shape = (3, sub_shape[0] // 3, sub_shape[1])
     subpattern_rgb = subpattern.reshape(controllable_shape, order="F")
     subpattern_rgb *= 255
 
     # pad to full pattern
     pattern = np.zeros((3, 128, 160), dtype=np.uint8)
-    topleft = [center[0] - controllable_shape[1] // 2, center[1] - controllable_shape[2] // 2]
+    top_left = [center[0] - controllable_shape[1] // 2, center[1] - controllable_shape[2] // 2]
     pattern[
         :,
-        topleft[0] : topleft[0] + controllable_shape[1],
-        topleft[1] : topleft[1] + controllable_shape[2],
+        top_left[0] : top_left[0] + controllable_shape[1],
+        top_left[1] : top_left[1] + controllable_shape[2],
     ] = subpattern_rgb.astype(np.uint8)
     return pattern
 
 
 def full2subpattern(
     pattern,
     shape,
@@ -272,14 +294,16 @@
         Distance from scene to mask. Not used if ``waveprop=False``.
     mask2sensor : float
         Distance from mask to sensor. Not used if ``waveprop=False``.
     color_system : :py:class:`~waveprop.color.ColorSystem`, optional
         Color system. Not used if ``waveprop=False``.
 
     """
+    assert waveprop_available
+
     if color_system is None:
         color_system = ColorSystem.rgb()
 
     is_torch = False
     device = None
     if torch_available and isinstance(mask, torch.Tensor):
         is_torch = True
```

### Comparing `lensless-1.0.6/lensless/hardware/trainable_mask.py` & `lensless-1.0.7/lensless/hardware/trainable_mask.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,54 +3,55 @@
 # ==================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
 # Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
 import abc
-import torch
+import omegaconf
 import numpy as np
-from lensless.utils.image import is_grayscale
-from lensless.hardware.slm import get_programmable_mask, get_intensity_psf
+import torch
+from lensless.utils.image import is_grayscale, rgb2gray
+from lensless.hardware.slm import full2subpattern, get_programmable_mask, get_intensity_psf
 from lensless.hardware.sensor import VirtualSensor
 from waveprop.devices import slm_dict
-from lensless.hardware.slm import full2subpattern
-from lensless.utils.image import rgb2gray
+from lensless.hardware.mask import CodedAperture
 
 
 class TrainableMask(torch.nn.Module, metaclass=abc.ABCMeta):
     """
     Abstract class for defining trainable masks.
 
     The following abstract methods need to be defined:
 
     - :py:class:`~lensless.hardware.trainable_mask.TrainableMask.get_psf`: returning the PSF of the mask.
     - :py:class:`~lensless.hardware.trainable_mask.TrainableMask.project`: projecting the mask parameters to a valid space (should be a subspace of [0,1]).
 
     """
 
-    def __init__(self, initial_mask, optimizer="Adam", lr=1e-3, **kwargs):
+    def __init__(self, optimizer="Adam", lr=1e-3, **kwargs):
         """
         Base constructor. Derived constructor may define new state variables
 
         Parameters
         ----------
-        initial_mask : :py:class:`~torch.Tensor`
-            Initial mask parameters.
         optimizer : str, optional
             Optimizer to use for updating the mask parameters, by default "Adam"
         lr : float, optional
             Learning rate for the mask parameters, by default 1e-3
         """
         super().__init__()
-        self._mask = torch.nn.Parameter(initial_mask)
-        self._optimizer = getattr(torch.optim, optimizer)([self._mask], lr=lr)
-        self.train_mask_vals = True
+        self._optimizer = optimizer
+        self._lr = lr
         self._counter = 0
 
+    def _set_optimizer(self, param):
+        """Set the optimizer for the mask parameters."""
+        self._optimizer = getattr(torch.optim, self._optimizer)(param, lr=self._lr)
+
     @abc.abstractmethod
     def get_psf(self):
         """
         Abstract method for getting the PSF of the mask. Should be fully compatible with pytorch autograd.
 
         Returns
         -------
@@ -62,74 +63,73 @@
     def update_mask(self):
         """Update the mask parameters. According to externaly updated gradiants."""
         self._optimizer.step()
         self._optimizer.zero_grad(set_to_none=True)
         self.project()
         self._counter += 1
 
-    def get_vals(self):
-        """Get the mask parameters."""
-        return self._mask
-
     @abc.abstractmethod
     def project(self):
         """Abstract method for projecting the mask parameters to a valid space (should be a subspace of [0,1])."""
         raise NotImplementedError
 
 
 class TrainablePSF(TrainableMask):
+    # class TrainablePSF(torch.nn.Module, TrainableMask):
     """
     Class for defining an object that directly optimizes the PSF, without any constraints on what can be realized physically.
 
     Parameters
     ----------
     grayscale : bool, optional
         Whether mask should be returned as grayscale when calling :py:class:`~lensless.hardware.trainable_mask.TrainableMask.get_psf`.
         Otherwise PSF will be returned as RGB. By default False.
     """
 
-    def __init__(self, initial_mask, optimizer="Adam", lr=1e-3, grayscale=False, **kwargs):
-        super().__init__(initial_mask, optimizer, lr, **kwargs)
-        assert (
-            len(initial_mask.shape) == 4
-        ), "Mask must be of shape (depth, height, width, channels)"
+    def __init__(self, initial_psf, grayscale=False, **kwargs):
+
+        super().__init__(**kwargs)
+        self._psf = torch.nn.Parameter(initial_psf)
+        initial_param = [self._psf]
+        self._set_optimizer(initial_param)
+
+        # checks
+        assert len(initial_psf.shape) == 4, "Mask must be of shape (depth, height, width, channels)"
         self.grayscale = grayscale
-        self._is_grayscale = is_grayscale(initial_mask)
+        self._is_grayscale = is_grayscale(initial_psf)
         if grayscale:
-            assert self._is_grayscale, "Mask must be grayscale"
+            assert self._is_grayscale, "PSF must be grayscale"
 
     def get_psf(self):
         if self._is_grayscale:
             if self.grayscale:
                 # simulation in grayscale
-                return self._mask
+                return self._psf
             else:
                 # replicate to 3 channels
-                return self._mask.expand(-1, -1, -1, 3)
+                return self._psf.expand(-1, -1, -1, 3)
         else:
             # assume RGB
-            return self._mask
+            return self._psf
 
     def project(self):
-        self._mask.data = torch.clamp(self._mask, 0, 1)
+        self._psf.data = torch.clamp(self._psf, 0, 1)
 
 
 class AdafruitLCD(TrainableMask):
     def __init__(
         self,
         initial_vals,
         sensor,
         slm,
-        optimizer="Adam",
-        lr=1e-3,
         train_mask_vals=True,
         color_filter=None,
         rotate=None,
         flipud=False,
-        use_waveprop=None,
+        use_waveprop=False,
         vertical_shift=None,
         horizontal_shift=None,
         scene2mask=None,
         mask2sensor=None,
         downsample=None,
         min_val=0,
         **kwargs,
@@ -140,35 +140,58 @@
         initial_vals : :py:class:`~torch.Tensor`
             Initial mask parameters.
         sensor : :py:class:`~lensless.hardware.sensor.VirtualSensor`
             Sensor object.
         slm_param : :py:class:`~lensless.hardware.slm.SLMParam`
             SLM parameters.
         rotate : float, optional
-            Rotation angle in degrees, by default None
+            Rotation angle in degrees, by default None.
         flipud : bool, optional
-            Whether to flip the mask vertically, by default False
+            Whether to flip the mask vertically, by default False.
+        use_waveprop : bool, optional
+            Whether to use wave propagation for simulating PSF. If False, PSF will simply be intensity of mask pattern, by default False.
+        vertical_shift : int, optional
+            Vertical shift of the mask, by default None.
+        horizontal_shift : int, optional
+            Horizontal shift of the mask, by default None.
+        scene2mask : :py:class:`~torch.Tensor`, optional
+            Distance from scene to mask. Used for wave propagation, by default None.
+        mask2sensor : :py:class:`~torch.Tensor`, optional
+            Distance from mask to sensor. Used for wave propagation, by default None.
+        downsample : int, optional
+            Downsample factor, by default None.
+        min_val : float, optional
+            Minimum value for mask weights, by default 0.
         """
 
-        super().__init__(initial_vals, **kwargs)
+        super().__init__(**kwargs)
+
         self.train_mask_vals = train_mask_vals
+        if train_mask_vals:
+            self._vals = torch.nn.Parameter(initial_vals)
+        else:
+            self._vals = initial_vals
+
+        initial_param = None
         if color_filter is not None:
-            self.color_filter = torch.nn.Parameter(color_filter)
+            self._color_filter = torch.nn.Parameter(color_filter)
             if train_mask_vals:
-                param = [self._mask, self.color_filter]
+                initial_param = [self._vals, self._color_filter]
             else:
-                del self._mask
-                self._mask = initial_vals
-                param = [self.color_filter]
-            self._optimizer = getattr(torch.optim, optimizer)(param, lr=lr)
+                initial_param = [self._color_filter]
         else:
-            self.color_filter = None
             assert (
                 train_mask_vals
             ), "If color filter is not trainable, mask values must be trainable"
+            initial_param = [self._vals]
+            self._color_filter = None
+        assert initial_param is not None, "Initial parameters must be set"
+
+        # set optimizer
+        self._set_optimizer(initial_param)
 
         self.slm_param = slm_dict[slm]
         self.device = slm
         self.sensor = VirtualSensor.from_name(sensor, downsample=downsample)
         self.rotate = rotate
         self.flipud = flipud
         self.use_waveprop = use_waveprop
@@ -184,20 +207,20 @@
         if self.use_waveprop:
             assert self.scene2mask is not None
             assert self.mask2sensor is not None
 
     def get_psf(self):
 
         mask = get_programmable_mask(
-            vals=self._mask,
+            vals=self._vals,
             sensor=self.sensor,
             slm_param=self.slm_param,
             rotate=self.rotate,
             flipud=self.flipud,
-            color_filter=self.color_filter,
+            color_filter=self._color_filter,
         )
 
         if self.vertical_shift is not None:
             mask = torch.roll(mask, self.vertical_shift, dims=1)
 
         if self.horizontal_shift is not None:
             mask = torch.roll(mask, self.horizontal_shift, dims=2)
@@ -222,93 +245,193 @@
         # normalize
         psf_in = psf_in / psf_in.norm()
 
         return psf_in
 
     def project(self):
         if self.train_mask_vals:
-            self._mask.data = torch.clamp(self._mask, self.min_val, 1)
-        if self.color_filter is not None:
-            self.color_filter.data = torch.clamp(self.color_filter, 0, 1)
+            self._vals.data = torch.clamp(self._vals, self.min_val, 1)
+        if self._color_filter is not None:
+            self._color_filter.data = torch.clamp(self._color_filter, 0, 1)
             # normalize each row to 1
-            self.color_filter.data = self.color_filter / self.color_filter.sum(
+            self._color_filter.data = self._color_filter / self._color_filter.sum(
                 dim=[1, 2]
             ).unsqueeze(-1).unsqueeze(-1)
 
 
+class TrainableCodedAperture(TrainableMask):
+    def __init__(
+        self,
+        sensor_name,
+        downsample=None,
+        binary=True,
+        torch_device="cuda",
+        **kwargs,
+    ):
+        """
+        TODO: Distinguish between separable and non-separable.
+        """
+
+        # 1) call base constructor so parameters can be set
+        super().__init__(**kwargs)
+
+        # 2) initialize mask
+        assert "distance_sensor" in kwargs, "Distance to sensor must be specified"
+        assert "method" in kwargs, "Method must be specified."
+        assert "n_bits" in kwargs, "Number of bits must be specified."
+        self._mask_obj = CodedAperture.from_sensor(
+            sensor_name,
+            downsample,
+            is_torch=True,
+            torch_device=torch_device,
+            **kwargs,
+        )
+
+        # 3) set learnable parameters (should be immediate attributes of the class)
+        self._row = None
+        self._col = None
+        self._mask = None
+        if self._mask_obj.row is not None:
+            # separable
+            self.separable = True
+            self._row = torch.nn.Parameter(self._mask_obj.row)
+            self._col = torch.nn.Parameter(self._mask_obj.col)
+            initial_param = [self._row, self._col]
+        else:
+            # non-separable
+            self.separable = False
+            self._mask = torch.nn.Parameter(self._mask_obj.mask)
+            initial_param = [self._mask]
+        self.binary = binary
+
+        # 4) set optimizer
+        self._set_optimizer(initial_param)
+
+        # 5) compute PSF
+        self._psf = None
+        self.project()
+
+    def get_psf(self):
+        return self._psf
+
+    def project(self):
+        with torch.no_grad():
+            if self.separable:
+                self._row.data = torch.clamp(self._row, 0, 1)
+                self._col.data = torch.clamp(self._col, 0, 1)
+                if self.binary:
+                    self._row.data = torch.round(self._row)
+                    self._col.data = torch.round(self._col)
+            else:
+                self._mask.data = torch.clamp(self._mask, 0, 1)
+                if self.binary:
+                    self._mask.data = torch.round(self._mask)
+
+        # recompute PSF
+        self._mask_obj.create_mask(self._row, self._col, mask=self._mask)
+        self._mask_obj.compute_psf()
+        self._psf = self._mask_obj.psf.unsqueeze(0)
+        self._psf = self._psf / self._psf.norm()
+
+
 """
 Utility functions to help prepare trainable masks.
 """
 
 mask_type_to_class = {
-    "TrainablePSF": TrainablePSF,
     "AdafruitLCD": AdafruitLCD,
+    "TrainablePSF": TrainablePSF,
+    "TrainableCodedAperture": TrainableCodedAperture,
+    "TrainableHeightVarying": None,
+    "TrainableMultiLensArray": None,
 }
 
 
 def prep_trainable_mask(config, psf=None, downsample=None):
 
     mask = None
     color_filter = None
     downsample = config["files"]["downsample"] if downsample is None else downsample
-    if config["trainable_mask"]["mask_type"] is not None:
-        mask_class = mask_type_to_class[config["trainable_mask"]["mask_type"]]
+    mask_type = config["trainable_mask"]["mask_type"]
+    if mask_type is not None:
+        assert mask_type in mask_type_to_class.keys(), (
+            f"Trainable mask type {mask_type} not supported. "
+            f"Supported types are {mask_type_to_class.keys()}"
+        )
+        mask_class = mask_type_to_class[mask_type]
 
-        if config["trainable_mask"]["initial_value"] == "random":
-            if psf is not None:
-                initial_mask = torch.rand_like(psf)
-            else:
-                sensor = VirtualSensor.from_name(
-                    config["simulation"]["sensor"], downsample=downsample
-                )
-                resolution = sensor.resolution
-                initial_mask = torch.rand((1, *resolution, 3))
+        # -- trainable mask object
+        if isinstance(config["trainable_mask"]["initial_value"], omegaconf.dictconfig.DictConfig):
 
-        elif config["trainable_mask"]["initial_value"] == "psf":
-            initial_mask = psf.clone()
+            # from mask config
+            mask = mask_class(
+                # mask = TrainableCodedAperture(
+                sensor_name=config.simulation.sensor,
+                downsample=downsample,
+                distance_sensor=config.simulation.mask2sensor,
+                optimizer=config.trainable_mask.optimizer,
+                lr=config.trainable_mask.mask_lr,
+                binary=config.trainable_mask.binary,
+                torch_device=config.torch_device,
+                **config.trainable_mask.initial_value,
+            )
 
-        # if file ending with "npy"
-        elif config["trainable_mask"]["initial_value"].endswith("npy"):
+        else:
 
-            pattern = np.load(config["trainable_mask"]["initial_value"])
-
-            initial_mask = full2subpattern(
-                pattern=pattern,
-                shape=config["trainable_mask"]["ap_shape"],
-                center=config["trainable_mask"]["ap_center"],
-                slm=config["trainable_mask"]["slm"],
-            )
-            initial_mask = torch.from_numpy(initial_mask.astype(np.float32))
+            if config["trainable_mask"]["initial_value"] == "random":
+                if psf is not None:
+                    initial_mask = torch.rand_like(psf)
+                else:
+                    sensor = VirtualSensor.from_name(
+                        config["simulation"]["sensor"], downsample=downsample
+                    )
+                    resolution = sensor.resolution
+                    initial_mask = torch.rand((1, *resolution, 3))
+
+            elif config["trainable_mask"]["initial_value"] == "psf":
+                initial_mask = psf.clone()
+
+            # if file ending with "npy"
+            elif config["trainable_mask"]["initial_value"].endswith("npy"):
+
+                pattern = np.load(config["trainable_mask"]["initial_value"])
+
+                initial_mask = full2subpattern(
+                    pattern=pattern,
+                    shape=config["trainable_mask"]["ap_shape"],
+                    center=config["trainable_mask"]["ap_center"],
+                    slm=config["trainable_mask"]["slm"],
+                )
+                initial_mask = torch.from_numpy(initial_mask.astype(np.float32))
 
-            # prepare color filter if needed
-            from waveprop.devices import slm_dict
-            from waveprop.devices import SLMParam as SLMParam_wp
-
-            slm_param = slm_dict[config["trainable_mask"]["slm"]]
-            if (
-                config["trainable_mask"]["train_color_filter"]
-                and SLMParam_wp.COLOR_FILTER in slm_param.keys()
-            ):
-                color_filter = slm_param[SLMParam_wp.COLOR_FILTER]
-                color_filter = torch.from_numpy(color_filter.copy()).to(dtype=torch.float32)
+                # prepare color filter if needed
+                from waveprop.devices import slm_dict
+                from waveprop.devices import SLMParam as SLMParam_wp
+
+                slm_param = slm_dict[config["trainable_mask"]["slm"]]
+                if (
+                    config["trainable_mask"]["train_color_filter"]
+                    and SLMParam_wp.COLOR_FILTER in slm_param.keys()
+                ):
+                    color_filter = slm_param[SLMParam_wp.COLOR_FILTER]
+                    color_filter = torch.from_numpy(color_filter.copy()).to(dtype=torch.float32)
 
-                # add small random values
-                color_filter = color_filter + 0.1 * torch.rand_like(color_filter)
+                    # TODO: add small random values?
+                    color_filter = color_filter + 0.1 * torch.rand_like(color_filter)
 
-        else:
-            raise ValueError(
-                f"Initial PSF value {config['trainable_mask']['initial_value']} not supported"
-            )
+            else:
+                raise ValueError(
+                    f"Initial PSF value {config['trainable_mask']['initial_value']} not supported"
+                )
 
-        # convert to grayscale if needed
-        if config["trainable_mask"]["grayscale"] and not is_grayscale(initial_mask):
-            initial_mask = rgb2gray(initial_mask)
-
-        mask = mask_class(
-            initial_mask,
-            optimizer="Adam",
-            downsample=downsample,
-            color_filter=color_filter,
-            **config["trainable_mask"],
-        )
+            # convert to grayscale if needed
+            if config["trainable_mask"]["grayscale"] and not is_grayscale(initial_mask):
+                initial_mask = rgb2gray(initial_mask)
+
+            mask = mask_class(
+                initial_mask,
+                downsample=downsample,
+                color_filter=color_filter,
+                **config["trainable_mask"],
+            )
 
     return mask
```

### Comparing `lensless-1.0.6/lensless/hardware/utils.py` & `lensless-1.0.7/lensless/hardware/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 import paramiko
 from pprint import pprint
 from paramiko.ssh_exception import AuthenticationException, BadHostKeyException, SSHException
 from lensless.hardware.sensor import SensorOptions
 import cv2
 from lensless.utils.image import print_image_info
 from lensless.utils.io import load_image
-
-
 import logging
 
 logging.getLogger("paramiko").setLevel(logging.WARNING)
 
+if os.name == "nt":
+    NULL_FILE = "nul"
+else:
+    NULL_FILE = "/dev/null 2>&1"
+
 
 def capture(
     rpi_username,
     rpi_hostname,
     sensor,
     bayer,
     exp,
@@ -152,16 +155,16 @@
             remotefile = f"~/{remote_fn}.dng"
             localfile = f"{fn}.dng"
             if output_path is not None:
                 localfile = os.path.join(output_path, localfile)
             if verbose:
                 print(f"\nCopying over picture as {localfile}...")
             os.system(
-                'scp "%s@%s:%s" %s >/dev/null 2>&1'
-                % (rpi_username, rpi_hostname, remotefile, localfile)
+                'scp "%s@%s:%s" %s >%s'
+                % (rpi_username, rpi_hostname, remotefile, localfile, NULL_FILE)
             )
 
             img = load_image(localfile, verbose=True, bayer=bayer, nbits_out=nbits_out)
 
             # print image properties
             print_image_info(img)
 
@@ -175,16 +178,16 @@
             remotefile = f"~/{remote_fn}.png"
             localfile = f"{fn}.png"
             if output_path is not None:
                 localfile = os.path.join(output_path, localfile)
             if verbose:
                 print(f"\nCopying over picture as {localfile}...")
             os.system(
-                'scp "%s@%s:%s" %s >/dev/null 2>&1'
-                % (rpi_username, rpi_hostname, remotefile, localfile)
+                'scp "%s@%s:%s" %s >%s'
+                % (rpi_username, rpi_hostname, remotefile, localfile, NULL_FILE)
             )
 
             img = load_image(localfile, verbose=True)
 
     # legacy software running on RPi
     else:
         # copy over file
@@ -192,16 +195,16 @@
         remotefile = f"~/{remote_fn}.png"
         localfile = f"{fn}.png"
         if output_path is not None:
             localfile = os.path.join(output_path, localfile)
         if verbose:
             print(f"\nCopying over picture as {localfile}...")
         os.system(
-            'scp "%s@%s:%s" %s >/dev/null 2>&1'
-            % (rpi_username, rpi_hostname, remotefile, localfile)
+            'scp "%s@%s:%s" %s >%s'
+            % (rpi_username, rpi_hostname, remotefile, localfile, NULL_FILE)
         )
 
         if rgb or gray:
             img = load_image(localfile, verbose=verbose)
 
         else:
 
@@ -266,17 +269,15 @@
 
     # assumes that `LenslessPiCam` is in home directory and environment inside `LenslessPiCam`
     rpi_python = "~/LenslessPiCam/lensless_env/bin/python"
     script = "~/LenslessPiCam/scripts/measure/prep_display_image.py"
     remote_tmp_file = "~/tmp_display.png"
     display_path = "~/LenslessPiCam_display/test.png"
 
-    os.system(
-        'scp %s "%s@%s:%s" >/dev/null 2>&1' % (fp, rpi_username, rpi_hostname, remote_tmp_file)
-    )
+    os.system(f"scp {fp} {rpi_username}@{rpi_hostname}:{remote_tmp_file} > {NULL_FILE}")
 
     # run script on Raspberry Pi to prepare image to display
     prep_command = f"{rpi_python} {script} --fp {remote_tmp_file} \
         --pad {pad} --vshift {vshift} --hshift {hshift} --screen_res {screen_res[0]} {screen_res[1]} \
         --brightness {brightness} --rot90 {rot90} --output_path {display_path} "
     if verbose:
         print(f"COMMAND : {prep_command}")
@@ -285,16 +286,16 @@
         shell=False,
         # stdout=DEVNULL
     )
 
 
 def check_username_hostname(username, hostname, timeout=10):
 
-    assert username is not None, "Username must be specified"
-    assert hostname is not None, "Hostname must be specified"
+    assert username is not None, "Raspberry Pi username must be specified"
+    assert hostname is not None, "Raspberry Pi hostname must be specified"
 
     client = paramiko.client.SSHClient()
     client.set_missing_host_key_policy(paramiko.AutoAddPolicy())
 
     try:
         # with suppress_stdout():
         client.connect(hostname, username=username, timeout=timeout)
```

### Comparing `lensless-1.0.6/lensless/recon/admm.py` & `lensless-1.0.7/lensless/recon/admm.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # Julien SAHLI [julien.sahli@epfl.ch]
 # #############################################################################
 
 
 import numpy as np
 from lensless.recon.recon import ReconstructionAlgorithm
 from scipy import fft
+from lensless.utils.io import load_data
+import time
 
 try:
     import torch
 
     torch_available = True
 except ImportError:
     torch_available = False
@@ -41,15 +43,15 @@
         psi=None,
         psi_adj=None,
         psi_gram=None,
         pad=False,
         norm="backward",
         # PnP
         denoiser=None,
-        **kwargs
+        **kwargs,
     ):
         """
 
         Parameters
         ----------
         psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
             Point spread function (PSF) that models forward propagation.
@@ -91,15 +93,17 @@
         if psf.shape[0] > 1:
             raise NotImplementedError(
                 "3D ADMM is not supported yet, use gradient descent or APGD instead."
             )
 
         # call reset() to initialize matrices
         self._proj = self._Psi
-        super(ADMM, self).__init__(psf, dtype, pad=pad, norm=norm, denoiser=denoiser, **kwargs)
+        super(ADMM, self).__init__(
+            psf, dtype, pad=pad, norm=norm, denoiser=denoiser, reset=False, **kwargs
+        )
 
         # set prior
         if psi is None:
             # use already defined Psi and PsiT
             self._PsiTPsi = finite_diff_gram(self._padded_shape, self._dtype, self.is_torch)
         else:
             assert psi_adj is not None
@@ -110,40 +114,29 @@
             # overwrite already defined Psi and PsiT
             self._Psi = psi
             self._PsiT = psi_adj
             self._PsiTPsi = psi_gram(self._padded_shape)
 
             # - need to reset with new projector
             self._proj = self._Psi
-            self.reset()
 
         # precompute_R_divmat (self._H computed by constructor with reset())
         if self.is_torch:
             self._PsiTPsi = self._PsiTPsi.to(self._psf.device)
-            self._R_divmat = 1.0 / (
-                self._mu1 * (torch.abs(self._convolver._Hadj * self._convolver._H))
-                + self._mu2 * torch.abs(self._PsiTPsi)
-                + self._mu3
-            ).type(self._complex_dtype)
-        else:
-            self._R_divmat = 1.0 / (
-                self._mu1 * (np.abs(self._convolver._Hadj * self._convolver._H))
-                + self._mu2 * np.abs(self._PsiTPsi)
-                + self._mu3
-            ).astype(self._complex_dtype)
 
         # check denoiser for PnP
         if self._denoiser is not None:
             self._denoiser_use_dual = denoiser["use_dual"]
 
             # - need to reset with new projector
             self._proj = self._denoiser
             # identify function
             self._PsiT = lambda x: x
-            self.reset()
+
+        self.reset()
 
     def _Psi(self, x):
         """
         Operator to map image to space that the image is assumed to be sparse
         in.
         """
         return finite_diff(x)
@@ -185,14 +178,21 @@
                 self._forward_out = torch.zeros_like(self._X)
                 self._Psi_out = torch.zeros_like(self._U)
 
             self._xi = torch.zeros_like(self._image_est)
             self._eta = torch.zeros_like(self._U)
             self._rho = torch.zeros_like(self._X)
 
+            # precompute _R_divmat
+            self._R_divmat = 1.0 / (
+                self._mu1 * (torch.abs(self._convolver._Hadj * self._convolver._H))
+                + self._mu2 * torch.abs(self._PsiTPsi)
+                + self._mu3
+            ).type(self._complex_dtype)
+
             # precompute_X_divmat
             self._X_divmat = 1.0 / (self._convolver._pad(torch.ones_like(self._psf)) + self._mu1)
             # self._X_divmat = 1.0 / (torch.ones_like(self._psf) + self._mu1)
 
         else:
             if self._initial_est is not None:
                 self._image_est = self._initial_est
@@ -213,14 +213,21 @@
                 self._forward_out = np.zeros_like(self._X)
                 self._Psi_out = np.zeros_like(self._U)
 
             self._xi = np.zeros_like(self._image_est)
             self._eta = np.zeros_like(self._U)
             self._rho = np.zeros_like(self._X)
 
+            # precompute R_divmat
+            self._R_divmat = 1.0 / (
+                self._mu1 * (np.abs(self._convolver._Hadj * self._convolver._H))
+                + self._mu2 * np.abs(self._PsiTPsi)
+                + self._mu3
+            ).astype(self._complex_dtype)
+
             # precompute_X_divmat
             self._X_divmat = 1.0 / (
                 self._convolver._pad(np.ones(self._psf_shape, dtype=self._dtype)) + self._mu1
             )
 
     def _U_update(self):
         """Total variation update."""
@@ -273,18 +280,22 @@
                 + self._convolver.deconvolve(self._mu1 * self._X - self._xi)
             )
 
         # rk = self._convolver._pad(rk)
 
         if self.is_torch:
             freq_space_result = self._R_divmat * torch.fft.rfft2(rk, dim=(-3, -2))
-            self._image_est = torch.fft.irfft2(freq_space_result, dim=(-3, -2))
+            self._image_est = torch.fft.irfft2(
+                freq_space_result, dim=(-3, -2), s=self._convolver._padded_shape[-3:-1]
+            )
         else:
             freq_space_result = self._R_divmat * fft.rfft2(rk, axes=(-3, -2))
-            self._image_est = fft.irfft2(freq_space_result, axes=(-3, -2))
+            self._image_est = fft.irfft2(
+                freq_space_result, axes=(-3, -2), s=self._convolver._padded_shape[-3:-1]
+            )
 
         # self._image_est = self._convolver._crop(res)
 
     def _xi_update(self):
         # to avoid computing forward model twice
         self._xi += self._mu1 * (self._forward_out - self._X)
 
@@ -380,7 +391,29 @@
             -1, 0, 0
         ] = -1
 
     if is_torch:
         return torch.fft.rfft2(gram, dim=(-3, -2))
     else:
         return fft.rfft2(gram, axes=(-3, -2))
+
+
+def apply_admm(psf_fp, data_fp, n_iter, verbose=False, **kwargs):
+
+    # load data
+    psf, data = load_data(psf_fp=psf_fp, data_fp=data_fp, plot=False, **kwargs)
+
+    # create reconstruction object
+    recon = ADMM(psf, n_iter=n_iter)
+
+    # set data
+    recon.set_data(data)
+
+    # perform reconstruction
+    start_time = time.time()
+    res = recon.apply(plot=False)
+    proc_time = time.time() - start_time
+
+    if verbose:
+        print(f"Reconstruction time : {proc_time} s")
+        print(f"Reconstruction shape: {res.shape}")
+    return res
```

### Comparing `lensless-1.0.6/lensless/recon/admm_pnp.py` & `lensless-1.0.7/lensless/recon/gd.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,240 +1,260 @@
+# #############################################################################
+# gradient_descent.py
+# =================
+# Authors :
+# Eric BEZZAM [ebezzam@gmail.com]
+# Julien SAHLI [julien.sahli@epfl.ch]
+# #############################################################################
+
+
 import numpy as np
-from lensless.recon import ReconstructionAlgorithm
-from scipy import fft
+from lensless.recon.recon import ReconstructionAlgorithm
+import inspect
+from lensless.utils.io import load_data
+import time
 
 try:
     import torch
 
     torch_available = True
 except ImportError:
     torch_available = False
 
 
-class ADMM_PnP(ReconstructionAlgorithm):
+class GradientDescentUpdate:
+    """Gradient descent update techniques."""
+
+    VANILLA = "vanilla"
+    NESTEROV = "nesterov"
+    FISTA = "fista"
+
+    @staticmethod
+    def all_values():
+        vals = []
+        for i in inspect.getmembers(GradientDescentUpdate):
+            # remove private and protected functions, and this function
+            if not i[0].startswith("_") and not callable(i[1]):
+                vals.append(i[1])
+        return vals
+
+
+def non_neg(xi):
     """
-    Object for applying ADMM (Alternating Direction Method of Multipliers) with
-    a non-negativity constraint and a total variation (TV) prior.
+    Clip input so that it is non-negative.
+
+    Parameters
+    ----------
+    xi : :py:class:`~numpy.ndarray`
+        Data to clip.
+
+    Returns
+    -------
+    nonneg : :py:class:`~numpy.ndarray`
+        Non-negative projection of input.
 
-    Paper about ADMM: https://web.stanford.edu/~boyd/papers/pdf/admm_distr_stats.pdf
+    """
+    if torch_available and isinstance(xi, torch.Tensor):
+        return torch.maximum(xi, torch.zeros_like(xi))
+    else:
+        return np.maximum(xi, 0)
 
-    Slides about ADMM: https://web.stanford.edu/class/ee364b/lectures/admm_slides.pdf
 
+class GradientDescent(ReconstructionAlgorithm):
+    """
+    Object for applying projected gradient descent.
     """
 
-    def __init__(
-        self,
-        psf,
-        proj,
-        dtype=None,
-        mu1=1e-6,
-        mu2=1e-5,
-        mu3=4e-5,
-        tau=0.0001,
-        pad=False,
-        norm="backward",
-        use_projection_dual=False,
-        **kwargs,
-    ):
+    def __init__(self, psf, dtype=None, proj=non_neg, **kwargs):
         """
 
         Parameters
         ----------
         psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
             Point spread function (PSF) that models forward propagation.
             Must be of shape (depth, height, width, channels) even if
             depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
             to load a PSF from a file such that it is in the correct format.
-        proj : :py:class:`function`
-            Projection function to apply at each iteration.
         dtype : float32 or float64
             Data type to use for optimization. Default is float32.
-        mu1 : float
-            Step size for updating primal/dual variables.
-        mu2 : float
-            Step size for updating primal/dual variables.
-        mu3 : float
-            Step size for updating primal/dual variables.
-        tau : float
-            Weight for L1 norm of `psi` applied to the image estimate.
-        pad : bool
-            Whether to pad the image with zeros before applying the PSF. Default
-            is False, as optimized data is already padded.
-        norm : str
-            Normalization to use for the convolution. Options are "forward",
-            "backward", and "ortho". Default is "backward".
-        use_projection_dual : bool
-            Whether to use dual update for the user specify projection. This result in an algorithm closer to ADMM.
-            During our testing, it seems to give better result with few iteration (<20) but worst otherwise.  Default is False.
-        """
-        self._mu1 = mu1
-        self._mu2 = mu2
-        self._mu3 = mu3
-        self._tau = tau
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        """
 
-        # TODO add check for proj
+        assert callable(proj)
         self._proj = proj
-        self._use_projection_dual = use_projection_dual
-
-        # 3D ADMM is not supported yet
-        assert len(psf.shape) == 4, "PSF must be 4D: (depth, height, width, channels)."
-        if psf.shape[0] > 1:
-            raise NotImplementedError(
-                "3D ADMM is not supported yet, use gradient descent or APGD instead."
-            )
+        super(GradientDescent, self).__init__(psf, dtype, **kwargs)
 
-        # call reset() to initialize matrices
-        super(ADMM_PnP, self).__init__(psf, dtype, pad=pad, norm=norm, **kwargs)
-
-        # precompute_R_divmat (self._H computed by constructor with reset())
-        if self.is_torch:
-            self._R_divmat = 1.0 / (
-                self._mu1 * (torch.abs(self._convolver._Hadj * self._convolver._H))
-                + self._mu2
-                + self._mu3
-            ).type(self._complex_dtype)
-        else:
-            self._R_divmat = 1.0 / (
-                self._mu1 * (np.abs(self._convolver._Hadj * self._convolver._H))
-                + self._mu2 * np.abs(self._PsiTPsi)
-                + self._mu3
-            ).astype(self._complex_dtype)
+        if self._denoiser is not None:
+            print("Using denoiser in gradient descent.")
+            # redefine projection function
+            self._proj = self._denoiser
 
     def reset(self):
         if self.is_torch:
-            # TODO initialize without padding
-            # initialize image estimate as [Batch, Depth, Height, Width, Channels]
             if self._initial_est is not None:
                 self._image_est = self._initial_est
             else:
-                self._image_est = torch.zeros([1] + self._padded_shape, dtype=self._dtype).to(
-                    self._psf.device
-                )
-
-            # self._image_est = torch.zeros_like(self._psf)
-            self._X = torch.zeros_like(self._image_est)
-            self._U = torch.zeros_like(self._proj(self._image_est))
-            self._W = torch.zeros_like(self._X)
-            if self._image_est.max():
-                # if non-zero
-                # self._forward_out = self._forward()
-                self._forward_out = self._convolver.convolve(self._image_est)
-            else:
-                self._forward_out = torch.zeros_like(self._X)
-
-            self._xi = torch.zeros_like(self._image_est)
-            self._eta = torch.zeros_like(self._U)
-            self._rho = torch.zeros_like(self._X)
-
-            # precompute_X_divmat
-            self._X_divmat = 1.0 / (self._convolver._pad(torch.ones_like(self._psf)) + self._mu1)
-            # self._X_divmat = 1.0 / (torch.ones_like(self._psf) + self._mu1)
+                # initial guess, half intensity image
+                psf_flat = self._psf.reshape(-1, self._psf_shape[3])
+                pixel_start = (
+                    torch.max(psf_flat, axis=0).values + torch.min(psf_flat, axis=0).values
+                ) / 2
+                # initialize image estimate as [Batch, Depth, Height, Width, Channels]
+                self._image_est = torch.ones_like(self._psf[None, ...]) * pixel_start
+
+            # set step size as < 2 / lipschitz
+            Hadj_flat = self._convolver._Hadj.reshape(-1, self._psf_shape[3])
+            H_flat = self._convolver._H.reshape(-1, self._psf_shape[3])
+            self._alpha = torch.real(1.8 / torch.max(torch.abs(Hadj_flat * H_flat), axis=0).values)
 
         else:
             if self._initial_est is not None:
                 self._image_est = self._initial_est
             else:
-                self._image_est = np.zeros([1] + self._padded_shape, dtype=self._dtype)
+                psf_flat = self._psf.reshape(-1, self._psf_shape[3])
+                pixel_start = (np.max(psf_flat, axis=0) + np.min(psf_flat, axis=0)) / 2
+                # initialize image estimate as [Batch, Depth, Height, Width, Channels]
+                self._image_est = np.ones_like(self._psf[None, ...]) * pixel_start
+
+            # set step size as < 2 / lipschitz
+            Hadj_flat = self._convolver._Hadj.reshape(-1, self._psf_shape[3])
+            H_flat = self._convolver._H.reshape(-1, self._psf_shape[3])
+            self._alpha = np.real(1.8 / np.max(Hadj_flat * H_flat, axis=0))
+
+    def _grad(self):
+        diff = self._convolver.convolve(self._image_est) - self._data
+        return self._convolver.deconvolve(diff)
 
-            # self._U = np.zeros(np.r_[self._padded_shape, [2]], dtype=self._dtype)
-            self._X = np.zeros_like(self._image_est)
-            self._U = np.zeros_like(self._proj(self._image_est))
-            self._W = np.zeros_like(self._X)
-            if self._image_est.max():
-                # if non-zero
-                # self._forward_out = self._forward()
-                self._forward_out = self._convolver.convolve(self._image_est)
-            else:
-                self._forward_out = np.zeros_like(self._X)
+    def _update(self, iter):
+        self._image_est -= self._alpha * self._grad()
+        self._image_est = self._form_image()
 
-            self._xi = np.zeros_like(self._image_est)
-            self._eta = np.zeros_like(self._U)
-            self._rho = np.zeros_like(self._X)
-
-            # precompute_X_divmat
-            self._X_divmat = 1.0 / (
-                self._convolver._pad(np.ones(self._psf_shape, dtype=self._dtype)) + self._mu1
-            )
-
-    def _U_update(self):
-        """Total variation update."""
-        # to avoid computing sparse operator twice
-        if self._use_projection_dual:
-            self._U = self._proj(self._U + self._eta / self._mu2)
+    def _form_image(self):
+        if self._denoiser is not None:
+            return self._proj(self._image_est, self._denoiser_noise_level)
         else:
-            self._U = self._proj(self._image_est)
+            return self._proj(self._image_est)
 
-    def _X_update(self):
-        # to avoid computing forward model twice
-        # self._X = self._X_divmat * (self._xi + self._mu1 * self._forward_out + self._data)
-        self._X = self._X_divmat * (
-            self._xi + self._mu1 * self._forward_out + self._convolver._pad(self._data)
-        )
 
-    def _W_update(self):
-        """Non-negativity update"""
-        if self.is_torch:
-            self._W = torch.maximum(
-                self._rho / self._mu3 + self._image_est, torch.zeros_like(self._image_est)
-            )
-        else:
-            self._W = np.maximum(self._rho / self._mu3 + self._image_est, 0)
+class NesterovGradientDescent(GradientDescent):
+    """
+    Object for applying projected gradient descent with Nesterov momentum for
+    acceleration.
 
-    def _image_update(self):
-        rk = (
-            (self._mu3 * self._W - self._rho)
-            + self._mu2 * self._U
-            + self._convolver.deconvolve(self._mu1 * self._X - self._xi)
-        )
+    A nice tutorial/ blog post on Nesterov momentum can be found
+    `here <https://machinelearningmastery.com/gradient-descent-with-nesterov-momentum-from-scratch/>`_.
 
-        # rk = self._convolver._pad(rk)
+    """
 
-        if self.is_torch:
-            freq_space_result = self._R_divmat * torch.fft.rfft2(rk, dim=(-3, -2))
-            self._image_est = torch.fft.irfft2(freq_space_result, dim=(-3, -2))
-        else:
-            freq_space_result = self._R_divmat * fft.rfft2(rk, axes=(-3, -2))
-            self._image_est = fft.irfft2(freq_space_result, axes=(-3, -2))
+    def __init__(self, psf, dtype=None, proj=non_neg, p=0, mu=0.9, **kwargs):
+        """
+
+        Parameters
+        ----------
+        psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
+        dtype : float32 or float64
+            Data type to use for optimization. Default is float32.
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        p : float
+            Momentum parameter that keeps track of changes. By default, this
+            is initialized to 0.
+        mu : float
+            Momentum parameter. Default is 0.9.
+        """
+        self._p = p
+        self._mu = mu
+        super(NesterovGradientDescent, self).__init__(psf, dtype, proj, **kwargs)
+
+    def reset(self, p=0, mu=0.9):
+        self._p = p
+        self._mu = mu
+        super(NesterovGradientDescent, self).reset()
 
-        # self._image_est = self._convolver._crop(res)
+    def _update(self, iter):
+        p_prev = self._p
+        self._p = self._mu * self._p - self._alpha * self._grad()
+        self._image_est += -self._mu * p_prev + (1 + self._mu) * self._p
+        # self._image_est = self._proj(self._image_est)
+        self._image_est = self._form_image()
 
-    def _xi_update(self):
-        # to avoid computing forward model twice
-        self._xi += self._mu1 * (self._forward_out - self._X)
 
-    def _eta_update(self):
-        # to avoid finite difference operataion again?
-        self._eta += self._mu2 * (self._image_est - self._U)
+class FISTA(GradientDescent):
+    """
+    Object for applying projected gradient descent with FISTA (Fast Iterative
+    Shrinkage-Thresholding Algorithm) for acceleration.
 
-    def _rho_update(self):
-        self._rho += self._mu3 * (self._image_est - self._W)
+    Paper: https://www.ceremade.dauphine.fr/~carlier/FISTA
 
-    def _update(self, iter):
-        self._U_update()
-        if torch.isnan(self._U).any():
-            raise RuntimeError("NaN encountered in U update.")
-        self._X_update()
-        if torch.isnan(self._X).any():
-            raise RuntimeError("NaN encountered in X update.")
-        self._W_update()
-        if torch.isnan(self._W).any():
-            raise RuntimeError("NaN encountered in W update.")
-        self._image_update()
-        if torch.isnan(self._image_est).any():
-            raise RuntimeError("NaN encountered in image update.")
-
-        # update forward and sparse operators
-        self._forward_out = self._convolver.convolve(self._image_est)
-
-        self._xi_update()
-        if self._use_projection_dual:
-            self._eta_update()
-        self._rho_update()
+    """
 
-    def _form_image(self):
-        image = self._convolver._crop(self._image_est)
+    def __init__(self, psf, dtype=None, proj=non_neg, tk=1.0, **kwargs):
+        """
 
-        # # TODO without cropping
-        # image = self._image_est
+        Parameters
+        ----------
+        psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
+            Point spread function (PSF) that models forward propagation.
+            Must be of shape (depth, height, width, channels) even if
+            depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
+            to load a PSF from a file such that it is in the correct format.
+        dtype : float32 or float64
+            Data type to use for optimization. Default is float32.
+        proj : :py:class:`function`
+            Projection function to apply at each iteration. Default is
+            non-negative.
+        tk : float
+            Initial step size parameter for FISTA. It is updated at each iteration
+            according to Eq. 4.2 of paper. By default, initialized to 1.0.
 
-        image[image < 0] = 0
-        return image
+        """
+        self._initial_tk = tk
+
+        super(FISTA, self).__init__(psf, dtype, proj, **kwargs)
+
+        self._tk = tk
+        self._xk = self._image_est
+
+    def reset(self, tk=None):
+        super(FISTA, self).reset()
+        if tk:
+            self._tk = tk
+        else:
+            self._tk = self._initial_tk
+        self._xk = self._image_est
+
+    def _update(self, iter):
+        self._image_est -= self._alpha * self._grad()
+        xk = self._form_image()
+        tk = (1 + np.sqrt(1 + 4 * self._tk**2)) / 2
+        self._image_est = xk + (self._tk - 1) / tk * (xk - self._xk)
+        self._tk = tk
+        self._xk = xk
+
+
+def apply_gradient_descent(psf_fp, data_fp, n_iter, verbose=False, proj=non_neg, **kwargs):
+
+    # load data
+    psf, data = load_data(psf_fp=psf_fp, data_fp=data_fp, plot=False, **kwargs)
+
+    # create reconstruction object
+    recon = GradientDescent(psf, n_iter=n_iter, proj=proj)
+
+    # set data
+    recon.set_data(data)
+
+    # perform reconstruction
+    start_time = time.time()
+    res = recon.apply(plot=False)
+    proc_time = time.time() - start_time
+
+    if verbose:
+        print(f"Reconstruction time : {proc_time} s")
+        print(f"Reconstruction shape: {res.shape}")
+    return res
```

### Comparing `lensless-1.0.6/lensless/recon/apgd.py` & `lensless-1.0.7/lensless/recon/apgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 
 class APGD(ReconstructionAlgorithm):
     def __init__(
         self,
         psf,
         max_iter=500,
-        dtype=np.float32,
+        dtype="float32",
         diff_penalty=None,
         prox_penalty=APGDPriors.NONNEG,
         acceleration=True,
         diff_lambda=0.001,
         prox_lambda=0.001,
         disp=100,
         rel_error=None,
```

### Comparing `lensless-1.0.6/lensless/recon/drunet/basicblock.py` & `lensless-1.0.7/lensless/recon/drunet/basicblock.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/recon/drunet/network_unet.py` & `lensless-1.0.7/lensless/recon/drunet/network_unet.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/recon/mirflickr.py` & `lensless-1.0.7/lensless/recon/mirflickr.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/recon/model_dict.py` & `lensless-1.0.7/lensless/recon/model_dict.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import torch
 from lensless.recon.utils import create_process_network
 from lensless.recon.unrolled_admm import UnrolledADMM
 from lensless.recon.trainable_inversion import TrainableInversion
 from lensless.hardware.trainable_mask import prep_trainable_mask
 import yaml
 from huggingface_hub import snapshot_download
+from collections import OrderedDict
 
 
 model_dir_path = os.path.join(os.path.dirname(__file__), "..", "..", "models")
 
 model_dict = {
     "diffusercam": {
         "mirflickr": {
@@ -54,60 +55,89 @@
         },
     },
     "digicam": {
         "celeba_26k": {
             "unrolled_admm10": "bezzam/digicam-celeba-unrolled-admm10",
             "unrolled_admm10_ft_psf": "bezzam/digicam-celeba-unrolled-admm10-ft-psf",
             "unet8M": "bezzam/digicam-celeba-unet8M",
+            "TrainInv+Unet8M": "bezzam/digicam-celeba-trainable-inv-unet8M",
             "unrolled_admm10_post8M": "bezzam/digicam-celeba-unrolled-admm10-post8M",
             "unrolled_admm10_ft_psf_post8M": "bezzam/digicam-celeba-unrolled-admm10-ft-psf-post8M",
             "pre8M_unrolled_admm10": "bezzam/digicam-celeba-pre8M-unrolled-admm10",
             "pre4M_unrolled_admm10_post4M": "bezzam/digicam-celeba-pre4M-unrolled-admm10-post4M",
-            "pre4M_unrolled_admm10_post4M_OLD": "bezzam/digicam-celeba-pre4M-unrolled-admm10-post4M_OLD",
             "pre4M_unrolled_admm10_ft_psf_post4M": "bezzam/digicam-celeba-pre4M-unrolled-admm10-ft-psf-post4M",
+            "Unet4M+TrainInv+Unet4M": "bezzam/digicam-celeba-unet4M-trainable-inv-unet4M",
             # baseline benchmarks which don't have model file but use ADMM
             "admm_measured_psf": "bezzam/digicam-celeba-admm-measured-psf",
             "admm_simulated_psf": "bezzam/digicam-celeba-admm-simulated-psf",
-        }
+        },
+        "mirflickr_single_25k": {
+            "U10": "bezzam/digicam-mirflickr-single-25k-unrolled-admm10",
+            "Unet8M": "bezzam/digicam-mirflickr-single-25k-unet8M",
+            "TrainInv+Unet8M": "bezzam/digicam-mirflickr-single-25k-trainable-inv-unet8M",
+            "U10+Unet8M": "bezzam/digicam-mirflickr-single-25k-unrolled-admm10-unet8M",
+            "Unet4M+TrainInv+Unet4M": "bezzam/digicam-mirflickr-single-25k-unet4M-trainable-inv-unet4M",
+            "Unet4M+U10+Unet4M": "bezzam/digicam-mirflickr-single-25k-unet4M-unrolled-admm10-unet4M",
+        },
+        "mirflickr_multi_25k": {
+            "Unet8M": "bezzam/digicam-mirflickr-multi-25k-unet8M",
+            "Unet4M+U10+Unet4M": "bezzam/digicam-mirflickr-multi-25k-unet4M-unrolled-admm10-unet4M",
+        },
     },
 }
 
 
-def download_model(camera, dataset, model):
+def remove_data_parallel(old_state_dict):
+    new_state_dict = OrderedDict()
+
+    for k, v in old_state_dict.items():
+        # remove `module.` from k
+        if "module." in k:
+            name = k.replace("module.", "")
+            # name = k[7:] # remove `module.`
+            new_state_dict[name] = v
+
+    return new_state_dict
+
+
+def download_model(camera, dataset, model, local_model_dir=None):
 
     """
     Download model from model_dict (if needed).
 
     Parameters
     ----------
     dataset : str
         Dataset used for training.
     model_name : str
         Name of model.
     """
 
+    if local_model_dir is None:
+        local_model_dir = model_dir_path
+
     if camera not in model_dict:
         raise ValueError(f"Camera {camera} not found in model_dict.")
 
     if dataset not in model_dict[camera]:
         raise ValueError(f"Dataset {dataset} not found in model_dict.")
 
     if model not in model_dict[camera][dataset]:
         raise ValueError(f"Model {model} not found in model_dict.")
 
     repo_id = model_dict[camera][dataset][model]
-    model_dir = os.path.join(model_dir_path, camera, dataset, model)
+    model_dir = os.path.join(local_model_dir, camera, dataset, model)
 
     if not os.path.exists(model_dir):
         snapshot_download(repo_id=repo_id, local_dir=model_dir)
 
     return model_dir
 
 
-def load_model(model_path, psf, device="cpu", legacy_denoiser=False):
+def load_model(model_path, psf, device="cpu", legacy_denoiser=False, verbose=True):
 
     """
     Load best model from model path.
 
     Parameters
     ----------
     model_path : str
@@ -138,15 +168,16 @@
             with torch.no_grad():
                 mask._mask = torch.nn.Parameter(torch.tensor(psf_learned))
                 psf = mask.get_psf().to(device)
 
     # load best model config
     model_checkpoint = os.path.join(model_path, "recon_epochBEST")
     assert os.path.exists(model_checkpoint), "Checkpoint does not exist"
-    print("Loading checkpoint from : ", model_checkpoint)
+    if verbose:
+        print("Loading checkpoint from : ", model_checkpoint)
     model_state_dict = torch.load(model_checkpoint, map_location=device)
 
     # load model
     pre_process = None
     post_process = None
 
     if config["reconstruction"]["pre_process"]["network"] is not None:
@@ -189,14 +220,17 @@
             legacy_denoiser=legacy_denoiser,
         )
 
     if mask is not None:
         psf_learned = torch.nn.Parameter(psf_learned)
         recon._set_psf(psf_learned)
 
+    if "device_ids" in config.keys() and config["device_ids"] is not None:
+        model_state_dict = remove_data_parallel(model_state_dict)
+
     # # return model_state_dict
     # if "_psf" in model_state_dict:
     #     # TODO: should not have to do this...
     #     del model_state_dict["_psf"]
 
     recon.load_state_dict(model_state_dict)
```

### Comparing `lensless-1.0.6/lensless/recon/recon.py` & `lensless-1.0.7/lensless/recon/recon.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 # Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
 """
 Reconstruction
 ==============
 
+Check out `this notebook <https://drive.google.com/file/d/1Wgt6ZMRZVuctLHaXxk7PEyPaBaUPvU33/view?usp=drive_link>`_
+on Google Colab for an overview of the reconstruction algorithms available in LenslessPiCam (analytic and learned).
+
 The core algorithmic component of ``LenslessPiCam`` is the abstract
 class :py:class:`~lensless.ReconstructionAlgorithm`. The five reconstruction
 strategies available in ``LenslessPiCam`` derive from this class:
 
 -  :py:class:`~lensless.GradientDescent`: projected gradient descent with a
    non-negativity constraint. Two accelerated approaches are also
    available: :py:class:`~lensless.NesterovGradientDescent` and
@@ -281,14 +284,15 @@
             if self._dtype == np.float32 or dtype == "float32":
                 self._complex_dtype = np.complex64
             elif self._dtype == np.float64 or dtype == "float64":
                 self._complex_dtype = np.complex128
             else:
                 raise ValueError(f"Unsupported dtype : {self._dtype}")
 
+        self._convolver_param = {"dtype": dtype, "pad": pad, **kwargs}
         self._convolver = RealFFTConvolve2D(psf, dtype=dtype, pad=pad, **kwargs)
         self._padded_shape = self._convolver._padded_shape
 
         if pad:
             self._image_est_shape = self._psf_shape
         else:
             self._image_est_shape = self._convolver._padded_shape
@@ -307,15 +311,15 @@
             assert "noise_level" in denoiser.keys()
 
             from lensless.recon.utils import get_drunet_function_v2, load_drunet
 
             device = self._psf.device
             if denoiser["network"] == "DruNet":
                 denoiser_model = load_drunet(requires_grad=False).to(device)
-                self._denoiser = get_drunet_function_v2(denoiser_model, device, mode="inference")
+                self._denoiser = get_drunet_function_v2(denoiser_model, mode="inference")
             else:
                 raise NotImplementedError(f"Unsupported denoiser: {denoiser['network']}")
             self._denoiser_noise_level = denoiser["noise_level"]
 
         if reset:
             self.reset()
 
@@ -441,26 +445,28 @@
         Set PSF.
 
         Parameters
         ----------
         psf : :py:class:`~numpy.ndarray` or :py:class:`~torch.Tensor`
             PSF to set.
         """
-        assert len(psf.shape) == 4, "PSF must be 4D: (depth, height, width, channels)."
-        assert psf.shape[3] == 3 or psf.shape[3] == 1, "PSF must either be rgb (3) or grayscale (1)"
+        assert (
+            psf.shape[-1] == 3 or psf.shape[-1] == 1
+        ), "PSF must either be rgb (3) or grayscale (1)"
         assert self._psf.shape == psf.shape, "new PSF must have same shape as old PSF"
         assert isinstance(psf, type(self._psf)), "new PSF must have same type as old PSF"
 
         self._psf = psf
         self._convolver = RealFFTConvolve2D(
             psf,
             dtype=self._convolver._psf.dtype,
             pad=self._convolver.pad,
             norm=self._convolver.norm,
         )
+        self.reset()
 
     def _progress(self):
         """
         Optional method for printing progress update, e.g. relative improvement
         in reconstruction.
         """
         return
```

### Comparing `lensless-1.0.6/lensless/recon/rfft_convolve.py` & `lensless-1.0.7/lensless/recon/rfft_convolve.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,18 +48,20 @@
 
         self.is_torch = False
         if torch_available and isinstance(psf, torch.Tensor):
             self.is_torch = True
 
         # prepare shapes for reconstruction
 
-        assert len(psf.shape) == 4, "Expected 4D PSF of shape (depth, width, height, channels)"
-        self._use_3d = psf.shape[0] != 1
-        self._is_rgb = psf.shape[3] == 3
-        assert self._is_rgb or psf.shape[3] == 1
+        assert (
+            len(psf.shape) >= 4
+        ), "Expected 4D PSF of shape ([batch], depth, width, height, channels)"
+        self._use_3d = psf.shape[-4] != 1
+        self._is_rgb = psf.shape[-1] == 3
+        assert self._is_rgb or psf.shape[-1] == 1
 
         # save normalization
         self.norm = norm
 
         # set dtype
         if dtype is None:
             if self.is_torch:
@@ -133,51 +135,68 @@
                 self._padded_data = x  # .type(self.dtype).to(self._psf.device)
             else:
                 self._padded_data[:] = x  # .astype(self.dtype)
 
         if self.is_torch:
             conv_output = torch.fft.ifftshift(
                 torch.fft.irfft2(
-                    torch.fft.rfft2(self._padded_data, dim=(-3, -2)) * self._H, dim=(-3, -2)
+                    torch.fft.rfft2(self._padded_data, dim=(-3, -2)) * self._H,
+                    dim=(-3, -2),
+                    s=self._padded_shape[-3:-1],
                 ),
                 dim=(-3, -2),
             )
 
         else:
             conv_output = fft.ifftshift(
-                fft.irfft2(fft.rfft2(self._padded_data, axes=(-3, -2)) * self._H, axes=(-3, -2)),
+                fft.irfft2(
+                    fft.rfft2(self._padded_data, axes=(-3, -2)) * self._H,
+                    axes=(-3, -2),
+                    s=self._padded_shape[-3:-1],
+                ),
                 axes=(-3, -2),
             )
         if self.pad:
-            return self._crop(conv_output)
-        else:
-            return conv_output
+            conv_output = self._crop(conv_output)
+
+        # ensure shape stays the same
+        assert conv_output.shape[-3:-1] == x.shape[-3:-1]
+        return conv_output
 
     def deconvolve(self, y):
         """
         Deconvolve with adjoint of pre-computed FFT of provided PSF.
         """
         if self.pad:
             self._padded_data = self._pad(y)
         else:
             if self.is_torch:
                 self._padded_data = y  # .type(self.dtype).to(self._psf.device)
             else:
                 self._padded_data[:] = y  # .astype(self.dtype)
+
         if self.is_torch:
             deconv_output = torch.fft.ifftshift(
                 torch.fft.irfft2(
-                    torch.fft.rfft2(self._padded_data, dim=(-3, -2)) * self._Hadj, dim=(-3, -2)
+                    torch.fft.rfft2(self._padded_data, dim=(-3, -2)) * self._Hadj,
+                    dim=(-3, -2),
+                    s=self._padded_shape[-3:-1],
                 ),
                 dim=(-3, -2),
             )
 
         else:
             deconv_output = fft.ifftshift(
-                fft.irfft2(fft.rfft2(self._padded_data, axes=(-3, -2)) * self._Hadj, axes=(-3, -2)),
+                fft.irfft2(
+                    fft.rfft2(self._padded_data, axes=(-3, -2)) * self._Hadj,
+                    axes=(-3, -2),
+                    s=self._padded_shape[-3:-1],
+                ),
                 axes=(-3, -2),
             )
 
         if self.pad:
-            return self._crop(deconv_output)
-        else:
-            return deconv_output
+            deconv_output = self._crop(deconv_output)
+
+        # ensure shape stays the same
+        assert deconv_output.shape[-3:-1] == y.shape[-3:-1]
+        return deconv_output
```

### Comparing `lensless-1.0.6/lensless/recon/tikhonov.py` & `lensless-1.0.7/lensless/recon/tikhonov.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/recon/trainable_inversion.py` & `lensless-1.0.7/lensless/recon/trainable_inversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     """ """
 
     def __init__(self, psf, dtype=None, K=1e-4, **kwargs):
         """
         Constructor for trainable inversion component as proposed in
         the FlatNet work: https://siddiquesalman.github.io/flatnet/
 
+        Their implementation: https://github.com/siddiquesalman/flatnet/blob/d1dc179666a08df58c4bdf83c4274310ba3cd186/models/fftlayer.py#L70
+
         Parameters
         ----------
         psf : :py:class:`~torch.Tensor`
             Point spread function (PSF) that models forward propagation.
             Must be of shape (depth, height, width, channels) even if
             depth = 1 and channels = 1. You can use :py:func:`~lensless.io.load_psf`
             to load a PSF from a file such that it is in the correct format.
```

### Comparing `lensless-1.0.6/lensless/recon/trainable_recon.py` & `lensless-1.0.7/lensless/recon/trainable_recon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # #############################################################################
 # trainable_recon.py
 # ==================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
+# Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
 import pathlib as plib
 from matplotlib import pyplot as plt
 from lensless.recon.recon import ReconstructionAlgorithm
 from lensless.utils.plot import plot_image
+from lensless.recon.rfft_convolve import RealFFTConvolve2D
 
 try:
     import torch
 
 except ImportError:
     raise ImportError("Pytorch is require to use trainable reconstruction algorithms.")
 
@@ -110,21 +112,17 @@
         """
         if isinstance(process, torch.nn.Module):
             # If the post_process is a torch module, we assume it is a DruNet like network.
             from lensless.recon.utils import get_drunet_function, get_drunet_function_v2
 
             process_model = process
             if self._legacy_denoiser:
-                process_function = get_drunet_function(
-                    process_model, self._psf.device, mode="train"
-                )
+                process_function = get_drunet_function(process_model, mode="train")
             else:
-                process_function = get_drunet_function_v2(
-                    process_model, self._psf.device, mode="train"
-                )
+                process_function = get_drunet_function_v2(process_model, mode="train")
         elif process is not None:
             # Otherwise, we assume it is a function.
             assert callable(process), "pre_process must be a callable function"
             process_function = process
             process_model = None
         else:
             process_function = None
@@ -187,36 +185,51 @@
         """
         if self.post_process_param is not None:
             self.post_process_param.requires_grad = True
         if self.post_process_model is not None:
             for param in self.post_process_model.parameters():
                 param.requires_grad = True
 
-    def batch_call(self, batch):
+    def forward(self, batch, psfs=None):
         """
         Method for performing iterative reconstruction on a batch of images.
         This implementation is a properly vectorized implementation of FISTA.
 
         Parameters
         ----------
         batch : :py:class:`~torch.Tensor` of shape (batch, depth, channels, height, width)
             The lensless images to reconstruct.
+        psfs : :py:class:`~torch.Tensor` of shape (batch, depth, channels, height, width)
+            The lensless images to reconstruct.
 
         Returns
         -------
         :py:class:`~torch.Tensor` of shape (batch, depth, channels, height, width)
             The reconstructed images.
         """
         self._data = batch
         assert len(self._data.shape) == 5, "batch must be of shape (N, D, C, H, W)"
         batch_size = batch.shape[0]
 
+        if psfs is not None:
+            # assert same shape
+            assert psfs.shape == batch.shape, "psfs must have the same shape as batch"
+            # -- update convolver
+            self._convolver = RealFFTConvolve2D(psfs.to(self._data.device), **self._convolver_param)
+        elif self._data.device != self._convolver._H.device:
+            # need for multi-GPU... TODO better solution?
+            self._convolver = RealFFTConvolve2D(
+                self._psf.to(self._data.device), **self._convolver_param
+            )
+
         # pre process data
         if self.pre_process is not None:
+            device_before = self._data.device
             self._data = self.pre_process(self._data, self.pre_process_param)
+            self._data = self._data.to(device_before)
 
         self.reset(batch_size=batch_size)
 
         # unrolled algorithm
         if not self.skip_unrolled:
             for i in range(self._n_iter):
                 self._update(i)
```

### Comparing `lensless-1.0.6/lensless/recon/unrolled_admm.py` & `lensless-1.0.7/lensless/recon/unrolled_admm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # #############################################################################
 # unrolled_admm.py
 # =================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
+# Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
 from lensless.recon.trainable_recon import TrainableReconstructionAlgorithm
 from lensless.recon.admm import soft_thresh, finite_diff, finite_diff_adj, finite_diff_gram
 
 
 try:
@@ -126,27 +127,31 @@
     def _PsiT(self, U):
         """
         Adjoint of `_Psi`.
         """
         return finite_diff_adj(U)
 
     def reset(self, batch_size=1):
+
+        if self._data is not None:
+            device = self._data.device
+        else:
+            device = self._convolver._H.device
+
         # ensure that mu1, mu2, mu3, tau are positive
-        self._mu1 = torch.abs(self._mu1_p)
-        self._mu2 = torch.abs(self._mu2_p)
-        self._mu3 = torch.abs(self._mu3_p)
-        self._tau = torch.abs(self._tau_p)
+        self._mu1 = torch.abs(self._mu1_p).to(device)
+        self._mu2 = torch.abs(self._mu2_p).to(device)
+        self._mu3 = torch.abs(self._mu3_p).to(device)
+        self._tau = torch.abs(self._tau_p).to(device)
 
         # TODO initialize without padding
         if self._initial_est is not None:
-            self._image_est = self._initial_est
+            self._image_est = self._initial_est.to(device)
         else:
-            self._image_est = torch.zeros([1] + self._padded_shape, dtype=self._dtype).to(
-                self._psf.device
-            )
+            self._image_est = torch.zeros([1] + self._padded_shape, dtype=self._dtype).to(device)
 
         self._X = torch.zeros_like(self._image_est)
         self._U = torch.zeros_like(self._Psi(self._image_est))
         self._W = torch.zeros_like(self._X)
         if self._image_est.max():
             # if non-zero
             self._forward_out = self._convolver.convolve(self._image_est)
@@ -155,26 +160,26 @@
             self._forward_out = torch.zeros_like(self._X)
             self._Psi_out = torch.zeros_like(self._U)
 
         self._xi = torch.zeros_like(self._image_est)
         self._eta = torch.zeros_like(self._U)
         self._rho = torch.zeros_like(self._X)
 
-        # precompute_R_divmat
+        # precompute_R_divmat [iter, batch, depth, height, width, channels]
         self._R_divmat = 1.0 / (
-            self._mu1[:, None, None, None, None]
-            * (torch.abs(self._convolver._Hadj * self._convolver._H))
-            + self._mu2[:, None, None, None, None] * torch.abs(self._PsiTPsi)
-            + self._mu3[:, None, None, None, None]
+            self._mu1[:, None, None, None, None, None]
+            * (torch.abs(self._convolver._Hadj * self._convolver._H))[None, ...]
+            + self._mu2[:, None, None, None, None, None] * torch.abs(self._PsiTPsi).to(device)
+            + self._mu3[:, None, None, None, None, None]
         ).type(self._complex_dtype)
 
-        # precompute_X_divmat
+        # precompute_X_divmat [iter, batch, depth, height, width, channels]
         self._X_divmat = 1.0 / (
-            self._convolver._pad(torch.ones_like(self._psf[None, ...]))
-            + self._mu1[:, None, None, None, None]
+            self._convolver._pad(torch.ones_like(self._convolver._psf))[None, ...]
+            + self._mu1[:, None, None, None, None, None]
         )
 
     def _U_update(self, iter):
         """Total variation update."""
         # to avoid computing sparse operator twice
         self._U = soft_thresh(
             self._Psi_out + self._eta / self._mu2[iter], self._tau[iter] / self._mu2[iter]
@@ -189,15 +194,17 @@
     def _image_update(self, iter):
         rk = (
             (self._mu3[iter] * self._W - self._rho)
             + self._PsiT(self._mu2[iter] * self._U - self._eta)
             + self._convolver.deconvolve(self._mu1[iter] * self._X - self._xi)
         )
         freq_space_result = self._R_divmat[iter] * torch.fft.rfft2(rk, dim=(-3, -2))
-        self._image_est = torch.fft.irfft2(freq_space_result, dim=(-3, -2))
+        self._image_est = torch.fft.irfft2(
+            freq_space_result, dim=(-3, -2), s=self._convolver._padded_shape[-3:-1]
+        )
 
     def _W_update(self, iter):
         """Non-negativity update"""
         self._W = torch.maximum(
             self._rho / self._mu3[iter] + self._image_est, torch.zeros_like(self._image_est)
         )
```

### Comparing `lensless-1.0.6/lensless/recon/unrolled_fista.py` & `lensless-1.0.7/lensless/recon/unrolled_fista.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/recon/utils.py` & `lensless-1.0.7/lensless/recon/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 # utils.py
 # =================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
 # Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
-
+import wandb
 import json
 import math
 import numpy as np
 import matplotlib.pyplot as plt
 import time
-from hydra.utils import get_original_cwd
 import os
 import torch
 from lensless.eval.benchmark import benchmark
 from lensless.hardware.trainable_mask import TrainableMask
 from tqdm import tqdm
 from lensless.recon.drunet.network_unet import UNetRes
 from lensless.utils.io import save_image
 from lensless.utils.plot import plot_image
+from lensless.utils.dataset import SimulatedDatasetTrainableMask
 
 
 def load_drunet(model_path=None, n_channels=3, requires_grad=False):
     """
     Load a pre-trained Drunet model.
 
     Parameters
@@ -50,15 +50,15 @@
                 from torchvision.datasets.utils import download_url
             except ImportError:
                 exit()
             msg = "Do you want to download the pretrained DRUNet model (130MB)?"
 
             # default to yes if no input is given
             valid = input("%s (Y/n) " % msg).lower() != "n"
-            output_path = os.path.join(get_original_cwd(), "models")
+            output_path = os.path.join(this_file_path, "..", "..", "models")
             if valid:
                 url = "https://drive.switch.ch/index.php/s/jTdeMHom025RFRQ/download"
                 filename = "drunet_color.pth"
                 download_url(url, output_path, filename=filename)
 
     assert os.path.exists(model_path), f"Model path {model_path} does not exist"
 
@@ -75,15 +75,15 @@
     model.eval()
     for _, v in model.named_parameters():
         v.requires_grad = requires_grad
 
     return model
 
 
-def apply_denoiser(model, image, noise_level=10, device="cpu", mode="inference"):
+def apply_denoiser(model, image, noise_level=10, mode="inference"):
     """
     Apply a pre-trained denoising model with input in the format Channel, Height, Width.
     An additionnal channel is added for the noise level as done in Drunet.
 
     Parameters
     ----------
     model : :py:class:`torch.nn.Module`
@@ -112,19 +112,18 @@
     # pad image H and W to next multiple of 8
     top = (8 - image.shape[-2] % 8) // 2
     bottom = (8 - image.shape[-2] % 8) - top
     left = (8 - image.shape[-1] % 8) // 2
     right = (8 - image.shape[-1] % 8) - left
     image = torch.nn.functional.pad(image, (left, right, top, bottom), mode="constant", value=0)
     # add noise level as extra channel
-    image = image.to(device)
     if isinstance(noise_level, torch.Tensor):
         noise_level = noise_level / 255.0
     else:
-        noise_level = torch.tensor([noise_level / 255.0]).to(device)
+        noise_level = torch.tensor([noise_level / 255.0])
 
     image = torch.cat(
         (
             image,
             noise_level.repeat(image.shape[0], 1, image.shape[2], image.shape[3]),
         ),
         dim=1,
@@ -143,15 +142,15 @@
     image = image[:, :, top:-bottom, left:-right]
     # convert back to NDHWC
     image = image.movedim(-3, -1)
     image = image.reshape(-1, depth, *image.shape[-3:])
     return image
 
 
-def get_drunet_function(model, device="cpu", mode="inference"):
+def get_drunet_function(model, mode="inference"):
     """
     Return a processing function that applies the DruNet model to an image.
     Legacy function to work with pre-trained models, use get_drunet_function_v2 instead.
 
     Parameters
     ----------
     model : :py:class:`torch.nn.Module`
@@ -164,47 +163,43 @@
 
     def process(image, noise_level):
         x_max = torch.amax(image, dim=(-2, -3), keepdim=True) + 1e-6
         image = apply_denoiser(
             model,
             image,
             noise_level=noise_level,
-            device=device,
             mode=mode,
         )
         image = torch.clip(image, min=0.0) * x_max
         return image
 
     return process
 
 
-def get_drunet_function_v2(model, device="cpu", mode="inference"):
+def get_drunet_function_v2(model, mode="inference"):
     """
     Return a processing function that applies the DruNet model to an image.
 
     Parameters
     ----------
     model : :py:class:`torch.nn.Module`
         DruNet like denoiser model
-    device : str
-        Device to use for computation. Can be "cpu" or "cuda".
     mode : str
         Mode to use for model. Can be "inference" or "train".
     """
 
     def process(image, noise_level):
         x_max = torch.amax(image, dim=(-1, -2, -3, -4), keepdim=True) + 1e-6
         image = apply_denoiser(
             model,
             image / x_max,
             noise_level=noise_level,
-            device=device,
             mode=mode,
         )
-        image = torch.clip(image, min=0.0) * x_max
+        image = torch.clip(image, min=0.0) * x_max.to(image.device)
         return image
 
     return process
 
 
 def measure_gradient(model):
     """
@@ -224,15 +219,15 @@
     for p in model.parameters():
         param_norm = p.grad.detach().data.norm(2)
         total_norm += param_norm.item() ** 2
     total_norm = total_norm**0.5
     return total_norm
 
 
-def create_process_network(network, depth=4, device="cpu", nc=None):
+def create_process_network(network, depth=4, device="cpu", nc=None, device_ids=None):
     """
     Helper function to create a process network.
 
     Parameters
     ----------
     network : str
         Name of network to use. Can be "DruNet" or "UnetRes".
@@ -251,34 +246,39 @@
         nc = [64, 128, 256, 512]
     else:
         assert len(nc) == 4
 
     if network == "DruNet":
         from lensless.recon.utils import load_drunet
 
-        process = load_drunet(requires_grad=True).to(device)
+        process = load_drunet(requires_grad=True)
         process_name = "DruNet"
     elif network == "UnetRes":
         from lensless.recon.drunet.network_unet import UNetRes
 
         n_channels = 3
         process = UNetRes(
             in_nc=n_channels + 1,
             out_nc=n_channels,
             nc=nc,
             nb=depth,
             act_mode="R",
             downsample_mode="strideconv",
             upsample_mode="convtranspose",
-        ).to(device)
+        )
         process_name = "UnetRes_d" + str(depth)
     else:
         process = None
         process_name = None
 
+    if process is not None:
+        if device_ids is not None:
+            process = torch.nn.DataParallel(process, device_ids=device_ids)
+        process = process.to(device)
+
     return (process, process_name)
 
 
 class Trainer:
     def __init__(
         self,
         recon,
@@ -297,14 +297,16 @@
         metric_for_best_model=None,
         save_every=None,
         gamma=None,
         logger=None,
         crop=None,
         clip_grad=1.0,
         unrolled_output_factor=False,
+        extra_eval_sets=None,
+        use_wandb=False,
         # for adding components during training
         pre_process=None,
         pre_process_delay=None,
         pre_process_freeze=None,
         pre_process_unfreeze=None,
         post_process=None,
         post_process_delay=None,
@@ -377,14 +379,16 @@
         post_process_unfreeze : int, optional
             Epoch at which to unfreeze post process component. Default is None.
 
 
         """
         global print
 
+        self.use_wandb = use_wandb
+
         self.device = recon._psf.device
         self.logger = logger
         if self.logger is not None:
             self.print = self.logger.info
         else:
             self.print = print
         self.recon = recon
@@ -412,34 +416,59 @@
             train_size = int((1 - test_size) * len(train_dataset))
             test_size = len(train_dataset) - train_size
             train_dataset, test_dataset = torch.utils.data.random_split(
                 train_dataset, [train_size, test_size]
             )
             self.print(f"Train size : {train_size}, Test size : {test_size}")
 
+        self.train_dataset = train_dataset
         self.train_dataloader = torch.utils.data.DataLoader(
             dataset=train_dataset,
             batch_size=batch_size,
             shuffle=True,
             pin_memory=(self.device != "cpu"),
         )
         self.test_dataset = test_dataset
+        self.extra_eval_sets = extra_eval_sets  # additional datasets to evaluate on
         self.lpips = lpips
         self.skip_NAN = skip_NAN
         self.eval_batch_size = eval_batch_size
+        self.train_multimask = False
+        if hasattr(train_dataset, "multimask"):
+            self.train_multimask = train_dataset.multimask
+
+        # check if Subset and if simulating dataset
+        self.simulated_dataset_trainable_mask = False
+        if isinstance(self.test_dataset, SimulatedDatasetTrainableMask):
+            # assuming the case for both training and testing
+            self.simulated_dataset_trainable_mask = True
 
         self.mask = mask
+        self.gamma = gamma
         if mask is not None:
             assert isinstance(mask, TrainableMask)
             self.use_mask = True
         else:
             self.use_mask = False
+        if self.use_mask:
+            # save original PSF
+            psf_np = self.mask.get_psf().detach().cpu().numpy()[0, ...]
+            psf_np = psf_np.squeeze()  # remove (potential) singleton color channel
+            np.save("psf_original.npy", psf_np)
+            fp = "psf_original.png"
+            save_image(psf_np, fp)
+            plot_image(psf_np, gamma=self.gamma)
+            fp_plot = "psf_original_plot.png"
+            plt.savefig(fp_plot)
+
+            if self.use_wandb:
+                wandb.log({"psf": wandb.Image(fp)}, step=0)
+                wandb.log({"psf_plot": wandb.Image(fp_plot)}, step=0)
 
         self.l1_mask = l1_mask
-        self.gamma = gamma
 
         # loss
         if loss == "l2":
             self.Loss = torch.nn.MSELoss()
         elif loss == "l1":
             self.Loss = torch.nn.L1Loss()
         else:
@@ -468,14 +497,15 @@
             assert self.post_process_freeze is None
 
         # optimizer
         self.clip_grad_norm = clip_grad
         self.optimizer_config = optimizer
         self.set_optimizer()
 
+        # metrics
         self.metrics = {
             "LOSS": [],  # train loss
             "LOSS_TEST": [],  # test loss
             "MSE": [],
             "MAE": [],
             "LPIPS_Vgg": [],
             "LPIPS_Alex": [],
@@ -492,14 +522,17 @@
         }
         if self.unrolled_output_factor:
             # -- add unrolled metrics
             for key in ["MSE", "MAE", "LPIPS_Vgg", "LPIPS_Alex", "PSNR", "SSIM"]:
                 self.metrics[key + "_unrolled"] = []
         if metric_for_best_model is not None:
             assert metric_for_best_model in self.metrics.keys()
+        if extra_eval_sets is not None:
+            for key in extra_eval_sets:
+                self.metrics[key] = dict()
         self.save_every = save_every
 
         # Backward hook that detect NAN in the gradient and print the layer weights
         if not self.skip_NAN:
 
             def detect_nan(grad):
                 if torch.isnan(grad).any():
@@ -517,19 +550,18 @@
                 if param.requires_grad:
                     param.register_hook(detect_nan)
                     if param.requires_grad:
                         param.register_hook(detect_nan)
 
     def set_optimizer(self, last_epoch=-1):
 
-        if self.optimizer_config.type == "Adam":
-            parameters = [{"params": self.recon.parameters()}]
-            self.optimizer = torch.optim.Adam(parameters, lr=self.optimizer_config.lr)
-        else:
-            raise ValueError(f"Unsupported optimizer : {self.optimizer_config.type}")
+        parameters = [{"params": self.recon.parameters()}]
+        self.optimizer = getattr(torch.optim, self.optimizer_config.type)(
+            parameters, lr=self.optimizer_config.lr
+        )
 
         # Scheduler
         if self.optimizer_config.slow_start:
 
             def learning_rate_function(epoch):
                 if epoch == 0:
                     return self.optimizer_config.slow_start
@@ -574,45 +606,59 @@
         -------
         float
             Mean loss of the epoch.
         """
         mean_loss = 0.0
         i = 1.0
         pbar = tqdm(data_loader)
-        for X, y in pbar:
+        for batch in pbar:
+
+            # get batch
+            if self.train_multimask:
+                X, y, psfs = batch
+                psfs = psfs.to(self.device)
+            else:
+                X, y = batch
+                psfs = None
+
             # send to device
             X = X.to(self.device)
             y = y.to(self.device)
 
             # update psf according to mask
             if self.use_mask:
                 self.recon._set_psf(self.mask.get_psf().to(self.device))
 
             # forward pass
-            y_pred = self.recon.batch_call(X.to(self.device))
+            y_pred = self.recon.forward(batch=X, psfs=psfs)
             if self.unrolled_output_factor:
                 unrolled_out = y_pred[1]
                 y_pred = y_pred[0]
 
             # normalizing each output
             eps = 1e-12
             y_pred_max = torch.amax(y_pred, dim=(-1, -2, -3), keepdim=True) + eps
             y_pred = y_pred / y_pred_max
 
             # normalizing y
             y_max = torch.amax(y, dim=(-1, -2, -3), keepdim=True) + eps
             y = y / y_max
 
-            self.optimizer.zero_grad(set_to_none=True)
             # convert to CHW for loss and remove depth
             y_pred = y_pred.reshape(-1, *y_pred.shape[-3:]).movedim(-1, -3)
             y = y.reshape(-1, *y.shape[-3:]).movedim(-1, -3)
 
             # extraction region of interest for loss
-            if self.crop is not None:
+            if hasattr(self.train_dataset, "alignment"):
+                if self.train_dataset.alignment is not None:
+                    y_pred = self.train_dataset.extract_roi(y_pred, axis=(-2, -1))
+                else:
+                    y_pred, y = self.train_dataset.extract_roi(y_pred, axis=(-2, -1), lensed=y)
+
+            elif self.crop is not None:
                 y_pred = y_pred[
                     ...,
                     self.crop["vertical"][0] : self.crop["vertical"][1],
                     self.crop["horizontal"][0] : self.crop["horizontal"][1],
                 ]
                 y = y[
                     ...,
@@ -631,15 +677,17 @@
                     y = y.repeat(1, 3, 1, 1)
 
                 # value for LPIPS needs to be in range [-1, 1]
                 loss_v = loss_v + self.lpips * torch.mean(
                     self.Loss_lpips(2 * y_pred - 1, 2 * y - 1)
                 )
             if self.use_mask and self.l1_mask:
-                loss_v = loss_v + self.l1_mask * torch.mean(torch.abs(self.mask._mask))
+                for p in self.mask.parameters():
+                    if p.requires_grad:
+                        loss_v = loss_v + self.l1_mask * torch.mean(torch.abs(p))
 
             if self.unrolled_output_factor:
                 # -- normalize
                 unrolled_out_max = torch.amax(unrolled_out, dim=(-1, -2, -3), keepdim=True) + eps
                 unrolled_out = unrolled_out / unrolled_out_max
 
                 # -- convert to CHW for loss and remove depth
@@ -669,58 +717,82 @@
 
                 # -- add unrolled loss to total loss
                 loss_v = loss_v + self.unrolled_output_factor * loss_unrolled
 
             # backward pass
             loss_v.backward()
 
+            # check mask parameters are learning
+            if self.use_mask:
+                for p in self.mask.parameters():
+                    assert p.grad is not None
+
             if self.clip_grad_norm is not None:
+                if self.use_mask:
+                    torch.nn.utils.clip_grad_norm_(self.mask.parameters(), self.clip_grad_norm)
                 torch.nn.utils.clip_grad_norm_(self.recon.parameters(), self.clip_grad_norm)
 
             # if any gradient is NaN, skip training step
             if self.skip_NAN:
-                is_NAN = False
+                recon_is_NAN = False
+                mask_is_NAN = False
                 for param in self.recon.parameters():
                     if param.grad is not None and torch.isnan(param.grad).any():
-                        is_NAN = True
+                        recon_is_NAN = True
                         break
-                if is_NAN:
-                    self.print("NAN detected in gradiant, skipping training step")
+                if self.use_mask:
+                    for param in self.mask.parameters():
+                        if param.grad is not None and torch.isnan(param.grad).any():
+                            mask_is_NAN = True
+                            break
+                if recon_is_NAN or mask_is_NAN:
+                    if recon_is_NAN:
+                        self.print(
+                            "NAN detected in reconstruction gradient, skipping training step"
+                        )
+                    if mask_is_NAN:
+                        self.print("NAN detected in mask gradient, skipping training step")
                     i += 1
                     continue
+
             self.optimizer.step()
+            self.optimizer.zero_grad(set_to_none=True)
 
             # update mask
             if self.use_mask:
                 self.mask.update_mask()
+                if self.simulated_dataset_trainable_mask:
+                    self.train_dataloader.dataset.set_psf()
 
             mean_loss += (loss_v.item() - mean_loss) * (1 / i)
             pbar.set_description(f"loss : {mean_loss}")
             i += 1
 
         self.print(f"loss : {mean_loss}")
 
         return mean_loss
 
-    def evaluate(self, mean_loss, save_pt, epoch, disp=None):
+    def evaluate(self, mean_loss, epoch, disp=None):
         """
         Evaluate the reconstruction algorithm on the test dataset.
 
         Parameters
         ----------
         mean_loss : float
             Mean loss of the last epoch.
-        save_pt : str
-            Path to save metrics dictionary to. If None, no logging of metrics.
         disp : list of int, optional
             Test set examples to visualize at the end of each epoch, by default None.
         """
         if self.test_dataset is None:
             return
 
+        if self.use_mask and self.simulated_dataset_trainable_mask:
+            with torch.no_grad():
+                self.test_dataset.set_psf()
+
         output_dir = None
         if disp is not None:
             output_dir = os.path.join("eval_recon")
             if not os.path.exists(output_dir):
                 os.mkdir(output_dir)
             output_dir = os.path.join(output_dir, str(epoch))
 
@@ -729,42 +801,99 @@
             self.recon,
             self.test_dataset,
             batchsize=self.eval_batch_size,
             save_idx=disp,
             output_dir=output_dir,
             crop=self.crop,
             unrolled_output_factor=self.unrolled_output_factor,
+            use_wandb=self.use_wandb,
+            epoch=epoch,
         )
 
         # update metrics with current metrics
         self.metrics["LOSS"].append(mean_loss)
+        if self.use_wandb:
+            wandb.log({"LOSS": mean_loss}, step=epoch)
         for key in current_metrics:
             self.metrics[key].append(current_metrics[key])
 
-        if save_pt:
-            # save dictionary metrics to file with json
-            with open(os.path.join(save_pt, "metrics.json"), "w") as f:
-                json.dump(self.metrics, f, indent=4)
-
         # check best metric
         if self.metrics["metric_for_best_model"] is None:
             eval_loss = current_metrics["MSE"]
             if self.lpips is not None:
                 eval_loss += self.lpips * current_metrics["LPIPS_Vgg"]
             if self.use_mask and self.l1_mask:
-                eval_loss += self.l1_mask * np.mean(np.abs(self.mask._mask.cpu().detach().numpy()))
+                with torch.no_grad():
+                    for p in self.mask.parameters():
+                        if p.requires_grad:
+                            eval_loss += self.l1_mask * np.mean(np.abs(p.cpu().detach().numpy()))
             if self.unrolled_output_factor:
                 unrolled_loss = current_metrics["MSE_unrolled"]
                 if self.lpips is not None:
                     unrolled_loss += self.lpips * current_metrics["LPIPS_Vgg_unrolled"]
                 eval_loss += self.unrolled_output_factor * unrolled_loss
         else:
             eval_loss = current_metrics[self.metrics["metric_for_best_model"]]
 
         self.metrics["LOSS_TEST"].append(eval_loss)
+        if self.use_wandb:
+            wandb.log({"LOSS_TEST": eval_loss}, step=epoch)
+
+        # add extra evaluation sets
+        extra_metrics_epoch = {}
+        if self.extra_eval_sets is not None:
+            for eval_set in self.extra_eval_sets:
+
+                # create output directory
+                output_dir = None
+                if disp is not None:
+                    output_dir = os.path.join("eval_recon")
+                    if not os.path.exists(output_dir):
+                        os.mkdir(output_dir)
+                    output_dir = os.path.join(output_dir, str(epoch) + f"_{eval_set}")
+
+                if hasattr(self.extra_eval_sets[eval_set], "multimask"):
+                    if not self.extra_eval_sets[eval_set].multimask:
+                        # need to set correct PSF for evaluation
+                        # TODO cleaner way to set PSF?
+                        self.recon._set_psf(self.extra_eval_sets[eval_set].psf.to(self.device))
+
+                # benchmarking
+                extra_metrics = benchmark(
+                    self.recon,
+                    self.extra_eval_sets[eval_set],
+                    batchsize=self.eval_batch_size,
+                    save_idx=disp,
+                    output_dir=output_dir,
+                    crop=self.crop,
+                    unrolled_output_factor=self.unrolled_output_factor,
+                    use_wandb=self.use_wandb,
+                    label=eval_set,
+                    epoch=epoch,
+                )
+
+                # add metrics to dictionary
+                for key in extra_metrics:
+                    if key not in self.metrics[eval_set]:
+                        self.metrics[eval_set][key] = [extra_metrics[key]]
+                    else:
+                        self.metrics[eval_set][key].append(extra_metrics[key])
+                    extra_metrics_epoch[f"{eval_set}_{key}"] = extra_metrics[key]
+
+            # set back PSF to original in case changed
+            # TODO: cleaner way?
+            if not self.train_multimask:
+                self.recon._set_psf(self.train_dataset.psf.to(self.device))
+
+        # log metrics to wandb
+        if self.use_wandb:
+            wandb.log(current_metrics, step=epoch)
+            if self.extra_eval_sets is not None:
+                wandb.log(extra_metrics_epoch, step=epoch)
+
         return eval_loss
 
     def on_epoch_end(self, mean_loss, save_pt, epoch, disp=None):
         """
         Called at the end of each epoch.
 
         Parameters
@@ -779,16 +908,15 @@
             Test set examples to visualize at the end of each epoch, by default None.
         """
         if save_pt is None:
             # Use current directory
             save_pt = os.getcwd()
 
         # save model
-        # self.save(path=save_pt, include_optimizer=False)
-        epoch_eval_metric = self.evaluate(mean_loss, save_pt, epoch, disp=disp)
+        epoch_eval_metric = self.evaluate(mean_loss, epoch, disp=disp)
         new_best = False
         if (
             self.metrics["metric_for_best_model"] == "PSNR"
             or self.metrics["metric_for_best_model"] == "SSIM"
         ):
             if epoch_eval_metric > self.metrics["best_eval_score"]:
                 self.metrics["best_eval_score"] = epoch_eval_metric
@@ -801,14 +929,18 @@
         if new_best:
             self.metrics["best_epoch"] = epoch
             self.save(path=save_pt, include_optimizer=False, epoch="BEST")
 
         if self.save_every is not None and epoch % self.save_every == 0:
             self.save(path=save_pt, include_optimizer=False, epoch=epoch)
 
+        # save dictionary metrics to file with json
+        with open(os.path.join(save_pt, "metrics.json"), "w") as f:
+            json.dump(self.metrics, f, indent=4)
+
     def train(self, n_epoch=1, save_pt=None, disp=None):
         """
         Train the reconstruction algorithm.
 
         Parameters
         ----------
         n_epoch : int, optional
@@ -817,15 +949,15 @@
             Path to save metrics dictionary to. If None, use current directory, by default None
         disp : list of int, optional
             test set examples to visualize at the end of each epoch, by default None.
         """
 
         start_time = time.time()
 
-        self.evaluate(-1, save_pt, epoch=0, disp=disp)
+        self.evaluate(mean_loss=1, epoch=0, disp=disp)
         for epoch in range(n_epoch):
 
             # add extra components (if specified)
             changing_n_param = False
             if epoch == self.pre_process_delay:
                 self.print("Adding pre process component")
                 self.recon.set_pre_process(self.pre_process)
@@ -866,42 +998,55 @@
 
         self.print(f"Train time [hour] : {(time.time() - start_time) / 3600} h")
 
     def save(self, epoch, path="recon", include_optimizer=False):
         # create directory if it does not exist
         if not os.path.exists(path):
             os.makedirs(path)
-        # save mask
-        if self.use_mask:
-            # torch.save(self.mask._mask, os.path.join(path, f"mask_epoch{epoch}.pt"))
 
-            # save mask as numpy array
-            if self.mask.train_mask_vals:
-                np.save(
-                    os.path.join(path, f"mask_epoch{epoch}.npy"),
-                    self.mask._mask.cpu().detach().numpy(),
-                )
+        # save mask parameters
+        if self.use_mask:
 
-            # if color_filter is an attribute
-            if hasattr(self.mask, "color_filter") and self.mask.color_filter is not None:
-                # save save numpy array
-                np.save(
-                    os.path.join(path, f"mask_color_filter_epoch{epoch}.npy"),
-                    self.mask.color_filter.cpu().detach().numpy(),
-                )
+            for name, param in self.mask.named_parameters():
+                # save as numpy array
+                if param.requires_grad:
+                    np.save(
+                        os.path.join(path, f"mask{name}_epoch{epoch}.npy"),
+                        param.cpu().detach().numpy(),
+                    )
 
             torch.save(
                 self.mask._optimizer.state_dict(), os.path.join(path, f"mask_optim_epoch{epoch}.pt")
             )
 
             psf_np = self.mask.get_psf().detach().cpu().numpy()[0, ...]
             psf_np = psf_np.squeeze()  # remove (potential) singleton color channel
             np.save(os.path.join(path, f"psf_epoch{epoch}.npy"), psf_np)
-            save_image(psf_np, os.path.join(path, f"psf_epoch{epoch}.png"))
+            fp = os.path.join(path, f"psf_epoch{epoch}.png")
+            save_image(psf_np, fp)
             plot_image(psf_np, gamma=self.gamma)
-            plt.savefig(os.path.join(path, f"psf_epoch{epoch}_plot.png"))
+            fp_plot = os.path.join(path, f"psf_epoch{epoch}_plot.png")
+            plt.savefig(fp_plot)
+
+            if self.use_wandb and epoch != "BEST":
+                wandb.log({"psf": wandb.Image(fp)}, step=epoch)
+                wandb.log({"psf_plot": wandb.Image(fp_plot)}, step=epoch)
+
+            if epoch == "BEST":
+                # save difference with original PSF
+                psf_original = np.load("psf_original.npy")
+                diff = psf_np - psf_original
+                np.save(os.path.join(path, "psf_epochBEST_diff.npy"), diff)
+                diff_abs = np.abs(diff)
+                save_image(diff_abs, os.path.join(path, "psf_epochBEST_diffabs.png"))
+                _, ax = plt.subplots()
+                im = ax.imshow(diff_abs, cmap="gray" if diff_abs.ndim == 2 else None)
+                plt.colorbar(im, ax=ax)
+                ax.set_title("Absolute difference with original PSF")
+                plt.savefig(os.path.join(path, "psf_epochBEST_diffabs_plot.png"))
 
         # save optimizer
         if include_optimizer:
             torch.save(self.optimizer.state_dict(), os.path.join(path, f"optim_epoch{epoch}.pt"))
+
         # save recon
         torch.save(self.recon.state_dict(), os.path.join(path, f"recon_epoch{epoch}"))
```

### Comparing `lensless-1.0.6/lensless/utils/dataset.py` & `lensless-1.0.7/lensless/utils/dataset.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 # dataset.py
 # =================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
 # Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
+from hydra.utils import get_original_cwd
 import numpy as np
 import glob
 import os
 import torch
 from abc import abstractmethod
-from torch.utils.data import Dataset
-from torchvision import transforms
+from torch.utils.data import Dataset, Subset
+from torchvision import datasets, transforms
+from torchvision.transforms import functional as F
+from lensless.hardware.trainable_mask import prep_trainable_mask, AdafruitLCD
 from lensless.utils.simulation import FarFieldSimulator
-from lensless.utils.io import load_image, load_psf
-from lensless.utils.image import resize
+from lensless.utils.io import load_image, load_psf, save_image
+from lensless.utils.image import is_grayscale, resize, rgb2gray
 import re
 from lensless.hardware.utils import capture
 from lensless.hardware.utils import display
 from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
+from datasets import load_dataset
+from huggingface_hub import hf_hub_download
+import cv2
+from lensless.hardware.sensor import sensor_dict, SensorParam
+from scipy.ndimage import rotate
 
 
 def convert(text):
     return int(text) if text.isdigit() else text.lower()
 
 
 def alphanum_key(key):
@@ -150,14 +158,15 @@
         if len(lensless.shape) == 3:
             lensless = lensless.unsqueeze(0)
         if len(lensed.shape) == 3:
             lensed = lensed.unsqueeze(0)
 
         if self.background is not None:
             lensless = lensless - self.background
+            lensless = torch.clamp(lensless, min=0)
 
         # add noise
         if self.input_snr is not None:
             from waveprop.noise import add_shot_noise
 
             lensless = add_shot_noise(lensless, self.input_snr)
 
@@ -845,21 +854,26 @@
         ).all(), "PSF shape should match simulator shape"
         assert (
             not simulator.quantize
         ), "Simulator should not perform quantization to maintain differentiability. Please set quantize=False"
 
         super(SimulatedDatasetTrainableMask, self).__init__(dataset, simulator, **kwargs)
 
-    def _get_images_pair(self, index):
-        # update psf
-        psf = self._mask.get_psf()
-        self.sim.set_point_spread_function(psf)
+    def set_psf(self, psf=None):
+        """
+        Set the PSF of the simulator.
 
-        # return simulated images
-        return super()._get_images_pair(index)
+        Parameters
+        ----------
+        psf : :py:class:`torch.Tensor`, optional
+            PSF to use for the simulation. If ``None``, the PSF of the mask is used.
+        """
+        if psf is None:
+            psf = self._mask.get_psf()
+        self.sim.set_point_spread_function(psf)
 
 
 class HITLDatasetTrainableMask(SimulatedDatasetTrainableMask):
     """
     Dataset of on-the-fly measurements and simulated ground-truth.
     """
 
@@ -942,7 +956,609 @@
 
         # flip image x and y if needed
         if self.capture_config.flip:
             img = torch.rot90(img, dims=(-3, -2), k=2)
 
         # return simulated images (replace simulated with measured)
         return img, lensed
+
+
+class DiffuserCamMirflickrHF(DualDataset):
+    def __init__(
+        self,
+        split,
+        repo_id="bezzam/DiffuserCam-Lensless-Mirflickr-Dataset",
+        psf="psf.tiff",
+        downsample=2,
+        flip_ud=True,
+        dtype="float32",
+        **kwargs,
+    ):
+        """
+        Parameters
+        ----------
+        split : str
+            Split of the dataset to use: 'train', 'test', or 'all'.
+        downsample : int, optional
+            Downsample factor of the PSF, which is 4x the resolution of the images, by default 6 for resolution of (180, 320).
+        flip_ud : bool, optional
+            If True, data is flipped up-down, by default ``True``. Otherwise data is upside-down.
+        """
+
+        # get dataset
+        self.dataset = load_dataset(repo_id, split=split)
+
+        # get PSF
+        psf_fp = hf_hub_download(repo_id=repo_id, filename=psf, repo_type="dataset")
+        psf, bg = load_psf(
+            psf_fp,
+            verbose=False,
+            downsample=downsample * 4,
+            return_bg=True,
+            flip_ud=flip_ud,
+            dtype=dtype,
+            bg_pix=(0, 15),
+        )
+        self.psf = torch.from_numpy(psf)
+
+        super(DiffuserCamMirflickrHF, self).__init__(
+            flip_ud=flip_ud, downsample=downsample, background=bg, **kwargs
+        )
+
+    def __len__(self):
+        return len(self.dataset)
+
+    def _get_images_pair(self, idx):
+        lensless = np.array(self.dataset[idx]["lensless"])
+        lensed = np.array(self.dataset[idx]["lensed"])
+
+        # normalize
+        lensless = lensless.astype(np.float32) / 255
+        lensed = lensed.astype(np.float32) / 255
+
+        return lensless, lensed
+
+
+class HFDataset(DualDataset):
+    def __init__(
+        self,
+        huggingface_repo,
+        split,
+        n_files=None,
+        psf=None,
+        rotate=False,  # just the lensless image
+        downsample=1,
+        downsample_lensed=1,
+        display_res=None,
+        sensor="rpi_hq",
+        slm="adafruit",
+        alignment=None,
+        return_mask_label=False,
+        save_psf=False,
+        simulation_config=dict(),
+        **kwargs,
+    ):
+        """
+        Wrapper for lensless datasets on Hugging Face.
+
+        Parameters
+        ----------
+        huggingface_repo : str
+            Hugging Face repository ID.
+        split : str or :py:class:`torch.utils.data.Dataset`
+            Split of the dataset to use: 'train', 'test', or 'all'. If a Dataset object is given, it is used directly.
+        n_files : int, optional
+            Number of files to load from the dataset, by default None, namely all.
+        psf : str, optional
+            File name of the PSF at the repository. If None, it is assumed that there is a mask pattern from which the PSF is simulated, by default None.
+        rotate : bool, optional
+            If True, lensless images and PSF are rotated 180 degrees. Lensed/original image is not rotated! By default False.
+        downsample : float, optional
+            Downsample factor of the lensless images, by default 1.
+        downsample_lensed : float, optional
+            Downsample factor of the lensed images, by default 1.
+        display_res : tuple, optional
+            Resolution of images when displayed on screen during measurement.
+        sensor : str, optional
+            If `psf` not provided, the sensor to use for the PSF simulation, by default "rpi_hq".
+        slm : str, optional
+            If `psf` not provided, the SLM to use for the PSF simulation, by default "adafruit".
+        alignment : dict, optional
+            Alignment parameters between lensless and lensed data.
+            If "top_left", "height", and "width" are provided, the region-of-interest from the reconstruction of ``lensless`` is extracted and ``lensed`` is reshaped to match.
+            If "crop" is provided, the region-of-interest is extracted from the simulated lensed image, namely a ``simulation`` configuration should be provided within ``alignment``.
+        return_mask_label : bool, optional
+            If multimask dataset, return the mask label (True) or the corresponding PSF (False).
+        save_psf : bool, optional
+            If multimask dataset, save the simulated PSFs.
+        simulation_config : dict, optional
+            Simulation parameters for PSF if using a mask pattern.
+
+        """
+
+        if isinstance(split, str):
+            if n_files is not None:
+                split = f"{split}[0:{n_files}]"
+            self.dataset = load_dataset(huggingface_repo, split=split)
+        elif isinstance(split, Dataset):
+            self.dataset = split
+        else:
+            raise ValueError("split should be a string or a Dataset object")
+
+        self.rotate = rotate
+        self.display_res = display_res
+        self.return_mask_label = return_mask_label
+
+        # deduce downsampling factor from the first image
+        data_0 = self.dataset[0]
+        self.downsample_lensless = downsample
+        self.downsample_lensed = downsample_lensed
+        lensless = np.array(data_0["lensless"])
+        if self.downsample_lensless != 1.0:
+            lensless = resize(lensless, factor=1 / self.downsample_lensless)
+        if psf is None:
+            sensor_res = sensor_dict[sensor][SensorParam.RESOLUTION]
+            downsample_fact = min(sensor_res / lensless.shape[:2])
+        else:
+            downsample_fact = 1
+
+        # deduce recon shape from original image
+        self.alignment = None
+        self.crop = None
+        if alignment is not None:
+            # preparing ground-truth in expected shape
+            if "top_left" in alignment:
+                self.alignment = dict(alignment.copy())
+                self.alignment["top_left"] = (
+                    int(self.alignment["top_left"][0] / downsample),
+                    int(self.alignment["top_left"][1] / downsample),
+                )
+                self.alignment["height"] = int(self.alignment["height"] / downsample)
+
+                original_aspect_ratio = display_res[1] / display_res[0]
+                self.alignment["width"] = int(self.alignment["height"] * original_aspect_ratio)
+
+            # preparing ground-truth as simulated measurement of original
+            elif "crop" in alignment:
+                assert "simulation" in alignment, "Simulation config should be provided"
+                self.crop = dict(alignment["crop"].copy())
+                self.crop["vertical"][0] = int(self.crop["vertical"][0] / downsample)
+                self.crop["vertical"][1] = int(self.crop["vertical"][1] / downsample)
+                self.crop["horizontal"][0] = int(self.crop["horizontal"][0] / downsample)
+                self.crop["horizontal"][1] = int(self.crop["horizontal"][1] / downsample)
+
+        # download all masks
+        # TODO: reshape directly with lensless image shape
+        self.multimask = False
+        if psf is not None:
+            # download PSF from huggingface
+            psf_fp = hf_hub_download(repo_id=huggingface_repo, filename=psf, repo_type="dataset")
+            psf, _ = load_psf(
+                psf_fp,
+                shape=lensless.shape,
+                return_float=True,
+                return_bg=True,
+                flip=rotate,
+                bg_pix=(0, 15),
+            )
+            self.psf = torch.from_numpy(psf)
+
+        elif "mask_label" in data_0:
+            self.multimask = True
+            mask_labels = []
+            for i in range(len(self.dataset)):
+                mask_labels.append(self.dataset[i]["mask_label"])
+            mask_labels = list(set(mask_labels))
+
+            # simulate all PSFs
+            self.psf = dict()
+            for label in mask_labels:
+                mask_fp = hf_hub_download(
+                    repo_id=huggingface_repo,
+                    filename=f"masks/mask_{label}.npy",
+                    repo_type="dataset",
+                )
+                mask_vals = np.load(mask_fp)
+                mask = AdafruitLCD(
+                    initial_vals=torch.from_numpy(mask_vals.astype(np.float32)),
+                    sensor=sensor,
+                    slm=slm,
+                    downsample=downsample_fact,
+                    flipud=rotate,
+                    use_waveprop=simulation_config.get("use_waveprop", False),
+                    scene2mask=simulation_config.get("scene2mask", None),
+                    mask2sensor=simulation_config.get("mask2sensor", None),
+                )
+                self.psf[label] = mask.get_psf().detach()
+
+                assert (
+                    self.psf[label].shape[-3:-1] == lensless.shape[:2]
+                ), f"PSF shape should match lensless shape: PSF {self.psf[label].shape[-3:-1]} vs lensless {lensless.shape[:2]}"
+
+                if save_psf:
+                    # same viewable image of PSF
+                    save_image(self.psf[label].squeeze().cpu().numpy(), f"psf_{label}.png")
+
+        else:
+
+            # single mask pattern
+            mask_fp = hf_hub_download(
+                repo_id=huggingface_repo, filename="mask_pattern.npy", repo_type="dataset"
+            )
+            mask_vals = np.load(mask_fp)
+            mask = AdafruitLCD(
+                initial_vals=torch.from_numpy(mask_vals.astype(np.float32)),
+                sensor=sensor,
+                slm=slm,
+                downsample=downsample_fact,
+                flipud=rotate,
+                use_waveprop=simulation_config.get("use_waveprop", False),
+                scene2mask=simulation_config.get("scene2mask", None),
+                mask2sensor=simulation_config.get("mask2sensor", None),
+            )
+            self.psf = mask.get_psf().detach()
+            assert (
+                self.psf.shape[-3:-1] == lensless.shape[:2]
+            ), "PSF shape should match lensless shape"
+
+            if save_psf:
+                # same viewable image of PSF
+                save_image(self.psf.squeeze().cpu().numpy(), "psf.png")
+
+        # create simulator
+        self.simulator = None
+        self.vertical_shift = None
+        self.horizontal_shift = None
+        if alignment is not None and "simulation" in alignment:
+            simulation_config = dict(alignment["simulation"].copy())
+            simulation_config["output_dim"] = tuple(self.psf.shape[-3:-1])
+            simulator = FarFieldSimulator(
+                is_torch=True,
+                **simulation_config,
+            )
+            self.simulator = simulator
+            if "vertical_shift" in simulation_config:
+                self.vertical_shift = int(simulation_config["vertical_shift"] / downsample)
+            if "horizontal_shift" in simulation_config:
+                self.horizontal_shift = int(simulation_config["horizontal_shift"] / downsample)
+
+        super(HFDataset, self).__init__(**kwargs)
+
+    def __len__(self):
+        return len(self.dataset)
+
+    def _get_images_pair(self, idx):
+
+        # load image
+        lensless_np = np.array(self.dataset[idx]["lensless"])
+        lensed_np = np.array(self.dataset[idx]["lensed"])
+
+        # convert to float
+        if lensless_np.dtype == np.uint8:
+            lensless_np = lensless_np.astype(np.float32) / 255
+            lensed_np = lensed_np.astype(np.float32) / 255
+        else:
+            # 16 bit
+            lensless_np = lensless_np.astype(np.float32) / 65535
+            lensed_np = lensed_np.astype(np.float32) / 65535
+
+        # downsample if necessary
+        if self.downsample_lensless != 1.0:
+            lensless_np = resize(
+                lensless_np, factor=1 / self.downsample_lensless, interpolation=cv2.INTER_NEAREST
+            )
+
+        lensless = lensless_np
+        lensed = lensed_np
+
+        if self.simulator is not None:
+            # convert to torch
+            lensless = torch.from_numpy(lensless_np)
+            lensed = torch.from_numpy(lensed_np)
+
+            # project original image to lensed space
+            with torch.no_grad():
+                lensed = self.simulator.propagate_image(lensed, return_object_plane=True)
+
+            if self.vertical_shift is not None:
+                lensed = torch.roll(lensed, self.vertical_shift, dims=-3)
+            if self.horizontal_shift is not None:
+                lensed = torch.roll(lensed, self.horizontal_shift, dims=-2)
+
+        elif self.alignment is not None:
+            lensed = resize(
+                lensed_np,
+                shape=(self.alignment["height"], self.alignment["width"], 3),
+                interpolation=cv2.INTER_NEAREST,
+            )
+        elif self.display_res is not None:
+            lensed = resize(
+                lensed_np, shape=(*self.display_res, 3), interpolation=cv2.INTER_NEAREST
+            )
+        elif self.downsample_lensed != 1.0:
+            lensed = resize(
+                lensed_np,
+                factor=1 / self.downsample_lensed,
+                interpolation=cv2.INTER_NEAREST,
+            )
+
+        return lensless, lensed
+
+    def __getitem__(self, idx):
+        lensless, lensed = super().__getitem__(idx)
+        if self.rotate:
+            lensless = torch.rot90(lensless, dims=(-3, -2), k=2)
+
+        # return corresponding PSF
+        if self.multimask:
+            mask_label = self.dataset[idx]["mask_label"]
+
+            if self.return_mask_label:
+                return lensless, lensed, mask_label
+            else:
+                return lensless, lensed, self.psf[mask_label]
+        else:
+            return lensless, lensed
+
+    def extract_roi(self, reconstruction, lensed=None, axis=(1, 2)):
+        n_dim = len(reconstruction.shape)
+        assert max(axis) < n_dim, "Axis should be within the dimensions of the reconstruction."
+
+        if self.alignment is not None:
+            top_left = self.alignment["top_left"]
+            height = self.alignment["height"]
+            width = self.alignment["width"]
+
+            # extract according to axis
+            index = [slice(None)] * n_dim
+            index[axis[0]] = slice(top_left[0], top_left[0] + height)
+            index[axis[1]] = slice(top_left[1], top_left[1] + width)
+            reconstruction = reconstruction[tuple(index)]
+
+            # rotate if necessary
+            angle = self.alignment.get("angle", 0)
+            if isinstance(reconstruction, torch.Tensor):
+                reconstruction = F.rotate(reconstruction, angle, expand=False)
+            else:
+                reconstruction = rotate(reconstruction, angle, axes=axis, reshape=False)
+
+        elif self.crop is not None:
+            vertical = self.crop["vertical"]
+            horizontal = self.crop["horizontal"]
+
+            # extract according to axis
+            index = [slice(None)] * n_dim
+            index[axis[0]] = slice(vertical[0], vertical[1])
+            index[axis[1]] = slice(horizontal[0], horizontal[1])
+            reconstruction = reconstruction[tuple(index)]
+            if lensed is not None:
+                lensed = lensed[tuple(index)]
+
+        if self.alignment is None and lensed is not None:
+            return reconstruction, lensed
+        else:
+            return reconstruction
+
+
+def simulate_dataset(config, generator=None):
+    """
+    Prepare datasets for training and testing.
+
+    Parameters
+    ----------
+    config : omegaconf.DictConfig
+        Configuration, e.g. from Hydra. See ``scripts/recon/train_learning_based.py`` for an example that uses this function.
+    generator : torch.Generator, optional
+        Random number generator, by default ``None``.
+    """
+
+    if "cuda" in config.torch_device and torch.cuda.is_available():
+        device = config.torch_device
+    else:
+        device = "cpu"
+
+    # -- prepare PSF
+    psf = None
+    if config.trainable_mask.mask_type is None or config.trainable_mask.initial_value == "psf":
+        psf_fp = os.path.join(get_original_cwd(), config.files.psf)
+        psf, _ = load_psf(
+            psf_fp,
+            downsample=config.files.downsample,
+            return_float=True,
+            return_bg=True,
+            bg_pix=(0, 15),
+        )
+        if config.files.diffusercam_psf:
+            transform_BRG2RGB = transforms.Lambda(lambda x: x[..., [2, 1, 0]])
+            psf = transform_BRG2RGB(torch.from_numpy(psf))
+
+        # drop depth dimension
+        psf = psf.to(device)
+
+    else:
+        # training mask / PSF
+        mask = prep_trainable_mask(config, psf)
+        psf = mask.get_psf().to(device)
+
+    # -- load dataset
+    pre_transform = None
+    transforms_list = [transforms.ToTensor()]
+    data_path = os.path.join(get_original_cwd(), "data")
+    if config.simulation.grayscale:
+        transforms_list.append(transforms.Grayscale())
+
+    if config.files.dataset == "mnist":
+        transform = transforms.Compose(transforms_list)
+        train_ds = datasets.MNIST(root=data_path, train=True, download=True, transform=transform)
+        test_ds = datasets.MNIST(root=data_path, train=False, download=True, transform=transform)
+
+    elif config.files.dataset == "fashion_mnist":
+        transform = transforms.Compose(transforms_list)
+        train_ds = datasets.FashionMNIST(
+            root=data_path, train=True, download=True, transform=transform
+        )
+        test_ds = datasets.FashionMNIST(
+            root=data_path, train=False, download=True, transform=transform
+        )
+    elif config.files.dataset == "cifar10":
+        transform = transforms.Compose(transforms_list)
+        train_ds = datasets.CIFAR10(root=data_path, train=True, download=True, transform=transform)
+        test_ds = datasets.CIFAR10(root=data_path, train=False, download=True, transform=transform)
+
+    elif config.files.dataset == "CelebA":
+        root = config.files.celeba_root
+        data_path = os.path.join(root, "celeba")
+        assert os.path.isdir(
+            data_path
+        ), f"Data path {data_path} does not exist. Make sure you download the CelebA dataset and provide the parent directory as 'config.files.celeba_root'. Download link: https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html"
+        transform = transforms.Compose(transforms_list)
+        if config.files.n_files is None:
+            train_ds = datasets.CelebA(
+                root=root, split="train", download=False, transform=transform
+            )
+            test_ds = datasets.CelebA(root=root, split="test", download=False, transform=transform)
+        else:
+            ds = datasets.CelebA(root=root, split="all", download=False, transform=transform)
+
+            ds = Subset(ds, np.arange(config.files.n_files))
+
+            train_size = int((1 - config.files.test_size) * len(ds))
+            test_size = len(ds) - train_size
+            train_ds, test_ds = torch.utils.data.random_split(
+                ds, [train_size, test_size], generator=generator
+            )
+    else:
+        raise NotImplementedError(f"Dataset {config.files.dataset} not implemented.")
+
+    if config.files.dataset != "CelebA":
+        if config.files.n_files is not None:
+            train_size = int((1 - config.files.test_size) * config.files.n_files)
+            test_size = config.files.n_files - train_size
+            train_ds = Subset(train_ds, np.arange(train_size))
+            test_ds = Subset(test_ds, np.arange(test_size))
+
+    # convert PSF
+    if config.simulation.grayscale and not is_grayscale(psf):
+        psf = rgb2gray(psf)
+
+    # check if gpu is available
+    device_conv = config.torch_device
+    if device_conv == "cuda" and torch.cuda.is_available():
+        device_conv = "cuda"
+    else:
+        device_conv = "cpu"
+
+    # create simulator
+    simulator = FarFieldSimulator(
+        psf=psf,
+        is_torch=True,
+        **config.simulation,
+    )
+
+    # create Pytorch dataset and dataloader
+    crop = config.files.crop.copy() if config.files.crop is not None else None
+    if mask is None:
+        train_ds_prop = SimulatedFarFieldDataset(
+            dataset=train_ds,
+            simulator=simulator,
+            dataset_is_CHW=True,
+            device_conv=device_conv,
+            flip=config.simulation.flip,
+            vertical_shift=config.files.vertical_shift,
+            horizontal_shift=config.files.horizontal_shift,
+            crop=crop,
+            downsample=config.files.downsample,
+            pre_transform=pre_transform,
+        )
+        test_ds_prop = SimulatedFarFieldDataset(
+            dataset=test_ds,
+            simulator=simulator,
+            dataset_is_CHW=True,
+            device_conv=device_conv,
+            flip=config.simulation.flip,
+            vertical_shift=config.files.vertical_shift,
+            horizontal_shift=config.files.horizontal_shift,
+            crop=crop,
+            downsample=config.files.downsample,
+            pre_transform=pre_transform,
+        )
+    else:
+        if config.measure is not None:
+
+            train_ds_prop = HITLDatasetTrainableMask(
+                rpi_username=config.measure.rpi_username,
+                rpi_hostname=config.measure.rpi_hostname,
+                celeba_root=config.files.celeba_root,
+                display_config=config.measure.display,
+                capture_config=config.measure.capture,
+                mask_center=config.trainable_mask.ap_center,
+                dataset=train_ds,
+                mask=mask,
+                simulator=simulator,
+                dataset_is_CHW=True,
+                device_conv=device_conv,
+                flip=config.simulation.flip,
+                vertical_shift=config.files.vertical_shift,
+                horizontal_shift=config.files.horizontal_shift,
+                crop=crop,
+                downsample=config.files.downsample,
+                pre_transform=pre_transform,
+            )
+
+            test_ds_prop = HITLDatasetTrainableMask(
+                rpi_username=config.measure.rpi_username,
+                rpi_hostname=config.measure.rpi_hostname,
+                celeba_root=config.files.celeba_root,
+                display_config=config.measure.display,
+                capture_config=config.measure.capture,
+                mask_center=config.trainable_mask.ap_center,
+                dataset=test_ds,
+                mask=mask,
+                simulator=simulator,
+                dataset_is_CHW=True,
+                device_conv=device_conv,
+                flip=config.simulation.flip,
+                vertical_shift=config.files.vertical_shift,
+                horizontal_shift=config.files.horizontal_shift,
+                crop=crop,
+                downsample=config.files.downsample,
+                pre_transform=pre_transform,
+            )
+
+        else:
+
+            train_ds_prop = SimulatedDatasetTrainableMask(
+                dataset=train_ds,
+                mask=mask,
+                simulator=simulator,
+                dataset_is_CHW=True,
+                device_conv=device_conv,
+                flip=config.simulation.flip,
+                vertical_shift=config.files.vertical_shift,
+                horizontal_shift=config.files.horizontal_shift,
+                crop=crop,
+                downsample=config.files.downsample,
+                pre_transform=pre_transform,
+            )
+            test_ds_prop = SimulatedDatasetTrainableMask(
+                dataset=test_ds,
+                mask=mask,
+                simulator=simulator,
+                dataset_is_CHW=True,
+                device_conv=device_conv,
+                flip=config.simulation.flip,
+                vertical_shift=config.files.vertical_shift,
+                horizontal_shift=config.files.horizontal_shift,
+                crop=crop,
+                downsample=config.files.downsample,
+                pre_transform=pre_transform,
+            )
+
+    return train_ds_prop, test_ds_prop, mask
+
+
+class MyDataParallel(torch.nn.DataParallel):
+    def __getattr__(self, name):
+        try:
+            return super().__getattr__(name)
+        except AttributeError:
+            return getattr(self.module, name)
```

### Comparing `lensless-1.0.6/lensless/utils/image.py` & `lensless-1.0.7/lensless/utils/image.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless/utils/io.py` & `lensless-1.0.7/lensless/utils/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     as_4d=False,
     downsample=None,
     bg=None,
     return_float=False,
     shape=None,
     dtype=None,
     normalize=True,
+    bgr_input=True,
 ):
     """
     Load image as numpy array.
 
     Parameters
     ----------
     fp : str
@@ -147,15 +148,15 @@
             red_gain=red_gain,
             black_level=black_level,
             ccm=ccm,
             nbits_out=nbits_out,
         )
 
     else:
-        if len(img.shape) == 3:
+        if len(img.shape) == 3 and bgr_input:
             img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
     original_dtype = img.dtype
 
     if flip:
         img = np.flipud(img)
         img = np.fliplr(img)
@@ -219,14 +220,15 @@
     blue_gain=None,
     red_gain=None,
     dtype=np.float32,
     nbits_out=None,
     single_psf=False,
     shape=None,
     use_3d=False,
+    bgr_input=True,
 ):
     """
     Load and process PSF for analysis or for reconstruction.
 
     Basic steps are:
     * Load image.
     * (Optionally) subtract background. Recommended.
@@ -292,14 +294,15 @@
             flip=flip,
             flip_ud=flip_ud,
             flip_lr=flip_lr,
             bayer=bayer,
             blue_gain=blue_gain,
             red_gain=red_gain,
             nbits_out=nbits_out,
+            bgr_input=bgr_input,
         )
 
     original_dtype = psf.dtype
     max_val = get_max_val(psf)
     psf = np.array(psf, dtype=dtype)
 
     if use_3d:
@@ -341,15 +344,15 @@
                 psf[:, :, :, i] -= bg_i
                 bg.append(bg_i)
 
         psf = np.clip(psf, a_min=0, a_max=psf.max())
         bg = np.array(bg)
 
     # resize
-    if downsample != 1:
+    if downsample != 1 or shape is not None:
         psf = resize(psf, shape=shape, factor=1 / downsample)
 
     if single_psf:
         if not grayscale:
             # TODO : in Lensless Learning, they sum channels --> `psf_diffuser = np.sum(psf_diffuser,2)`
             # https://github.com/Waller-Lab/LenslessLearning/blob/master/pre-trained%20reconstructions.ipynb
             psf = np.sum(psf, axis=3)
@@ -376,25 +379,28 @@
     psf_fp,
     data_fp,
     return_float=True,
     downsample=None,
     bg_pix=(5, 25),
     plot=True,
     flip=False,
+    flip_ud=False,
+    flip_lr=False,
     bayer=False,
     blue_gain=None,
     red_gain=None,
     gamma=None,
     gray=False,
     dtype=None,
     single_psf=False,
     shape=None,
-    torch=False,
+    use_torch=False,
     torch_device="cpu",
     normalize=False,
+    bgr_input=True,
 ):
     """
     Load data for image reconstruction.
 
     Parameters
     ----------
     psf_fp : str
@@ -460,35 +466,41 @@
     psf, bg = load_psf(
         psf_fp,
         downsample=downsample,
         return_float=return_float,
         bg_pix=bg_pix,
         return_bg=True,
         flip=flip,
+        flip_ud=flip_ud,
+        flip_lr=flip_lr,
         bayer=bayer,
         blue_gain=blue_gain,
         red_gain=red_gain,
         dtype=dtype,
         single_psf=single_psf,
         shape=shape,
         use_3d=use_3d,
+        bgr_input=bgr_input,
     )
 
     # load and process raw measurement
     data = load_image(
         data_fp,
         flip=flip,
+        flip_ud=flip_ud,
+        flip_lr=flip_lr,
         bayer=bayer,
         blue_gain=blue_gain,
         red_gain=red_gain,
         bg=bg,
         as_4d=True,
         return_float=return_float,
         shape=shape,
         normalize=normalize,
+        bgr_input=bgr_input,
     )
 
     if data.shape != psf.shape:
         # in DiffuserCam dataset, images are already reshaped
         data = resize(data, shape=psf.shape)
 
     if data.shape[3] > 1 and psf.shape[3] == 1:
@@ -518,15 +530,15 @@
         ax = plot_image(psf[0], gamma=gamma)
         ax.set_title("PSF of the first depth")
         ax = plot_image(data[0], gamma=gamma)
         ax.set_title("Raw data")
 
     psf = np.array(psf, dtype=dtype)
     data = np.array(data, dtype=dtype)
-    if torch:
+    if use_torch:
         import torch
 
         if dtype == np.float32:
             torch_dtype = torch.float32
         elif dtype == np.float64:
             torch_dtype = torch.float64
 
@@ -543,20 +555,34 @@
 
     if img_tmp.dtype == np.uint16 or img_tmp.dtype == np.uint8:
         img_tmp = img_tmp.astype(np.float32)
 
     if normalize:
         img_tmp -= img_tmp.min()
         img_tmp /= img_tmp.max()
+    else:
+        normalized = False
+        if img_tmp.min() < 0:
+            img_tmp -= img_tmp.min()
+            normalize = True
+        if img_tmp.max() > 1:
+            img_tmp /= img_tmp.max()
+            normalize = True
+        if normalized:
+            print(f"Warning (out of range): {fp} normalizing data to [0, 1]")
 
     if img_tmp.dtype == np.float64 or img_tmp.dtype == np.float32:
         img_tmp *= max_val
         img_tmp = img_tmp.astype(np.uint8)
 
-    img_tmp = Image.fromarray(img_tmp)
+    # RGB
+    if len(img_tmp.shape) == 3 and img_tmp.shape[2] == 3:
+        img_tmp = Image.fromarray(img_tmp)
+    else:
+        img_tmp = Image.fromarray(img_tmp.squeeze())
     img_tmp.save(fp)
 
 
 def get_dtype(dtype=None, is_torch=False):
     """
     Get dtype for numpy or torch.
```

### Comparing `lensless-1.0.6/lensless/utils/plot.py` & `lensless-1.0.7/lensless/utils/plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 # Julien SAHLI [julien.sahli@epfl.ch]
 # #############################################################################
 
 
 import numpy as np
 import warnings
 import matplotlib.pyplot as plt
+import os
+import json
 
 from lensless.utils.image import FLOAT_DTYPES, get_max_val, gamma_correction, autocorr2d
 
 
 def plot_image(img, ax=None, gamma=None, normalize=True):
     """
     Plot image data.
@@ -282,7 +284,78 @@
 
     if ax is None:
         _, ax = plt.subplots()
 
     ax.imshow(autocorr_img, cmap="gray", vmin=0, vmax=max_val_plot)
     ax.axis("off")
     return ax, autocorr
+
+
+def compare_models(model_paths, max_epoch=None, linewidth=2, fontsize=18, metrics=None):
+    """
+    Plot train and test loss for multiple models, and print metrics for best epoch.
+
+    Parameters
+    ----------
+    model_paths : dict
+        Dictionary of model names and their paths.
+    max_epoch : int, optional
+        Maximum epoch to plot. Default is None.
+    linewidth : int, optional
+        Line width for plot. Default is 2.
+    fontsize : int, optional
+        Font size for plot. Default is 18.
+    metrics : list, optional
+        List of metrics to print. Default is ["PSNR", "SSIM", "LPIPS_Vgg"].
+    """
+
+    if metrics is None:
+        metrics = ["PSNR", "SSIM", "LPIPS_Vgg"]
+
+    # plot train and test loss
+    import matplotlib.colors as mcolors
+
+    plot_colors = list(mcolors.TABLEAU_COLORS.keys())
+
+    _, ax = plt.subplots()
+    for model in model_paths:
+        model_path = model_paths[model]
+        _metrics_path = os.path.join(model_path, "metrics.json")
+
+        assert os.path.exists(_metrics_path), f"Path {_metrics_path} does not exist"
+        _test_metrics = json.load(open(_metrics_path))
+
+        color = plot_colors.pop()
+        train_loss = np.array(_test_metrics["LOSS"])
+        if max_epoch is not None:
+            train_loss = train_loss[: max_epoch + 1]
+        ax.plot(
+            train_loss, label=model + " (train)", color=color, linestyle="--", linewidth=linewidth
+        )
+
+        test_loss = np.array(_test_metrics["MSE"]) + np.array(_test_metrics["LPIPS_Vgg"])
+        if max_epoch is not None:
+            test_loss = test_loss[: max_epoch + 1]
+        ax.plot(test_loss, label=model + " (test)", linestyle="-", color=color, linewidth=linewidth)
+
+        # best_epoch = np.argmin(test_loss)
+        best_epoch = _test_metrics["best_epoch"]
+        print(f"\n-- {model} --")
+        print(f"Best epoch for {model}: {best_epoch} / {len(test_loss)-1}")
+        print(f"Best test loss for {model}: {test_loss[best_epoch]}")
+        # print metrics
+        for _metric in metrics:
+            print(f"{_metric}: {np.array(_test_metrics[_metric])[best_epoch]:.3}")
+
+    # set font size
+    ax.tick_params(axis="both", which="major", labelsize=fontsize)
+    ax.set_xlabel("Epoch", fontsize=fontsize)
+    ax.set_title("Train-test loss", fontsize=fontsize)
+
+    # legend outside
+    ax.legend(loc="upper right", fontsize=fontsize)
+    # ax.set_ylim([0.4, 1]);
+    if max_epoch is not None:
+        ax.set_xlim([0, max_epoch])
+
+    ax.grid()
+    return ax
```

### Comparing `lensless-1.0.6/lensless/utils/simulation.py` & `lensless-1.0.7/lensless/utils/simulation.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/lensless.egg-info/SOURCES.txt` & `lensless-1.0.7/lensless.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 lensless.egg-info/top_level.txt
 lensless/eval/__init__.py
 lensless/eval/benchmark.py
 lensless/eval/metric.py
 lensless/hardware/__init__.py
 lensless/hardware/aperture.py
 lensless/hardware/constants.py
+lensless/hardware/fabrication.py
 lensless/hardware/mask.py
 lensless/hardware/sensor.py
 lensless/hardware/slm.py
 lensless/hardware/trainable_mask.py
 lensless/hardware/utils.py
 lensless/recon/__init__.py
 lensless/recon/admm.py
-lensless/recon/admm_pnp.py
 lensless/recon/apgd.py
 lensless/recon/gd.py
 lensless/recon/mirflickr.py
 lensless/recon/model_dict.py
 lensless/recon/recon.py
 lensless/recon/rfft_convolve.py
 lensless/recon/tikhonov.py
@@ -40,55 +40,54 @@
 lensless/recon/drunet/network_unet.py
 lensless/utils/__init__.py
 lensless/utils/dataset.py
 lensless/utils/image.py
 lensless/utils/io.py
 lensless/utils/plot.py
 lensless/utils/simulation.py
+notebooks/test_kc_dataset.py
 profile/admm.py
 profile/diffusercam_admm.py
 profile/diffusercam_gd.py
 profile/gradient_descent.py
 scripts/demo.py
 scripts/classify/train_celeba_vit.py
-scripts/data/16bit_image.py
-scripts/data/download_diffusercam_huggingface.py
+scripts/data/authenticate.py
+scripts/data/authenticate_roc.py
 scripts/data/prepare_mirflickr_subset.py
+scripts/data/rename_mirflickr25k.py
+scripts/data/upload_dataset_huggingface.py
 scripts/data/upload_diffusercam_huggingface.py
 scripts/data/3d/mat_to_npy.py
 scripts/data/3d/mat_to_npz.py
 scripts/data/3d/npy_to_obj.py
 scripts/data/3d/npy_to_tiff.py
 scripts/demo/telegram_bot.py
 scripts/eval/benchmark_recon.py
 scripts/eval/compute_metrics_from_original.py
-scripts/eval/mirflickr_admm.py
 scripts/hardware/config_digicam.py
 scripts/hardware/digicam_measure_psfs.py
 scripts/hardware/set_digicam_mask_distance.py
 scripts/measure/analyze_image.py
 scripts/measure/analyze_measured_dataset.py
 scripts/measure/collect_dataset_on_device.py
-scripts/measure/collect_mnist.py
-scripts/measure/collect_mnist_on_device.py
-scripts/measure/compare_measured_original.py
-scripts/measure/digicam_capture.py
-scripts/measure/digicam_example.py
 scripts/measure/on_device_capture.py
 scripts/measure/prep_display_image.py
 scripts/measure/remote_capture.py
 scripts/measure/remote_display.py
 scripts/recon/admm.py
-scripts/recon/admm_mirflickr.py
 scripts/recon/apgd_pycsou.py
 scripts/recon/dataset.py
 scripts/recon/demo.py
 scripts/recon/diffusercam_mirflickr.py
+scripts/recon/digicam_mirflickr.py
 scripts/recon/gradient_descent.py
-scripts/recon/train_unrolled.py
+scripts/recon/mirflickr_hugging_face.py
+scripts/recon/recon_miniset.py
+scripts/recon/train_learning_based.py
 scripts/sim/dataset.py
 scripts/sim/digicam_psf.py
 scripts/sim/mask_dataset.py
 scripts/sim/mask_single_file.py
 scripts/sim/single_file.py
 scripts/sim/torch_custom_dataset.py
 scripts/sim/torch_dataset.py
```

### Comparing `lensless-1.0.6/profile/admm.py` & `lensless-1.0.7/profile/admm.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 psf, data = load_data(
     psf_fp=psf_fp,
     data_fp=data_fp,
     downsample=downsample,
     plot=False,
     gray=gray,
     dtype=dtype,
-    torch=True,
+    use_torch=True,
 )
 
 recon = ADMM(psf, dtype=dtype)
 recon.set_data(data)
 res = recon.apply(n_iter=n_iter, save=save, disp_iter=None, plot=False)
 recon.reset()
 total_time = 0
@@ -87,15 +87,15 @@
 psf, data = load_data(
     psf_fp=psf_fp,
     data_fp=data_fp,
     downsample=downsample,
     plot=False,
     gray=gray,
     dtype=dtype,
-    torch=True,
+    use_torch=True,
     torch_device="cuda",
 )
 
 recon = ADMM(psf, dtype=dtype)
 recon.set_data(data)
 res = recon.apply(n_iter=n_iter, save=save, disp_iter=None, plot=False)
 recon.reset()
```

### Comparing `lensless-1.0.6/profile/diffusercam_admm.py` & `lensless-1.0.7/profile/diffusercam_admm.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/profile/diffusercam_gd.py` & `lensless-1.0.7/profile/diffusercam_gd.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/profile/gradient_descent.py` & `lensless-1.0.7/profile/gradient_descent.py`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 psf, data = load_data(
     psf_fp=psf_fp,
     data_fp=data_fp,
     downsample=downsample,
     plot=False,
     gray=gray,
     dtype=dtype,
-    torch=True,
+    use_torch=True,
 )
 
 recon = FISTA(psf, dtype=dtype)
 recon.set_data(data)
 res = recon.apply(n_iter=n_iter, save=save, disp_iter=None, plot=False)
 recon.reset()
 total_time = 0
@@ -116,15 +116,15 @@
 psf, data = load_data(
     psf_fp=psf_fp,
     data_fp=data_fp,
     downsample=downsample,
     plot=False,
     gray=gray,
     dtype=dtype,
-    torch=True,
+    use_torch=True,
     torch_device="cuda",
 )
 
 recon = FISTA(psf, dtype=dtype)
 recon.set_data(data)
 res = recon.apply(n_iter=n_iter, save=save, disp_iter=None, plot=False)
 recon.reset()
```

### Comparing `lensless-1.0.6/scripts/classify/train_celeba_vit.py` & `lensless-1.0.7/scripts/classify/train_celeba_vit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Fine-tune ViT on CelebA dataset measured with lensless camera.
 Original tutorial: https://huggingface.co/blog/fine-tune-vit
 
 First, set-up HuggingFace libraries:
 ```
-pip install datasets transformers
+pip install datasets transformers[torch] scikit-learn tensorboardX
 ```
 
 Raw measurement datasets can be download from SwitchDrive.
 This will be done by the script if the dataset is not found.
 ```
 # 10K measurements (13.1 GB)
 python scripts/classify/train_celeba_vit.py \
@@ -38,14 +38,16 @@
 input.raw_data=path/to/raw/data \
 preprocess.data_dim=[48,64]
 ```
 
 Other hyperparameters for classification can be found in
 `configs/train_celeba_classifier.yaml`.
 
+# TODO: update with Hugging Face dataset: https://huggingface.co/datasets/bezzam/DigiCam-CelebA-10K
+
 """
 
 import warnings
 from transformers import ViTImageProcessor, ViTForImageClassification
 from transformers import TrainingArguments, Trainer, TrainerCallback
 import numpy as np
 import torch
@@ -193,27 +195,21 @@
         _train_transforms.append(
             RandomResizedCrop(
                 size,
                 scale=(0.9, 1.0),
                 ratio=(0.9, 1.1),
             )
         )
-    _train_transforms.append(
-        Resize(size),
-        CenterCrop(size),
-    )
+    _train_transforms += [Resize(size), CenterCrop(size)]
     if config.augmentation.horizontal_flip:
         if config.data.raw:
             warnings.warn("Horizontal flip is not supported for raw data, Skipping!")
         else:
             _train_transforms.append(RandomHorizontalFlip())
-    _train_transforms.append(
-        ToTensor(),
-        normalize,
-    )
+    _train_transforms += [ToTensor(), normalize]
     _train_transforms = Compose(_train_transforms)
 
     _val_transforms = Compose(
         [
             Resize(size),
             CenterCrop(size),
             ToTensor(),
```

### Comparing `lensless-1.0.6/scripts/data/3d/mat_to_npy.py` & `lensless-1.0.7/scripts/data/3d/mat_to_npy.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/data/3d/mat_to_npz.py` & `lensless-1.0.7/scripts/data/3d/mat_to_npz.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/data/3d/npy_to_obj.py` & `lensless-1.0.7/scripts/data/3d/npy_to_obj.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/data/3d/npy_to_tiff.py` & `lensless-1.0.7/scripts/data/3d/npy_to_tiff.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/data/prepare_mirflickr_subset.py` & `lensless-1.0.7/scripts/data/prepare_mirflickr_subset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/data/upload_diffusercam_huggingface.py` & `lensless-1.0.7/scripts/data/upload_diffusercam_huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 Push DiffuserCam dataset to HuggingFace.
 
 ```bash
 # install
 pip install datasets
 pip install huggingface_hub
 pip install joblib
+pip install git+https://github.com/pvigier/perlin-numpy.git@5e26837db14042e51166eb6cad4c0df2c1907016
+pip install git+https://github.com/ebezzam/slm-controller.git
 
 # make a write token on HuggingFace
 
 # run
 python scripts/data/upload_diffusercam_huggingface.py \
 hf_token=... \
 ```
@@ -39,15 +41,15 @@
     dir_diffuser = config.dir_diffuser
     dir_lensed = config.dir_lensed
     psf_fp = config.psf_fp
     hf_token = config.hf_token
     file_ext = config.file_ext
     n_files = config.n_files
     n_jobs = config.n_jobs
-    normalize = False
+    normalize = config.normalize
 
     assert hf_token is not None, "Please provide a HuggingFace token."
 
     start_time = time.time()
 
     # get all lensless-lensed pairs
     files_diffuser = glob.glob(os.path.join(dir_diffuser, "*" + file_ext))
```

### Comparing `lensless-1.0.6/scripts/demo/telegram_bot.py` & `lensless-1.0.7/scripts/demo/telegram_bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 import os
 from PIL import Image, ImageFont
 import shutil
 import pytz
 from datetime import datetime
 from lensless.hardware.utils import check_username_hostname
+from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
 
 # for displaying emojis
 from emoji import EMOJI_DATA
 from lensless.utils.io import load_psf
 from pilmoji import Pilmoji
 
 from telegram import __version__ as TG_VER
@@ -47,32 +48,35 @@
 RPI_USERNAME = None
 RPI_HOSTNAME = None
 RPI_LENSED_USERNAME = None
 RPI_LENSED_HOSTNAME = None
 CONFIG_FN = None
 DEFAULT_ALGO = None
 ALGO_TEXT = None
+MASK_PARAM = None
 
 
 OVERLAY_ALPHA = None
 OVERLAY_1 = None
 OVERLAY_2 = None
 OVERLAY_3 = None
 
 SETUP_FP = "scripts/demo/setup.png"
 INPUT_FP = "user_photo.jpg"
 RAW_DATA_FP = "raw_data.png"
 OUTPUT_FOLDER = "demo_lensless"
 BUSY = False
-supported_algos = ["fista", "admm", "unrolled"]
+# supported_algos = ["fista", "admm", "unrolled"]
+supported_algos = ["fista", "admm"]
 supported_input = ["mnist", "thumb", "face"]
 TIMEOUT = 1 * 60  # 10 minutes
 
 BRIGHTNESS = 100
-EXPOSURE = 0.02
+# EXPOSURE = 0.02
+EXPOSURE = 0.5
 LOW_LIGHT_THRESHOLD = 100
 SATURATION_THRESHOLD = 0.05
 
 PSF_FP = None
 PSF_FP_GAMMA = os.path.join(OUTPUT_FOLDER, "psf_gamma.png")
 BACKGROUND_FP = None
 
@@ -113,15 +117,55 @@
 async def check_incoming_message(update: Update, context: ContextTypes.DEFAULT_TYPE):
 
     global BUSY, queries_count
 
     # create folder for user
     user_folder = get_user_folder(update)
     if not os.path.exists(user_folder):
-        os.makedirs(user_folder)
+        os.makedirs(user_folder, exist_ok=True)
+
+        if MASK_PARAM is not None:
+
+            import torch
+            from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
+            from lensless.hardware.trainable_mask import AdafruitLCD
+            from lensless.utils.io import save_image
+
+            user_id = int(os.path.basename(user_folder))
+            np.random.seed(user_id % (2**32 - 1))  # TODO set user ID as seed
+            mask_vals = np.random.uniform(0, 1, MASK_PARAM.mask_shape)
+
+            # simulate PSF
+            full_pattern = adafruit_sub2full(
+                mask_vals,
+                center=MASK_PARAM.mask_center,
+            )
+            set_programmable_mask(
+                full_pattern,
+                device=MASK_PARAM.device,
+                rpi_username=RPI_USERNAME,
+                rpi_hostname=RPI_HOSTNAME,
+            )
+            mask_vals_torch = torch.from_numpy(mask_vals.astype(np.float32))
+            mask = AdafruitLCD(
+                initial_vals=mask_vals_torch,
+                sensor=MASK_PARAM.sensor,
+                slm=MASK_PARAM.device,
+                downsample=MASK_PARAM.downsample,
+                flipud=MASK_PARAM.flipud,
+            )
+            psf = mask.get_psf().detach().numpy()
+
+            # save PSF as PNG
+            psf_fp = os.path.join(user_folder, "psf.png")
+            save_image(psf[0], psf_fp)
+
+            # save as NPY
+            psf_npy_fp = os.path.join(user_folder, "psf.npy")
+            np.save(psf_npy_fp, psf)
 
     if BUSY:
         return "System is busy. Please wait for the current job to finish and try again."
 
     # if message from a while ago, ignore
     utc = pytz.UTC
     now = utc.localize(datetime.now())
@@ -228,14 +272,17 @@
     4. Reconstruct
     """
 
     global BUSY, EXPOSURE
 
     # EXPOSURE = 0.02
 
+    vshift = -26
+    pad = 10
+
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     algo = update.message.caption
     if algo is not None:
@@ -248,15 +295,15 @@
         # # call python script for full process
         # os.system(f"python scripts/demo.py plot=False fp={INPUT_FP} output={OUTPUT_FOLDER}")
 
         # -- send to display
         user_folder = get_user_folder(update)
         original_file_path = os.path.join(user_folder, INPUT_FP)
         os.system(
-            f"python scripts/measure/remote_display.py -cn {CONFIG_FN} fp={original_file_path} rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME}"
+            f"python scripts/measure/remote_display.py -cn {CONFIG_FN} fp={original_file_path} rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME} display.pad={pad} display.vshift={vshift}"
         )
         await update.message.reply_text(
             "Image sent to display.", reply_to_message_id=update.message.message_id
         )
 
         await take_picture_and_reconstruct(update, context, algo)
 
@@ -287,14 +334,121 @@
         )
 
     os.system(
         f"python scripts/measure/remote_capture.py -cn {CONFIG_FN} plot=False rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME} output={user_subfolder} capture.exp={EXPOSURE}"
     )
 
 
+def overlay(user_subfolder):
+
+    if OVERLAY_1 is not None or OVERLAY_2 is not None or OVERLAY_3 is not None:
+
+        alpha = OVERLAY_ALPHA
+
+        reconstructed_path = os.path.join(user_subfolder, "reconstructed.png")
+
+        img1 = Image.open(reconstructed_path)
+        img1 = img1.convert("RGBA")
+
+        for overlay_config in [OVERLAY_1, OVERLAY_2, OVERLAY_3]:
+            if overlay_config is not None:
+                overlay_img = Image.open(overlay_config.fp)
+                overlay_img = overlay_img.convert("RGBA")
+                overlay_img.putalpha(alpha)
+                new_width = int(img1.width * overlay_config.scaling)
+                overlay_img = overlay_img.resize(
+                    (new_width, int(new_width * overlay_img.height / overlay_img.width))
+                )
+                img1.paste(
+                    overlay_img,
+                    (overlay_config.position[0], overlay_config.position[1]),
+                    overlay_img,
+                )
+
+        OUTPUT_FP = os.path.join(user_subfolder, "reconstructed_overlay.png")
+        img1.convert("RGB").save(OUTPUT_FP)
+
+    else:
+
+        OUTPUT_FP = os.path.join(user_subfolder, "reconstructed.png")
+
+    return OUTPUT_FP
+
+
+async def random_mask(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
+    """
+    Set random mask and reconstruct (with ADMM).
+    """
+
+    algo = "admm"
+
+    # get user subfolder
+    user_subfolder = get_user_folder(update)
+
+    # get seed for random mask
+    seed = int(os.path.basename(user_subfolder))
+    # add random number to seed
+    seed += np.random.randint(0, 1000)
+    os.system(
+        f"python scripts/recon/demo.py -cn {CONFIG_FN} plot=False recon.algo={algo} output={user_subfolder} camera.psf.seed={seed}"
+    )
+
+    # -- send back, with watermark if provided
+    OUTPUT_FP = overlay(user_subfolder)
+    await update.message.reply_photo(
+        OUTPUT_FP,
+        caption=f"Reconstruction ({algo})",
+        reply_to_message_id=update.message.message_id,
+    )
+
+    # simulate BAD PSF
+    import torch
+    from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
+    from lensless.hardware.trainable_mask import AdafruitLCD
+    from lensless.utils.io import save_image
+
+    np.random.seed(seed % (2**32 - 1))
+    mask_vals = np.random.uniform(0, 1, MASK_PARAM.mask_shape)
+
+    # simulate PSF
+    full_pattern = adafruit_sub2full(
+        mask_vals,
+        center=MASK_PARAM.mask_center,
+    )
+    set_programmable_mask(
+        full_pattern, device=MASK_PARAM.device, rpi_username=RPI_USERNAME, rpi_hostname=RPI_HOSTNAME
+    )
+    mask_vals_torch = torch.from_numpy(mask_vals.astype(np.float32))
+    mask = AdafruitLCD(
+        initial_vals=mask_vals_torch,
+        sensor=MASK_PARAM.sensor,
+        slm=MASK_PARAM.device,
+        downsample=MASK_PARAM.downsample,
+        flipud=MASK_PARAM.flipud,
+    )
+    psf = mask.get_psf().detach().numpy()
+
+    # save PSF as PNG
+    psf_fp = os.path.join(user_subfolder, "psf_bad.png")
+    save_image(psf[0], psf_fp)
+    await update.message.reply_photo(
+        psf_fp,
+        caption="Incorrect PSF used for reconstruction",
+        reply_to_message_id=update.message.message_id,
+    )
+
+    # send back false and ground truth PSF
+    psf_fp = os.path.join(user_subfolder, "psf.png")
+    await update.message.reply_photo(
+        psf_fp,
+        caption="Correct PSF (your key)",
+        reply_to_message_id=update.message.message_id,
+    )
+
+
 async def reconstruct(update: Update, context: ContextTypes.DEFAULT_TYPE, algo, query=None) -> None:
 
     supported = check_algo(algo)
     if not supported:
         await update.message.reply_text(
             f"Unsupported algorithm: {algo}. Please specify from: {supported_algos}",
             reply_to_message_id=update.message.message_id,
@@ -321,74 +475,64 @@
     await update.message.reply_text(
         f"Reconstructing with {algo}...", reply_to_message_id=update.message.message_id
     )
     if PSF_FP is not None:
         os.system(
             f"python scripts/recon/demo.py -cn {CONFIG_FN} plot=False recon.algo={algo} output={user_subfolder} camera.psf={PSF_FP} recon.downsample=1 camera.background={BACKGROUND_FP}"
         )
+    elif MASK_PARAM is not None:
+        # get seed for random mask
+        seed = int(os.path.basename(user_subfolder))
+        os.system(
+            f"python scripts/recon/demo.py -cn {CONFIG_FN} plot=False recon.algo={algo} output={user_subfolder} camera.psf.seed={seed}"
+        )
     else:
         os.system(
             f"python scripts/recon/demo.py -cn {CONFIG_FN} plot=False recon.algo={algo} output={user_subfolder}"
         )
 
     # -- send back, with watermark if provided
-    if OVERLAY_1 is not None or OVERLAY_2 is not None or OVERLAY_3 is not None:
-
-        alpha = OVERLAY_ALPHA
-
-        reconstructed_path = os.path.join(user_subfolder, "reconstructed.png")
-
-        img1 = Image.open(reconstructed_path)
-        img1 = img1.convert("RGBA")
-
-        for overlay_config in [OVERLAY_1, OVERLAY_2, OVERLAY_3]:
-            if overlay_config is not None:
-                overlay_img = Image.open(overlay_config.fp)
-                overlay_img = overlay_img.convert("RGBA")
-                overlay_img.putalpha(alpha)
-                new_width = int(img1.width * overlay_config.scaling)
-                overlay_img = overlay_img.resize(
-                    (new_width, int(new_width * overlay_img.height / overlay_img.width))
-                )
-                img1.paste(
-                    overlay_img,
-                    (overlay_config.position[0], overlay_config.position[1]),
-                    overlay_img,
-                )
-
-        OUTPUT_FP = os.path.join(user_subfolder, "reconstructed_overlay.png")
-        img1.convert("RGB").save(OUTPUT_FP)
-
-        # return photo
-        await update.message.reply_photo(
-            OUTPUT_FP,
-            caption=f"Reconstruction ({algo})",
-            reply_to_message_id=update.message.message_id,
-        )
-
-    else:
-        OUTPUT_FP = os.path.join(user_subfolder, "reconstructed.png")
-        await update.message.reply_photo(
-            OUTPUT_FP,
-            caption=f"Reconstruction ({algo})",
-            reply_to_message_id=update.message.message_id,
-        )
+    OUTPUT_FP = overlay(user_subfolder)
+    await update.message.reply_photo(
+        OUTPUT_FP,
+        caption=f"Reconstruction ({algo})",
+        reply_to_message_id=update.message.message_id,
+    )
 
 
 async def take_picture_and_reconstruct(
     update: Update, context: ContextTypes.DEFAULT_TYPE, algo, query=None
 ) -> None:
 
     if query is not None:
         user_subfolder = get_user_folder_from_query(query)
         responder = query.message
     else:
         user_subfolder = get_user_folder(update)
         responder = update.message
 
+    # (if DigiCam) set mask pattern
+    if MASK_PARAM is not None:
+        print("Setting mask pattern...")
+        # get seed for random mask
+        seed = int(os.path.basename(user_subfolder))
+        np.random.seed(seed % (2**32 - 1))
+        mask_vals = np.random.uniform(0, 1, MASK_PARAM.mask_shape)
+        full_pattern = adafruit_sub2full(
+            mask_vals,
+            center=MASK_PARAM.mask_center,
+        )
+        # setting mask
+        set_programmable_mask(
+            full_pattern,
+            device=MASK_PARAM.device,
+            rpi_username=RPI_USERNAME,
+            rpi_hostname=RPI_HOSTNAME,
+        )
+
     await take_picture(update, context, query=query)
 
     # check for saturation
     OUTPUT_FP = os.path.join(user_subfolder, "raw_data_8bit.png")
     # -- load picture to check for saturation
     img = np.array(Image.open(OUTPUT_FP))
     ratio = np.sum(img == 255) / np.prod(img.shape)
@@ -467,17 +611,17 @@
 
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     algo = DEFAULT_ALGO
-    vshift = -10
+    vshift = -26
     brightness = 100
-    # EXPOSURE = 0.08
+    EXPOSURE = 1
 
     # copy image to INPUT_FP
     user_folder = get_user_folder(update)
     original_file_path = os.path.join(user_folder, INPUT_FP)
     os.system(f"cp data/original/mnist_3.png {original_file_path}")
 
     # -- send to display
@@ -506,26 +650,27 @@
 
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     algo = DEFAULT_ALGO
-    vshift = -10
+    vshift = -26
     brightness = 80
-    # EXPOSURE = 0.02
+    EXPOSURE = 0.5
+    pad = 10
 
     # copy image to INPUT_FP
     user_folder = get_user_folder(update)
     original_file_path = os.path.join(user_folder, INPUT_FP)
     os.system(f"cp data/original/thumbs_up.png {original_file_path}")
 
     # -- send to display
     os.system(
-        f"python scripts/measure/remote_display.py -cn {CONFIG_FN} fp={original_file_path} display.vshift={vshift} display.brightness={brightness} rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME}"
+        f"python scripts/measure/remote_display.py -cn {CONFIG_FN} fp={original_file_path} display.pad={pad} display.vshift={vshift} display.brightness={brightness} rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME}"
     )
     await update.message.reply_text(
         f"Image sent to display with brightness {brightness}.",
         reply_to_message_id=update.message.message_id,
     )
 
     await take_picture_and_reconstruct(update, context, algo)
@@ -545,17 +690,17 @@
 
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     algo = DEFAULT_ALGO
-    vshift = 0
+    vshift = -20
     brightness = 80
-    # EXPOSURE = 0.02
+    EXPOSURE = 1
 
     # copy image to INPUT_FP
     user_folder = get_user_folder(update)
     original_file_path = os.path.join(user_folder, INPUT_FP)
     os.system(f"cp data/original/face.jpg {original_file_path}")
 
     # -- send to display
@@ -599,25 +744,34 @@
     # -- measurement
     os.system(
         f"python scripts/measure/remote_capture.py -cn demo_measure_psf rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME}"
     )
     OUTPUT_FP = os.path.join(OUTPUT_FOLDER, "raw_data.png")
     await update.message.reply_photo(
         OUTPUT_FP,
-        caption="PSF (zoom in to see caustic pattern)",
+        caption="PSF (zoom in to see pattern)",
         reply_to_message_id=update.message.message_id,
     )
 
     # send back ground truth PSF
     if PSF_FP is not None:
         await update.message.reply_photo(
             PSF_FP_GAMMA,
             caption="PSF used for reconstructions",
             reply_to_message_id=update.message.message_id,
         )
+    elif MASK_PARAM is not None:
+        # return pre-computed PSF
+        user_folder = get_user_folder(update)
+        psf_fp = os.path.join(user_folder, "psf.png")
+        await update.message.reply_photo(
+            psf_fp,
+            caption="PSF used for reconstructions",
+            reply_to_message_id=update.message.message_id,
+        )
 
     BUSY = False
 
 
 async def button(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     """Parses the CallbackQuery and updates the message text."""
 
@@ -649,19 +803,20 @@
         )
         await query.edit_message_text(text=f"Image sent to display with brightness {BRIGHTNESS}.")
         # await update.message.reply_text("Image sent to display.", reply_to_message_id=update.message.message_id)
 
     elif "exposure" in query.message.text:
 
         EXPOSURE = float(query.data)
-        # await query.edit_message_text(text=f"Image sent to display with exposure of {EXPOSURE} seconds.")
+        await query.edit_message_text(text=f"Exposure set to {EXPOSURE} seconds.")
 
-    algo = DEFAULT_ALGO
-    # send query instead of update as it has the message data
-    await take_picture_and_reconstruct(update, context, algo, query=query)
+    # TODO not working with mask
+    # algo = DEFAULT_ALGO
+    # # send query instead of update as it has the message data
+    # await take_picture_and_reconstruct(update, context, algo, query=query)
     BUSY = False
 
 
 async def brightness_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
 
     """
     Set brightness, re-capture, and reconstruct.
@@ -711,33 +866,37 @@
 
 async def exposure_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
 
     """
     Set exposure, re-capture, and reconstruct.
     """
 
-    # check INPUT_FP exists
-    user_folder = get_user_folder(update)
-    original_file_path = os.path.join(user_folder, INPUT_FP)
-    if not os.path.exists(original_file_path):
-        await update.message.reply_text(
-            "Please set an image first.", reply_to_message_id=update.message.message_id
-        )
-        return
+    # # check INPUT_FP exists
+    # user_folder = get_user_folder(update)
+    # original_file_path = os.path.join(user_folder, INPUT_FP)
+    # if not os.path.exists(original_file_path):
+    #     await update.message.reply_text(
+    #         "Please set an image first.", reply_to_message_id=update.message.message_id
+    #     )
+    #     return
 
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     # vals = {0.02: "very low", 0.05: "low", 0.1: "medium", 0.2: "high", 0.5: "very high"}
+    # -- tape based
     vals = {0.02: "very low", 0.035: "low", 0.05: "medium", 0.065: "high", 0.08: "very high"}
+    # -- digicam
+    vals = {0.25: "very low", 0.5: "low", 0.75: "medium", 1: "high", 1.25: "very high"}
 
     current_exp = vals[EXPOSURE]
-    del vals[EXPOSURE]
+    if EXPOSURE in vals:
+        del vals[EXPOSURE]
     keys = list(vals.keys())
     keyboard = [
         [
             InlineKeyboardButton(f"{vals[keys[0]]} ({keys[0]})", callback_data=f"{keys[0]}"),
             InlineKeyboardButton(f"{vals[keys[1]]} ({keys[1]})", callback_data=f"{keys[1]}"),
         ],
         [
@@ -757,39 +916,39 @@
     )
 
 
 async def emoji(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
 
     global BUSY, EXPOSURE
 
-    # EXPOSURE = 0.02
+    EXPOSURE = 0.7
 
     res = await check_incoming_message(update, context)
     if res is not None:
         await update.message.reply_text(res, reply_to_message_id=update.message.message_id)
         return
 
     # create image from emoji
     text = update.message.text
-    size = 30
+    size = 15
     with Image.new("RGB", (size, size), (0, 0, 0)) as image:
         font = ImageFont.truetype(
             "/usr/share/fonts/truetype/freefont/FreeMono.ttf", size, encoding="unic"
         )
 
         with Pilmoji(image) as pilmoji:
             pilmoji.text((0, 0), text.strip(), (0, 0, 0), font, align="center")
 
         # save image
         user_folder = get_user_folder(update)
         original_file_path = os.path.join(user_folder, INPUT_FP)
         image.save(original_file_path)
 
     # display
-    vshift = -10
+    vshift = -20
     brightness = 80
     os.system(
         f"python scripts/measure/remote_display.py -cn {CONFIG_FN} fp={original_file_path} rpi.username={RPI_USERNAME} rpi.hostname={RPI_HOSTNAME} display.vshift={vshift} display.brightness={brightness}"
     )
     await update.message.reply_text(
         f"Image sent to display with brightness {brightness}.",
         reply_to_message_id=update.message.message_id,
@@ -808,17 +967,16 @@
 
 @hydra.main(version_base=None, config_path="../../configs", config_name="telegram_demo")
 def main(config) -> None:
     """Start the bot."""
 
     global TOKEN, WHITELIST_USERS, RPI_USERNAME, RPI_HOSTNAME, RPI_LENSED_USERNAME, RPI_LENSED_HOSTNAME, CONFIG_FN
     global DEFAULT_ALGO, ALGO_TEXT, HELP_TEXT, supported_algos
-    # global OVERLAY_BOTTOMLEFT, OVERLAY_BOTTOMRIGHT, OVERLAY_TOPLEFT, OVERLAY_TOPRIGHT
     global OVERLAY_ALPHA, OVERLAY_1, OVERLAY_2, OVERLAY_3
-    global PSF_FP, BACKGROUND_FP
+    global PSF_FP, BACKGROUND_FP, MASK_PARAM
 
     TOKEN = config.token
 
     WHITELIST_USERS = config.whitelist
     if WHITELIST_USERS is None:
         WHITELIST_USERS = []
 
@@ -843,63 +1001,76 @@
 
     input_commands = ["/" + input for input in supported_input]
     HELP_TEXT = (
         "Through this bot, you can send a photo to the lensless camera setup in our lab at EPFL (shown above). "
         "The photo will be:\n\n1. Displayed on a screen.\n2. Our lensless camera will "
         "take a picture.\n3. A reconstruction will be sent back through the bot.\n4. "
         "The raw data will also be sent back."
-        "\n\nIf you do not feel comfortable sending one "
-        f"of your own pictures, you can use the {input_commands} commands to set "
-        "the image on the display with one of our inputs. Or even send an emoij 😎"
+        # "\n\nIf you do not feel comfortable sending one "
+        # f"of your own pictures, you can use the {input_commands} commands to set "
+        # "the image on the display with one of our inputs. Or even send an emoij 😎"
+        f"\n\n⚠️ Try one of the {input_commands} commands to use images we've configured. "
+        "Or even send an emoij 😎 "
+        "You can also send your own image (but brightness/exposure may need to be adjusted)."
         "\n\nAll previous data is overwritten "
         "when a new image is sent, and everything is deleted when the process running on the "
         "server is shut down."
     )
 
     if config.supported_algos is not None:
         supported_algos = config.supported_algos
 
     algo_commands = ["/" + algo for algo in supported_algos]
     ALGO_TEXT = (
         f"By default, the reconstruction is done with /{DEFAULT_ALGO}, but you "
         "can specify the algorithm (on the last measurement) with the corresponding "
         f"command: {algo_commands}."
         "\n\nAll provided algorithms require an estimate of the point spread function (PSF). "
-        "You can measure a (proxy) PSF with /psf (a point source like "
-        "image will be displayed on the screen). "
-        "In practice, we measure the PSF with single white LED. The used PSF is sent also sent "
-        "back with the /psf command."
+        "Each user has their unique mask pattern according to the Telegram ID. "
+        "\n\n⚠️ After doing a measurement/reconstruction, you can try running /random_mask "
+        "to see what would be the reconstruction if you use a different (wrong) mask, "
+        "as if someone (like a hacker!) were trying to decode your data with a different mask."
+        # "\n\nAll provided algorithms require an estimate of the point spread function (PSF). "
+        # "You can measure a (proxy) PSF with /psf (a point source like "
+        # "image will be displayed on the screen). "
+        # "In practice, we measure the PSF with single white LED. The used PSF is sent also sent "
+        # "back with the /psf command."
         "\n\nMore info: go.epfl.ch/lensless"
     )
 
     # make output folder
     if not os.path.exists(OUTPUT_FOLDER):
         os.makedirs(OUTPUT_FOLDER)
 
     # load and downsample PSF beforehand
     if config.psf is not None:
-        from lensless.utils.io import save_image
-
-        psf, bg = load_psf(
-            config.psf.fp, downsample=config.psf.downsample, return_float=True, return_bg=True
-        )
 
-        # save to demo folder
-        PSF_FP = os.path.join(OUTPUT_FOLDER, "psf.png")
-        save_image(psf[0], PSF_FP)
+        if "fp" in config.psf:
+            from lensless.utils.io import save_image
 
-        # save with gamma correction
-        from lensless.utils.image import gamma_correction
-
-        psf_gamma = gamma_correction(psf[0], gamma=1.5)
-        save_image(psf_gamma, PSF_FP_GAMMA)
+            psf, bg = load_psf(
+                config.psf.fp, downsample=config.psf.downsample, return_float=True, return_bg=True
+            )
 
-        # save background array
-        BACKGROUND_FP = os.path.join(OUTPUT_FOLDER, "psf_bg.npy")
-        np.save(BACKGROUND_FP, bg)
+            # save to demo folder
+            PSF_FP = os.path.join(OUTPUT_FOLDER, "psf.png")
+            save_image(psf[0], PSF_FP)
+
+            # save with gamma correction
+            from lensless.utils.image import gamma_correction
+
+            psf_gamma = gamma_correction(psf[0], gamma=1.5)
+            save_image(psf_gamma, PSF_FP_GAMMA)
+
+            # save background array
+            BACKGROUND_FP = os.path.join(OUTPUT_FOLDER, "psf_bg.npy")
+            np.save(BACKGROUND_FP, bg)
+        elif "device" in config.psf:
+            # programmable mask
+            MASK_PARAM = config.psf
 
     # Create the Application and pass it your bot's token.
     assert TOKEN is not None
     application = Application.builder().token(TOKEN).build()
 
     if not config.idle:
 
@@ -912,15 +1083,14 @@
 
         # on different commands - answer in Telegram
         application.add_handler(CommandHandler("start", start))
         application.add_handler(CommandHandler("help", help_command))
         application.add_handler(CommandHandler("mnist", mnist_command, block=False))
         application.add_handler(CommandHandler("thumb", thumb_command, block=False))
         application.add_handler(CommandHandler("face", face_command, block=False))
-        application.add_handler(CommandHandler("psf", psf_command, block=False))
         # application.add_handler(CommandHandler("brightness", brightness_command, block=False))
 
         # different algorithms
         application.add_handler(CommandHandler("fista", fista, block=False))
         application.add_handler(CommandHandler("admm", admm, block=False))
         application.add_handler(CommandHandler("unrolled", unrolled, block=False))
         application.add_handler(CommandHandler("unet", unet, block=False))
@@ -937,14 +1107,20 @@
         # exposure input
         application.add_handler(CommandHandler("exposure", exposure_command, block=False))
         application.add_handler(CallbackQueryHandler(button))
 
         # emoji input
         application.add_handler(MessageHandler(filters.TEXT & ~filters.COMMAND, emoji, block=False))
 
+        if MASK_PARAM is not None:
+            application.add_handler(CommandHandler("random_mask", random_mask, block=False))
+        else:
+            # to dim for measuring PSF of DigiCam?
+            application.add_handler(CommandHandler("psf", psf_command, block=False))
+
         # Run the bot until the user presses Ctrl-C
         application.run_polling()
 
     else:
 
         application.add_handler(CommandHandler("help", help_command))
         application.add_handler(MessageHandler(None, not_running_command))
```

### Comparing `lensless-1.0.6/scripts/demo.py` & `lensless-1.0.7/scripts/demo.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 from lensless.utils.io import save_image
 from lensless.utils.image import resize
 import cv2
 import matplotlib.pyplot as plt
 from lensless import FISTA, ADMM
 from lensless.hardware.utils import check_username_hostname, display
 from lensless.utils.io import load_image, load_psf
+import omegaconf
+from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
+from lensless.hardware.trainable_mask import AdafruitLCD
+from torch import from_numpy
 
 
 @hydra.main(version_base=None, config_path="../configs", config_name="demo")
 def demo(config):
 
     check_username_hostname(config.rpi.username, config.rpi.hostname)
     RPI_USERNAME = config.rpi.username
@@ -33,15 +37,42 @@
     else:
         save = False
 
     # 1) Copy file to Raspberry Pi
     print("\nCopying over picture...")
     display(fp=display_fp, rpi_username=RPI_USERNAME, rpi_hostname=RPI_HOSTNAME, **config.display)
 
-    # 2) Take picture
+    # 2) (If DigiCam) set mask pattern
+    mask = None
+    flipud = False
+    if isinstance(config.camera.psf, omegaconf.dictconfig.DictConfig):
+        print("\nSetting mask pattern...")
+        np.random.seed(config.camera.psf.seed % (2**32 - 1))
+        mask_vals = np.random.uniform(0, 1, config.camera.psf.mask_shape)
+        full_pattern = adafruit_sub2full(
+            mask_vals,
+            center=config.camera.psf.mask_center,
+        )
+        set_programmable_mask(
+            full_pattern,
+            device=config.camera.psf.device,
+            rpi_username=RPI_USERNAME,
+            rpi_hostname=RPI_HOSTNAME,
+        )
+        mask_vals_torch = from_numpy(mask_vals.astype(np.float32))
+        flipud = config.camera.psf.flipud
+        mask = AdafruitLCD(
+            initial_vals=mask_vals_torch,
+            sensor=config.capture.sensor,
+            slm=config.camera.psf.device,
+            downsample=config.recon.downsample,
+            flipud=flipud,
+        )
+
+    # 3) Take picture
     time.sleep(config.capture.delay)  # for picture to display
     print("\nTaking picture...")
 
     remote_fn = "remote_capture"
     pic_command = (
         f"{config.rpi.python} {config.capture.script} bayer=True fn={remote_fn} exp={config.capture.exp} iso={config.capture.iso} "
         f"config_pause={config.capture.config_pause} sensor_mode={config.capture.sensor_mode} nbits_out={config.capture.nbits_out}"
@@ -127,25 +158,29 @@
     ax.set_title("Raw data")
     if save:
         plt.savefig(os.path.join(save, "raw.png"))
     pixel_histogram(img)
     if save:
         plt.savefig(os.path.join(save, "histogram.png"))
 
-    # 3) Reconstruct
+    # 4) Reconstruct
 
     # -- prepare data
-    psf, bg = load_psf(
-        to_absolute_path(config.camera.psf),
-        downsample=config.recon.downsample,
-        return_float=True,
-        return_bg=True,
-        dtype=config.recon.dtype,
-    )
-    psf = np.array(psf, dtype=config.recon.dtype)
+    if mask is not None:
+        psf = mask.get_psf().detach().numpy()
+        bg = np.zeros(psf.shape[-1])
+    else:
+        psf, bg = load_psf(
+            to_absolute_path(config.camera.psf),
+            downsample=config.recon.downsample,
+            return_float=True,
+            return_bg=True,
+            dtype=config.recon.dtype,
+        )
+        psf = np.array(psf, dtype=config.recon.dtype)
     ax = plot_image(psf[0], gamma=config.recon.gamma)
     ax.set_title("PSF")
     if save:
         plt.savefig(os.path.join(save, "psf.png"))
 
     data = np.array(img, dtype=config.recon.dtype)
     data -= bg
@@ -170,14 +205,19 @@
         elif config.recon.dtype == "float64":
             torch_dtype = torch.float64
         else:
             raise ValueError("dtype must be float32 or float64")
 
         psf = torch.from_numpy(psf).type(torch_dtype).to(config.recon.torch_device)
         data = torch.from_numpy(data).type(torch_dtype).to(config.recon.torch_device)
+        if flipud:
+            data = torch.rot90(data, dims=(-3, -2), k=2)
+    else:
+        if flipud:
+            data = np.rot90(data, k=2, axes=(-3, -2))
 
     # -- apply algo
     start_time = time.time()
 
     if config.recon.algo == "fista":
         algo_params = config.recon.fista
         recon = FISTA(
```

### Comparing `lensless-1.0.6/scripts/eval/benchmark_recon.py` & `lensless-1.0.7/scripts/eval/benchmark_recon.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import glob
 import json
 import os
 import pathlib as plib
 from lensless.eval.benchmark import benchmark
 import matplotlib.pyplot as plt
 from lensless import ADMM, FISTA, GradientDescent, NesterovGradientDescent
-from lensless.utils.dataset import DiffuserCamTestDataset, DigiCamCelebA
+from lensless.utils.dataset import DiffuserCamTestDataset, DigiCamCelebA, HFDataset
 from lensless.utils.io import save_image
 
 import torch
 from torch.utils.data import Subset
 
 
 @hydra.main(version_base=None, config_path="../../configs", config_name="benchmark")
@@ -48,19 +48,19 @@
     # check if GPU is available
     if torch.cuda.is_available() and config.device[:4] == "cuda":
         device = config.device
     else:
         device = "cpu"
 
     # Benchmark dataset
+    crop = None
     dataset = config.dataset
     if dataset == "DiffuserCam":
         benchmark_dataset = DiffuserCamTestDataset(n_files=n_files, downsample=downsample)
         psf = benchmark_dataset.psf.to(device)
-        crop = None
 
     elif dataset == "DigiCamCelebA":
 
         dataset = DigiCamCelebA(
             data_dir=os.path.join(get_original_cwd(), config.files.dataset),
             celeba_root=config.files.celeba_root,
             psf_path=os.path.join(get_original_cwd(), config.files.psf),
@@ -70,22 +70,40 @@
             simulation_config=config.simulation,
             crop=config.files.crop,
         )
         dataset.psf = dataset.psf.to(device)
         psf = dataset.psf
         crop = dataset.crop
 
+        if config.n_files is not None:
+            dataset = Subset(dataset, np.arange(config.n_files))
+            dataset.psf = dataset.dataset.psf
+
         # train-test split
         train_size = int((1 - config.files.test_size) * len(dataset))
         test_size = len(dataset) - train_size
         _, benchmark_dataset = torch.utils.data.random_split(
             dataset, [train_size, test_size], generator=generator
         )
-        if config.n_files is not None:
-            benchmark_dataset = Subset(benchmark_dataset, np.arange(config.n_files))
+    elif dataset == "HFDataset":
+        benchmark_dataset = HFDataset(
+            huggingface_repo=config.huggingface.repo,
+            split="test",
+            display_res=config.huggingface.image_res,
+            rotate=config.huggingface.rotate,
+            downsample=config.huggingface.downsample,
+            alignment=config.huggingface.alignment,
+            simulation_config=config.simulation,
+        )
+        if benchmark_dataset.multimask:
+            # get first PSF for initialization
+            first_psf_key = list(benchmark_dataset.psf.keys())[0]
+            psf = benchmark_dataset.psf[first_psf_key].to(device)
+        else:
+            psf = benchmark_dataset.psf.to(device)
     else:
         raise ValueError(f"Dataset {dataset} not supported")
 
     print(f"Number of files : {len(benchmark_dataset)}")
     print(f"Data shape :  {benchmark_dataset[0][0].shape}")
 
     model_list = []  # list of algoritms to benchmark
@@ -261,14 +279,20 @@
                 "ReconstructionError": 22.14,
             }
         else:
             raise ValueError(f"Baseline {baseline_label} not supported")
 
     # for each metrics plot the results comparing each model
     metrics_to_plot = ["SSIM", "PSNR", "MSE", "LPIPS_Vgg", "LPIPS_Alex", "ReconstructionError"]
+    available_metrics = list(results[model_name][n_iter_range[0]].keys())
+    metrics_to_plot = [metric for metric in metrics_to_plot if metric in available_metrics]
+    # print metrics being skipped
+    skipped_metrics = [metric for metric in metrics_to_plot if metric not in available_metrics]
+    if len(skipped_metrics) > 0:
+        print(f"Metrics {skipped_metrics} not available and will be skipped")
     for metric in metrics_to_plot:
         plt.figure()
         # plot benchmarked algorithm
         for model_name in results.keys():
             plt.plot(
                 n_iter_range,
                 [results[model_name][n_iter][metric] for n_iter in n_iter_range],
```

### Comparing `lensless-1.0.6/scripts/eval/compute_metrics_from_original.py` & `lensless-1.0.7/scripts/eval/compute_metrics_from_original.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/hardware/config_digicam.py` & `lensless-1.0.7/scripts/hardware/config_digicam.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/hardware/digicam_measure_psfs.py` & `lensless-1.0.7/scripts/hardware/digicam_measure_psfs.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/measure/analyze_image.py` & `lensless-1.0.7/scripts/measure/analyze_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -143,14 +143,17 @@
     img_grey = rgb2gray(img[None, ...])
     ax = plot_image(img_grey, gamma=gamma, normalize=True, ax=ax_gray[0])
     ax.set_title("Grayscale")
     ax = pixel_histogram(img_grey, ax=ax_gray[1], nbits=nbits)
     ax.set_title("Histogram")
     fig_gray.savefig("grey_analysis.png")
 
+    img_grey = img_grey.squeeze()
+    img = img.squeeze()
+
     if lens:
         # determine PSF width
         plot_cross_section(
             img_grey, color="gray", plot_db_drop=width, ax=ax_gray[2], plot_width=plot_width
         )
         _, ax_cross = plt.subplots(ncols=3, nrows=1, num="RGB widths", figsize=(15, 5))
         for i, c in enumerate(["r", "g", "b"]):
@@ -162,14 +165,15 @@
                 max_val=2**nbits - 1,
                 plot_width=plot_width,
             )
             if i > 0:
                 ax.set_ylabel("")
 
     elif lensless:
+
         # plot autocorrelations and width
         # -- grey
         _, ax_auto = plt.subplots(ncols=4, nrows=2, num="Autocorrelations", figsize=(15, 5))
         _, autocorr_grey = plot_autocorr2d(img_grey, ax=ax_auto[0][0])
         plot_cross_section(
             autocorr_grey, color="gray", plot_db_drop=width, ax=ax_auto[1][0], plot_width=plot_width
         )
```

### Comparing `lensless-1.0.6/scripts/measure/analyze_measured_dataset.py` & `lensless-1.0.7/scripts/measure/analyze_measured_dataset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/measure/collect_dataset_on_device.py` & `lensless-1.0.7/scripts/measure/collect_dataset_on_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,24 +19,40 @@
 import pathlib as plib
 import shutil
 import tqdm
 from picamerax import PiCamera
 from fractions import Fraction
 from PIL import Image
 from lensless.utils.io import save_image
+import re
+import glob
+from lensless.hardware.slm import set_programmable_mask, adafruit_sub2full
+
 
 from lensless.hardware.constants import (
     RPI_HQ_CAMERA_CCM_MATRIX,
     RPI_HQ_CAMERA_BLACK_LEVEL,
 )
 import picamerax.array
 from lensless.utils.image import bayer2rgb_cc, resize
 import cv2
 
 
+def convert(text):
+    return int(text) if text.isdigit() else text.lower()
+
+
+def alphanum_key(key):
+    return [convert(c) for c in re.split("([0-9]+)", key)]
+
+
+def natural_sort(arr):
+    return sorted(arr, key=alphanum_key)
+
+
 @hydra.main(version_base=None, config_path="../../configs", config_name="collect_dataset")
 def collect_dataset(config):
 
     input_dir = config.input_dir
     output_dir = config.output_dir
     if output_dir is None:
         # create in same directory as input with timestamp
@@ -44,29 +60,47 @@
 
     MAX_TRIES = config.max_tries
     MIN_LEVEL = config.min_level
     MAX_LEVEL = config.max_level
 
     # if output dir exists check how many files done
     print(f"Output directory : {output_dir}")
-    start_idx = 0
+    start_idx = config.start_idx
     if os.path.exists(output_dir):
         files = list(plib.Path(output_dir).glob(f"*.{config.output_file_ext}"))
         start_idx = len(files)
         print("\nNumber of completed measurements :", start_idx)
-
-    # make output directory if need be
-    output_dir = plib.Path(output_dir)
-    output_dir.mkdir(exist_ok=True)
+        output_dir = plib.Path(output_dir)
+        if config.masks is not None:
+            mask_dir = plib.Path(output_dir) / "masks"
+    else:
+
+        # make output directory
+        output_dir = plib.Path(output_dir)
+        output_dir.mkdir(exist_ok=True)
+
+        if config.masks is not None:
+            # make masks for measurements
+            mask_dir = plib.Path(output_dir) / "masks"
+            mask_dir.mkdir(exist_ok=True)
+
+            np.random.seed(config.masks.seed)
+            for i in range(config.masks.n):
+                mask_fp = mask_dir / f"mask_{i}.npy"
+                mask_vals = np.random.uniform(0, 1, config.masks.shape)
+                np.save(mask_fp, mask_vals)
 
     # assert input directory exists
     assert os.path.exists(input_dir)
 
     # get number of files with glob
-    files = list(plib.Path(input_dir).glob(f"*.{config.input_file_ext}"))
+    # files = list(plib.Path(input_dir).glob(f"*.{config.input_file_ext}"))
+    files = glob.glob(os.path.join(input_dir, f"*.{config.input_file_ext}"))
+    files = natural_sort(files)
+    files = [plib.Path(f) for f in files]
     n_files = len(files)
     print(f"\nNumber of {config.input_file_ext} files :", n_files)
     if config.n_files:
         print(f"TEST : collecting first {config.n_files} files!")
         files = files[: config.n_files]
         n_files = len(files)
 
@@ -134,26 +168,26 @@
         else:
             g = camera.awb_gains
 
         camera.awb_mode = "off"
         camera.awb_gains = g
 
         # for parameters to settle
-        time.sleep(5)
+        time.sleep(config.capture.config_pause)
 
         print("Capturing at resolution: ", res)
         print("AWB gains", float(camera.awb_gains[0]), float(camera.awb_gains[1]))
 
     init_brightness = config.display.brightness
 
     # loop over files with tqdm
     exposure_vals = []
     brightness_vals = []
     n_tries_vals = []
-    for i, _file in enumerate(tqdm.tqdm(files), start=start_idx):
+    for i, _file in enumerate(tqdm.tqdm(files[start_idx:])):
 
         # save file in output directory as PNG
         output_fp = output_dir / _file.name
         output_fp = output_fp.with_suffix(f".{config.output_file_ext}")
 
         # if not done, perform measurement
         if not os.path.isfile(output_fp):
@@ -168,97 +202,122 @@
                 screen_res = np.array(config.display.screen_res)
                 hshift = config.display.hshift
                 vshift = config.display.vshift
                 pad = config.display.pad
                 brightness = init_brightness
                 display_image_path = config.display.output_fp
                 rot90 = config.display.rot90
-                os.system(
-                    f"python scripts/measure/prep_display_image.py --fp {_file} --output_path {display_image_path} --screen_res {screen_res[0]} {screen_res[1]} --hshift {hshift} --vshift {vshift} --pad {pad} --brightness {brightness} --rot90 {rot90}"
-                )
-
-                time.sleep(config.capture.delay)
-
-                # -- take picture
-                max_pixel_val = 0
-                fact = 2
-                n_tries = 0
-
-                camera.shutter_speed = init_shutter_speed
-                time.sleep(5)
-
-                current_screen_brightness = init_brightness
-                current_shutter_speed = camera.shutter_speed
-                print(f"current shutter speed: {current_shutter_speed}")
-                print(f"current screen brightness: {current_screen_brightness}")
-
-                while max_pixel_val < MIN_LEVEL or max_pixel_val > MAX_LEVEL:
-
-                    if n_tries > MAX_TRIES:
-                        print("Max number of tries reached!")
-                        break
-
-                    # get bayer data
-                    stream = picamerax.array.PiBayerArray(camera)
-                    camera.capture(stream, "jpeg", bayer=True)
-                    output_bayer = np.sum(stream.array, axis=2).astype(np.uint16)
-
-                    # convert to RGB
-                    output = bayer2rgb_cc(
-                        output_bayer,
-                        nbits=12,
-                        blue_gain=float(g[1]),
-                        red_gain=float(g[0]),
-                        black_level=RPI_HQ_CAMERA_BLACK_LEVEL,
-                        ccm=RPI_HQ_CAMERA_CCM_MATRIX,
-                        nbits_out=8,
+                display_command = f"python scripts/measure/prep_display_image.py --fp {_file} --output_path {display_image_path} --screen_res {screen_res[0]} {screen_res[1]} --hshift {hshift} --vshift {vshift} --pad {pad} --brightness {brightness} --rot90 {rot90}"
+                if config.display.landscape:
+                    display_command += " --landscape"
+                if config.display.image_res is not None:
+                    display_command += (
+                        f" --image_res {config.display.image_res[0]} {config.display.image_res[1]}"
                     )
+                # print(display_command)
+                os.system(display_command)
 
-                    if down:
-                        output = resize(
-                            output[None, ...], factor=1 / down, interpolation=cv2.INTER_CUBIC
-                        )[0]
-
-                    # print range
-                    print(f"{output_fp}, range: {output.min()} - {output.max()}")
-                    max_pixel_val = output.max()
-
-                    if max_pixel_val < MIN_LEVEL:
-                        current_shutter_speed = init_shutter_speed * fact
-                        camera.shutter_speed = current_shutter_speed
-                        time.sleep(5)
-                        print(f"increasing shutter speed to {current_shutter_speed}")
-                        fact += 1
-
-                    elif max_pixel_val > MAX_LEVEL:
-
-                        current_screen_brightness = current_screen_brightness - 10
-
-                        screen_res = np.array(config.display.screen_res)
-                        hshift = config.display.hshift
-                        vshift = config.display.vshift
-                        pad = config.display.pad
-                        brightness = current_screen_brightness
-                        display_image_path = config.display.output_fp
-                        rot90 = config.display.rot90
-                        os.system(
-                            f"python scripts/measure/prep_display_image.py --fp {_file} --output_path {display_image_path} --screen_res {screen_res[0]} {screen_res[1]} --hshift {hshift} --vshift {vshift} --pad {pad} --brightness {brightness} --rot90 {rot90}"
-                        )
-                        print(f"decreasing screen brightness to {current_screen_brightness}")
+                time.sleep(config.display.delay)
 
-                        time.sleep(config.capture.delay)
+                if not config.capture.skip:
 
-                    n_tries += 1
+                    # -- set mask pattern
+                    if config.masks is not None:
+                        mask_idx = (i + start_idx) % config.masks.n
+                        mask_fp = mask_dir / f"mask_{mask_idx}.npy"
+                        print("using mask: ", mask_fp)
+                        mask_vals = np.load(mask_fp)
+                        full_pattern = adafruit_sub2full(
+                            mask_vals,
+                            center=config.masks.center,
+                        )
+                        set_programmable_mask(full_pattern, device=config.masks.device)
 
-                    # save image
-                    save_image(output, output_fp)
+                    # -- take picture
+                    max_pixel_val = 0
+                    fact_increase = 2
+                    fact_decrease = 1.5
+                    n_tries = 0
+
+                    camera.shutter_speed = init_shutter_speed
+                    time.sleep(config.capture.config_pause)
+
+                    current_screen_brightness = init_brightness
+                    current_shutter_speed = camera.shutter_speed
+                    print(f"current shutter speed: {current_shutter_speed}")
+                    print(f"current screen brightness: {current_screen_brightness}")
+
+                    while max_pixel_val < MIN_LEVEL or max_pixel_val > MAX_LEVEL:
+
+                        # get bayer data
+                        stream = picamerax.array.PiBayerArray(camera)
+                        camera.capture(stream, "jpeg", bayer=True)
+                        output_bayer = np.sum(stream.array, axis=2).astype(np.uint16)
+
+                        # convert to RGB
+                        output = bayer2rgb_cc(
+                            output_bayer,
+                            nbits=12,
+                            blue_gain=float(g[1]),
+                            red_gain=float(g[0]),
+                            black_level=RPI_HQ_CAMERA_BLACK_LEVEL,
+                            ccm=RPI_HQ_CAMERA_CCM_MATRIX,
+                            nbits_out=8,
+                        )
 
-                exposure_vals.append(current_shutter_speed / 1e6)
-                brightness_vals.append(current_screen_brightness)
-                n_tries_vals.append(n_tries)
+                        if down:
+                            output = resize(
+                                output[None, ...], factor=1 / down, interpolation=cv2.INTER_CUBIC
+                            )[0]
+
+                        # save image
+                        save_image(output, output_fp, normalize=False)
+
+                        # print range
+                        print(f"{output_fp}, range: {output.min()} - {output.max()}")
+
+                        n_tries += 1
+                        if n_tries > MAX_TRIES:
+                            print("Max number of tries reached!")
+                            break
+
+                        max_pixel_val = output.max()
+                        if max_pixel_val < MIN_LEVEL:
+                            # increase exposure
+                            current_shutter_speed = int(current_shutter_speed * fact_increase)
+                            time.sleep(config.capture.config_pause)
+                            print(f"increasing shutter speed to {current_shutter_speed}")
+
+                        elif max_pixel_val > MAX_LEVEL:
+
+                            # decrease exposure
+                            current_shutter_speed = int(current_shutter_speed / fact_decrease)
+                            camera.shutter_speed = current_shutter_speed
+                            time.sleep(config.capture.config_pause)
+                            print(f"decreasing shutter speed to {current_shutter_speed}")
+
+                            # # decrease screen brightness
+                            # current_screen_brightness = current_screen_brightness - 10
+                            # screen_res = np.array(config.display.screen_res)
+                            # hshift = config.display.hshift
+                            # vshift = config.display.vshift
+                            # pad = config.display.pad
+                            # brightness = current_screen_brightness
+                            # display_image_path = config.display.output_fp
+                            # rot90 = config.display.rot90
+                            # os.system(
+                            #     f"python scripts/measure/prep_display_image.py --fp {_file} --output_path {display_image_path} --screen_res {screen_res[0]} {screen_res[1]} --hshift {hshift} --vshift {vshift} --pad {pad} --brightness {brightness} --rot90 {rot90}"
+                            # )
+                            # print(f"decreasing screen brightness to {current_screen_brightness}")
+
+                            # time.sleep(config.display.delay)
+
+                    exposure_vals.append(current_shutter_speed / 1e6)
+                    brightness_vals.append(current_screen_brightness)
+                    n_tries_vals.append(n_tries)
 
         # check if runtime is exceeded
         if config.runtime:
             proc_time = time.time() - start_time
             if proc_time > runtime_sec:
                 print(f"-- measured {i+1} / {n_files} files")
                 break
```

### Comparing `lensless-1.0.6/scripts/measure/on_device_capture.py` & `lensless-1.0.7/scripts/measure/on_device_capture.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/measure/prep_display_image.py` & `lensless-1.0.7/scripts/measure/prep_display_image.py`

 * *Files 11% similar despite different names*

```diff
@@ -57,57 +57,75 @@
 )
 @click.option(
     "--rot90",
     default=0,
     type=int,
     help="How many times to rotate provided image by 90 degrees.",
 )
-def display(fp, pad, output_path, vshift, brightness, screen_res, hshift, rot90):
+@click.option(
+    "--landscape",
+    is_flag=True,
+    help="Force landscape.",
+)
+@click.option(
+    "--image_res",
+    default=None,
+    nargs=2,
+    type=int,
+    help="Image resolution in pixels (width, height).",
+)
+def display(
+    fp, pad, output_path, vshift, brightness, screen_res, hshift, rot90, landscape, image_res
+):
     interpolation = cv2.INTER_NEAREST
 
     # load image
     img_og = cv2.imread(fp, cv2.IMREAD_UNCHANGED)
     img_og = cv2.cvtColor(img_og, cv2.COLOR_BGR2RGB)
+    if landscape:
+        if img_og.shape[0] > img_og.shape[1]:
+            img_og = np.rot90(img_og)
 
     # rotate image
     if rot90:
         img_og = np.rot90(img_og, k=rot90)
 
         # if odd, swap hshift and vshift
         if rot90 % 2:
             vshift, hshift = hshift, vshift
 
     if screen_res:
         image_height, image_width = img_og.shape[:2]
         img = np.zeros((screen_res[1], screen_res[0], 3), dtype=img_og.dtype)
 
-        # set image with padding and correct aspect ratio
-        if screen_res[0] < screen_res[1]:
+        if image_res is None:
+            # set image with padding and correct aspect ratio
+            if screen_res[0] < screen_res[1]:
 
-            max_ratio = screen_res[1] / float(image_height)
+                max_ratio = screen_res[1] / float(image_height)
 
-            new_width = int(screen_res[0] / (1 + 2 * pad / 100))
-            ratio = new_width / float(image_width)
-            # new_height = int(ratio * image_height)
+                new_width = int(screen_res[0] / (1 + 2 * pad / 100))
+                ratio = new_width / float(image_width)
+                # new_height = int(ratio * image_height)
 
-        else:
+            else:
 
-            max_ratio = screen_res[0] / float(image_width)
+                max_ratio = screen_res[0] / float(image_width)
 
-            new_height = int(screen_res[1] / (1 + 2 * pad / 100))
-            ratio = new_height / float(image_height)
-            # new_width = int(ratio * image_width)
+                new_height = int(screen_res[1] / (1 + 2 * pad / 100))
+                ratio = new_height / float(image_height)
+                # new_width = int(ratio * image_width)
 
-        ratio = min(ratio, max_ratio)
-        new_width = int(ratio * image_width)
-        new_height = int(ratio * image_height)
+            ratio = min(ratio, max_ratio)
+            new_width = int(ratio * image_width)
+            new_height = int(ratio * image_height)
+            image_res = (new_width, new_height)
 
-        image_res = (new_width, new_height)
+        # set image within screen
         img_og = cv2.resize(img_og, image_res, interpolation=interpolation)
-
         img[: image_res[1], : image_res[0]] = img_og
 
         # center
         img = np.roll(img, shift=int((screen_res[1] - image_res[1]) / 2), axis=0)
         img = np.roll(img, shift=int((screen_res[0] - image_res[0]) / 2), axis=1)
 
     else:
```

### Comparing `lensless-1.0.6/scripts/measure/remote_capture.py` & `lensless-1.0.7/scripts/measure/remote_capture.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
             # write RGB data
             if not bayer:
                 cv2.imwrite(localfile, cv2.cvtColor(img, cv2.COLOR_RGB2BGR))
 
     # save image as viewable 8 bit
     fp = os.path.join(save, f"{fn}_8bit.png")
-    save_image(img, fp)
+    save_image(img, fp, normalize=True)
 
     # plot RGB
     if plot:
         if not gray:
             ax = plot_image(img, gamma=gamma)
             ax.set_title("RGB")
             if save:
```

### Comparing `lensless-1.0.6/scripts/measure/remote_display.py` & `lensless-1.0.7/scripts/measure/remote_display.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/recon/admm.py` & `lensless-1.0.7/scripts/recon/admm.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         red_gain=config["preprocess"]["red_gain"],
         plot=config["display"]["plot"],
         flip=config["preprocess"]["flip"],
         gamma=config["display"]["gamma"],
         gray=config["preprocess"]["gray"],
         single_psf=config["preprocess"]["single_psf"],
         shape=config["preprocess"]["shape"],
-        torch=config.torch,
+        use_torch=config.torch,
         torch_device=config.torch_device,
         bg_pix=config.preprocess.bg_pix,
         normalize=config.preprocess.normalize,
     )
 
     disp = config["display"]["disp"]
     if disp < 0:
```

### Comparing `lensless-1.0.6/scripts/recon/apgd_pycsou.py` & `lensless-1.0.7/scripts/recon/apgd_pycsou.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/recon/dataset.py` & `lensless-1.0.7/scripts/recon/dataset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,202 +1,195 @@
 """
-Apply ADMM reconstruction to folder.
+Apply ADMM reconstruction to a dataset downloaded from HuggingFace.
+
+By default, to 25 files from DiffuserCam MirFlickr test set: https://huggingface.co/datasets/bezzam/DiffuserCam-Lensless-Mirflickr-Dataset/viewer/default/test
 
 ```
 python scripts/recon/dataset.py
 ```
 
+To apply to CelebA measured with DigiCam: https://huggingface.co/datasets/bezzam/DigiCam-CelebA-10K/viewer/default/test
+You can run the following command:
+```python
+python scripts/recon/dataset.py -cn recon_celeba_digicam
+```
+
 To run APGD, use the following command:
 ```
+# (first-time): pip install git+https://github.com/matthieumeo/pycsou.git@38e9929c29509d350a7ff12c514e2880fdc99d6e
 python scripts/recon/dataset.py algo=apgd
 ```
 
 To just copy resized raw data, use the following command:
 ```
-python scripts/recon/dataset.py algo=null preprocess.data_dim=[48,64]
+python scripts/recon/dataset.py algo=null data_dim=[48,64]
 ```
 
 """
 
 import hydra
-from hydra.utils import to_absolute_path
 import os
 import time
-import numpy as np
-from lensless.utils.io import load_psf, load_image, save_image
-from lensless import ADMM
 import torch
-import glob
+from lensless.utils.io import save_image
+from lensless import ADMM
 from tqdm import tqdm
-from lensless.recon.apgd import APGD
 from joblib import Parallel, delayed
+import numpy as np
+from lensless.utils.dataset import DiffuserCamMirflickrHF, HFDataset
+from lensless.eval.metric import psnr, lpips
+from lensless.utils.image import resize
 
 
 @hydra.main(version_base=None, config_path="../../configs", config_name="recon_dataset")
-def admm_dataset(config):
+def recon_dataset(config):
 
     algo = config.algo
-
-    # get raw data file paths
-    dataset = to_absolute_path(config.input.raw_data)
-    if not os.path.isdir(dataset):
-        print(f"No dataset found at {dataset}")
-        try:
-            from torchvision.datasets.utils import download_and_extract_archive
-        except ImportError:
-            exit()
-        msg = "Do you want to download the sample CelebA dataset measured with a random Adafruit LCD pattern (1.2 GB)?"
-
-        # default to yes if no input is given
-        valid = input("%s (Y/n) " % msg).lower() != "n"
-        if valid:
-            url = "https://drive.switch.ch/index.php/s/m89D1tFEfktQueS/download"
-            filename = "celeba_adafruit_random_2mm_20230720_1K.zip"
-            download_and_extract_archive(
-                url, os.path.dirname(dataset), filename=filename, remove_finished=True
-            )
-    data_fps = sorted(glob.glob(os.path.join(dataset, "*.png")))
-    if config.n_files is not None:
-        data_fps = data_fps[: config.n_files]
-    n_files = len(data_fps)
-
-    # load PSF
-    psf_fp = to_absolute_path(config.input.psf)
-    flip = config.preprocess.flip
-    dtype = config.input.dtype
-    print("\nPSF:")
-    psf, bg = load_psf(
-        psf_fp,
-        verbose=True,
-        downsample=config.preprocess.downsample,
-        return_bg=True,
-        flip=flip,
-        dtype=dtype,
-    )
-    print(f"Downsampled PSF shape: {psf.shape}")
-
-    data_dim = None
-    if config.preprocess.data_dim is not None:
-        data_dim = tuple(config.preprocess.data_dim) + (psf.shape[-1],)
+    if config.dataset == "diffusercam":
+        dataset = DiffuserCamMirflickrHF(split=config.split, downsample=config.downsample)
     else:
-        data_dim = psf.shape
+        dataset = HFDataset(
+            huggingface_repo=config.dataset,
+            split=config.split,
+            downsample=config.downsample,
+            alignment=config.alignment,
+            rotate=config.rotate,
+            psf=config.psf_fn,
+        )
+
+    psf = dataset.psf.to(config.torch_device)
+    data_dim = dataset.psf.shape
+    n_files = len(dataset)
+    if config.n_files is not None:
+        n_files = min(n_files, config.n_files)
+    print(f"Reconstructing {n_files} files...")
 
-    # -- create output folder
-    output_folder = to_absolute_path(config.output_folder)
+    # create output folder
+    output_folder = config.output_folder
+    if output_folder is None:
+        output_folder = os.path.join(os.getcwd(), os.path.basename(config.dataset))
     if algo == "apgd":
         output_folder = output_folder + f"_apgd{config.apgd.max_iter}"
     elif algo == "admm":
         output_folder = output_folder + f"_admm{config.admm.n_iter}"
     else:
         output_folder = output_folder + "_raw"
     output_folder = output_folder + f"_{data_dim[-3]}x{data_dim[-2]}"
     os.makedirs(output_folder, exist_ok=True)
+    print(f"Output folder: {output_folder}")
 
     # -- apply reconstruction
+    psnr_scores = []
+    lpips_scores = []
+    recon = None
     if algo == "apgd":
 
+        from lensless.recon.apgd import APGD
+
+        psf = psf.cpu().numpy()
+
         start_time = time.time()
 
         def recover(i):
 
             # reconstruction object
             recon = APGD(psf=psf, **config.apgd)
 
-            data_fp = data_fps[i]
-
-            # load data
-            data = load_image(
-                data_fp, flip=flip, bg=bg, as_4d=True, return_float=True, shape=data_dim
-            )
-            data = data[0]  # first depth
+            lensless, lensed = dataset[i]
+            lensless = lensless.numpy()
+            lensed = lensed.numpy()
 
             # apply reconstruction
-            recon.set_data(data)
-            img = recon.apply(
+            recon.set_data(lensless)
+            res = recon.apply(
                 disp_iter=config.display.disp,
                 gamma=config.display.gamma,
                 plot=config.display.plot,
             )
 
             # -- extract region of interest and save
-            if config.roi is not None:
-                roi = config.roi
-                img = img[roi[0] : roi[2], roi[1] : roi[3]]
-
-            bn = os.path.basename(data_fp)
-            output_fp = os.path.join(output_folder, bn)
-            save_image(img, output_fp)
+            if config.dataset != "diffusercam":
+                res, lensed = dataset.extract_roi(res[np.newaxis], lensed)
+                res = res[0]
+
+            # compute metrics
+            scores = psnr(lensed[0], res), lpips(lensed[0], res)
+
+            output_fp = os.path.join(output_folder, f"{i}.png")
+            save_image(res, output_fp, normalize=True)
+            return scores
 
         n_jobs = config.apgd.n_jobs
         if n_jobs > 1:
-            Parallel(n_jobs=n_jobs)(delayed(recover)(i) for i in range(n_files))
+            scores = Parallel(n_jobs=n_jobs)(delayed(recover)(i) for i in range(n_files))
+            psnr_scores = [s[0] for s in scores]
+            lpips_scores = [s[1] for s in scores]
         else:
             for i in tqdm(range(n_files)):
-                recover(i)
+                scores = recover(i)
+                psnr_scores.append(scores[0])
+                lpips_scores.append(scores[1])
 
     else:
 
-        if config.torch:
-            torch_dtype = torch.float32
-            torch_device = config.torch_device
-            psf = torch.from_numpy(psf).type(torch_dtype).to(torch_device)
-
         # create reconstruction object
-        recon = None
         if config.algo == "admm":
             recon = ADMM(psf, **config.admm)
 
         # loop over files and apply reconstruction
         start_time = time.time()
-
         for i in tqdm(range(n_files)):
-            data_fp = data_fps[i]
 
-            # load data
-            data = load_image(
-                data_fp, flip=flip, bg=bg, as_4d=True, return_float=True, shape=data_dim
-            )
-
-            if config.torch:
-                data = torch.from_numpy(data).type(torch_dtype).to(torch_device)
+            # load and prepare data
+            lensless, lensed = dataset[i]
 
             if recon is not None:
 
                 # set data
-                recon.set_data(data)
+                recon.set_data(lensless.to(psf.device))
 
                 # apply reconstruction
                 res = recon.apply(
                     n_iter=config.admm.n_iter,
                     disp_iter=config.display.disp,
                     gamma=config.display.gamma,
                     plot=config.display.plot,
                 )
 
+                # -- extract region of interest
+                if config.dataset != "diffusercam":
+                    res, lensed = dataset.extract_roi(res, lensed)
+                if recon is not None:
+                    # compute metrics
+                    lensed_np = lensed.cpu().numpy()
+                    res_np = res.cpu().numpy()
+                    psnr_scores.append(psnr(lensed_np, res_np))
+                    lpips_scores.append(lpips(lensed_np[0], res_np[0]))
+
             else:
 
                 # copy resized raw data
-                res = data
+                data_dim = list(config.data_dim) + [psf.shape[-1]]
+                res = resize(lensless.cpu().numpy(), shape=data_dim)
 
             # save reconstruction as PNG
             # -- take first depth
-            if config.torch:
+            if isinstance(res, torch.Tensor):
                 img = res[0].cpu().numpy()
             else:
                 img = res[0]
+            output_fp = os.path.join(output_folder, f"{i}.png")
+            save_image(img, output_fp, normalize=True)
 
-            # -- extract region of interest
-            if config.roi is not None:
-                img = img[config.roi[0] : config.roi[2], config.roi[1] : config.roi[3]]
-
-            bn = os.path.basename(data_fp)
-            output_fp = os.path.join(output_folder, bn)
-            save_image(img, output_fp)
-
-        print(f"Processing time : {time.time() - start_time} s")
-        # time per file
-        print(f"Time per file : {(time.time() - start_time) / n_files} s")
-        print("Files saved to: ", output_folder)
+    if len(psnr_scores) > 0:
+        # print average metrics
+        print(f"Avg PSNR: {np.mean(psnr_scores)}")
+        print(f"Avg LPIPS: {np.mean(lpips_scores)}")
+
+    print(f"Processing time : {time.time() - start_time} s")
+    # time per file
+    print(f"Time per file : {(time.time() - start_time) / n_files} s")
+    print("Files saved to: ", output_folder)
 
 
 if __name__ == "__main__":
-    admm_dataset()
+    recon_dataset()
```

### Comparing `lensless-1.0.6/scripts/recon/demo.py` & `lensless-1.0.7/scripts/recon/demo.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import time
 from lensless.utils.plot import plot_image
 from lensless.utils.io import save_image
 from lensless.utils.image import resize, gamma_correction
 import matplotlib.pyplot as plt
 from lensless import FISTA, ADMM
 from lensless.utils.io import load_image, load_psf
+import omegaconf
+from lensless.hardware.trainable_mask import AdafruitLCD
 
 
 @hydra.main(version_base=None, config_path="../../configs", config_name="demo")
 def demo(config):
 
     start_time = time.time()
 
@@ -46,78 +48,86 @@
 
     data = np.array(img, dtype=config.recon.dtype)
     if len(data.shape) == 3:
         data = data[np.newaxis, :, :, :]
     elif len(data.shape) == 2:
         data = data[np.newaxis, :, :, np.newaxis]
 
-    if config.recon.algo == "unet":
-
-        raise ValueError("Not implemented yet. Issues with TensorFlow and PyTorch compatability...")
-
-        # -- resize data to fit model input
-        data = resize(data, shape=config.recon.unet.input_shape)
+    # -- PSF
+    flipud = False
+    if isinstance(config.camera.psf, omegaconf.dictconfig.DictConfig):
+        import torch
+
+        np.random.seed(config.camera.psf.seed % (2**32 - 1))
+        mask_vals = np.random.uniform(0, 1, config.camera.psf.mask_shape)
+        mask_vals_torch = torch.from_numpy(mask_vals.astype(np.float32))
+        flipud = config.camera.psf.flipud
+        mask = AdafruitLCD(
+            initial_vals=mask_vals_torch,
+            sensor=config.capture.sensor,
+            slm=config.camera.psf.device,
+            downsample=config.recon.downsample,
+            flipud=flipud,
+        )
+        psf = mask.get_psf().detach().numpy()
+        bg = np.zeros(psf.shape[-1])
 
-        # -- normalize data between [-1, 1]
-        # data /= np.linalg.norm(data.ravel())
-        data /= data.max()
-        data = np.array(data, dtype=config.recon.dtype)
-        data = data * 2 - 1
+    elif config.camera.background is not None:
+        psf = load_psf(
+            to_absolute_path(config.camera.psf),
+            downsample=config.recon.downsample,
+            return_float=True,
+            return_bg=False,
+            dtype=config.recon.dtype,
+        )
+        bg = np.load(to_absolute_path(config.camera.background))
 
     else:
-
-        # -- PSF
-        if config.camera.background is not None:
-            psf = load_psf(
-                to_absolute_path(config.camera.psf),
-                downsample=config.recon.downsample,
-                return_float=True,
-                return_bg=False,
-                dtype=config.recon.dtype,
-            )
-            bg = np.load(to_absolute_path(config.camera.background))
-
+        psf, bg = load_psf(
+            to_absolute_path(config.camera.psf),
+            downsample=config.recon.downsample,
+            return_float=True,
+            return_bg=True,
+            dtype=config.recon.dtype,
+        )
+    psf = np.array(psf, dtype=config.recon.dtype)
+    if config.plot:
+        ax = plot_image(psf[0], gamma=config.recon.gamma)
+        ax.set_title("PSF")
+        if save:
+            plt.savefig(os.path.join(save, "psf.png"))
+
+    # -- prepare data
+    if data.min() > 0:
+        data -= bg
+    data = np.clip(data, a_min=0, a_max=data.max())
+
+    if data.shape != psf.shape:
+        # in DiffuserCam dataset, images are already reshaped
+        data = resize(data, shape=psf.shape)
+    data /= np.linalg.norm(data.ravel())
+    data = np.array(data, dtype=config.recon.dtype)
+
+    if config.recon.use_torch:
+        import torch
+
+        if config.recon.dtype == "float32":
+            torch_dtype = torch.float32
+        elif config.recon.dtype == "float64":
+            torch_dtype = torch.float64
         else:
-            psf, bg = load_psf(
-                to_absolute_path(config.camera.psf),
-                downsample=config.recon.downsample,
-                return_float=True,
-                return_bg=True,
-                dtype=config.recon.dtype,
-            )
-        psf = np.array(psf, dtype=config.recon.dtype)
-        if config.plot:
-            ax = plot_image(psf[0], gamma=config.recon.gamma)
-            ax.set_title("PSF")
-            if save:
-                plt.savefig(os.path.join(save, "psf.png"))
-
-        # -- prepare data
-        if data.min() > 0:
-            data -= bg
-        data = np.clip(data, a_min=0, a_max=data.max())
-
-        if data.shape != psf.shape:
-            # in DiffuserCam dataset, images are already reshaped
-            data = resize(data, shape=psf.shape)
-        data /= np.linalg.norm(data.ravel())
-        data = np.array(data, dtype=config.recon.dtype)
-
-        if config.recon.use_torch:
-            import torch
-
-            if config.recon.dtype == "float32":
-                torch_dtype = torch.float32
-            elif config.recon.dtype == "float64":
-                torch_dtype = torch.float64
-            else:
-                raise ValueError("dtype must be float32 or float64")
+            raise ValueError("dtype must be float32 or float64")
 
-            psf = torch.from_numpy(psf).type(torch_dtype).to(config.recon.torch_device)
-            data = torch.from_numpy(data).type(torch_dtype).to(config.recon.torch_device)
+        psf = torch.from_numpy(psf).type(torch_dtype).to(config.recon.torch_device)
+        data = torch.from_numpy(data).type(torch_dtype).to(config.recon.torch_device)
+        if flipud:
+            data = torch.rot90(data, dims=(-3, -2), k=2)
+    else:
+        if flipud:
+            data = np.rot90(data, k=2, axes=(-3, -2))
 
     print(f"Setup time : {time.time() - start_time} s")
 
     # -- apply algo
     start_time = time.time()
 
     if config.recon.algo == "fista":
@@ -142,55 +152,36 @@
             **algo_params,
         )
         print("Loading checkpoint from : ", algo_params.checkpoint_fp)
         assert os.path.exists(algo_params.checkpoint_fp), "Checkpoint does not exist"
         recon.load_state_dict(
             torch.load(algo_params.checkpoint_fp, map_location=config.recon.torch_device)
         )
-    elif config.recon.algo == "unet":
-        import tensorflow as tf
-
-        algo_params = config.recon.unet
-
-        if algo_params.gpu:
-            # set gpu to the less used one
-            import setGPU
-        else:
-            os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
-
-        print("Loading checkpoint from : ", algo_params.model_path)
-        assert os.path.exists(algo_params.model_path), "Model path does not exist"
-
-        model = tf.saved_model.load(algo_params.model_path)
     else:
         raise ValueError(f"Unsupported algorithm: {config.recon.algo}")
 
     print("Applying : ", config.recon.algo)
-    if config.recon.algo == "unet":
 
-        final_image = model(data)
-
-    else:
-        if config.recon.use_torch:
-            with torch.no_grad():
-                recon.set_data(data)
-                res = recon.apply(
-                    gamma=config.recon.gamma,
-                    save=save,
-                    plot=config.plot,
-                    disp_iter=algo_params["disp_iter"],
-                )
-        else:
+    if config.recon.use_torch:
+        with torch.no_grad():
             recon.set_data(data)
             res = recon.apply(
                 gamma=config.recon.gamma,
                 save=save,
                 plot=config.plot,
                 disp_iter=algo_params["disp_iter"],
             )
+    else:
+        recon.set_data(data)
+        res = recon.apply(
+            gamma=config.recon.gamma,
+            save=save,
+            plot=config.plot,
+            disp_iter=algo_params["disp_iter"],
+        )
     print(f"Processing time : {time.time() - start_time} s")
 
     if config.plot:
         final_image = res[0]
     else:
         final_image = res
```

### Comparing `lensless-1.0.6/scripts/recon/diffusercam_mirflickr.py` & `lensless-1.0.7/scripts/recon/diffusercam_mirflickr.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/recon/gradient_descent.py` & `lensless-1.0.7/scripts/recon/gradient_descent.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         red_gain=config["preprocess"]["red_gain"],
         plot=config["display"]["plot"],
         flip=config["preprocess"]["flip"],
         gamma=config["display"]["gamma"],
         gray=config["preprocess"]["gray"],
         single_psf=config["preprocess"]["single_psf"],
         shape=config["preprocess"]["shape"],
-        torch=config.torch,
+        use_torch=config.torch,
         torch_device=config.torch_device,
     )
 
     disp = config["display"]["disp"]
     if disp < 0:
         disp = None
```

### Comparing `lensless-1.0.6/scripts/recon/train_unrolled.py` & `lensless-1.0.7/scripts/recon/train_learning_based.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,337 +1,77 @@
 # #############################################################################
-# train_unrolled.py
-# =================
+# train_learning_based.py
+# =======================
 # Authors :
 # Yohann PERRON [yohann.perron@gmail.com]
 # Eric BEZZAM [ebezzam@gmail.com]
 # #############################################################################
 
 """
 Train unrolled version of reconstruction algorithm.
 
 ```
-python scripts/recon/train_unrolled.py
+python scripts/recon/train_learning_based.py
 ```
 
 By default it uses the configuration from the file `configs/train_unrolledADMM.yaml`.
 
 To train pre- and post-processing networks, use the following command:
 ```
-python scripts/recon/train_unrolled.py -cn train_pre-post-processing
+python scripts/recon/train_learning_based.py -cn train_unrolled_pre_post
 ```
 
 To fine-tune the DiffuserCam PSF, use the following command:
 ```
-python scripts/recon/train_unrolled.py -cn fine-tune_PSF
+python scripts/recon/train_learning_based.py -cn fine-tune_PSF
 ```
 
-To train a PSF from scratch with a simulated dataset, use the following command:
-```
-python scripts/recon/train_unrolled.py -cn train_psf_from_scratch
-```
 
 """
 
+import wandb
 import logging
 import hydra
 from hydra.utils import get_original_cwd
 import os
 import numpy as np
 import time
-from lensless import UnrolledFISTA, UnrolledADMM, TrainableInversion
+from lensless.hardware.trainable_mask import prep_trainable_mask
+from lensless import ADMM, UnrolledFISTA, UnrolledADMM, TrainableInversion
 from lensless.utils.dataset import (
     DiffuserCamMirflickr,
-    SimulatedFarFieldDataset,
-    SimulatedDatasetTrainableMask,
     DigiCamCelebA,
-    HITLDatasetTrainableMask,
+    HFDataset,
+    MyDataParallel,
+    simulate_dataset,
 )
 from torch.utils.data import Subset
-import lensless.hardware.trainable_mask
-from lensless.hardware.slm import full2subpattern
-from lensless.hardware.sensor import VirtualSensor
 from lensless.recon.utils import create_process_network
-from lensless.utils.image import rgb2gray, is_grayscale
-from lensless.utils.simulation import FarFieldSimulator
 from lensless.recon.utils import Trainer
 import torch
-from torchvision import transforms, datasets
-from lensless.utils.io import load_psf
 from lensless.utils.io import save_image
 from lensless.utils.plot import plot_image
-from lensless import ADMM
 import matplotlib.pyplot as plt
 
 # A logger for this file
 log = logging.getLogger(__name__)
 
 
-def simulate_dataset(config, generator=None):
-
-    if config.torch_device == "cuda" and torch.cuda.is_available():
-        device = "cuda"
-    else:
-        device = "cpu"
-
-    # -- prepare PSF
-    psf = None
-    if config.trainable_mask.mask_type is None or config.trainable_mask.initial_value == "psf":
-        psf_fp = os.path.join(get_original_cwd(), config.files.psf)
-        psf, _ = load_psf(
-            psf_fp,
-            downsample=config.files.downsample,
-            return_float=True,
-            return_bg=True,
-            bg_pix=(0, 15),
-        )
-        if config.files.diffusercam_psf:
-            transform_BRG2RGB = transforms.Lambda(lambda x: x[..., [2, 1, 0]])
-            psf = transform_BRG2RGB(torch.from_numpy(psf))
-
-        # drop depth dimension
-        psf = psf.to(device)
-
-    else:
-        # training mask / PSF
-        mask = prep_trainable_mask(config, psf)
-        psf = mask.get_psf().to(device)
-
-    # -- load dataset
-    pre_transform = None
-    transforms_list = [transforms.ToTensor()]
-    data_path = os.path.join(get_original_cwd(), "data")
-    if config.simulation.grayscale:
-        transforms_list.append(transforms.Grayscale())
-
-    if config.files.dataset == "mnist":
-        transform = transforms.Compose(transforms_list)
-        train_ds = datasets.MNIST(root=data_path, train=True, download=True, transform=transform)
-        test_ds = datasets.MNIST(root=data_path, train=False, download=True, transform=transform)
-    elif config.files.dataset == "fashion_mnist":
-        transform = transforms.Compose(transforms_list)
-        train_ds = datasets.FashionMNIST(
-            root=data_path, train=True, download=True, transform=transform
-        )
-        test_ds = datasets.FashionMNIST(
-            root=data_path, train=False, download=True, transform=transform
-        )
-    elif config.files.dataset == "cifar10":
-        transform = transforms.Compose(transforms_list)
-        train_ds = datasets.CIFAR10(root=data_path, train=True, download=True, transform=transform)
-        test_ds = datasets.CIFAR10(root=data_path, train=False, download=True, transform=transform)
-    elif config.files.dataset == "CelebA":
-        root = config.files.celeba_root
-        data_path = os.path.join(root, "celeba")
-        assert os.path.isdir(
-            data_path
-        ), f"Data path {data_path} does not exist. Make sure you download the CelebA dataset and provide the parent directory as 'config.files.celeba_root'. Download link: https://mmlab.ie.cuhk.edu.hk/projects/CelebA.html"
-        transform = transforms.Compose(transforms_list)
-        if config.files.n_files is None:
-            train_ds = datasets.CelebA(
-                root=root, split="train", download=False, transform=transform
-            )
-            test_ds = datasets.CelebA(root=root, split="test", download=False, transform=transform)
-        else:
-            ds = datasets.CelebA(root=root, split="all", download=False, transform=transform)
-
-            ds = Subset(ds, np.arange(config.files.n_files))
-
-            train_size = int((1 - config.files.test_size) * len(ds))
-            test_size = len(ds) - train_size
-            train_ds, test_ds = torch.utils.data.random_split(
-                ds, [train_size, test_size], generator=generator
-            )
-    else:
-        raise NotImplementedError(f"Dataset {config.files.dataset} not implemented.")
-
-    # convert PSF
-    if config.simulation.grayscale and not is_grayscale(psf):
-        psf = rgb2gray(psf)
-
-    # check if gpu is available
-    device_conv = config.torch_device
-    if device_conv == "cuda" and torch.cuda.is_available():
-        device_conv = "cuda"
-    else:
-        device_conv = "cpu"
-
-    # create simulator
-    simulator = FarFieldSimulator(
-        psf=psf,
-        is_torch=True,
-        **config.simulation,
-    )
-
-    # create Pytorch dataset and dataloader
-    crop = config.files.crop.copy() if config.files.crop is not None else None
-    if mask is None:
-        train_ds_prop = SimulatedFarFieldDataset(
-            dataset=train_ds,
-            simulator=simulator,
-            dataset_is_CHW=True,
-            device_conv=device_conv,
-            flip=config.simulation.flip,
-            vertical_shift=config.files.vertical_shift,
-            horizontal_shift=config.files.horizontal_shift,
-            crop=crop,
-            downsample=config.files.downsample,
-            pre_transform=pre_transform,
-        )
-        test_ds_prop = SimulatedFarFieldDataset(
-            dataset=test_ds,
-            simulator=simulator,
-            dataset_is_CHW=True,
-            device_conv=device_conv,
-            flip=config.simulation.flip,
-            vertical_shift=config.files.vertical_shift,
-            horizontal_shift=config.files.horizontal_shift,
-            crop=crop,
-            downsample=config.files.downsample,
-            pre_transform=pre_transform,
-        )
-    else:
-        if config.measure is not None:
-
-            train_ds_prop = HITLDatasetTrainableMask(
-                rpi_username=config.measure.rpi_username,
-                rpi_hostname=config.measure.rpi_hostname,
-                celeba_root=config.files.celeba_root,
-                display_config=config.measure.display,
-                capture_config=config.measure.capture,
-                mask_center=config.trainable_mask.ap_center,
-                dataset=train_ds,
-                mask=mask,
-                simulator=simulator,
-                dataset_is_CHW=True,
-                device_conv=device_conv,
-                flip=config.simulation.flip,
-                vertical_shift=config.files.vertical_shift,
-                horizontal_shift=config.files.horizontal_shift,
-                crop=crop,
-                downsample=config.files.downsample,
-                pre_transform=pre_transform,
-            )
-
-            test_ds_prop = HITLDatasetTrainableMask(
-                rpi_username=config.measure.rpi_username,
-                rpi_hostname=config.measure.rpi_hostname,
-                celeba_root=config.files.celeba_root,
-                display_config=config.measure.display,
-                capture_config=config.measure.capture,
-                mask_center=config.trainable_mask.ap_center,
-                dataset=test_ds,
-                mask=mask,
-                simulator=simulator,
-                dataset_is_CHW=True,
-                device_conv=device_conv,
-                flip=config.simulation.flip,
-                vertical_shift=config.files.vertical_shift,
-                horizontal_shift=config.files.horizontal_shift,
-                crop=crop,
-                downsample=config.files.downsample,
-                pre_transform=pre_transform,
-            )
-
-        else:
-
-            train_ds_prop = SimulatedDatasetTrainableMask(
-                dataset=train_ds,
-                mask=mask,
-                simulator=simulator,
-                dataset_is_CHW=True,
-                device_conv=device_conv,
-                flip=config.simulation.flip,
-                vertical_shift=config.files.vertical_shift,
-                horizontal_shift=config.files.horizontal_shift,
-                crop=crop,
-                downsample=config.files.downsample,
-                pre_transform=pre_transform,
-            )
-            test_ds_prop = SimulatedDatasetTrainableMask(
-                dataset=test_ds,
-                mask=mask,
-                simulator=simulator,
-                dataset_is_CHW=True,
-                device_conv=device_conv,
-                flip=config.simulation.flip,
-                vertical_shift=config.files.vertical_shift,
-                horizontal_shift=config.files.horizontal_shift,
-                crop=crop,
-                downsample=config.files.downsample,
-                pre_transform=pre_transform,
-            )
-
-    return train_ds_prop, test_ds_prop, mask
-
-
-def prep_trainable_mask(config, psf=None, downsample=None):
-    mask = None
-    color_filter = None
-    downsample = config.files.downsample if downsample is None else downsample
-    if config.trainable_mask.mask_type is not None:
-        mask_class = getattr(lensless.hardware.trainable_mask, config.trainable_mask.mask_type)
-
-        if config.trainable_mask.initial_value == "random":
-            if psf is not None:
-                initial_mask = torch.rand_like(psf)
-            else:
-                sensor = VirtualSensor.from_name(config.simulation.sensor, downsample=downsample)
-                resolution = sensor.resolution
-                initial_mask = torch.rand((1, *resolution, 3))
-        elif config.trainable_mask.initial_value == "psf":
-            initial_mask = psf.clone()
-        # if file ending with "npy"
-        elif config.trainable_mask.initial_value.endswith("npy"):
-            pattern = np.load(os.path.join(get_original_cwd(), config.trainable_mask.initial_value))
-
-            initial_mask = full2subpattern(
-                pattern=pattern,
-                shape=config.trainable_mask.ap_shape,
-                center=config.trainable_mask.ap_center,
-                slm=config.trainable_mask.slm,
-            )
-            initial_mask = torch.from_numpy(initial_mask.astype(np.float32))
-
-            # prepare color filter if needed
-            from waveprop.devices import slm_dict
-            from waveprop.devices import SLMParam as SLMParam_wp
-
-            slm_param = slm_dict[config.trainable_mask.slm]
-            if (
-                config.trainable_mask.train_color_filter
-                and SLMParam_wp.COLOR_FILTER in slm_param.keys()
-            ):
-                color_filter = slm_param[SLMParam_wp.COLOR_FILTER]
-                color_filter = torch.from_numpy(color_filter.copy()).to(dtype=torch.float32)
-
-                # add small random values
-                color_filter = color_filter + 0.1 * torch.rand_like(color_filter)
-        else:
-            raise ValueError(
-                f"Initial PSF value {config.trainable_mask.initial_value} not supported"
-            )
-
-        if config.trainable_mask.grayscale and not is_grayscale(initial_mask):
-            initial_mask = rgb2gray(initial_mask)
+@hydra.main(version_base=None, config_path="../../configs", config_name="train_unrolledADMM")
+def train_learned(config):
 
-        mask = mask_class(
-            initial_mask,
-            optimizer="Adam",
-            downsample=downsample,
-            color_filter=color_filter,
-            **config.trainable_mask,
+    if config.wandb_project is not None:
+        # start a new wandb run to track this script
+        wandb.init(
+            # set the wandb project where this run will be logged
+            project=config.wandb_project,
+            # track hyperparameters and run metadata
+            config=dict(config),
         )
 
-    return mask
-
-
-@hydra.main(version_base=None, config_path="../../configs", config_name="train_unrolledADMM")
-def train_unrolled(config):
-
     # set seed
     seed = config.seed
     torch.manual_seed(seed)
     np.random.seed(seed)
     generator = torch.Generator().manual_seed(seed)
 
     if config.start_delay is not None:
@@ -342,27 +82,34 @@
         print(f"\nScript will start at {start_time}")
         time.sleep(delay)
 
     save = config.save
     if save:
         save = os.getcwd()
 
-    if config.torch_device == "cuda" and torch.cuda.is_available():
-        log.info("Using GPU for training.")
-        device = "cuda"
+    use_cuda = False
+    if "cuda" in config.torch_device and torch.cuda.is_available():
+        # if config.torch_device == "cuda" and torch.cuda.is_available():
+        log.info(f"Using GPU for training. Main device : {config.torch_device}")
+        device = config.torch_device
+        use_cuda = True
     else:
         log.info("Using CPU for training.")
         device = "cpu"
+    device_ids = config.device_ids
+    if device_ids is not None:
+        log.info(f"Using multiple GPUs : {device_ids}")
 
     # load dataset and create dataloader
     train_set = None
     test_set = None
     psf = None
     crop = None
-    if "DiffuserCam" in config.files.dataset:
+    mask = None
+    if "DiffuserCam" in config.files.dataset and config.files.huggingface_dataset is False:
 
         original_path = os.path.join(get_original_cwd(), config.files.dataset)
         psf_path = os.path.join(get_original_cwd(), config.files.psf)
         dataset = DiffuserCamMirflickr(
             dataset_dir=original_path,
             psf_path=psf_path,
             downsample=config.files.downsample,
@@ -378,23 +125,14 @@
             test_indices = test_indices[: config.files.n_files]
 
         train_set = Subset(dataset, train_indices)
         test_set = Subset(dataset, test_indices)
 
         # -- if learning mask
         mask = prep_trainable_mask(config, dataset.psf)
-        if mask is not None:
-            # plot initial PSF
-            psf_np = mask.get_psf().detach().cpu().numpy()[0, ...]
-            if config.trainable_mask.grayscale:
-                psf_np = psf_np[:, :, -1]
-
-            save_image(psf_np, os.path.join(save, "psf_initial.png"))
-            plot_image(psf_np, gamma=config.display.gamma)
-            plt.savefig(os.path.join(save, "psf_initial_plot.png"))
 
         psf = dataset.psf
 
     elif "celeba_adafruit" in config.files.dataset:
 
         dataset = DigiCamCelebA(
             data_dir=os.path.join(get_original_cwd(), config.files.dataset),
@@ -423,87 +161,185 @@
         )
 
         # -- if learning mask
         downsample = config.files.downsample * 4  # measured files are 4x downsampled
         mask = prep_trainable_mask(config, dataset.psf, downsample=downsample)
 
         if mask is not None:
-            # plot initial PSF
-            with torch.no_grad():
-                psf_np = mask.get_psf().detach().cpu().numpy()[0, ...]
-                if config.trainable_mask.grayscale:
-                    psf_np = psf_np[:, :, -1]
-
-            save_image(psf_np, os.path.join(save, "psf_initial.png"))
-            plot_image(psf_np, gamma=config.display.gamma)
-            plt.savefig(os.path.join(save, "psf_initial_plot.png"))
-
-            # save original PSF as well
+            # save original PSF
             psf_meas = dataset.psf.detach().cpu().numpy()[0, ...]
             plot_image(psf_meas, gamma=config.display.gamma)
             plt.savefig(os.path.join(save, "psf_meas_plot.png"))
 
             with torch.no_grad():
                 psf = mask.get_psf().to(dataset.psf)
 
         else:
 
             psf = dataset.psf
 
-        # print info about PSF
-        log.info(f"PSF shape : {psf.shape}")
-        log.info(f"PSF min : {psf.min()}")
-        log.info(f"PSF max : {psf.max()}")
-        log.info(f"PSF dtype : {psf.dtype}")
-        log.info(f"PSF norm : {psf.norm()}")
+    elif config.files.huggingface_dataset is True:
+
+        split_train = "train"
+        split_test = "test"
+        if config.files.split_seed is not None:
+            from datasets import load_dataset, concatenate_datasets
+
+            seed = config.files.split_seed
+            generator = torch.Generator().manual_seed(seed)
+
+            # - combine train and test into single dataset
+            train_split = "train"
+            test_split = "test"
+            if config.files.n_files is not None:
+                train_split = f"train[:{config.files.n_files}]"
+                test_split = f"test[:{config.files.n_files}]"
+            train_dataset = load_dataset(config.files.dataset, split=train_split)
+            test_dataset = load_dataset(config.files.dataset, split=test_split)
+            dataset = concatenate_datasets([test_dataset, train_dataset])
+
+            # - split into train and test
+            train_size = int((1 - config.files.test_size) * len(dataset))
+            test_size = len(dataset) - train_size
+            split_train, split_test = torch.utils.data.random_split(
+                dataset, [train_size, test_size], generator=generator
+            )
+
+        train_set = HFDataset(
+            huggingface_repo=config.files.dataset,
+            psf=config.files.huggingface_psf,
+            split=split_train,
+            display_res=config.files.image_res,
+            rotate=config.files.rotate,
+            downsample=config.files.downsample,
+            downsample_lensed=config.files.downsample_lensed,
+            alignment=config.alignment,
+            save_psf=config.files.save_psf,
+            n_files=config.files.n_files,
+            simulation_config=config.simulation,
+        )
+        test_set = HFDataset(
+            huggingface_repo=config.files.dataset,
+            psf=config.files.huggingface_psf,
+            split=split_test,
+            display_res=config.files.image_res,
+            rotate=config.files.rotate,
+            downsample=config.files.downsample,
+            downsample_lensed=config.files.downsample_lensed,
+            alignment=config.alignment,
+            save_psf=config.files.save_psf,
+            n_files=config.files.n_files,
+            simulation_config=config.simulation,
+        )
+        if train_set.multimask:
+            # get first PSF for initialization
+            if device_ids is not None:
+                first_psf_key = list(train_set.psf.keys())[device_ids[0]]
+            else:
+                first_psf_key = list(train_set.psf.keys())[0]
+            psf = train_set.psf[first_psf_key].to(device)
+        else:
+            psf = train_set.psf.to(device)
+        crop = test_set.crop  # same for train set
+
+        # -- if learning mask
+        mask = prep_trainable_mask(config, psf)
+        if mask is not None:
+            assert not train_set.multimask
 
     else:
 
         train_set, test_set, mask = simulate_dataset(config, generator=generator)
         psf = train_set.psf
         crop = train_set.crop
 
+    if not hasattr(train_set, "multimask"):
+        train_set.multimask = False
+    if not hasattr(test_set, "multimask"):
+        test_set.multimask = False
+
     assert train_set is not None
-    assert psf is not None
+    # if not hasattr(test_set, "psfs"):
+    #     assert psf is not None
+
+    # print info about PSF
+    log.info(f"PSF shape : {psf.shape}")
+    log.info(f"PSF min : {psf.min()}")
+    log.info(f"PSF max : {psf.max()}")
+    log.info(f"PSF dtype : {psf.dtype}")
+    log.info(f"PSF norm : {psf.norm()}")
+
+    if config.files.extra_eval is not None:
+        # TODO only support Hugging Face DigiCam datasets for now
+        extra_eval_sets = dict()
+        for eval_set in config.files.extra_eval:
+
+            extra_eval_sets[eval_set] = HFDataset(
+                split="test",
+                downsample=config.files.downsample,  # needs to be same size
+                n_files=config.files.n_files,
+                simulation_config=config.simulation,
+                **config.files.extra_eval[eval_set],
+            )
 
     # reconstruct lensless with ADMM
     with torch.no_grad():
-        if config.test_idx is not None:
+        if config.eval_disp_idx is not None:
 
             log.info("Reconstruction a few images with ADMM...")
 
-            for i, _idx in enumerate(config.test_idx):
+            for i, _idx in enumerate(config.eval_disp_idx):
 
-                lensless, lensed = test_set[_idx]
+                if test_set.multimask:
+                    # multimask
+                    # lensless, lensed, _ = test_set[_idx]  # using wrong PSF
+                    lensless, lensed, psf = test_set[_idx]
+                    psf = psf.to(device)
+                else:
+                    lensless, lensed = test_set[_idx]
                 recon = ADMM(psf)
 
                 recon.set_data(lensless.to(psf.device))
                 res = recon.apply(disp_iter=None, plot=False, n_iter=10)
                 res_np = res[0].cpu().numpy()
                 res_np = res_np / res_np.max()
 
                 lensed_np = lensed[0].cpu().numpy()
 
                 lensless_np = lensless[0].cpu().numpy()
                 save_image(lensless_np, f"lensless_raw_{_idx}.png")
 
                 # -- plot lensed and res on top of each other
-                if config.training.crop_preloss:
+                cropped = False
+
+                if hasattr(test_set, "alignment"):
+                    if test_set.alignment is not None:
+                        res_np = test_set.extract_roi(res_np, axis=(0, 1))
+                    else:
+                        res_np, lensed_np = test_set.extract_roi(
+                            res_np, lensed=lensed_np, axis=(0, 1)
+                        )
+
+                    cropped = True
+
+                elif config.training.crop_preloss:
                     assert crop is not None
 
                     res_np = res_np[
                         crop["vertical"][0] : crop["vertical"][1],
                         crop["horizontal"][0] : crop["horizontal"][1],
                     ]
                     lensed_np = lensed_np[
                         crop["vertical"][0] : crop["vertical"][1],
                         crop["horizontal"][0] : crop["horizontal"][1],
                     ]
-                    if i == 0:
-                        log.info(f"Cropped shape :  {res_np.shape}")
+                    cropped = True
+
+                if cropped and i == 0:
+                    log.info(f"Cropped shape :  {res_np.shape}")
 
                 save_image(res_np, f"lensless_recon_{_idx}.png")
                 save_image(lensed_np, f"lensed_{_idx}.png")
 
                 plt.figure()
                 plt.imshow(lensed_np, alpha=0.4)
                 plt.imshow(res_np, alpha=0.7)
@@ -516,23 +352,25 @@
 
     # Load pre-process model
     pre_process, pre_process_name = create_process_network(
         config.reconstruction.pre_process.network,
         config.reconstruction.pre_process.depth,
         nc=config.reconstruction.pre_process.nc,
         device=device,
+        device_ids=device_ids,
     )
     pre_proc_delay = config.reconstruction.pre_process.delay
 
     # Load post-process model
     post_process, post_process_name = create_process_network(
         config.reconstruction.post_process.network,
         config.reconstruction.post_process.depth,
         nc=config.reconstruction.post_process.nc,
         device=device,
+        device_ids=device_ids,
     )
     post_proc_delay = config.reconstruction.post_process.delay
 
     if config.reconstruction.post_process.train_last_layer:
         for name, param in post_process.named_parameters():
             if "m_tail" in name:
                 param.requires_grad = True
@@ -576,39 +414,44 @@
             tk=config.reconstruction.unrolled_fista.tk,
             pad=True,
             learn_tk=config.reconstruction.unrolled_fista.learn_tk,
             pre_process=pre_process if pre_proc_delay is None else None,
             post_process=post_process if post_proc_delay is None else None,
             skip_unrolled=config.reconstruction.skip_unrolled,
             return_unrolled_output=True if config.unrolled_output_factor > 0 else False,
-        ).to(device)
+        )
     elif config.reconstruction.method == "unrolled_admm":
         recon = UnrolledADMM(
             psf,
             n_iter=config.reconstruction.unrolled_admm.n_iter,
             mu1=config.reconstruction.unrolled_admm.mu1,
             mu2=config.reconstruction.unrolled_admm.mu2,
             mu3=config.reconstruction.unrolled_admm.mu3,
             tau=config.reconstruction.unrolled_admm.tau,
             pre_process=pre_process if pre_proc_delay is None else None,
             post_process=post_process if post_proc_delay is None else None,
             skip_unrolled=config.reconstruction.skip_unrolled,
             return_unrolled_output=True if config.unrolled_output_factor > 0 else False,
-        ).to(device)
+        )
     elif config.reconstruction.method == "trainable_inv":
         recon = TrainableInversion(
             psf,
             K=config.reconstruction.trainable_inv.K,
             pre_process=pre_process if pre_proc_delay is None else None,
             post_process=post_process if post_proc_delay is None else None,
             return_unrolled_output=True if config.unrolled_output_factor > 0 else False,
-        ).to(device)
+        )
     else:
         raise ValueError(f"{config.reconstruction.method} is not a supported algorithm")
 
+    if device_ids is not None:
+        recon = MyDataParallel(recon, device_ids=device_ids)
+    if use_cuda:
+        recon.to(device)
+
     # constructing algorithm name by appending pre and post process
     algorithm_name = config.reconstruction.method
     if config.reconstruction.pre_process.network is not None:
         algorithm_name = pre_process_name + "_" + algorithm_name
     if config.reconstruction.post_process.network is not None:
         algorithm_name += "_" + post_process_name
 
@@ -645,16 +488,18 @@
         pre_process_unfreeze=config.reconstruction.pre_process.unfreeze,
         post_process=post_process,
         post_process_delay=post_proc_delay,
         post_process_freeze=config.reconstruction.post_process.freeze,
         post_process_unfreeze=config.reconstruction.post_process.unfreeze,
         clip_grad=config.training.clip_grad,
         unrolled_output_factor=config.unrolled_output_factor,
+        extra_eval_sets=extra_eval_sets if config.files.extra_eval is not None else None,
+        use_wandb=True if config.wandb_project is not None else False,
     )
 
     trainer.train(n_epoch=config.training.epoch, save_pt=save, disp=config.eval_disp_idx)
 
     log.info(f"Results saved in {save}")
 
 
 if __name__ == "__main__":
-    train_unrolled()
+    train_learned()
```

### Comparing `lensless-1.0.6/scripts/sim/dataset.py` & `lensless-1.0.7/scripts/sim/dataset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/digicam_psf.py` & `lensless-1.0.7/scripts/sim/digicam_psf.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/mask_dataset.py` & `lensless-1.0.7/scripts/sim/mask_dataset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/mask_single_file.py` & `lensless-1.0.7/scripts/sim/mask_single_file.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/single_file.py` & `lensless-1.0.7/scripts/sim/single_file.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/torch_custom_dataset.py` & `lensless-1.0.7/scripts/sim/torch_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/scripts/sim/torch_dataset.py` & `lensless-1.0.7/scripts/sim/torch_dataset.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/setup.py` & `lensless-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/test/test_algos.py` & `lensless-1.0.7/test/test_algos.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     for gray in [True, False]:
         psf, _ = load_data(
             psf_fp=psf_fp,
             data_fp=data_fp,
             downsample=downsample,
             plot=False,
             gray=gray,
-            torch=False,
+            use_torch=False,
         )
         recon = algorithm(psf)
         assert recon._initial_est is None
         random_init = np.random.rand(*recon._image_est_shape)
         recon._set_initial_estimate(random_init)
         assert isinstance(recon._initial_est, np.ndarray)
         assert np.allclose(recon._initial_est, random_init)
@@ -67,15 +67,15 @@
     for gray in [True, False]:
         psf, _ = load_data(
             psf_fp=psf_fp,
             data_fp=data_fp,
             downsample=downsample,
             plot=False,
             gray=gray,
-            torch=True,
+            use_torch=True,
         )
         recon = algorithm(psf)
         assert recon._initial_est is None
         random_init = torch.rand(*recon._image_est.shape)
         recon._set_initial_estimate(random_init)
         assert isinstance(recon._initial_est, torch.Tensor)
         assert np.allclose(recon._initial_est, random_init)
@@ -93,15 +93,15 @@
             psf, data = load_data(
                 psf_fp=psf_fp,
                 data_fp=data_fp,
                 downsample=downsample,
                 plot=False,
                 gray=gray,
                 dtype=dtype,
-                torch=False,
+                use_torch=False,
             )
             recon = algorithm(psf, dtype=dtype)
             recon.set_data(data)
             res = recon.apply(n_iter=_n_iter, disp_iter=None, plot=False)
             assert len(psf.shape) == 4
             assert psf.shape[3] == (1 if gray else 3)
             assert res.dtype == psf.dtype, f"Got {res.dtype}, expected {dtype}"
@@ -116,15 +116,15 @@
             psf, data = load_data(
                 psf_fp=psf_fp,
                 data_fp=data_fp,
                 downsample=downsample,
                 plot=False,
                 gray=gray,
                 dtype=dtype,
-                torch=True,
+                use_torch=True,
             )
             recon = algorithm(psf, dtype=dtype, n_iter=_n_iter)
             recon.set_data(data)
             res = recon.apply(disp_iter=None, plot=False)
             assert recon._n_iter == _n_iter
             assert len(psf.shape) == 4
             assert psf.shape[3] == (1 if gray else 3)
@@ -140,15 +140,15 @@
                         psf, data = load_data(
                             psf_fp=psf_fp,
                             data_fp=data_fp,
                             downsample=downsample,
                             plot=False,
                             gray=gray,
                             dtype=dtype,
-                            torch=False,
+                            use_torch=False,
                         )
                         recon = APGD(
                             psf,
                             dtype=dtype,
                             prox_penalty=prox_penalty,
                             diff_penalty=diff_penalty,
                             rel_error=None,
@@ -179,15 +179,15 @@
                 psf, n_iter=_n_iter, dtype=dtype, pre_process=pre_process, post_process=post_process
             )
 
             assert (
                 next(recon.parameters(), None) is not None
             ), f"{algorithm.__name__} has no trainable parameters"
 
-            res = recon.batch_call(data)
+            res = recon.forward(data)
             loss = torch.mean(res)
             loss.backward()
 
             assert (
                 data.shape[0] == res.shape[0]
             ), f"Batch dimension changed: got {res.shape[0]} expected {data.shape[0]}"
 
@@ -211,16 +211,16 @@
 
         def post_process(x, noise):
             return x
 
         recon = algorithm(
             psf, dtype=dtype, n_iter=_n_iter, pre_process=pre_process, post_process=post_process
         )
-        res1 = recon.batch_call(data1)
-        res2 = recon.batch_call(data2)
+        res1 = recon.forward(data1)
+        res2 = recon.forward(data2)
         recon.set_data(data2[0])
         res3 = recon.apply(disp_iter=None, plot=False)
 
         # main test
         torch.testing.assert_close(res1[0, 0, ...], res2[0, 0, ...])
         torch.testing.assert_close(res1[0, 0, ...], res3[0, ...])
         # small test
```

### Comparing `lensless-1.0.6/test/test_convolver.py` & `lensless-1.0.7/test/test_convolver.py`

 * *Files identical despite different names*

### Comparing `lensless-1.0.6/test/test_io.py` & `lensless-1.0.7/test/test_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     for is_torch in [True, False]:
         psf, data = load_data(
             psf_fp=psf_fp,
             data_fp=data_fp,
             downsample=downsample,
             plot=False,
             dtype="float32",
-            torch=is_torch,
+            use_torch=is_torch,
         )
         data = data[0]  # drop first depth dimension
 
         # try with 4D
         psf_gray = rgb2gray(psf, keepchanneldim=False)
         assert len(psf_gray.shape) == 3
         psf_gray = rgb2gray(psf, keepchanneldim=True)
```

### Comparing `lensless-1.0.6/test/test_masks.py` & `lensless-1.0.7/test/test_masks.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 dz = 4e-3
 
 
 def test_flatcam():
 
     mask1 = CodedAperture(
         method="MURA",
-        n_bits=25,
+        n_bits=23,
         resolution=resolution,
         feature_size=d1,
         distance_sensor=dz,
     )
     assert np.all(mask1.mask.shape == resolution)
 
     desired_psf_shape = np.array(tuple(resolution) + (len(mask1.psf_wavelength),))
@@ -39,20 +39,21 @@
 
     mask = PhaseContour(
         noise_period=(8, 8),
         resolution=resolution,
         feature_size=d1,
         distance_sensor=dz,
     )
-    assert np.all(mask.mask.shape == resolution)
+    assert np.all(mask.shape == resolution)
     desired_psf_shape = np.array(tuple(resolution) + (len(mask.psf_wavelength),))
     assert np.all(mask.psf.shape == desired_psf_shape)
 
+    u1 = mask.height_map_to_field(wavelength=mask.design_wv)
     Mp = np.sqrt(mask.target_psf) * np.exp(
-        1j * np.angle(fresnel_conv(mask.mask, mask.design_wv, d1, dz, dtype=np.float32)[0])
+        1j * np.angle(fresnel_conv(u1, mask.design_wv, d1, dz, dtype=np.float32)[0])
     )
     assert mse(abs(Mp), np.sqrt(mask.target_psf)) < 0.1
     assert psnr(abs(Mp), np.sqrt(mask.target_psf)) > 30
     assert abs(1 - ssim(abs(Mp), np.sqrt(mask.target_psf), channel_axis=None)) < 0.1
 
 
 def test_fza():
@@ -68,29 +69,29 @@
 def test_classmethod():
 
     downsample = 8
 
     mask1 = CodedAperture.from_sensor(
         sensor_name="rpi_hq", downsample=downsample, distance_sensor=dz
     )
-    assert np.all(mask1.mask.shape == resolution)
+    assert np.all(mask1.shape == resolution)
     desired_psf_shape = np.array(tuple(resolution) + (len(mask1.psf_wavelength),))
     assert np.all(mask1.psf.shape == desired_psf_shape)
 
     mask2 = PhaseContour.from_sensor(
         sensor_name="rpi_hq", downsample=downsample, distance_sensor=dz
     )
-    assert np.all(mask2.mask.shape == resolution)
+    assert np.all(mask2.shape == resolution)
     desired_psf_shape = np.array(tuple(resolution) + (len(mask2.psf_wavelength),))
     assert np.all(mask2.psf.shape == desired_psf_shape)
 
     mask3 = FresnelZoneAperture.from_sensor(
         sensor_name="rpi_hq", downsample=downsample, distance_sensor=dz
     )
-    assert np.all(mask3.mask.shape == resolution)
+    assert np.all(mask3.shape == resolution)
     desired_psf_shape = np.array(tuple(resolution) + (len(mask3.psf_wavelength),))
     assert np.all(mask3.psf.shape == desired_psf_shape)
 
 
 if __name__ == "__main__":
     test_flatcam()
     test_phlatcam()
```

### Comparing `lensless-1.0.6/test/test_sensor.py` & `lensless-1.0.7/test/test_sensor.py`

 * *Files identical despite different names*

