# Comparing `tmp/spiakid-simulation-1.20.tar.gz` & `tmp/spiakid_simulation-1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid-simulation-1.20.tar", last modified: Mon Mar 11 13:35:57 2024, max compression
+gzip compressed data, was "spiakid_simulation-1.21.tar", last modified: Tue May 14 08:51:26 2024, max compression
```

## Comparing `spiakid-simulation-1.20.tar` & `spiakid_simulation-1.21.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.285669 spiakid-simulation-1.20/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid-simulation-1.20/LICENSE
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid-simulation-1.20/MANIFEST.in
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1244 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid-simulation-1.20/README.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid-simulation-1.20/README_for_pip.md
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      657 2024-03-11 13:03:27.000000 spiakid-simulation-1.20/pyproject.toml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-03-11 13:35:57.285669 spiakid-simulation-1.20/setup.cfg
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.273669 spiakid-simulation-1.20/spiakid_simulation/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.273669 spiakid-simulation-1.20/spiakid_simulation/Example/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.277669 spiakid-simulation-1.20/spiakid_simulation/Example/Calib/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Calib/Trans.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2899 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Sim_10obj.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Sim_Gaussian.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4198 2024-03-11 12:55:42.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Sim_phase.ipynb
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4910 2024-03-11 12:55:54.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Sim_psf.ipynb
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.277669 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Template_10obj.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Template_Gaussian.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      939 2024-03-11 13:31:26.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Template_phase.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      652 2024-03-11 12:00:07.000000 spiakid-simulation-1.20/spiakid_simulation/Example/Template_psf.yaml
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17923 2024-03-11 13:31:31.000000 spiakid-simulation-1.20/spiakid_simulation/PhotonSimulator.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid-simulation-1.20/spiakid_simulation/Simulation.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid-simulation-1.20/spiakid_simulation/__init__.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.277669 spiakid-simulation-1.20/spiakid_simulation/electronics/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid-simulation-1.20/spiakid_simulation/electronics/Yaml_rw.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid-simulation-1.20/spiakid_simulation/electronics/cmplxIQ_params.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid-simulation-1.20/spiakid_simulation/electronics/data_reading.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6797 2024-03-08 10:33:27.000000 spiakid-simulation-1.20/spiakid_simulation/electronics/filter.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid-simulation-1.20/spiakid_simulation/electronics/resonator.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/IQ/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5248 2024-02-07 10:08:15.000000 spiakid-simulation-1.20/spiakid_simulation/functions/IQ/IQ_sim.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/noise/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4704 2024-03-08 08:20:26.000000 spiakid-simulation-1.20/spiakid_simulation/functions/noise/noise.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/output/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1619 2024-02-06 16:11:41.000000 spiakid-simulation-1.20/spiakid_simulation/functions/output/HDF5_creation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/phase/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid-simulation-1.20/spiakid_simulation/functions/phase/calib_read.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3828 2024-03-08 10:30:36.000000 spiakid-simulation-1.20/spiakid_simulation/functions/phase/phase_conversion.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/photon/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid-simulation-1.20/spiakid_simulation/functions/photon/black_body.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid-simulation-1.20/spiakid_simulation/functions/photon/contamination.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid-simulation-1.20/spiakid_simulation/functions/photon/photon_gen_image.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2787 2024-02-07 10:15:08.000000 spiakid-simulation-1.20/spiakid_simulation/functions/photon/rot.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6025 2024-03-11 12:36:09.000000 spiakid-simulation-1.20/spiakid_simulation/functions/photon/sim_image_photon.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/theory/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid-simulation-1.20/spiakid_simulation/functions/theory/Calc.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid-simulation-1.20/spiakid_simulation/functions/theory/MKID.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid-simulation-1.20/spiakid_simulation/functions/theory/SC.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/timeline/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2397 2024-03-08 10:06:00.000000 spiakid-simulation-1.20/spiakid_simulation/functions/timeline/timeline.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid-simulation-1.20/spiakid_simulation/functions/utils.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/functions/yaml/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid-simulation-1.20/spiakid_simulation/functions/yaml/yaml_rw.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/image_process/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2759 2024-02-26 13:53:15.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/PSF_interface.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/interface.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/interface_mult.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/test_displacement.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    13512 2024-03-11 09:04:27.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/turbulence.py
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3267 2024-02-08 16:13:39.000000 spiakid-simulation-1.20/spiakid_simulation/image_process/image_generation.py
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/spiakid_simulation.egg-info/
--rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1244 2024-03-11 13:35:57.000000 spiakid-simulation-1.20/spiakid_simulation.egg-info/PKG-INFO
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-03-11 13:35:57.000000 spiakid-simulation-1.20/spiakid_simulation.egg-info/SOURCES.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-03-11 13:35:57.000000 spiakid-simulation-1.20/spiakid_simulation.egg-info/dependency_links.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       63 2024-03-11 13:35:57.000000 spiakid-simulation-1.20/spiakid_simulation.egg-info/requires.txt
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-03-11 13:35:57.000000 spiakid-simulation-1.20/spiakid_simulation.egg-info/top_level.txt
-drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-03-11 13:35:57.281669 spiakid-simulation-1.20/test/
--rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid-simulation-1.20/test/test_simu.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10177 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/LICENSE
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      184 2024-02-15 13:53:03.000000 spiakid_simulation-1.21/MANIFEST.in
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1406 2024-02-08 10:38:39.000000 spiakid_simulation-1.21/README.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      643 2024-02-26 13:13:11.000000 spiakid_simulation-1.21/README_for_pip.md
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-05-14 08:39:56.000000 spiakid_simulation-1.21/pyproject.toml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       38 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/setup.cfg
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.406870 spiakid_simulation-1.21/spiakid_simulation/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.446870 spiakid_simulation-1.21/spiakid_simulation/Example/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.446870 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      125 2024-04-22 12:39:15.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Trans.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3627 2024-04-22 12:39:15.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3799 2024-04-23 11:59:54.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_ph_calib.csv
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4239 2024-03-11 12:55:11.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_10obj.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4538 2024-03-11 12:55:31.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_Gaussian.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4251 2024-05-14 08:30:04.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_phase.ipynb
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4910 2024-03-11 12:55:54.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Sim_psf.ipynb
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    42863 2024-02-15 13:48:36.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      665 2024-03-11 13:03:11.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_10obj.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      541 2024-03-11 12:10:32.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_Gaussian.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1091 2024-05-14 08:30:45.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_phase.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      652 2024-03-11 12:00:07.000000 spiakid_simulation-1.21/spiakid_simulation/Example/Template_psf.yaml
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    18211 2024-05-14 08:35:05.000000 spiakid_simulation-1.21/spiakid_simulation/PhotonSimulator.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      978 2024-02-26 13:07:20.000000 spiakid_simulation-1.21/spiakid_simulation/Simulation.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        0 2023-10-12 08:37:50.000000 spiakid_simulation-1.21/spiakid_simulation/__init__.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/electronics/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      523 2024-02-07 10:08:03.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/Yaml_rw.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    12011 2023-11-06 16:00:40.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/cmplxIQ_params.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      677 2023-11-07 14:19:59.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/data_reading.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     7406 2024-04-22 13:16:25.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/filter.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    53144 2023-11-06 15:58:05.000000 spiakid_simulation-1.21/spiakid_simulation/electronics/resonator.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/IQ/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5250 2024-05-14 08:38:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/IQ/IQ_sim.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/noise/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5029 2024-04-22 13:11:36.000000 spiakid_simulation-1.21/spiakid_simulation/functions/noise/noise.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/output/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2364 2024-04-23 09:17:38.000000 spiakid_simulation-1.21/spiakid_simulation/functions/output/HDF5_creation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/phase/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1507 2024-02-07 10:11:13.000000 spiakid_simulation-1.21/spiakid_simulation/functions/phase/calib_read.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     5319 2024-04-23 08:47:14.000000 spiakid_simulation-1.21/spiakid_simulation/functions/phase/phase_conversion.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/photon/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3431 2024-02-29 09:30:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/black_body.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      264 2023-11-02 10:55:48.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/contamination.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2512 2023-10-06 09:10:32.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/photon_gen_image.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     4573 2024-05-14 08:35:26.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/rot.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6529 2024-05-14 08:23:43.000000 spiakid_simulation-1.21/spiakid_simulation/functions/photon/sim_image_photon.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.478870 spiakid_simulation-1.21/spiakid_simulation/functions/theory/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     6198 2023-08-28 15:04:02.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/Calc.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14485 2023-09-18 12:50:04.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/MKID.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    10145 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/theory/SC.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/functions/timeline/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3249 2024-05-14 07:22:08.000000 spiakid_simulation-1.21/spiakid_simulation/functions/timeline/timeline.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      579 2023-08-28 10:56:06.000000 spiakid_simulation-1.21/spiakid_simulation/functions/utils.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/functions/yaml/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      522 2024-02-15 12:49:21.000000 spiakid_simulation-1.21/spiakid_simulation/functions/yaml/yaml_rw.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/image_process/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     2759 2024-05-13 13:42:02.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/PSF_interface.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    16411 2023-12-14 15:07:47.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    17502 2024-03-08 16:54:53.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface_mult.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     1732 2023-12-14 14:48:00.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/test_displacement.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)    14479 2024-05-13 13:40:17.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/turbulence.py
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3166 2024-05-14 08:14:01.000000 spiakid_simulation-1.21/spiakid_simulation/image_process/image_generation.py
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/spiakid_simulation.egg-info/
+-rw-r--r--   0 sfaes     (4303) sfaes     (2722)     1265 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/PKG-INFO
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)     3108 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)        1 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       69 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/requires.txt
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)       19 2024-05-14 08:51:26.000000 spiakid_simulation-1.21/spiakid_simulation.egg-info/top_level.txt
+drwxrwxr-x   0 sfaes     (4303) sfaes     (2722)        0 2024-05-14 08:51:26.482870 spiakid_simulation-1.21/test/
+-rw-rw-r--   0 sfaes     (4303) sfaes     (2722)      157 2023-09-18 12:50:04.000000 spiakid_simulation-1.21/test/test_simu.py
```

### Comparing `spiakid-simulation-1.20/LICENSE` & `spiakid_simulation-1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/PKG-INFO` & `spiakid_simulation-1.21/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.20
+Version: 1.21
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: pyyaml
 Requires-Dist: astropy
 Requires-Dist: scipy
 Requires-Dist: lmfit
 Requires-Dist: h5py
 Requires-Dist: spectral_cube
+Requires-Dist: ephem
 
 # Simulator of data for the project SPIAKID
 
 This project contains the **simulator of data** for the **SPIAKID** project.
 
 The **SPIAKID** (SpectroPhotometric Imaging in Astronomy with Kinetic Inductance Detectors) project aims at designing, building and deploying on the sky a spectrophotometric imager based on Kinetic Inductance detectors. More information can be found on the [SPIAKID project homepage](https://www.observatoiredeparis.psl.eu/spiakid.html).
```

### Comparing `spiakid-simulation-1.20/README.md` & `spiakid_simulation-1.21/README.md`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/README_for_pip.md` & `spiakid_simulation-1.21/README_for_pip.md`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/pyproject.toml` & `spiakid_simulation-1.21/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "spiakid-simulation"
-version = "1.20"
+version = "1.21"
 authors = [
     { name="Sebastien Faes", email="faesebastien@gmail.com"}
 ]
 description = "Data simulation of SPIAKID project"
 readme = "README_for_pip.md"
 requires-python = "<=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 
-dependencies = ["numpy","matplotlib","pyyaml","astropy","scipy","lmfit","h5py","spectral_cube"]
+dependencies = ["numpy","matplotlib","pyyaml","astropy","scipy","lmfit","h5py","spectral_cube","ephem"]
 
 [project.urls]
 "Homepage" = "https://spiakid.pages.obspm.fr/simulation/index.html"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv` & `spiakid_simulation-1.21/spiakid_simulation/Example/Calib/Wv_IQ_calib.csv`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Sim_10obj.ipynb` & `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_10obj.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Sim_Gaussian.ipynb` & `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_Gaussian.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Sim_phase.ipynb` & `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_phase.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933407738095238%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(9, 'plt.xlim([0,10])\\n'), (10, 'plt.ylim([0,10])\\n')]}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'test_sim'}, 'vscode': {'interpreter': {'hash': "*

 * *               "'dfb37601284865693e222cd633375a890560064f9bd2e85521c3342b21ec05f3'}}}"}*

```diff
@@ -68,14 +68,16 @@
                 "lbd = []\n",
                 "for i in range(len(sim.photon_dict)):\n",
                 "    x.append(sim.photon_dict[i][0])\n",
                 "    y.append(sim.photon_dict[i][1])\n",
                 "    lbd.append(sim.photon_dict[i][2])\n",
                 "plt.scatter(x,y,c=lbd)\n",
                 "plt.colorbar()\n",
+                "plt.xlim([0,10])\n",
+                "plt.ylim([0,10])\n",
                 "plt.title('Distribution of all photon')"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -151,15 +153,15 @@
                 "plt.xlabel('Time')\n",
                 "plt.ylabel('Filtered Phase')"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "sim_env",
+            "display_name": "test_sim",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
@@ -170,14 +172,14 @@
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
             "version": "3.10.12"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
-                "hash": "8670868e01929712f50dd97a406782e899e5f5ce47feda352077786530c2f839"
+                "hash": "dfb37601284865693e222cd633375a890560064f9bd2e85521c3342b21ec05f3"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Sim_psf.ipynb` & `spiakid_simulation-1.21/spiakid_simulation/Example/Sim_psf.ipynb`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G000M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT3750G100M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4000G050M250K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4125G300M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT4500G000P050K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5000G150M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5125G350M175K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5250G450M300K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT5875G000M075K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6625G350M025K200A000.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT6875G450M150K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G450M200K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7000G500M050K200A020.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT` & `spiakid_simulation-1.21/spiakid_simulation/Example/Spectrum/FT7250G500M225K200A040.DAT`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Template_10obj.yaml` & `spiakid_simulation-1.21/spiakid_simulation/Example/Template_10obj.yaml`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Template_Gaussian.yaml` & `spiakid_simulation-1.21/spiakid_simulation/Example/Template_Gaussian.yaml`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Template_phase.yaml` & `spiakid_simulation-1.21/spiakid_simulation/Example/Template_phase.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 # Simulation
 
-sim_file: Simulation_phase.hdf5
+sim_file: /spiakid/data/Simulation_Image/Simulation_phase_1obj.hdf5
 process_nb: 5
 
 1-Photon_Generation:
   telescope:
     exposition_time: 1
     diameter: 3.5
     obscuration: 1
     latitude: 25
-    transmittance: Calib/Trans.csv
+    transmittance: spiakid_simulation/Example/Calib/Trans.csv
     detector: 
       pix_nbr: 10
       pix_size: 0.5
   star:
     number: 1
     distance: 
       min: 5
-      max: 15
+      max: 7
     wavelength_array: 
       min: 0.4
       max: 0.8
       nbr: 40
-    spectrum_folder: Spectrum
+    spectrum_folder: spiakid_simulation/Example/Spectrum
   sky:
     method: Simulation
     contamination: False
     rotation: True
     fov_method: fix
     guide:
       alt: 5
       az: 20
   PSF:
     method: turbulence
     pix_nbr: 50
-    size: 1
-    seeing: 1
-    wind: 10
+    size: 0.5
+    seeing: 0.5
+    wind: 50
     L0: 30.
+    file: psf.fits
 
 2-Timeline:
   point_nb: 1000000
 
 3-Phase:
-  Calib_File: Calib/Wv_ph_calib.csv
+  Calib_File: spiakid_simulation/Example/Calib/Wv_ph_calib.csv
   Phase_Noise: 10
   Decay: 33000.0
   Readout_Noise:
-    scale: 2
+    scale: 0.5
     type: Gaussian
   Phase: true
 
 4-Electronic:
   nperseg: 4000
   template_time: 0.004
   trigerinx: 1000
   point_nb: 4000
-  save_file: Amp_2.csv
 
+
+
+5-Output:
+  save: 'photon_list'
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Example/Template_psf.yaml` & `spiakid_simulation-1.21/spiakid_simulation/Example/Template_psf.yaml`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/PhotonSimulator.py` & `spiakid_simulation-1.21/spiakid_simulation/PhotonSimulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from pathlib import Path
 from scipy import signal as sg
 from scipy import interpolate
 import pickle
 from astropy.io import fits
 from scipy import interpolate
-import time
+
 import spiakid_simulation.functions.output.HDF5_creation as hdf
 import spiakid_simulation.functions.yaml.yaml_rw as yml
 import spiakid_simulation.functions.noise.noise as N
 import spiakid_simulation.functions.timeline.timeline as Tl
 import spiakid_simulation.functions.phase.phase_conversion as Ph
 import spiakid_simulation.functions.phase.calib_read as Cr
 import spiakid_simulation.functions.IQ.IQ_sim as IQ
@@ -42,21 +42,21 @@
     def __init__(self, yaml_path):
 
 
         # Reading all config in the yaml
         self.config = yml.read_yaml(yaml_path)
         path = self.type_variable(self.config['sim_file'],'sim_file',[str])
         process_nb = self.type_variable(self.config['process_nb'],'process_nb',[int])
-        start = time.time()
+ 
         if Path(path).exists():
-                print('Simulation exist')   # The name given to the simulation is already taken
+                # print('Simulation exist')   # The name given to the simulation is already taken
                 self.result = Re.load_dict_from_hdf5(path)
 
         else:
-            print('Creating the simulation')
+            # print('Creating the simulation')
                 
             sim_config = self.config['1-Photon_Generation']
 
             telescope = sim_config['telescope']
             pix_size = self.type_variable(telescope['detector']['pix_size'], 'pix_size',[float,int])
             exposure_time = self.type_variable(telescope['exposition_time'],'exposition_time',[float,int])
             pix_nbr = self.type_variable(telescope['detector']['pix_nbr'],'detector pix_nbr',[int])
@@ -68,102 +68,94 @@
             star = sim_config['star']
             nb_object = self.type_variable(star['number'],'number',[int])
             distance =  (self.type_variable(star['distance']['min'],'distance_min',[float,int]) ,self.type_variable(star['distance']['max'],'distance_max',[float,int]))
             spectrum = self.type_variable(star['spectrum_folder'],'spectrum_folder',[str])
             wavelength_array = np.linspace(self.type_variable(star['wavelength_array']['min'],'wv_min',[float,int]), self.type_variable(star['wavelength_array']['max'],'wv_max',[float,int]), self.type_variable(star['wavelength_array']['nbr'],'wv_nbr',[int]))
             
             sky = sim_config['sky']
-            sky_method = self.type_variable(sky['method'],'sky_method',[str])
+            
             alt = self.type_variable(sky['guide']['alt'],'altitude',[float,int]) * np.pi / 180 
             az = self.type_variable(sky['guide']['az'],'azimuth',[float,int]) * np.pi / 180
-            contamination = self.type_variable(sky['contamination'],'contamination',[bool])
+
             rotation = self.type_variable(sky['rotation'],'rotation',[bool])
 
-            if self.type_variable(sky['fov_method'],'fov_method',[str]) == 'fix':
-                sky_fov = pix_size
-            elif self.type_variable(sky['fov_method'],'fov_method',[str]) == 'time_dep':
-                sky_fov = int(pix_size + exposure_time/100)   # A revoir !
-            else:
-                print('sky FOV is not defined')
 
                 
             #   Creation of stars with their spectrum
-            self.star_pos,self.star_spec = IG.image_sim(Image_size=int(pix_nbr/pix_size*sky_fov), object_number=nb_object, distance=distance, Path_file=path,Wavelength=wavelength_array,spectrum = spectrum,save = False)
+            self.star_pos,self.star_spec = IG.image_sim(Image_size=int(pix_nbr/pix_size), object_number=nb_object, distance=distance, Path_file=path,Wavelength=wavelength_array,spectrum = spectrum,save = False)
 
             rot = np.zeros(len(self.star_pos),dtype = object)
             alt_ev = np.zeros(len(self.star_pos),dtype = object)
-
+            
             #   Rotation effect
             if rotation == True:
-                end = time.time()
-                print('Earth rotation effect',end-start)
+               
+                # print('Earth rotation effect')
                 coo_guide = [alt,az]
                 for st in range(len(self.star_pos)):
-                    rot[st],alt_ev[st] =Rot.rotation(lat_tel=latitude,coo_guide=coo_guide,coo_star=self.star_pos[st], time = exposure_time,size=pix_nbr)
+                    rot[st],alt_ev[st],alt_az_t,ra_dec_t,ang =Rot.rotation(lat_tel=latitude,coo_guide=coo_guide,coo_star=self.star_pos[st], time = exposure_time,size=pix_nbr)
 
             else:
                 for st in range(len(self.star_pos)):
                     rot[st] = [interpolate.interp1d([0,exposure_time],[self.star_pos[st][1],self.star_pos[st][1]]),interpolate.interp1d([0,exposure_time],[self.star_pos[st][2],self.star_pos[st][2]])]
                     alt_ev[st] = interpolate.interp1d([0,exposure_time],[np.pi/2,np.pi/2])
-                
+                    alt_az_t =[alt,az,0]
+                    ra_dec_t = [0,0,0]
+                    ang = 0
 
                     
             try: trans_Path = self.type_variable(telescope['transmittance'],'transmittance',[str])
             except: trans_Path = False
 
             #   Creation of photons
             self.photon_list = SI.photon(wavelength_array,self.star_spec,exposure_time,tel_diam,process_nb,trans_Path)   
                 
                 #   Point Source Function
             try: sim_config['PSF']
             except:
-                print('No PSF -> Point')
+                # print('No PSF -> Point')
                 psf_grid = np.zeros(shape = (pix_nbr,pix_nbr,len(wavelength_array)))
                 psf_grid[int(pix_nbr/2),int(pix_nbr/2),:] = 1
                 point = np.linspace(0,1,pix_nbr)
                 psf = interpolate.RegularGridInterpolator((point,point,wavelength_array),psf_grid)
                 psf_pix_nbr = pix_nbr
                 psf_size = pix_size * pix_nbr
                 self.psf_visu = psf_grid
             else:
                 turb = sim_config['PSF']
                 if self.type_variable(sim_config['PSF']['method'],'method',[str]) == 'turbulence':
-                    end = time.time()
-                    print('PSF computing',end-start) 
+                    
                     seeing = self.type_variable(turb['seeing'],'seeing',[float,int])
                     wind = self.type_variable(turb['wind'],'wind',[float,int,tuple,list])
                     L0 = self.type_variable(turb['L0'],'L0',[float,int])
                     psf_size = self.type_variable(turb['size'],'psf size',[float,int])
                     psf_pix_nbr = self.type_variable(turb['pix_nbr'],'psf pix_nbr',[int])
                     try: save_link = turb['file'] 
                     except: save_link = 0
                     if np.shape(wind)==():
-                        self.psf_visu = Tf.PSF_creation(psf_size, psf_pix_nbr, wavelength_array, seeing, wind, tel_diam, obscuration, L0,exposure_time,save_link)
+                        self.psf_visu = Tf.PSF_creation(psf_size, psf_pix_nbr, wavelength_array, seeing, wind, tel_diam, obscuration, L0,exposure_time,process_nb,save_link)
                     else:
                         coeff = self.type_variable(turb['coeff'],'coeff',[list,tuple])
                         self.psf_visu = Tf.PSF_creation_mult(psf_size, psf_pix_nbr,  wavelength_array, seeing, wind, tel_diam, obscuration, L0,exposure_time,coeff,save_link)
                 elif self.type_variable(sim_config['PSF']['method'],'method',[str]) == 'Download': 
                         file = fits.open(self.type_variable(turb['file'],'PSF_file',[str]))[0]
                         self.psf_visu = file.data
                         list_axis = [file.header['NAXIS1'],file.header['NAXIS2'],file.header['NAXIS3']]
                         if (list_axis.count(file.header['NAXIS1']) == 2)  and (file.header['CUNIT1'] == 'arcsec'):
                             psf_pix_nbr = file.header['NAXIS1']
                             psf_size = psf_pix_nbr * file.header['CDELT1']
                         else:
                             if file.header['CUNIT2'] == 'arcsec':
                                 psf_pix_nbr =file.header['NAXIS2']
                                 psf_size = psf_pix_nbr * file.header['CDELT2']
-                            else:
-                                 print('Spatial dimension unit have to be arcsec')
-             
-
-                points = np.linspace(0,1,psf_pix_nbr)
-                psf = interpolate.RegularGridInterpolator((points,points,wavelength_array),self.psf_visu)
-            end = time.time()
-            print('Computing position',end-start)
+                            # else:
+                            #      print('Spatial dimension unit have to be arcsec')
+                Points = np.linspace(0,1,psf_pix_nbr)
+                psf = interpolate.RegularGridInterpolator((Points,Points,wavelength_array),self.psf_visu)
+      
             # Computing position of photon on the PSF 
             max_psf = []
        
             max_point = np.linspace(0,len(wavelength_array)-1,len(wavelength_array))
             for i in range(len(max_point)): max_psf.append(np.max(self.psf_visu[:,:,i])+0.01)
             # we add 0.01 to be sure to be above
            
@@ -173,14 +165,16 @@
             self.photon_dict_on_PSF = SI.photon_pos_on_PSF(self.star_pos, self.photon_list, psf, np.shape(self.psf_visu)[0],max_func, process_nb)
             lam0 = (max(wavelength_array)+min(wavelength_array))/2
             psf2detect = psf_pix_nbr / psf_size
          
             self.photon_dict = SI.photon_proj(self.photon_dict_on_PSF,self.star_pos,psf2detect,rot,alt_ev,pix_nbr,pix_size,lam0)
         
             self.wavelength, self.time = SI.detector_scale(detector_dim=detector_dim, photon_dict=self.photon_dict)
+
+            # self.calib_dict = SI.photon_calib(detector_dim, [star['wavelength_array']['min'],star['wavelength_array']['max']]) 
             
 
         
 
             # Do we want to simulate the phase or IQ ?
             try:self.config['3-Phase']
             except:
@@ -189,45 +183,47 @@
                 # We don't want to simulate nor the phase neither IQ
                 except: pass
                 # We want to simulate IQ
                 else:
                     #   NOT UPDATED
                     # Creation of the Timeline
                     point_nb = self.type_variable(self.config['2-Timeline']['point_nb'],'point_nb',[int])
-                    print('Timeline creation')
+                    # print('Timeline creation')
                     self.photon_timeline = Tl.sorting(exposure_time,self.wavelength,point_nb,self.time, process_nb) 
+                    self.photon_timeline_calib = Tl.sorting_calib(detector_dim,point_nb,[star['wavelength_array']['min'],star['wavelength_array']['max']])
                     self.IQ_Compute(obj = '3-IQ')
 
             else:
 
                 # Creation of the Timeline
                 point_nb = self.type_variable(self.config['2-Timeline']['point_nb'],'point_nb',[int])
-                end = time.time()
-                print('Timeline creation',end-start)
+              
                 self.photon_timeline = Tl.sorting(exposure_time,self.wavelength,point_nb,self.time, process_nb) 
+                self.photon_timeline_calib = Tl.sorting_calib(detector_dim,point_nb,[star['wavelength_array']['min'],star['wavelength_array']['max']])
+                # print('Phase')
                 self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=self.photon_timeline, nb_process=process_nb, Filter = False)
              
             try:self.config['4-Electronic']
             except:
                 pass
             else:
                 wavelength, photon_time = np.zeros(detector_dim,dtype = float), np.zeros(detector_dim, dtype = float)
                 photon_timeline = Tl.sorting(exposure_time,wavelength,point_nb,photon_time, process_nb)
                 self.phase_compute(detector_dim=detector_dim,obj = '3-Phase',timeline=photon_timeline, nb_process=process_nb,Filter = True)
 
             try: self.config['5-Output']['save']
             except: pass
             else:
                 if self.type_variable(self.config['5-Output']['save'],'save',[str]) == 'Simulation':
-                    print('Saving in HDF5 at: ' + str(path))
+                    # print('Saving in HDF5 at: ' + str(path))
                     hdf.save_dict_to_hdf5(self.config, path,self,pix_nbr)
 
                 elif self.type_variable(self.config['5-Output']['save'],'save',[str]) == 'photon_list':
-                    print('Saving the photon list at:' +str(path))
-                    hdf.save_photon_list(path,self.config, self.fil_phase,self.filtered_noise)
+                    # print('Saving the photon list at:' +str(path))
+                    hdf.save_photon_list(path,self.config, self.fil_phase,self.filtered_noise,alt_az_t,ra_dec_t,self.fil_phase_calib,ang)
 
 
 
 
     def phase_compute(self, detector_dim, obj, timeline, nb_process, Filter = False):
 
             # Reading convertion coeff
@@ -250,35 +246,36 @@
                         conv_phase.append(self.config[obj]['Conv_phase'])
             phase_noise = self.type_variable(self.config[obj]['Phase_Noise'],'Phase_noise',[float,int])
             decay = - self.type_variable(self.config[obj]['Decay'],'Decay',[float,int])
             
             #Conversion photon to phase
             if Filter == False:
        
-                print('Computing phase')
+                # print('Computing phase')
                 self.phase_conversion = Ph.phase_conv(timeline,pix = pix,conv_wv=conv_wv, conv_phase=conv_phase, resolution = phase_noise, process_nb=nb_process)
-              
+                self.phase_conversion_calib = Ph.phase_conv_calib(self.photon_timeline_calib,pix,conv_wv,conv_phase,phase_noise, nb_process)
                 #Adding exponential
                 self.phase_exp = Ph.exp_adding(self.phase_conversion, decay, nb_process)
-
+                self.phase_exp_calib = Ph.exp_adding_calib(self.phase_conversion_calib, decay, nb_process)
                 # Adding Noise
                 if self.config[obj]['Readout_Noise']['type'] == 'Gaussian':
                     phase = np.copy(self.phase_exp)
-                  
+                    
                     scale = self.type_variable(self.config[obj]['Readout_Noise']['scale'],'scale',[float,int])
                     self.phase =  N.gaussian(phase,scale=scale)
+                    self.phase_calib =  N.gaussian_calib(self.phase_exp_calib,scale=scale)
                 elif self.config[obj]['Readout_Noise']['type'] == 'Poisson':
                     phase = np.copy(self.phase_exp)
                     self.phase = N.poisson(phase)
                 else:
                     pass
             
             elif Filter == True:
             
-                print('Filtering the phase')
+                # print('Filtering the phase')
                 try: self.config['4-Electronic']['file']
                 except: 
                     self.noise = Ph.phase_conv(timeline,pix = pix,conv_wv=conv_wv, conv_phase=conv_phase, resolution = phase_noise, process_nb=nb_process)
                     # Adding Noise
                     if self.config[obj]['Readout_Noise']['type'] == 'Gaussian':
                         phase = np.copy(self.noise)
                         scale = self.type_variable(self.config[obj]['Readout_Noise']['scale'],'scale',[float,int])
@@ -311,14 +308,15 @@
                         file.close
                 else: 
                     file = open(self.config['4-Electronic']['file'],'rb')
                     self.filter,self.filtered_noise= pickle.load(file)
                     file.close()
  
                 self.fil_phase = Fi.filtering(self.phase,self.filter, nb_process)
+                self.fil_phase_calib = Fi.filtering_calib(self.phase_calib,self.filter,nb_process)
 
 
      
     
     def IQ_Compute(self,obj):
 
             try: self.config[obj]['Calib_file_csv']
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/Simulation.py` & `spiakid_simulation-1.21/spiakid_simulation/Simulation.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/electronics/Yaml_rw.py` & `spiakid_simulation-1.21/spiakid_simulation/electronics/Yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/electronics/cmplxIQ_params.py` & `spiakid_simulation-1.21/spiakid_simulation/electronics/cmplxIQ_params.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/electronics/data_reading.py` & `spiakid_simulation-1.21/spiakid_simulation/electronics/data_reading.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/electronics/filter.py` & `spiakid_simulation-1.21/spiakid_simulation/electronics/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,8 +168,27 @@
     for i,j,result in res:
          _,_,value = result.get()
          sig[i,j] = value
     
     pool.close()
     pool.join()
 
-    return(sig)
+    return(sig)
+
+
+def filtering_calib(data,filter,nb_process):
+    dim = np.shape(data[0][1])
+    sig_calib = []
+
+    for wv in range(len(data)):
+        pool = mp.Pool(nb_process)
+        res = []
+        sig = np.zeros_like(data[wv][1],dtype = object)
+        for i in range(dim[0]):
+            for j in range(dim[1]):
+                results = pool.apply_async(par_filtering,args=(data[wv][1][i,j],filter[i,j],i,j))
+                res.append((i,j,results))
+        for i,j,result in res:
+            _,_,value = result.get()
+            sig[i,j] = value
+        sig_calib.append([data[wv][0],sig])
+    return(sig_calib)
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/electronics/resonator.py` & `spiakid_simulation-1.21/spiakid_simulation/electronics/resonator.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/IQ/IQ_sim.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/IQ/IQ_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         I for each photon on each pixel
     
     Q: array
         Q for each photon on each pixel
     
     """
     dim = np.shape(Photon)
-    print(dim)
+    # print(dim)
     I,Q = np.zeros(dim,dtype = object),np.zeros(dim,dtype = object)
     
     IQ_dict = read_csv(Path,sep='/')
    
     
     for i in range(dim[0]):
         for j in range(dim[1]):
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/noise/noise.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/noise/noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,24 @@
         for i in range(dim[0]):
             for j in range(dim[1]):
                 signal[i,j] = np.zeros(np.shape(x[i,j]))
                 signal[i,j][0] = x[i,j][0]
                 signal[i,j][1] = x[i,j][1] + rand.normal(loc = 0,scale = scale, size = len(x[i,j][1]))
     return(signal)
 
+def gaussian_calib(data,scale):
+    
+    dim = np.shape(data[0][1])
+    for wv in range(len(data)):
+        for i in range(dim[0]):
+            for j in range(dim[1]):
+                data[wv][1][i,j][1] = np.array(data[wv][1][i,j][1]) + rand.normal(loc = 0,scale = scale, size = len(data[wv][1][i,j][1]))
+
+    return(data)
+
 def poisson(x):
     r""" Add Poisson noise on the signal
 
     Parameters:
     -----------
 
     x: array
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/output/HDF5_creation.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/output/HDF5_creation.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,18 +31,28 @@
         for j in range(size):
             h5file['wavelength/'+str(i)+'_'+str(j)] = sim.wavelength[i,j]
             h5file['time/'+str(i)+'_'+str(j)] = sim.time[i,j]
             h5file['phase/'+str(i)+'_'+str(j)] = sim.phase[i,j]
 
     
 
-def save_photon_list(filename,dic,filtered_signal,noise):
+def save_photon_list(filename,dic,filtered_signal,noise,alt_az_t,ra_dec_t,filtered_calib,ang):
     h5file = h5py.File(filename, 'w')
     recursively_save_dict_contents_to_group(h5file, '/', dic)
     size, _ = np.shape(filtered_signal)
-    
+    wv_step = np.linspace(start = dic['1-Photon_Generation']['star']['wavelength_array']['min']+0.05,stop = dic['1-Photon_Generation']['star']['wavelength_array']['max']-0.05, num = 3)
+    h5file['Coord/alt_az'] = alt_az_t
+    h5file['Coord/ra_dec'] = ra_dec_t
+    h5file['Coord/ang'] = ang
     for i in range(size):
         for j in range(size):
             m_noise = max(noise[i,j][1])
             peaks, _ = find_peaks(filtered_signal[i,j][1],prominence = 10, height=m_noise)
             h5file['Photons/'+str(i)+'_'+str(j)]  = [np.float32(filtered_signal[i,j][0][peaks]), np.float32(filtered_signal[i,j][1][peaks])]
+    for wv in range(len(wv_step)):
+        for i in range(size):
+            for j in range(size):
+                m_noise = max(noise[i,j][1])
+                peaks, _ = find_peaks(filtered_calib[wv][1][i,j][1],prominence = 10, height=m_noise)
+                h5file['Calib/'+str(wv_step[wv])+'/'+str(i)+'_'+str(j)]  = [np.float32(filtered_calib[wv][1][i,j][0][peaks]), np.float32(filtered_calib[wv][1][i,j][1][peaks])]
+
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/phase/calib_read.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/phase/calib_read.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/phase/phase_conversion.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/phase/phase_conversion.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,14 +47,37 @@
         _,_,value = result.get()
         signal[i,j] = value
     pool.close()
     pool.join()
     return(signal)
 
 
+def phase_conv_calib(data,pix,conv_wv,conv_phase,resolution, process_nb):
+    signal_calib = []
+    dim_x,dim_y = np.shape(data[0][1])
+    dict = {}
+    for i in range(len(pix)):
+        dict[pix[i]] = [conv_wv[i],conv_phase[i]]
+    for wv in range(len(data)):
+        signal = np.zeros(shape=(dim_x,dim_y),dtype = object)
+        pool = mp.Pool(process_nb)
+        res = []
+        for i in range(dim_x):
+            for j in range(dim_y):
+                results = pool.apply_async(photon2phase,args=(data[wv][1][i,j],dict[str(i)+'_'+str(j)][0],dict[str(i)+'_'+str(j)][1], resolution,i,j))
+                res.append((i,j,results))
+        for i,j,result in res:
+            _,_,value = result.get()
+            signal[i,j] = value
+        pool.close()
+        pool.join()
+        signal_calib.append([wv,signal])
+
+    return(signal_calib)
+
 def photon2phase(Photon,conv_wv,conv_phase, resolution,i,j):
     r"""Convert the wavelength in phase
 
     Parameters:
     -----------
 
     Photon: array
@@ -113,14 +136,33 @@
     for i,j,result in res:
         _,_,value = result.get()
         signal[i,j] = value
     pool.close()
     pool.join()
     return(signal)
 
+def exp_adding_calib(data,decay,process_nb):
+    signal_calib = []
+    dim = np.shape(data[0][1])
+    for wv in range(len(data)):
+        pool = mp.Pool(process_nb)
+        res = []
+        signal = np.zeros(dim,dtype = object)
+        for i in range(dim[0]):
+            for j in range(dim[1]):
+                results = pool.apply_async(exp, args=(data[wv][1][i,j],decay,i,j))
+                res.append((i,j,results))
+        for i,j,result in res:
+            _,_,value = result.get()
+            signal[i,j] = value
+          
+        pool.close()
+        pool.join()
+        signal_calib.append([data[wv][0],signal])
+    return(signal_calib)
 
 def exp(sig,decay,i,j):
     r""" Add the exponential decay after the photon arrival
 
     Parameters:
     -----------
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/photon/black_body.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/photon/black_body.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/photon/photon_gen_image.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/photon/photon_gen_image.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/photon/rot.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/photon/rot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,51 @@
 import numpy as np
 from scipy import interpolate
+from astropy.coordinates import SkyCoord, EarthLocation, Angle, ICRS, FK5
+from astropy.timeseries import TimeSeries
+from astropy.time import Time
+from astropy import units as u
 
 
+
+def ParallacticAngle(locationAltAz, time, location,locationFK5):
+  a = locationAltAz.az.radian - np.pi
+  z = np.pi/2 - locationAltAz.alt.radian
+  
+  SiderealTime = Time(time,location = location).sidereal_time('mean').radian
+  # print(SiderealTime,locationFK5.ra.radian)
+  H = SiderealTime - locationFK5.ra.radian
+  cosS = np.cos(a)*np.cos(H)+np.sin(a)*np.sin(H)*np.sin(location.lat.radian)
+  
+  if z > np.pi*0.01:
+    sinS=np.cos(location.lat.radian)*np.sin(H)/np.sin(z)
+  else:
+    sinS=np.cos(location.lat.radian)*np.sin(a)/np.cos(locationFK5.dec.radian)
+  ParaAngle = np.arctan2(sinS,cosS)
+  return np.degrees(ParaAngle)
+
 def rotation(lat_tel,coo_guide,coo_star,time,size):
   # omega = -7.2921 * 10 **-5 # radian/sec
-  omega = 7.292115 * 10**-5 
-  t = np.linspace(0,time,time * 10)
+  omega = -7.292115 * 10**-5 
+  
+  loc = EarthLocation(lon = -17.89*u.deg,lat =lat_tel*u.rad, height = 2200*u.m)
+  # print(loc.lon)
+  t = np.linspace(0,time,time+1 )
+  period = TimeSeries(time_start='2020-01-01 20:00:00',time_delta = 1*u.s,n_samples =len(t))
   alt, az = coo_guide
   X0, Y0, Z0 = [np.cos(alt)*np.cos(az), -np.cos(alt)*np.sin(az), np.sin(alt)]
   coo_guide = np.array([X0,Y0,Z0])
   # print('coo_guide: ',coo_guide)
   R_inv = np.array([[-X0*Z0/np.sqrt((X0**2+Y0**2)*(X0**2+Y0**2+Z0**2)), Y0/np.sqrt(X0**2+Y0**2), X0/np.sqrt(X0**2+Y0**2+Z0**2)],
                   [-Y0*Z0/np.sqrt((X0**2+Y0**2)*(X0**2+Y0**2+Z0**2)), -X0/np.sqrt(X0**2+Y0**2), Y0/np.sqrt(X0**2+Y0**2+Z0**2)],
                   [np.sqrt(X0**2+Y0**2)/np.sqrt((X0**2+Y0**2+Z0**2)), 0, Z0/np.sqrt(X0**2+Y0**2+Z0**2)]])
   new_pos_x = np.zeros(len(t))
   new_pos_y = np.zeros(len(t))
   alt_ev = np.zeros(len(t))
+  alt_az_guide = []
   for i in range (len(t)):
     normalisation = 2 * size
     coo = [coo_star[1]/normalisation,coo_star[2]/normalisation]
 
     z = np.sqrt(1-coo[0]**2 - coo[1]**2)
 
     coo.append(z)
@@ -37,15 +63,17 @@
                 [(1-np.cos(theta))*np.cos(lat_tel)*np.sin(lat_tel), np.cos(lat_tel)*np.sin(theta), np.sin(lat_tel)**2+np.cos(lat_tel)**2*np.cos(theta)]])
 
     pos_guide_t = Up@coo_guide
     pos_star_t = Up@coo_star_XYZ
     X0_t = pos_guide_t[0]
     Y0_t = pos_guide_t[1]
     Z0_t = pos_guide_t[2]
-
+    new_alt = np.arcsin(Z0_t)
+    new_az = np.arccos(X0_t/np.cos(new_alt))
+    alt_az_guide.append([new_alt,new_az])
     r1 = pos_star_t - pos_guide_t
 
 
     R_t = np.array([[-X0_t*Z0_t/np.sqrt((X0_t**2+Y0_t**2)*(X0_t**2+Y0_t**2+Z0_t**2)), -Y0_t*Z0_t/np.sqrt((X0_t**2+Y0_t**2)*(X0_t**2+Y0_t**2+Z0_t**2)), np.sqrt(X0_t**2 + Y0_t**2)/np.sqrt(X0_t**2+Y0_t**2+Z0_t**2)],
               [Y0_t/np.sqrt(X0_t**2 + Y0_t**2), -X0_t/np.sqrt(X0_t**2+Y0_t**2), 0],
               [X0_t/np.sqrt(X0_t**2 + Y0_t**2 + Z0_t**2), Y0_t/np.sqrt(X0_t**2 + Y0_t**2 + Z0_t**2), Z0_t/np.sqrt(X0_t**2 + Y0_t**2 + Z0_t**2)]])
 
@@ -53,14 +81,28 @@
     norm = np.sqrt(res[0]**2+res[1]**2)
     angle = np.arctan2(res[1],res[0])
     x = norm * np.cos(angle)
     y = norm * np.sin(angle)
     new_pos_x[i] = x * normalisation
     new_pos_y[i] = y * normalisation
     alt_ev[i] = np.arcsin(Z0_t)
-    # print(new_pos)
+    # print(new_pos_x)
 
   new_pos_func_x = interpolate.interp1d(t,new_pos_x)
   new_pos_func_y = interpolate.interp1d(t,new_pos_y)
   new_pos = (new_pos_func_x,new_pos_func_y)
   alt_func = interpolate.interp1d(t,alt_ev)
-  return(new_pos,alt_func)
+  alt_az_guide = np.array(alt_az_guide)
+  coord = SkyCoord(alt=alt_az_guide[:,0], az=alt_az_guide[:,1], unit='rad', frame = 'altaz', location = loc, obstime = period.time)
+  icrs = coord.transform_to('icrs')
+  
+  alt_az_t = []
+  ra_dec_t = []
+  ang = []
+  period.time.format = 'isot'
+  fk5 = FK5(equinox = period.time[0])
+  locationFK5 = icrs.transform_to(fk5)
+  for i in range(len(coord)):
+    alt_az_t.append([coord[i].alt.rad,coord[i].az.rad,i])
+    ra_dec_t.append([icrs.ra[i].rad,icrs.dec[i].rad,i])
+    ang.append(ParallacticAngle(locationAltAz=coord[i], time = period.time[i],location = loc, locationFK5= locationFK5[i]))
+  return(new_pos,alt_func,alt_az_t,ra_dec_t,ang)
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/photon/sim_image_photon.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/photon/sim_image_photon.py`

 * *Files 16% similar despite different names*

```diff
@@ -86,20 +86,18 @@
 
 def photon_pos_on_PSF(star_pos,photon_dic,PSF,PSF_size,max_func, nb_process):
     dict_photon = {}
     for st in range(len(star_pos)):
         
         ph_list = []
         pool = mp.Pool(nb_process)
-        print(len(photon_dic[st]),'photon to compute')
+        # print(len(photon_dic[st]),'photon to compute')
         for ph in range(len(photon_dic[st])):
-            
-            lbd = photon_dic[st][ph][0]
-            time = photon_dic[st][ph][1]
-            res = pool.apply_async(rejct_filter,args=(max_func,lbd,PSF,time,PSF_size))
+
+            res = pool.apply_async(rejct_filter,args=(max_func,photon_dic[st][ph][0],PSF,photon_dic[st][ph][1],PSF_size))
             ph_list.append(res.get())
 
         pool.close()
         pool.join()
         dict_photon[st] = ph_list
      
     return(dict_photon)
@@ -162,8 +160,30 @@
     S0 = 1.0/Lam0
     S = 1.0/Lam
     N0_1 = 1.0E-8*((2371.34+683939.7/(130-S0**2)+4547.3/(38.9-S0**2))*D1+
             (6487.31+58.058*S0**2-0.71150*S0**4+0.08851*S0**6)*D2)
     N_1 = 1.0E-8*((2371.34+683939.7/(130-S**2)+4547.3/(38.9-S**2))*D1+
             (6487.31+58.058*S**2-0.71150*S**4+0.08851*S**6)*D2)
     DR = np.tan(Z)*(N0_1-N_1)*206264.8
-    return (DR)
+    return (DR)
+
+
+def photon_calib(dim,wv_inter):
+    wv_step = np.linspace(start = wv_inter[0],stop = wv_inter[1], num = 3)
+
+    x_det,y_det = dim
+    dict_wv = []
+    for wv in wv_step:
+
+        Wavelength = np.zeros(dim,dtype = object)
+        Time = np.zeros(dim,dtype = object)
+        
+
+        for i in range(x_det):
+            for j in range(y_det):
+             
+                Wavelength[i,j] = np.ones(shape = 2000) * wv
+                Time[i,j] = np.linspace(0,1,2000)
+        dict_wv.append([wv,Wavelength,Time])
+
+    # print(len(dict_wv))
+    return(dict_wv)
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/theory/Calc.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/theory/Calc.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/theory/MKID.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/theory/MKID.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/theory/SC.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/theory/SC.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/utils.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/utils.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/functions/yaml/yaml_rw.py` & `spiakid_simulation-1.21/spiakid_simulation/functions/yaml/yaml_rw.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/PSF_interface.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/PSF_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,14 @@
     var = DoubleVar()
     scale = Scale(fenetre, variable=var,from_=0,to=nbr_wv,orient=HORIZONTAL,length=1000,showvalue=0)
     scale.grid(column = 0,row = 2,columnspan=2)    
     scale.bind("<ButtonRelease-1>",PSF_plot)
 
     var2 = DoubleVar()
     var2.set(size)
-    scale_2 = Scale(fenetre,variable=var2,from_=0,to=size,orient=VERTICAL,length=500)
+    scale_2 = Scale(fenetre,variable=var2,from_=1,to=size,orient=VERTICAL,length=500)
     scale_2.grid(column = 3,row =0)
     scale_2.bind("<ButtonRelease-1>",PSF_plot)    
 
     Text = Label(fenetre,text=0.4)
     Text.grid(column = 0, row = 3,columnspan=2)
     fenetre.mainloop()
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/interface.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/interface_mult.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/interface_mult.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/test_displacement.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/test_displacement.py`

 * *Files identical despite different names*

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/atmosphere/turbulence.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/atmosphere/turbulence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from astropy.io import fits
 from scipy import interpolate
 import pickle
+import multiprocessing as mp
 
 def generate_Kolmo_screen(N, pixelSize, r0, L0):
     """
     Generate a couple of AO-compensated screens.
 
     Parameters
     ----------
@@ -198,50 +199,66 @@
 def makeven(i):
     # Increments the argument if odd number. Makes it even.
     if i%2:
         i += 1
     return i
 
 
-def PSF_creation(fov_tot, nb_pixels_img, wavelength_array, seeing, wind, D, obscuration, L0,obs_time,save_link = 0):
+def PSF_creation(fov_tot, nb_pixels_img, wavelength_array, seeing, wind, D, obscuration, L0,obs_time,process_nb,save_link = 0):
 
     pixel_screen_size, Ntot, r0 = set_parameters( fov_tot,wavelength_array, seeing,wind,obs_time )
-  
+   
     Npsf = nb_pixels_img
     N,_ = screen_size(Ntot,Npsf)
-    
+  
     phi1, _= generate_Kolmo_screen(N, pixel_screen_size, r0, L0)
 
     lam_short = np.min(np.array(wavelength_array))
 
     psf_pixel_size = fov_tot / nb_pixels_img
+    # print(nb_pixels_img)
     Displacement = displacement(Ntot,Npsf)
+   
     Disp_x = Displacement[0]
-
+    if len(Disp_x) > 1000:
+        Disp_x = Disp_x[:999]
     stack_psf = np.zeros(shape = (nb_pixels_img,nb_pixels_img,len(wavelength_array)))   # Initialisation of satck psf
+    
+    
+
+
     for i in range(len(wavelength_array)):
         
         wavelength_scaling_factor = wavelength_array[i] / lam_short
         Npad = int(np.round(nb_pixels_img * wavelength_scaling_factor))
         Npad = makeven(Npad)  
+        pool = mp.Pool(process_nb)
+        res = []
         for k in range(0,len(Disp_x)): 
-          
-            a = Displacement[1][k]
-            b = nb_pixels_img+Displacement[1][k]
-            c = 0+Displacement[0][k]
-            d = nb_pixels_img+Displacement[0][k]
-            local_phase = phi1[int(a):int(b), int(c):int(d)]
             
-            im = compute_PSF(pad_array(local_phase / wavelength_scaling_factor, Npad), pixel_screen_size, D, obscuration)
-            im = crop_array(im, nb_pixels_img)
+            # a = Displacement[1][k]
+            # b = Npsf+Displacement[1][k]
+            # c = 0+Displacement[0][k]
+            # d = Npsf+Displacement[0][k]
+            # local_phase = phi1[int(a):int(b), int(c):int(d)]
+        
+            # im = compute_PSF(pad_array(local_phase / wavelength_scaling_factor, Npad), pixel_screen_size, D, obscuration)
+  
+            # im = crop_array(im, nb_pixels_img)
 
-            im = im / np.sum(im)
+            # im = im / np.sum(im)
             # Normalisation ?
+            results = pool.apply_async(ParImCompute,args = (k, Displacement, Npsf, phi1, wavelength_scaling_factor, Npad, pixel_screen_size, D, obscuration))
+            res.append((k,results))
 
-            stack_psf[:,:,i] += im / len(Disp_x)
+        for k,result in res:
+            _,value = result.get()
+            stack_psf[:,:,i] += value / len(Disp_x)
+        pool.close()
+        pool.join()
    
     if save_link:
         hdr = fits.Header()
         hdr['CTYPE3'] = 'RA---CAR'
         hdr['CTYPE2'] = 'DEC--CAR'
         hdr['CTYPE1'] = 'WAVE'
         hdr['CUNIT3'] = 'arcsec'
@@ -255,14 +272,26 @@
         hdr['CDELT2'] = psf_pixel_size
         primary_hdu = fits.PrimaryHDU(stack_psf,header=hdr)
 
         hdul = fits.HDUList([primary_hdu])
         hdul.writeto(save_link,overwrite=True)
     return(stack_psf)
 
+
+def ParImCompute(k, Displacement, Npsf, phi1, wavelength_scaling_factor, Npad, pixel_screen_size, D, obscuration):
+    a = Displacement[1][k]
+    b = Npsf+Displacement[1][k]
+    c = 0+Displacement[0][k]
+    d = Npsf+Displacement[0][k]
+    local_phase = phi1[int(a):int(b), int(c):int(d)]
+    im = compute_PSF(pad_array(local_phase / wavelength_scaling_factor, Npad), pixel_screen_size, D, obscuration)
+    im = crop_array(im, Npsf)
+    im = im / np.sum(im)
+    return(k,im)
+
 def displacement(Ntot,Npsf):
     N,new_ntot  = screen_size(Ntot,Npsf)
 
     Disp_x = np.zeros(new_ntot+1)
     Disp_y = np.zeros(new_ntot+1)
     Disp_x[0] = 0
     Disp_y[0] = 0
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation/image_process/image_generation.py` & `spiakid_simulation-1.21/spiakid_simulation/image_process/image_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numpy as np
 import numpy.random as rand
-import matplotlib.pyplot as plt
+
 from pathlib import Path
-from scipy import signal
-from scipy.optimize import least_squares
+
 from astropy.io import fits
 from scipy import interpolate
-from scipy.ndimage import convolve
+
+import multiprocessing as mp
 
 def image_sim(Image_size, object_number, distance,Path_file,Wavelength,spectrum,save = False):  # Wavelength in µm
     r""" Simulate an image of the sky night and save the datacube in WCS compatible format.
 
         Parameters:
         -----------
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation.egg-info/PKG-INFO` & `spiakid_simulation-1.21/spiakid_simulation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiakid-simulation
-Version: 1.20
+Version: 1.21
 Summary: Data simulation of SPIAKID project
 Author-email: Sebastien Faes <faesebastien@gmail.com>
 Project-URL: Homepage, https://spiakid.pages.obspm.fr/simulation/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: <=3.11
 Description-Content-Type: text/markdown
@@ -13,14 +13,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: pyyaml
 Requires-Dist: astropy
 Requires-Dist: scipy
 Requires-Dist: lmfit
 Requires-Dist: h5py
 Requires-Dist: spectral_cube
+Requires-Dist: ephem
 
 # Simulator of data for the project SPIAKID
 
 This project contains the **simulator of data** for the **SPIAKID** project.
 
 The **SPIAKID** (SpectroPhotometric Imaging in Astronomy with Kinetic Inductance Detectors) project aims at designing, building and deploying on the sky a spectrophotometric imager based on Kinetic Inductance detectors. More information can be found on the [SPIAKID project homepage](https://www.observatoiredeparis.psl.eu/spiakid.html).
```

### Comparing `spiakid-simulation-1.20/spiakid_simulation.egg-info/SOURCES.txt` & `spiakid_simulation-1.21/spiakid_simulation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

