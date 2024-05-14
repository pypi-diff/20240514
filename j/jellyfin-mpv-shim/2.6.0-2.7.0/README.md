# Comparing `tmp/jellyfin-mpv-shim-2.6.0.tar.gz` & `tmp/jellyfin-mpv-shim-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyfin-mpv-shim-2.6.0.tar", last modified: Wed Mar  8 03:08:49 2023, max compression
+gzip compressed data, was "jellyfin-mpv-shim-2.7.0.tar", last modified: Tue May 14 01:36:02 2024, max compression
```

## Comparing `jellyfin-mpv-shim-2.6.0.tar` & `jellyfin-mpv-shim-2.7.0.tar`

### file list

```diff
@@ -1,291 +1,315 @@
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/
--rw-r--r--   0 ian       (1000) ian       (1000)      316 2023-02-25 22:55:04.000000 jellyfin-mpv-shim-2.6.0/MANIFEST.in
--rw-r--r--   0 ian       (1000) ian       (1000)    44343 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)    38310 2023-02-25 22:56:24.000000 jellyfin-mpv-shim-2.6.0/README.md
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.718534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/
--rw-r--r--   0 ian       (1000) ian       (1000)       25 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)      660 2023-02-17 22:23:05.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/action_thread.py
--rw-r--r--   0 ian       (1000) ian       (1000)     3333 2023-02-21 05:29:13.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/bifdecode.py
--rw-r--r--   0 ian       (1000) ian       (1000)     8954 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/bulk_subtitle.py
--rw-r--r--   0 ian       (1000) ian       (1000)      352 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/cli_mgr.py
--rw-r--r--   0 ian       (1000) ian       (1000)    10752 2023-03-04 06:01:52.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/clients.py
--rw-r--r--   0 ian       (1000) ian       (1000)     6833 2023-02-25 22:29:36.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/conf.py
--rw-r--r--   0 ian       (1000) ian       (1000)     1735 2023-02-24 22:10:52.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/conffile.py
--rw-r--r--   0 ian       (1000) ian       (1000)      593 2023-03-08 02:49:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/constants.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.718534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/
--rw-r--r--   0 ian       (1000) ian       (1000)     2160 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md
--rw-r--r--   0 ian       (1000) ian       (1000)     2971 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/README.md
--rw-r--r--   0 ian       (1000) ian       (1000)     7249 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json
--rw-r--r--   0 ian       (1000) ian       (1000)    10428 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json
--rw-r--r--   0 ian       (1000) ian       (1000)     6781 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack.json
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/
--rw-r--r--   0 ian       (1000) ian       (1000)     1596 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     1604 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     2884 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6594 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6179 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     4705 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6695 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     2848 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     4340 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     3923 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    69921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    35916 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    17136 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    70020 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    36016 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    17198 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   308873 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   144204 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   308660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   144075 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6482 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6184 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6571 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    73443 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    37685 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    18638 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   290257 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   146743 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    16063 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     4988 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6590 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    73584 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    37714 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    18667 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   290040 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   146811 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     4159 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     6548 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    13921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    16217 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   246177 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    70598 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    12729 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)    26173 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)     7444 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl
--rw-r--r--   0 ian       (1000) ian       (1000)   331721 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook
--rw-r--r--   0 ian       (1000) ian       (1000)    48421 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook
--rw-r--r--   0 ian       (1000) ian       (1000)   655609 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook
--rw-r--r--   0 ian       (1000) ian       (1000)    88885 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook
--rw-r--r--   0 ian       (1000) ian       (1000)   169871 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook
--rw-r--r--   0 ian       (1000) ian       (1000)      664 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook
--rw-r--r--   0 ian       (1000) ian       (1000)      666 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook
--rw-r--r--   0 ian       (1000) ian       (1000)      624 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook
--rw-r--r--   0 ian       (1000) ian       (1000)      625 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/display_mirror/
--rw-r--r--   0 ian       (1000) ian       (1000)     5714 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/display_mirror/__init__.py
--rw-r--r--   0 ian       (1000) ian       (1000)     9236 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/display_mirror/helpers.py
--rw-r--r--   0 ian       (1000) ian       (1000)     6149 2022-06-11 04:16:20.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/event_handler.py
--rw-r--r--   0 ian       (1000) ian       (1000)    14658 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/gui_mgr.py
--rw-r--r--   0 ian       (1000) ian       (1000)      909 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/i18n.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/
--rw-r--r--   0 ian       (1000) ian       (1000)    15441 2023-03-08 02:49:44.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml
--rw-r--r--   0 ian       (1000) ian       (1000)      160 2021-04-20 00:09:50.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.desktop
--rw-r--r--   0 ian       (1000) ian       (1000)    12729 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-128.png
--rw-r--r--   0 ian       (1000) ian       (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-16.png
--rw-r--r--   0 ian       (1000) ian       (1000)    19703 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-256.png
--rw-r--r--   0 ian       (1000) ian       (1000)     1661 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-32.png
--rw-r--r--   0 ian       (1000) ian       (1000)     2444 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-48.png
--rw-r--r--   0 ian       (1000) ian       (1000)     6709 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-64.png
--rw-r--r--   0 ian       (1000) ian       (1000)     2034 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/log_utils.py
--rw-r--r--   0 ian       (1000) ian       (1000)    16674 2023-02-21 05:29:13.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/media.py
--rw-r--r--   0 ian       (1000) ian       (1000)    19948 2023-02-17 02:41:30.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/menu.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/af/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     4303 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/am/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      538 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ar/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    10209 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/be/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    11610 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bg/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    11617 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bn/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      538 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ca/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     6039 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cs/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9656 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cy/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8130 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/da/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.722534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8699 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/de/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9436 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/el/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    11494 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/en_GB/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8870 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/eo/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8722 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9223 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_419/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9449 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_AR/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9411 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/et/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8441 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fa/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    10463 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fi/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9450 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fil/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8989 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fr/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9722 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/he/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8756 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hi/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     3604 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hr/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8680 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hu/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9812 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/id/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8625 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/it/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9375 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ja/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     1069 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/jbo/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     1956 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kk/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9136 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/km/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      329 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kn/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      541 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ko/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8899 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ml/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      547 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/mn/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)      974 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nb_NO/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8617 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nds/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     1523 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nl/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9174 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pl/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9475 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     3164 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_BR/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9107 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_PT/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9210 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ro/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9009 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ru/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    11130 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sk/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9514 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sl/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8873 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sq/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     3481 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sr/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8820 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sv/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8818 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ta/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    14276 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/tr/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8996 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ug/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     1289 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/uk/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)    11715 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/vi/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9475 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hans/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     9059 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.714533 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hant/
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 ian       (1000) ian       (1000)     8460 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo
--rw-r--r--   0 ian       (1000) ian       (1000)     1249 2023-02-16 21:16:23.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/mouse.lua
--rwxr-xr-x   0 ian       (1000) ian       (1000)     3145 2021-04-20 00:53:31.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/mpv_shim.py
--rw-r--r--   0 ian       (1000) ian       (1000)    38326 2023-03-08 02:40:56.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/player.py
--rw-r--r--   0 ian       (1000) ian       (1000)     1180 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/rich_presence.py
--rw-r--r--   0 ian       (1000) ian       (1000)     2106 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/settings_base.py
--rw-r--r--   0 ian       (1000) ian       (1000)     5568 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/svp_integration.py
--rw-r--r--   0 ian       (1000) ian       (1000)    23065 2023-02-15 02:33:10.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/syncplay.py
--rw-r--r--   0 ian       (1000) ian       (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/systray.png
--rw-r--r--   0 ian       (1000) ian       (1000)     3412 2023-02-25 22:58:52.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/thumbfast.lua
--rw-r--r--   0 ian       (1000) ian       (1000)     1974 2023-02-21 04:22:14.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/timeline.py
--rw-r--r--   0 ian       (1000) ian       (1000)   102016 2023-03-06 22:55:52.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/trickplay-osc.lua
--rw-r--r--   0 ian       (1000) ian       (1000)     5757 2023-02-21 05:32:46.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/trickplay.py
--rw-r--r--   0 ian       (1000) ian       (1000)     2740 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/update_check.py
--rw-r--r--   0 ian       (1000) ian       (1000)     8312 2023-02-15 00:27:41.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/utils.py
--rw-r--r--   0 ian       (1000) ian       (1000)     7835 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/video_profile.py
--rw-r--r--   0 ian       (1000) ian       (1000)     1385 2023-02-13 06:22:58.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/win_utils.py
-drwxr-xr-x   0 ian       (1000) ian       (1000)        0 2023-03-08 03:08:49.718534 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/
--rw-r--r--   0 ian       (1000) ian       (1000)    44343 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/PKG-INFO
--rw-r--r--   0 ian       (1000) ian       (1000)     8999 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/SOURCES.txt
--rw-r--r--   0 ian       (1000) ian       (1000)        1 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/dependency_links.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       71 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/entry_points.txt
--rw-r--r--   0 ian       (1000) ian       (1000)      214 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/requires.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       18 2023-03-08 03:08:49.000000 jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/top_level.txt
--rw-r--r--   0 ian       (1000) ian       (1000)       38 2023-03-08 03:08:49.726534 jellyfin-mpv-shim-2.6.0/setup.cfg
--rw-r--r--   0 ian       (1000) ian       (1000)     1609 2023-03-08 02:49:49.000000 jellyfin-mpv-shim-2.6.0/setup.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    36330 2024-05-13 18:21:11.000000 jellyfin-mpv-shim-2.7.0/LICENSE.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      316 2023-02-25 22:55:04.000000 jellyfin-mpv-shim-2.7.0/MANIFEST.in
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    39199 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/PKG-INFO
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    38603 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/README.md
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       25 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/__init__.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      660 2023-02-17 22:23:05.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/action_thread.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1704 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bifdecode.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8952 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bulk_subtitle.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      352 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/cli_mgr.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10750 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/clients.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6890 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conf.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1735 2023-02-24 22:10:52.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conffile.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      593 2024-05-13 21:21:39.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/constants.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.596825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2160 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2971 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/README.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7249 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10428 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6781 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack.json
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1596 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1604 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2884 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6594 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6179 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4705 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6695 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2848 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4340 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     3923 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    69921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    35916 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    17136 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    70020 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    36016 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    17198 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   308873 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   144204 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   308660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   144075 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6482 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6184 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6571 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    73443 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    37685 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18638 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   290257 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   146743 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16063 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4988 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6590 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    73584 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    37714 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18667 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   290040 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   146811 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4159 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6548 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    13921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16217 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   246177 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    70598 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    26173 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7444 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   331721 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    48421 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   655609 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    88885 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   169871 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      664 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      666 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      624 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      625 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     5714 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/__init__.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9235 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/helpers.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7620 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/index.html
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18550 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/jellyfin.css
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6149 2022-06-11 04:16:20.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/event_handler.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    14650 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/gui_mgr.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      909 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/i18n.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    15961 2024-05-14 00:53:53.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      160 2021-04-20 00:09:50.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.desktop
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-128.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-16.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    19703 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-256.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1661 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-32.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2444 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-48.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6709 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-64.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2366 2024-05-14 00:00:06.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/log_utils.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16222 2024-05-14 00:37:26.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/media.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    19810 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/menu.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4893 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      538 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10706 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11509 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12209 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4358 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9722 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9098 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9569 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9197 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9129 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9408 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12144 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8802 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8722 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9666 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9827 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9654 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9084 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10970 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9443 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9524 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9653 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1645 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9245 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9992 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4272 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9532 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9735 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9024 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9305 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7698 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1956 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9136 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      329 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      541 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9349 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7522 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9544 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      330 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      547 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      974 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8998 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1523 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12586 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9259 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9404 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9626 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9514 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9661 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9432 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11836 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9494 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9289 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9382 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8820 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9248 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    15084 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9425 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1289 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11612 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9588 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8987 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8854 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1249 2023-02-16 21:16:23.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mouse.lua
+-rwxr-xr-x   0 izzie     (1000) izzie     (1000)     3226 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mpv_shim.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    38325 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/player.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1180 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/rich_presence.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2106 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/settings_base.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     5568 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/svp_integration.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    23065 2023-02-15 02:33:10.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/syncplay.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/systray.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     3412 2023-02-25 22:58:52.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/thumbfast.lua
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1974 2023-02-21 04:22:14.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/timeline.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   101980 2024-05-13 21:22:11.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay-osc.lua
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4780 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2740 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/update_check.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10115 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/utils.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7835 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/video_profile.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1385 2023-02-13 06:22:58.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/win_utils.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    39199 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/PKG-INFO
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9452 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/SOURCES.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)        1 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/dependency_links.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       70 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/entry_points.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      214 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/requires.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       18 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/top_level.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       38 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/setup.cfg
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2128 2024-05-13 22:26:09.000000 jellyfin-mpv-shim-2.7.0/setup.py
```

### Comparing `jellyfin-mpv-shim-2.6.0/PKG-INFO` & `jellyfin-mpv-shim-2.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,698 +1,701 @@
 Metadata-Version: 2.1
 Name: jellyfin-mpv-shim
-Version: 2.6.0
+Version: 2.7.0
 Summary: Cast media from Jellyfin Mobile and Web apps to MPV.
 Home-page: https://github.com/jellyfin/jellyfin-mpv-shim
-Author: Ian Walton
-Author-email: iwalton3@gmail.com
+Author: Izzie Walton
+Author-email: izzie@iwalton.com
 License: GPLv3
-Description: # Jellyfin MPV Shim
-        
-        [![Current Release](https://img.shields.io/github/release/jellyfin/jellyfin-mpv-shim.svg)](https://github.com/jellyfin/jellyfin-mpv-shim/releases)
-        [![PyPI](https://img.shields.io/pypi/v/jellyfin-mpv-shim)](https://pypi.org/project/jellyfin-mpv-shim/)
-        [![Translation Status](https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-mpv-shim/svg-badge.svg)](https://translate.jellyfin.org/projects/jellyfin/jellyfin-mpv-shim/)
-        [![Code Stype](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        Jellyfin MPV Shim is a cross-platform cast client for Jellyfin.
-        It has support for all your advanced media files without transcoding, as well as tons of
-        features which set it apart from other multimedia clients:
-        
-         - Direct play most media using MPV.
-         - Watch videos with friends using SyncPlay.
-         - Offers a shim mode which runs in the background.
-         - The Jellyfin mobile apps can fully control the client.
-         - [Reconfigure subtitles](https://github.com/jellyfin/jellyfin-mpv-shim#menu) for an entire season at once.
-         - Supports all of the [MPV keyboard shortcuts](https://github.com/jellyfin/jellyfin-mpv-shim#keyboard-shortcuts).
-         - Enhance your video with [Shader Packs](https://github.com/jellyfin/jellyfin-mpv-shim#menu) and [SVP Integration](https://github.com/jellyfin/jellyfin-mpv-shim#svp-integration).
-         - Optionally share your media activity with friends using Discord Rich Presence.
-         - Most features, as well as MPV itself, [can be extensively configured](https://github.com/jellyfin/jellyfin-mpv-shim#configuration).
-         - You can configure the player to use an [external MPV player](https://github.com/jellyfin/jellyfin-mpv-shim#external-mpv) of your choice.
-         - Enable a chromecast-like experience with [Display Mirroring](https://github.com/jellyfin/jellyfin-mpv-shim#display-mirroring).
-         - You can [trigger commands to run](https://github.com/jellyfin/jellyfin-mpv-shim#shell-command-triggers) when certain events happen.
-        
-        To learn more, keep reading. This README explains everything, including [configuration](https://github.com/jellyfin/jellyfin-mpv-shim#configuration), [tips & tricks](https://github.com/jellyfin/jellyfin-mpv-shim#tips-and-tricks), and [development information](https://github.com/jellyfin/jellyfin-mpv-shim#development).
-        
-        ## Getting Started
-        
-        If you are on Windows, simply [download the binary](https://github.com/jellyfin/jellyfin-mpv-shim/releases).
-        If you are using Linux, you can [install via flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim) or [install via pip](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#linux-installation). If you are on macOS, see the [macOS Installation](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#osx-installation)
-        section below.
-        
-        To use the client, simply launch it and log into your Jellyfin server. You’ll need to enter the
-        URL to your server, for example `http://server_ip:8096` or `https://secure_domain`. Make sure to
-        include the subdirectory and port number if applicable. You can then cast your media
-        from another Jellyfin application.
-        
-        The application runs with a notification icon by default. You can use this to edit the server settings,
-        view the application log, open the config folder, and open the application menu. Unlike Plex MPV Shim,
-        authorization tokens for your server are stored on your device, but you are able to cast to the player
-        regardless of location.
-        
-        Note: Due to the huge number of questions and issues that have been submitted about URLs, I now tolerate
-        bare IP addresses and not specifying the port by default. If you want to connect to port 80 instead of
-        8096, you must add the `:80` to the URL because `:8096` is now the default.
-        
-        ## Limitations
-        
-         - Music playback and Live TV are not supported.
-         - The client can’t be shared seamlessly between multiple users on the same server. ([Link to issue.](https://features.jellyfin.org/posts/319/mark-device-as-shared))
-        
-        ### Known Issues
-        
-        Please also note that the on-screen controller for MPV (if available) cannot change the
-        audio and subtitle track configurations for transcoded media. It also cannot load external
-        subtitles. You must either [use the menu](https://github.com/jellyfin/jellyfin-mpv-shim#menu) or the application you casted from.
-        
-        Please note the following issues with controlling SyncPlay:
-         - If you attempt to join a SyncPlay group when casting to MPV Shim, it will play the media but it will not activate SyncPlay.
-             - You can, however, proceed to activate SyncPlay [using the menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
-         - If you would like to create a group or join a group for currently playing media, [use menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
-         - SyncPlay as of 10.7.0 is new and kind of fragile. You may need to rejoin or even restart the client. Please report any issues you find.
-        
-        Music playback sort-of works, but repeat, shuffle, and gapless playback have not been implemented and
-        would require major changes to the application to properly support, as it was built for video.
-        
-        The shader packs feature is sensitive to graphics hardware. It may simply just not work on your computer.
-        You may be able to use the log files to get some more diagnostic information. If you're really unlucky,
-        you'll have to disable the feature by pressing `k` to restore basic functionality.
-        If you find the solution for your case, *please* send me any information you can provide, as every test case helps.
-        
-        ## Advanced Features
-        
-        ### Menu
-        
-        To open the menu, press **c** on your computer or use the navigation controls
-        in the mobile/web app.
-        
-        The menu enables you to:
-         - Adjust video transcoding quality.
-         - Change the default transcoder settings.
-         - Change subtitles or audio, while knowing the track names.
-         - Change subtitles or audio for an entire series at once.
-         - Mark the media as unwatched and quit.
-         - Enable and disable SyncPlay.
-         - Configure shader packs and SVP profiles.
-         - Take screenshots.
-        
-        On your computer, use the mouse or arrow keys, enter, and escape to navigate.
-        On your phone, use the arrow buttons, ok, back, and home to navigate.
-        
-        ### Shader Packs 
-        
-        Shader packs are a recent feature addition that allows you to easily use advanced video
-        shaders and video quality settings. These usually require a lot of configuration to use,
-        but MPV Shim's default shader pack comes with [FSRCNNX](https://github.com/igv/FSRCNN-TensorFlow)
-        and [Anime4K](https://github.com/bloc97/Anime4K) preconfigured. Try experimenting with video
-        profiles! It may greatly improve your experience.
-        
-        Shader Packs are ready to use as of the most recent MPV Shim version. To use, simply
-        navigate to the **Video Playback Profiles** option and select a profile.
-        
-        For details on the shader settings, please see [default-shader-pack](https://github.com/iwalton3/default-shader-pack).
-        If you would like to customize the shader pack, there are details in the configuration section.
-        
-        ### SVP Integration
-        
-        SVP integration allows you to easily configure SVP support, change profiles, and enable/disable
-        SVP without having to exit the player. It is not enabled by default, please see the configuration
-        instructions for instructions on how to enable it.
-        
-        ### Display Mirroring
-        
-        This feature allows media previews to show on your display before you cast the media,
-        similar to Chromecast. It is not enabled by default. To enable it, do one of the following:
-        
-         - Using the systray icon, click "Application Menu". Go to preferences and enable display mirroring.
-             - Use the arrow keys, escape, and enter to navigate the menu.
-         - Cast media to the player and press `c`. Go to preferences and enable display mirroring.
-         - In the config file (see below), change `display_mirroring` to `true`.
-        
-        Then restart the application for the change to take effect. To quit the application on Windows with
-        display mirroring enabled, press Alt+F4.
-        
-        ### Keyboard Shortcuts
-        
-        This program supports most of the [keyboard shortcuts from MPV](https://mpv.io/manual/stable/#interactive-control). The custom keyboard shortcuts are:
-        
-         - < > to skip episodes
-         - q to close player
-         - w to mark watched and skip
-         - u to mark unwatched and quit
-         - c to open the menu
-         - k disable shader packs
-        
-        Here are the notable MPV keyboard shortcuts:
-        
-         - space - Pause/Play
-         - left/right - Seek by 5 seconds
-         - up/down - Seek by 1 minute
-         - s - Take a screenshot
-         - S - Take a screenshot without subtitles
-         - f - Toggle fullscreen
-         - ,/. - Seek by individual frames
-         - \[/\] - Change video speed by 10%
-         - {/} - Change video speed by 50%
-         - backspace - Reset speed
-         - m - Mute
-         - d - Enable/disable deinterlace
-         - Ctrl+Shift+Left/Right - Adjust subtitle delay.
-        
-        ## Configuration
-        
-        The configuration file is located in different places depending on your platform. You can also open the
-        configuration folder using the systray icon if you are using the shim version. When you launch the program
-        on Linux or macOS from the terminal, the location of the config file will be printed. The locations are:
-         - Windows - `%appdata%\jellyfin-mpv-shim\conf.json`
-         - Linux - `~/.config/jellyfin-mpv-shim/conf.json`
-         - Linux (Flatpak) - `~/.var/app/com.github.iwalton3.jellyfin-mpv-shim/config/jellyfin-mpv-shim/conf.json`
-         - macOS - `~/Library/Application Support/jellyfin-mpv-shim/conf.json`
-         - CygWin - `~/.config/jellyfin-mpv-shim/conf.json`
-        
-        You can specify a custom configuration folder with the `--config` option.
-        
-        ### Transcoding
-        
-        You can adjust the basic transcoder settings via the menu.
-        
-        - `always_transcode` - This will tell the client to always transcode. Default: `false`
-            - This may be useful if you are using limited hardware that cannot handle advanced codecs.
-            - Please note that Jellyfin may still direct play files that meet the transcode profile
-              requirements. There is nothing I can do on my end to disable this, but you can reduce
-              the bandwidth setting to force a transcode.
-        - `transcode_hdr` - Force transcode HDR videos to SDR. Default: `false`
-        - `transcode_dolby_vision` - Force transcode Dolby Vision videos to SDR. Default: `true`
-            - If your computer can handle it, you can get tone mapping to work for this using `vo=gpu-next`.
-            - Note that `vo=gpu-next` is considered experimental by MPV at this time.
-        - `transcode_hi10p` - Force transcode 10 bit color videos to 8 bit color. Default: `false`
-        - `remote_kbps` - Bandwidth to permit for remote streaming. Default: `10000`
-        - `local_kbps` - Bandwidth to permit for local streaming. Default: `2147483`
-        - `direct_paths` - Play media files directly from the SMB or NFS source. Default: `false`
-            - `remote_direct_paths` - Apply this even when the server is detected as remote. Default: `false`
-        - `allow_transcode_to_h265` - Allow the server to transcode media *to* `hevc`. Default: `false`
-            - If you enable this, it'll allow remuxing to HEVC but it'll also break force transcoding of Dolby Vision and HDR content if those settings are used. (See [this bug](https://github.com/jellyfin/jellyfin/issues/9313).)
-        - `prefer_transcode_to_h265` - Requests the server to transcode media *to* `hevc` as the default. Default: `false`
-        - `transcode_warning` - Display a warning the first time media transcodes in a session. Default: `true`
-        - `force_video_codec` - Force a specified video codec to be played. Default: `null`
-            - This can be used in tandem with `always_transcode` to force the client to transcode into
-              the specified format.
-            - This may have the same limitations as `always_transcode`.
-            - This will override `transcode_to_h265`, `transcode_h265` and `transcode_hi10p`.
-        - `force_audio_codec` - Force a specified audio codec to be played. Default: `null`
-            - This can be used in tandeom with `always_transcode` to force the client to transcode into
-              the specified format.
-            - This may have the same limitations as `always_transcode`.
-        
-        ### Features
-        
-        You can use the config file to enable and disable features.
-        
-         - `fullscreen` - Fullscreen the player when starting playback. Default: `true`
-         - `enable_gui` - Enable the system tray icon and GUI features. Default: `true`
-         - `enable_osc` - Enable the MPV on-screen controller. Default: `true`
-            - It may be useful to disable this if you are using an external player that already provides a user interface.
-         - `media_key_seek` - Use the media next/prev keys to seek instead of skip episodes. Default: `false`
-         - `use_web_seek` - Use the seek times set in Jellyfin web for arrow key seek. Default: `false`
-         - `display_mirroring` - Enable webview-based display mirroring (content preview). Default: `false`
-         - `screenshot_menu` - Allow taking screenshots from menu. Default: `true`
-         - `check_updates` - Check for updates via GitHub. Default: `true`
-            - This requests the GitHub releases page and checks for a new version.
-            - Update checks are performed when playing media, once per day.
-         - `notify_updates` - Display update notification when playing media. Default: `true`
-            - Notification will only display once until the application is restarted. 
-         - `discord_presence` - Enable Discord rich presence support. Default: `false`
-         - `menu_mouse` - Enable mouse support in the menu. Default: `true`
-             - This requires MPV to be compiled with lua support.
-        
-        ### Shell Command Triggers
-        
-        You can execute shell commands on media state using the config file:
-        
-         - `media_ended_cmd` - When all media has played.
-         - `pre_media_cmd` - Before the player displays. (Will wait for finish.)
-         - `stop_cmd` - After stopping the player.
-         - `idle_cmd` - After no activity for `idle_cmd_delay` seconds.
-         - `idle_when_paused` - Consider the player idle when paused. Default: `false`
-         - `stop_idle` - Stop the player when idle. (Requires `idle_when_paused`.) Default: `false`
-         - `play_cmd` - After playback starts.
-         - `idle_ended_cmd` - After player stops being idle.
-        
-        ### Subtitle Visual Settings
-        
-        These settings may not works for some subtitle codecs or if subtitles are being burned in
-        during a transcode. You can configure custom styled subtitle settings through the MPV config file.
-        
-         - `subtitle_size` - The size of the subtitles, in percent. Default: `100`
-         - `subtitle_color` - The color of the subtitles, in hex. Default: `#FFFFFFFF`
-         - `subtitle_position` - The position (top, bottom, middle). Default: `bottom`
-        
-        ### External MPV
-        
-        The client now supports using an external copy of MPV, including one that is running prior to starting
-        the client. This may be useful if your distribution only provides MPV as a binary executable (instead
-        of as a shared library), or to connect to MPV-based GUI players. Please note that SMPlayer exhibits
-        strange behaviour when controlled in this manner. External MPV is currently the only working backend
-        for media playback on macOS.
-        
-        - `mpv_ext` - Enable usage of the external player by default. Default: `false`
-            - The external player may still be used by default if `libmpv1` is not available.
-        - `mpv_ext_path` - The path to the `mpv` binary to use. By default it uses the one in the PATH. Default: `null`
-            - If you are using Windows, make sure to use two backslashes. Example: `C:\\path\\to\\mpv.exe`
-        - `mpv_ext_ipc` - The path to the socket to control MPV. Default: `null`
-            - If unset, the socket is a randomly selected temp file.
-            - On Windows, this is just a name for the socket, not a path like on Linux.
-        - `mpv_ext_start` - Start a managed copy of MPV with the client. Default: `true`
-            - If not specified, the user must start MPV prior to launching the client.
-            - MPV must be launched with `--input-ipc-server=[value of mpv_ext_ipc]`.
-        - `mpv_ext_no_ovr` - Disable built-in mpv configuration files and use user defaults.
-            - Please note that some scripts and settings, such as ones to keep MPV open, may break
-              functionality in MPV Shim.
-        
-        ### Keyboard Shortcuts
-        
-        You can reconfigure the custom keyboard shortcuts. You can also set them to `null` to disable the shortcut. Please note that disabling keyboard shortcuts may make some features unusable. Additionally, if you remap `q`, using the default shortcut will crash the player.
-        
-         - `kb_stop` - Stop playback and close MPV. (Default: `q`)
-         - `kb_prev` - Go to the previous video. (Default: `<`)
-         - `kb_next` - Go to the next video. (Default: `>`)
-         - `kb_watched` - Mark the video as watched and skip. (Default: `w`)
-         - `kb_unwatched` - Mark the video as unwatched and quit. (Default: `u`)
-         - `kb_menu` - Open the configuration menu. (Default: `c`)
-         - `kb_menu_esc` - Leave the menu. Exits fullscreen otherwise. (Default: `esc`)
-         - `kb_menu_ok` - "ok" for menu. (Default: `enter`)
-         - `kb_menu_left` - "left" for menu. Seeks otherwise. (Default: `left`)
-         - `kb_menu_right` - "right" for menu. Seeks otherwise. (Default: `right`)
-         - `kb_menu_up` - "up" for menu. Seeks otherwise. (Default: `up`)
-         - `kb_menu_down` - "down" for menu. Seeks otherwise. (Default: `down`)
-         - `kb_pause` - Pause. Also "ok" for menu. (Default: `space`)
-         - `kb_fullscreen` - Toggle fullscreen. (Default: `f`)
-         - `kb_debug` - Trigger `pdb` debugger. (Default: `~`)
-         - `kb_kill_shader` - Disable shader packs. (Default: `k`)
-         - `seek_up` - Time to seek for "up" key. (Default: `60`)
-         - `seek_down` - Time to seek for "down" key. (Default: `-60`)
-         - `seek_right` - Time to seek for "right" key. (Default: `5`)
-         - `seek_left` - Time to seek for "left" key. (Default: `-5`)
-         - `media_keys` - Enable binding of MPV to media keys. Default: `true`
-         - `seek_v_exact` - Use exact seek for up/down keys. Default: `false`
-         - `seek_h_exact` - Use exact seek for left/right keys. Default: `false`
-        
-        ### Shader Packs
-        
-        Shader packs allow you to import MPV config and shader presets into MPV Shim and easily switch
-        between them at runtime through the built-in menu. This enables easy usage and switching of
-        advanced MPV video playback options, such as video upscaling, while being easy to use.
-        
-        If you select one of the presets from the shader pack, it will override some MPV configurations
-        and any shaders manually specified in `mpv.conf`. If you would like to customize the shader pack,
-        use `shader_pack_custom`.
-        
-         - `shader_pack_enable` - Enable shader pack. (Default: `true`)
-         - `shader_pack_custom` - Enable to use a custom shader pack. (Default: `false`)
-            - If you enable this, it will copy the default shader pack to the `shader_pack` config folder.
-            - This initial copy will only happen if the `shader_pack` folder didn't exist.
-            - This shader pack will then be used instead of the built-in one from then on.
-         - `shader_pack_remember` - Automatically remember the last used shader profile. (Default: `true`)
-         - `shader_pack_profile` - The default profile to use. (Default: `null`)
-            - If you use `shader_pack_remember`, this will be updated when you set a profile through the UI.
-         - `shader_pack_subtype` - The profile group to use. The default pack contains `lq` and `hq` groups. Use `hq` if you have a fancy graphics card.
-        
-        ### Trickplay Thumbnails
-        
-        MPV will automatically display thumbnail previews. By default it uses the Jellyfin chapter images
-        but it can also use JellyScrub as the source. Please note that this feature will download and
-        uncompress all of the chapter images before it becomes available for a video. For a 4 hour movie this
-        causes disk usage of about 250 MB, but for the average TV episode it is around 40 MB. It also requires
-        overriding the default MPV OSC, which may conflict with some custom user script. Trickplay is compatible
-        with any OSC that uses [thumbfast](https://github.com/po5/thumbfast), as I have added a [compatibility layer](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/jellyfin_mpv_shim/thumbfast.lua).
-        
-         - `thumbnail_enable` - Enable thumbnail feature. (Default: `true`)
-         - `thumbnail_jellyscrub` - Use JellyScrub as the thumbnail source instead of chapter images. (Default: `false`)
-         - `thumbnail_osc_builtin` - Disable this setting if you want to use your own custom osc but leave trickplay enabled. (Default: `true`)
-         - `thumbnail_preferred_size` - The ideal size for thumbnails. (Default: `320`)
-        
-        ### SVP Integration
-        
-        To enable SVP integration, set `svp_enable` to `true` and enable "External control via HTTP" within SVP
-        under Settings > Control options. Adjust the `svp_url` and `svp_socket` settings if needed.
-        
-         - `svp_enable` - Enable SVP integration. (Default: `false`)
-         - `svp_url` - URL for SVP web API. (Default: `http://127.0.0.1:9901/`)
-         - `svp_socket` - Custom MPV socket to use for SVP.
-            - Default on Windows: `mpvpipe`
-            - Default on other platforms: `/tmp/mpvsocket`
-        
-        Currently on Windows the built-in MPV does not work with SVP. You must download MPV yourself.
-        
-         - Download the latest MPV build [from here](https://sourceforge.net/projects/mpv-player-windows/files/64bit/).
-         - Follow the [vapoursynth instructions](https://github.com/shinchiro/mpv-winbuild-cmake/wiki/Setup-vapoursynth-for-mpv).
-             - Make sure to use the latest Python, not Python 3.7.
-         - In the config file, set `mpv_ext` to `true` and `mpv_ext_path` to the path to `mpv.exe`.
-             - Make sure to use two backslashes per each backslash in the path.
-        
-        ### SyncPlay
-        
-        You probably don't need to change these, but they are defined here in case you
-        need to.
-        
-         - `sync_max_delay_speed` - Delay in ms before changing video speed to sync playback. Default: `50`
-         - `sync_max_delay_skip` - Delay in ms before skipping through the video to sync playback. Default: `300`
-         - `sync_method_thresh` - Delay in ms before switching sync method. Default: `2000`
-         - `sync_speed_time` - Duration in ms to change playback speed. Default: `1000`
-         - `sync_speed_attempts` - Number of attempts before speed changes are disabled. Default: `3`
-         - `sync_attempts` - Number of attempts before disabling sync play. Default: `5`
-         - `sync_revert_seek` - Attempt to revert seek via MPV OSC. Default: `true`
-             - This could break if you use revert-seek markers or scripts that use it.
-         - `sync_osd_message` - Write syncplay status messages to OSD. Default: `true`
-        
-        ### Debugging
-        
-        These settings assist with debugging. You will often be asked to configure them when reporting an issue.
-        
-         - `log_decisions` - Log the full media decisions and playback URLs. Default: `false`
-         - `mpv_log_level` - Log level to use for mpv. Default: `info`
-            - Options: fatal, error, warn, info, v, debug, trace
-         - `sanitize_output` - Prevent the writing of server auth tokens to logs. Default: `true`
-         - `write_logs` - Write logs to the config directory for debugging. Default: `false`
-        
-        ### Other Configuration Options
-        
-        Other miscellaneous configuration options. You probably won't have to change these.
-        
-         - `player_name` - The name of the player that appears in the cast menu. Initially set from your hostname.
-         - `client_uuid` - The identifier for the client. Set to a random value on first run.
-         - `audio_output` - Currently has no effect. Default: `hdmi`
-         - `playback_timeout` - Timeout to wait for MPV to start loading video in seconds. Default: `30`
-            - If you're hitting this, it means files on your server probably got corrupted or deleted.
-            - It could also happen if you try to play an unsupported video format. These are rare.
-         - `lang` - Allows overriding system locale. (Enter a language code.) Default: `null`
-            - MPV Shim should use your OS language by default.
-         - `ignore_ssl_cert` - Ignore SSL certificates. Default: `false`
-            - Please consider getting a certificate from Let's Encrypt instead of using this.
-         - `connect_retry_mins` - Number of minutes to retry connecting before showing login window. Default: `0`
-            - This only applies for when you first launch the program.
-         - `lang_filter` - Limit track selection to desired languages. Default: `und,eng,jpn,mis,mul,zxx`
-            - Note that you need to turn on the options below for this to actually do something.
-            - If you remove `und` from the list, it will ignore untagged items.
-            - Languages are typically in [ISO 639-2/B](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes),
-              but if you have strange files this may not be the case.
-         - `lang_filter_sub` - Apply the language filter to subtitle selection. Default: `False`
-         - `lang_filter_audio` - Apply the language filter to audio selection. Default: `False`
-         - `screenshot_dir` - Sets where screenshots go.
-            - Default is the desktop on Windows and unset (current directory) on other platforms.
-         - `force_set_played` - This forcibly sets items as played when MPV playback finished.
-            - If you have files with malformed timestamps that don't get marked as played, enable this.
-         - `raise_mpv` - Windows only. Disable this if you are fine with MPV sometimes appearing behind other windows when playing.
-         - `health_check_interval` - The number of seconds between each client health check. Null disables it. Default: `300`
-        
-        ### Skip Intro Support
-        
-        This functionality is considered experimental and requires the third-party [SkipIntro server plugin](https://github.com/ConfusedPolarBear/intro-skipper). It works the same ways as it did on MPV Shim for Plex.
-        
-         - `skip_intro_always` - Always skip intros, without asking. Default: `false`
-         - `skip_intro_prompt` - Prompt to skip intro via seeking. Default: `false`
-        
-        ### MPV Configuration
-        
-        You can configure mpv directly using the `mpv.conf` and `input.conf` files. (It is in the same folder as `conf.json`.)
-        This may be useful for customizing video upscaling, keyboard shortcuts, or controlling the application
-        via the mpv IPC server.
-        
-        ### Authorization
-        
-        The `cred.json` file contains the authorization information. If you are having problems with the client,
-        such as the Now Playing not appearing or want to delete a server, you can delete this file and add the
-        servers again.
-        
-        ## Tips and Tricks
-        
-        Various tips have been found that allow the media player to support special
-        functionality, albeit with more configuration required.
-        
-        ### Open on Specific Monitor (#19)
-        
-        Please note: Edits to the `mpv.conf` will not take effect until you restart the application. You can open the config directory by using the menu option in the system tray icon.
-        
-        **Option 1**: Select fullscreen output screen through MPV.
-        Determine which screen you would like MPV to show up on.
-         - If you are on Windows, right click the desktop and select "Display Settings". Take the monitor number and subtract one.
-         - If you are on Linux, run `xrandr`. The screen number is the number you want. If there is only one proceed to **Option 2**.
-        
-        Add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration), replacing `0` with the number from the previous step:
-        ```
-        fs=yes
-        fs-screen=0
-        ```
-        
-        **Option 2**: (Linux Only) If option 1 does not work, both of your monitors are likely configured as a single "screen".
-        
-        Run `xrandr`. It should look something like this:
-        
-        ```
-        Screen 0: minimum 8 x 8, current 3520 x 1080, maximum 16384 x 16384
-        VGA-0 connected 1920x1080+0+0 (normal left inverted right x axis y axis) 521mm x 293mm
-           1920x1080     60.00*+
-           1680x1050     59.95  
-           1440x900      59.89  
-           1280x1024     75.02    60.02  
-           1280x960      60.00  
-           1280x800      59.81  
-           1280x720      60.00  
-           1152x864      75.00  
-           1024x768      75.03    70.07    60.00  
-           800x600       75.00    72.19    60.32    56.25  
-           640x480       75.00    59.94  
-        LVDS-0 connected 1600x900+1920+180 (normal left inverted right x axis y axis) 309mm x 174mm
-           1600x900      59.98*+
-        ```
-        
-        If you want MPV to open on VGA-0 for instance, add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration):
-        ```
-        fs=yes
-        geometry=1920x1080+0+0
-        ```
-        **Option 3**: (Linux Only) If your window manager supports it, you can tell the window manager to always open on a specific screen.
-        
-         - For OpenBox: https://forums.bunsenlabs.org/viewtopic.php?id=1199
-         - For i3: https://unix.stackexchange.com/questions/96798/i3wm-start-applications-on-specific-workspaces-when-i3-starts/363848#363848
-        
-        ### Control Volume with Mouse Wheel (#48)
-        
-        Add the following to `input.conf`:
-        ```
-        WHEEL_UP add volume 5
-        WHEEL_DOWN add volume -5
-        ```
-        
-        ### MPRIS Plugin (#54)
-        
-        Set `mpv_ext` to `true` in the config. Add `script=/path/to/mpris.so` to `mpv.conf`.
-        
-        ### Run Multiple Instances (#45)
-        
-        You can pass `--config /path/to/folder` to run another copy of the player. Please 
-        note that running multiple copies of the desktop client is currently not supported. 
-        
-        ### Audio Passthrough
-        
-        You can edit `mpv.conf` to support audio passthrough. A [user on Reddit](https://reddit.com/r/jellyfin/comments/fru6xo/new_cross_platform_desktop_client_jellyfin_mpv/fns7vyp) had luck with this config:
-        ```
-        audio-spdif=ac3,dts,eac3 # (to use the passthrough to receiver over hdmi)
-        audio-channels=2 # (not sure this is necessary, but i keep it in because it works)
-        af=scaletempo,lavcac3enc=yes:640:3 # (for aac 5.1 tracks to the receiver)
-        ```
-        
-        ### MPV Crashes with "The sub-scale option must be a floating point number or a ratio"
-        
-        Run the jellyfin-mpv-shim program with LC_NUMERIC=C.
-        
-        ### Use with gnome-mpv/celluloid (#61)
-        
-        You can use `gnome-mpv` with MPV Shim, but you must launch `gnome-mpv` separately before MPV Shim. (`gnome-mpv` doesn't support the MPV command options directly.)
-        
-        Configure MPV Shim with the following options (leave the other ones):
-        ```json
-        {
-            "mpv_ext": true,
-            "mpv_ext_ipc": "/tmp/gmpv-socket",
-            "mpv_ext_path": null,
-            "mpv_ext_start": false,
-            "enable_osc": false
-        }
-        ```
-        Then within `gnome-mpv`, click the application icon (top left) > Preferences. Configure the following Extra MPV Options:
-        ```
-        --idle --input-ipc-server=/tmp/gmpv-socket
-        ```
-        
-        ### Heavy Memory Usage
-        
-        A problem has been identified where MPV can use a ton of RAM after media has been played,
-        and this RAM is not always freed when the player goes into idle mode. Some users have
-        found that using external MPV lessens the memory leak. To enable external MPV on Windows:
-        
-         - [Download a copy of MPV](https://sourceforge.net/projects/mpv-player-windows/files/64bit/)
-         - Unzip it with 7zip.
-         - Configure `mpv_ext` to `true`. (See the config section.)
-         - Configure `mpv_ext_path` to `C:\\replace\\with\\path\\to\\mpv.exe`. (Note usage of two `\\`.)
-         - Run the program and wait. (You'll probably have to use it for a while.)
-         - Let me know if the high memory usage is with `mpv.exe` or the shim itself.
-        
-        On Linux, the process is similar, except that you don't need to set the `mpv_ext_path` variable.
-        On macOS, external MPV is already the default and is the only supported player mode.
-        
-        In the long term, I may look into a method of terminating MPV when not in use. This will require
-        a lot of changes to the software. 
-        
-        ### Player Sizing (#91)
-        
-        MPV by default may force the window size to match the video aspect ratio, instead of allowing
-        resizing and centering the video accordingly. Add the following to `mpv.conf` to enable resizing
-        of the window freely, if desired:
-        ```
-        no-keepaspect-window
-        ```
-        
-        ## Development
-        
-        If you'd like to run the application without installing it, run `./run.py`.
-        The project is written entirely in Python 3. There are no closed-source
-        components in this project. It is fully hackable.
-        
-        The project is dependent on `python-mpv`, `python-mpv-jsonipc`, and `jellyfin-apiclient-python`. If you are
-        using Windows and would like mpv to be maximize properly, `pywin32` is also needed. The GUI
-        component uses `pystray` and `tkinter`, but there is a fallback cli mode. The mirroring dependencies
-        are `Jinja2` and `pywebview`, along with platform-specific dependencies. (See the installation and building
-        guides for details on platform-specific dependencies for display mirroring.)
-        
-        This project is based Plex MPV Shim, which is based on https://github.com/wnielson/omplex, which
-        is available under the terms of the MIT License. The project was ported to python3, modified to
-        use mpv as the player, and updated to allow all features of the remote control api for video playback.
-        
-        The Jellyfin API client comes from [Jellyfin for Kodi](https://github.com/jellyfin/jellyfin-kodi/tree/master/jellyfin_kodi).
-        The API client was originally forked for this project and is now a [separate package](https://github.com/iwalton3/jellyfin-apiclient-python).
-        
-        The css file for desktop mirroring is from [jellyfin-chromecast](https://github.com/jellyfin/jellyfin-chromecast/tree/5194d2b9f0120e0eb8c7a81fe546cb9e92fcca2b) and is subject to GPL v2.0.
-        
-        The shaders included in the shader pack are also available under verious open source licenses,
-        [which you can read about here](https://github.com/iwalton3/default-shader-pack/blob/master/LICENSE.md).
-        
-        ### Local Dev Installation
-        
-        If you are on Windows there are additional dependencies. Please see the Windows Build Instructions.
-        
-        1. Install the dependencies: `sudo pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
-            - If you run `./gen_pkg.sh --install`, it will also fetch these for you.
-        2. Clone this repository: `git clone https://github.com/jellyfin/jellyfin-mpv-shim`
-            - You can also download a zip build.
-        3. `cd` to the repository: `cd jellyfin-mpv-shim`
-        4. Run prepare script: `./gen_pkg.sh`
-            - To do this manually, download the web client, shader pack, and build the language files.
-        5. Ensure you have a copy of `libmpv1` or `mpv` available.
-        6. Install any platform-specific dependencies from the respective install tutorials.
-        7. You should now be able to run the program with `./run.py`. Installation is possible with `sudo pip3 install .`.
-            - You can also install the package with `./gen_pkg.sh --install`.
-        
-        ### Translation
-        
-        This project uses gettext for translation. The current template language file is `base.pot` in `jellyfin_mpv_shim/messages/`.
-        
-        To regenerate `base.pot` and update an existing translation with new strings:
-        ```bash
-        ./regen_pot.sh
-        ```
-        
-        To compile all `*.po` files to `*.mo`:
-        ```bash
-        ./gen_pkg.sh --skip-build
-        ```
-        
-        ## Linux Installation
-        
-        You can [install the software from flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim). The pip installation is less integrated but takes up less space if you're not already using flatpak.
-        
-        If you are on Linux, you can install via pip. You'll need [libmpv1](https://github.com/Kagami/mpv.js/blob/master/README.md#get-libmpv) or `mpv` installed.
-        ```bash
-        sudo pip3 install --upgrade jellyfin-mpv-shim
-        ```
-        If you would like the GUI and systray features, also install `pystray` and `tkinter`:
-        ```bash
-        sudo pip3 install pystray
-        sudo apt install python3-tk
-        ```
-        If you would like display mirroring support, install the mirroring dependencies:
-        ```bash
-        sudo apt install python3-jinja2 python3-webview
-        # -- OR --
-        sudo pip3 install jellyfin-mpv-shim[mirror]
-        sudo apt install gir1.2-webkit2-4.0
-        ```
-        Discord rich presence support:
-        ```bash
-        sudo pip3 install jellyfin-mpv-shim[discord]
-        ```
-        You can build mpv from source to get better codec support. Execute the following:
-        ```bash
-        sudo pip3 install --upgrade python-mpv
-        sudo apt install autoconf automake libtool libharfbuzz-dev libfreetype6-dev libfontconfig1-dev libx11-dev libxrandr-dev libvdpau-dev libva-dev mesa-common-dev libegl1-mesa-dev yasm libasound2-dev libpulse-dev libuchardet-dev zlib1g-dev libfribidi-dev git libgnutls28-dev libgl1-mesa-dev libsdl2-dev cmake wget python g++ libluajit-5.1-dev
-        git clone https://github.com/mpv-player/mpv-build.git
-        cd mpv-build
-        echo --enable-libmpv-shared > mpv_options
-        ./rebuild -j4
-        sudo ./install
-        sudo ldconfig
-        ```
-        
-        ## <h2 id="osx-installation">macOS Installation</h2>
-        Currently on macOS only the external MPV backend seems to be working. I cannot test on macOS, so please report any issues you find.
-        
-        To install the CLI version:
-        
-        1. Install brew. ([Instructions](https://brew.sh/))
-        2. Install python3 and mpv. `brew install python mpv`
-        3. Install jellyfin-mpv-shim. `pip3 install --upgrade jellyfin-mpv-shim`
-        4. Run `jellyfin-mpv-shim`.
-        
-        If you'd like to install the GUI version, you need a working copy of tkinter.
-        
-        1. Install pyenv. ([Instructions](https://medium.com/python-every-day/python-development-on-macos-with-pyenv-2509c694a808))
-        2. Install TK and mpv. `brew install tcl-tk mpv`
-        3. Install python3 with TK support. `FLAGS="-I$(brew --prefix tcl-tk)/include" pyenv install 3.8.1`
-        4. Set this python3 as the default. `pyenv global 3.8.1`
-        5. Install jellyfin-mpv-shim and pystray. `pip3 install --upgrade 'jellyfin-mpv-shim[gui]'`
-        6. Run `jellyfin-mpv-shim`.
-        
-        Display mirroring is not tested on macOS, but may be installable with 'pip3 install --upgrade 'jellyfin-mpv-shim[mirror]'`.
-        
-        ## Building on Windows
-        
-        There is a prebuilt version for Windows in the releases section. When
-        following these directions, please take care to ensure both the python
-        and libmpv libraries are either 64 or 32 bit. (Don't mismatch them.)
-        
-        If you'd like to build the installer, please install [Inno Setup](https://jrsoftware.org/isinfo.php) to build
-        the installer. If you'd like to build a 32 bit version, download the 32 bit version of mpv-1.dll and
-        copy it into a new folder called mpv32. You'll also need [WebBrowserInterop.x86.dll](https://github.com/r0x0r/pywebview/blob/master/webview/lib/WebBrowserInterop.x86.dll?raw=true).
-        You may also need to edit the batch file for 32 bit builds to point to the right python executable.
-        
-        1. Install Git for Windows. Open Git Bash and run `git clone https://github.com/jellyfin/jellyfin-mpv-shim; cd jellyfin-mpv-shim`.
-            - You can update the project later with `git pull`.
-        2. Install [Python3](https://www.python.org/downloads/) with PATH enabled. Install [7zip](https://ninite.com/7zip/).
-        3. After installing python3, open `cmd` as admin and run `pip install --upgrade pyinstaller python-mpv jellyfin-apiclient-python pywin32 pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
-            - Details: https://github.com/pyinstaller/pyinstaller/issues/4346
-        4. Download [libmpv](https://sourceforge.net/projects/mpv-player-windows/files/libmpv/).
-        5. Extract the `mpv-2.dll` from the file and move it to the `jellyfin-mpv-shim` folder.
-        6. Open a regular `cmd` prompt. Navigate to the `jellyfin-mpv-shim` folder.
-        7. Run `get_pywebview_natives.py`.
-        8. Run `./gen_pkg.sh --skip-build` using the Git for Windows console.
-            - This builds the translation files and downloads the shader packs.
-        9. Run `build-win.bat`.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: discord
 Provides-Extra: gui
 Provides-Extra: mirror
+License-File: LICENSE.md
+
+# Jellyfin MPV Shim
+
+[![Current Release](https://img.shields.io/github/release/jellyfin/jellyfin-mpv-shim.svg)](https://github.com/jellyfin/jellyfin-mpv-shim/releases)
+[![PyPI](https://img.shields.io/pypi/v/jellyfin-mpv-shim)](https://pypi.org/project/jellyfin-mpv-shim/)
+[![Translation Status](https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-mpv-shim/svg-badge.svg)](https://translate.jellyfin.org/projects/jellyfin/jellyfin-mpv-shim/)
+[![Code Stype](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Jellyfin MPV Shim is a cross-platform cast client for Jellyfin.
+It has support for all your advanced media files without transcoding, as well as tons of
+features which set it apart from other multimedia clients:
+
+ - Direct play most media using MPV.
+ - Watch videos with friends using SyncPlay.
+ - Offers a shim mode which runs in the background.
+ - The Jellyfin mobile apps can fully control the client.
+ - [Reconfigure subtitles](https://github.com/jellyfin/jellyfin-mpv-shim#menu) for an entire season at once.
+ - Supports all of the [MPV keyboard shortcuts](https://github.com/jellyfin/jellyfin-mpv-shim#keyboard-shortcuts).
+ - Enhance your video with [Shader Packs](https://github.com/jellyfin/jellyfin-mpv-shim#menu) and [SVP Integration](https://github.com/jellyfin/jellyfin-mpv-shim#svp-integration).
+ - Optionally share your media activity with friends using Discord Rich Presence.
+ - Most features, as well as MPV itself, [can be extensively configured](https://github.com/jellyfin/jellyfin-mpv-shim#configuration).
+ - You can configure the player to use an [external MPV player](https://github.com/jellyfin/jellyfin-mpv-shim#external-mpv) of your choice.
+ - Enable a chromecast-like experience with [Display Mirroring](https://github.com/jellyfin/jellyfin-mpv-shim#display-mirroring).
+ - You can [trigger commands to run](https://github.com/jellyfin/jellyfin-mpv-shim#shell-command-triggers) when certain events happen.
+
+To learn more, keep reading. This README explains everything, including [configuration](https://github.com/jellyfin/jellyfin-mpv-shim#configuration), [tips & tricks](https://github.com/jellyfin/jellyfin-mpv-shim#tips-and-tricks), and [development information](https://github.com/jellyfin/jellyfin-mpv-shim#development).
+
+## Getting Started
+
+If you are on Windows, simply [download the binary](https://github.com/jellyfin/jellyfin-mpv-shim/releases).
+If you are using Linux, you can [install via flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim) or [install via pip](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#linux-installation). If you are on macOS, see the [macOS Installation](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#osx-installation)
+section below.
+
+To use the client, simply launch it and log into your Jellyfin server. You’ll need to enter the
+URL to your server, for example `http://server_ip:8096` or `https://secure_domain`. Make sure to
+include the subdirectory and port number if applicable. You can then cast your media
+from another Jellyfin application.
+
+The application runs with a notification icon by default. You can use this to edit the server settings,
+view the application log, open the config folder, and open the application menu. Unlike Plex MPV Shim,
+authorization tokens for your server are stored on your device, but you are able to cast to the player
+regardless of location.
+
+Note: Due to the huge number of questions and issues that have been submitted about URLs, I now tolerate
+bare IP addresses and not specifying the port by default. If you want to connect to port 80 instead of
+8096, you must add the `:80` to the URL because `:8096` is now the default.
+
+## Limitations
+
+ - Music playback and Live TV are not supported.
+ - The client can’t be shared seamlessly between multiple users on the same server. ([Link to issue.](https://features.jellyfin.org/posts/319/mark-device-as-shared))
+
+### Known Issues
+
+Please also note that the on-screen controller for MPV (if available) cannot change the
+audio and subtitle track configurations for transcoded media. It also cannot load external
+subtitles. You must either [use the menu](https://github.com/jellyfin/jellyfin-mpv-shim#menu) or the application you casted from.
+
+Please note the following issues with controlling SyncPlay:
+ - If you attempt to join a SyncPlay group when casting to MPV Shim, it will play the media but it will not activate SyncPlay.
+     - You can, however, proceed to activate SyncPlay [using the menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
+ - If you would like to create a group or join a group for currently playing media, [use menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
+ - SyncPlay as of 10.7.0 is new and kind of fragile. You may need to rejoin or even restart the client. Please report any issues you find.
+
+Music playback sort-of works, but repeat, shuffle, and gapless playback have not been implemented and
+would require major changes to the application to properly support, as it was built for video.
+
+The shader packs feature is sensitive to graphics hardware. It may simply just not work on your computer.
+You may be able to use the log files to get some more diagnostic information. If you're really unlucky,
+you'll have to disable the feature by pressing `k` to restore basic functionality.
+If you find the solution for your case, *please* send me any information you can provide, as every test case helps.
+
+## Advanced Features
+
+### Menu
+
+To open the menu, press **c** on your computer or use the navigation controls
+in the mobile/web app.
+
+The menu enables you to:
+ - Adjust video transcoding quality.
+ - Change the default transcoder settings.
+ - Change subtitles or audio, while knowing the track names.
+ - Change subtitles or audio for an entire series at once.
+ - Mark the media as unwatched and quit.
+ - Enable and disable SyncPlay.
+ - Configure shader packs and SVP profiles.
+ - Take screenshots.
+
+On your computer, use the mouse or arrow keys, enter, and escape to navigate.
+On your phone, use the arrow buttons, ok, back, and home to navigate.
+
+### Shader Packs
+
+Shader packs are a recent feature addition that allows you to easily use advanced video
+shaders and video quality settings. These usually require a lot of configuration to use,
+but MPV Shim's default shader pack comes with [FSRCNNX](https://github.com/igv/FSRCNN-TensorFlow)
+and [Anime4K](https://github.com/bloc97/Anime4K) preconfigured. Try experimenting with video
+profiles! It may greatly improve your experience.
+
+Shader Packs are ready to use as of the most recent MPV Shim version. To use, simply
+navigate to the **Video Playback Profiles** option and select a profile.
+
+For details on the shader settings, please see [default-shader-pack](https://github.com/iwalton3/default-shader-pack).
+If you would like to customize the shader pack, there are details in the configuration section.
+
+### SVP Integration
+
+SVP integration allows you to easily configure SVP support, change profiles, and enable/disable
+SVP without having to exit the player. It is not enabled by default, please see the configuration
+instructions for instructions on how to enable it.
+
+### Display Mirroring
+
+This feature allows media previews to show on your display before you cast the media,
+similar to Chromecast. It is not enabled by default. To enable it, do one of the following:
+
+ - Using the systray icon, click "Application Menu". Go to preferences and enable display mirroring.
+     - Use the arrow keys, escape, and enter to navigate the menu.
+ - Cast media to the player and press `c`. Go to preferences and enable display mirroring.
+ - In the config file (see below), change `display_mirroring` to `true`.
+
+Then restart the application for the change to take effect. To quit the application on Windows with
+display mirroring enabled, press Alt+F4.
+
+### Keyboard Shortcuts
+
+This program supports most of the [keyboard shortcuts from MPV](https://mpv.io/manual/stable/#interactive-control). The custom keyboard shortcuts are:
+
+ - < > to skip episodes
+ - q to close player
+ - w to mark watched and skip
+ - u to mark unwatched and quit
+ - c to open the menu
+ - k disable shader packs
+
+Here are the notable MPV keyboard shortcuts:
+
+ - space - Pause/Play
+ - left/right - Seek by 5 seconds
+ - up/down - Seek by 1 minute
+ - s - Take a screenshot
+ - S - Take a screenshot without subtitles
+ - f - Toggle fullscreen
+ - ,/. - Seek by individual frames
+ - \[/\] - Change video speed by 10%
+ - {/} - Change video speed by 50%
+ - backspace - Reset speed
+ - m - Mute
+ - d - Enable/disable deinterlace
+ - Ctrl+Shift+Left/Right - Adjust subtitle delay.
+
+## Configuration
+
+The configuration file is located in different places depending on your platform. You can also open the
+configuration folder using the systray icon if you are using the shim version. When you launch the program
+on Linux or macOS from the terminal, the location of the config file will be printed. The locations are:
+ - Windows - `%appdata%\jellyfin-mpv-shim\conf.json`
+ - Linux - `~/.config/jellyfin-mpv-shim/conf.json`
+ - Linux (Flatpak) - `~/.var/app/com.github.iwalton3.jellyfin-mpv-shim/config/jellyfin-mpv-shim/conf.json`
+ - macOS - `~/Library/Application Support/jellyfin-mpv-shim/conf.json`
+ - CygWin - `~/.config/jellyfin-mpv-shim/conf.json`
+
+You can specify a custom configuration folder with the `--config` option.
+
+### Transcoding
+
+You can adjust the basic transcoder settings via the menu.
+
+- `always_transcode` - This will tell the client to always transcode. Default: `false`
+    - This may be useful if you are using limited hardware that cannot handle advanced codecs.
+    - Please note that Jellyfin may still direct play files that meet the transcode profile
+      requirements. There is nothing I can do on my end to disable this, but you can reduce
+      the bandwidth setting to force a transcode.
+- `transcode_hdr` - Force transcode HDR videos to SDR. Default: `false`
+- `transcode_dolby_vision` - Force transcode Dolby Vision videos to SDR. Default: `true`
+    - If your computer can handle it, you can get tone mapping to work for this using `vo=gpu-next`.
+    - Note that `vo=gpu-next` is considered experimental by MPV at this time.
+- `transcode_hi10p` - Force transcode 10 bit color videos to 8 bit color. Default: `false`
+- `transcode_hevc` - Force transcode HEVC videos. Default: `false`
+- `transcode_av1` - Force transcode AV1 videos. Default: `false`
+- `transcode_4k` - Force transcode videos over 1080p. Default: `false`
+- `remote_kbps` - Bandwidth to permit for remote streaming. Default: `10000`
+- `local_kbps` - Bandwidth to permit for local streaming. Default: `2147483`
+- `direct_paths` - Play media files directly from the SMB or NFS source. Default: `false`
+    - `remote_direct_paths` - Apply this even when the server is detected as remote. Default: `false`
+- `allow_transcode_to_h265` - Allow the server to transcode media *to* `hevc`. Default: `false`
+    - If you enable this, it'll allow remuxing to HEVC but it'll also break force transcoding of Dolby Vision and HDR content if those settings are used. (See [this bug](https://github.com/jellyfin/jellyfin/issues/9313).)
+- `prefer_transcode_to_h265` - Requests the server to transcode media *to* `hevc` as the default. Default: `false`
+- `transcode_warning` - Display a warning the first time media transcodes in a session. Default: `true`
+- `force_video_codec` - Force a specified video codec to be played. Default: `null`
+    - This can be used in tandem with `always_transcode` to force the client to transcode into
+      the specified format.
+    - This may have the same limitations as `always_transcode`.
+    - This will override `transcode_to_h265`, `transcode_h265` and `transcode_hi10p`.
+- `force_audio_codec` - Force a specified audio codec to be played. Default: `null`
+    - This can be used in tandeom with `always_transcode` to force the client to transcode into
+      the specified format.
+    - This may have the same limitations as `always_transcode`.
+
+### Features
+
+You can use the config file to enable and disable features.
+
+ - `fullscreen` - Fullscreen the player when starting playback. Default: `true`
+ - `enable_gui` - Enable the system tray icon and GUI features. Default: `true`
+ - `enable_osc` - Enable the MPV on-screen controller. Default: `true`
+    - It may be useful to disable this if you are using an external player that already provides a user interface.
+ - `media_key_seek` - Use the media next/prev keys to seek instead of skip episodes. Default: `false`
+ - `use_web_seek` - Use the seek times set in Jellyfin web for arrow key seek. Default: `false`
+ - `display_mirroring` - Enable webview-based display mirroring (content preview). Default: `false`
+ - `screenshot_menu` - Allow taking screenshots from menu. Default: `true`
+ - `check_updates` - Check for updates via GitHub. Default: `true`
+    - This requests the GitHub releases page and checks for a new version.
+    - Update checks are performed when playing media, once per day.
+ - `notify_updates` - Display update notification when playing media. Default: `true`
+    - Notification will only display once until the application is restarted.
+ - `discord_presence` - Enable Discord rich presence support. Default: `false`
+ - `menu_mouse` - Enable mouse support in the menu. Default: `true`
+     - This requires MPV to be compiled with lua support.
+
+### Shell Command Triggers
+
+You can execute shell commands on media state using the config file:
+
+ - `media_ended_cmd` - When all media has played.
+ - `pre_media_cmd` - Before the player displays. (Will wait for finish.)
+ - `stop_cmd` - After stopping the player.
+ - `idle_cmd` - After no activity for `idle_cmd_delay` seconds.
+ - `idle_when_paused` - Consider the player idle when paused. Default: `false`
+ - `stop_idle` - Stop the player when idle. (Requires `idle_when_paused`.) Default: `false`
+ - `play_cmd` - After playback starts.
+ - `idle_ended_cmd` - After player stops being idle.
+
+### Subtitle Visual Settings
+
+These settings may not works for some subtitle codecs or if subtitles are being burned in
+during a transcode. You can configure custom styled subtitle settings through the MPV config file.
+
+ - `subtitle_size` - The size of the subtitles, in percent. Default: `100`
+ - `subtitle_color` - The color of the subtitles, in hex. Default: `#FFFFFFFF`
+ - `subtitle_position` - The position (top, bottom, middle). Default: `bottom`
+
+### External MPV
+
+The client now supports using an external copy of MPV, including one that is running prior to starting
+the client. This may be useful if your distribution only provides MPV as a binary executable (instead
+of as a shared library), or to connect to MPV-based GUI players. Please note that SMPlayer exhibits
+strange behaviour when controlled in this manner. External MPV is currently the only working backend
+for media playback on macOS. Additionally, due to Flatpak sandbox restrictions, external mpv is not
+practical to use in most cases for the Flatpak version.
+
+- `mpv_ext` - Enable usage of the external player by default. Default: `false`
+    - The external player may still be used by default if `libmpv1` is not available.
+- `mpv_ext_path` - The path to the `mpv` binary to use. By default it uses the one in the PATH. Default: `null`
+    - If you are using Windows, make sure to use two backslashes. Example: `C:\\path\\to\\mpv.exe`
+- `mpv_ext_ipc` - The path to the socket to control MPV. Default: `null`
+    - If unset, the socket is a randomly selected temp file.
+    - On Windows, this is just a name for the socket, not a path like on Linux.
+- `mpv_ext_start` - Start a managed copy of MPV with the client. Default: `true`
+    - If not specified, the user must start MPV prior to launching the client.
+    - MPV must be launched with `--input-ipc-server=[value of mpv_ext_ipc]`.
+- `mpv_ext_no_ovr` - Disable built-in mpv configuration files and use user defaults.
+    - Please note that some scripts and settings, such as ones to keep MPV open, may break
+      functionality in MPV Shim.
+
+### Keyboard Shortcuts
+
+You can reconfigure the custom keyboard shortcuts. You can also set them to `null` to disable the shortcut. Please note that disabling keyboard shortcuts may make some features unusable. Additionally, if you remap `q`, using the default shortcut will crash the player.
+
+ - `kb_stop` - Stop playback and close MPV. (Default: `q`)
+ - `kb_prev` - Go to the previous video. (Default: `<`)
+ - `kb_next` - Go to the next video. (Default: `>`)
+ - `kb_watched` - Mark the video as watched and skip. (Default: `w`)
+ - `kb_unwatched` - Mark the video as unwatched and quit. (Default: `u`)
+ - `kb_menu` - Open the configuration menu. (Default: `c`)
+ - `kb_menu_esc` - Leave the menu. Exits fullscreen otherwise. (Default: `esc`)
+ - `kb_menu_ok` - "ok" for menu. (Default: `enter`)
+ - `kb_menu_left` - "left" for menu. Seeks otherwise. (Default: `left`)
+ - `kb_menu_right` - "right" for menu. Seeks otherwise. (Default: `right`)
+ - `kb_menu_up` - "up" for menu. Seeks otherwise. (Default: `up`)
+ - `kb_menu_down` - "down" for menu. Seeks otherwise. (Default: `down`)
+ - `kb_pause` - Pause. Also "ok" for menu. (Default: `space`)
+ - `kb_fullscreen` - Toggle fullscreen. (Default: `f`)
+ - `kb_debug` - Trigger `pdb` debugger. (Default: `~`)
+ - `kb_kill_shader` - Disable shader packs. (Default: `k`)
+ - `seek_up` - Time to seek for "up" key. (Default: `60`)
+ - `seek_down` - Time to seek for "down" key. (Default: `-60`)
+ - `seek_right` - Time to seek for "right" key. (Default: `5`)
+ - `seek_left` - Time to seek for "left" key. (Default: `-5`)
+ - `media_keys` - Enable binding of MPV to media keys. Default: `true`
+ - `seek_v_exact` - Use exact seek for up/down keys. Default: `false`
+ - `seek_h_exact` - Use exact seek for left/right keys. Default: `false`
+
+### Shader Packs
+
+Shader packs allow you to import MPV config and shader presets into MPV Shim and easily switch
+between them at runtime through the built-in menu. This enables easy usage and switching of
+advanced MPV video playback options, such as video upscaling, while being easy to use.
+
+If you select one of the presets from the shader pack, it will override some MPV configurations
+and any shaders manually specified in `mpv.conf`. If you would like to customize the shader pack,
+use `shader_pack_custom`.
+
+ - `shader_pack_enable` - Enable shader pack. (Default: `true`)
+ - `shader_pack_custom` - Enable to use a custom shader pack. (Default: `false`)
+    - If you enable this, it will copy the default shader pack to the `shader_pack` config folder.
+    - This initial copy will only happen if the `shader_pack` folder didn't exist.
+    - This shader pack will then be used instead of the built-in one from then on.
+ - `shader_pack_remember` - Automatically remember the last used shader profile. (Default: `true`)
+ - `shader_pack_profile` - The default profile to use. (Default: `null`)
+    - If you use `shader_pack_remember`, this will be updated when you set a profile through the UI.
+ - `shader_pack_subtype` - The profile group to use. The default pack contains `lq` and `hq` groups. Use `hq` if you have a fancy graphics card.
+
+### Trickplay Thumbnails
+
+MPV will automatically display thumbnail previews. By default it uses the Trickplay images and falls back to chapter images. Please note that this feature will download and
+uncompress all of the chapter images before it becomes available for a video. For a 4 hour movie this
+causes disk usage of about 250 MB, but for the average TV episode it is around 40 MB. It also requires
+overriding the default MPV OSC, which may conflict with some custom user script. Trickplay is compatible
+with any OSC that uses [thumbfast](https://github.com/po5/thumbfast), as I have added a [compatibility layer](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/jellyfin_mpv_shim/thumbfast.lua).
+
+ - `thumbnail_enable` - Enable thumbnail feature. (Default: `true`)
+ - `thumbnail_osc_builtin` - Disable this setting if you want to use your own custom osc but leave trickplay enabled. (Default: `true`)
+ - `thumbnail_preferred_size` - The ideal size for thumbnails. (Default: `320`)
+
+### SVP Integration
+
+To enable SVP integration, set `svp_enable` to `true` and enable "External control via HTTP" within SVP
+under Settings > Control options. Adjust the `svp_url` and `svp_socket` settings if needed.
+
+ - `svp_enable` - Enable SVP integration. (Default: `false`)
+ - `svp_url` - URL for SVP web API. (Default: `http://127.0.0.1:9901/`)
+ - `svp_socket` - Custom MPV socket to use for SVP.
+    - Default on Windows: `mpvpipe`
+    - Default on other platforms: `/tmp/mpvsocket`
+
+Currently on Windows the built-in MPV does not work with SVP. You must download MPV yourself.
+
+ - Download the latest MPV build [from here](https://sourceforge.net/projects/mpv-player-windows/files/64bit/).
+ - Follow the [vapoursynth instructions](https://github.com/shinchiro/mpv-winbuild-cmake/wiki/Setup-vapoursynth-for-mpv).
+     - Make sure to use the latest Python, not Python 3.7.
+ - In the config file, set `mpv_ext` to `true` and `mpv_ext_path` to the path to `mpv.exe`.
+     - Make sure to use two backslashes per each backslash in the path.
+
+### SyncPlay
+
+You probably don't need to change these, but they are defined here in case you
+need to.
+
+ - `sync_max_delay_speed` - Delay in ms before changing video speed to sync playback. Default: `50`
+ - `sync_max_delay_skip` - Delay in ms before skipping through the video to sync playback. Default: `300`
+ - `sync_method_thresh` - Delay in ms before switching sync method. Default: `2000`
+ - `sync_speed_time` - Duration in ms to change playback speed. Default: `1000`
+ - `sync_speed_attempts` - Number of attempts before speed changes are disabled. Default: `3`
+ - `sync_attempts` - Number of attempts before disabling sync play. Default: `5`
+ - `sync_revert_seek` - Attempt to revert seek via MPV OSC. Default: `true`
+     - This could break if you use revert-seek markers or scripts that use it.
+ - `sync_osd_message` - Write syncplay status messages to OSD. Default: `true`
+
+### Debugging
+
+These settings assist with debugging. You will often be asked to configure them when reporting an issue.
+
+ - `log_decisions` - Log the full media decisions and playback URLs. Default: `false`
+ - `mpv_log_level` - Log level to use for mpv. Default: `info`
+    - Options: fatal, error, warn, info, v, debug, trace
+ - `sanitize_output` - Prevent the writing of server auth tokens to logs. Default: `true`
+ - `write_logs` - Write logs to the config directory for debugging. Default: `false`
+
+### Other Configuration Options
+
+Other miscellaneous configuration options. You probably won't have to change these.
+
+ - `player_name` - The name of the player that appears in the cast menu. Initially set from your hostname.
+ - `client_uuid` - The identifier for the client. Set to a random value on first run.
+ - `audio_output` - Currently has no effect. Default: `hdmi`
+ - `playback_timeout` - Timeout to wait for MPV to start loading video in seconds. Default: `30`
+    - If you're hitting this, it means files on your server probably got corrupted or deleted.
+    - It could also happen if you try to play an unsupported video format. These are rare.
+ - `lang` - Allows overriding system locale. (Enter a language code.) Default: `null`
+    - MPV Shim should use your OS language by default.
+ - `ignore_ssl_cert` - Ignore SSL certificates. Default: `false`
+    - Please consider getting a certificate from Let's Encrypt instead of using this.
+ - `connect_retry_mins` - Number of minutes to retry connecting before showing login window. Default: `0`
+    - This only applies for when you first launch the program.
+ - `lang_filter` - Limit track selection to desired languages. Default: `und,eng,jpn,mis,mul,zxx`
+    - Note that you need to turn on the options below for this to actually do something.
+    - If you remove `und` from the list, it will ignore untagged items.
+    - Languages are typically in [ISO 639-2/B](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes),
+      but if you have strange files this may not be the case.
+ - `lang_filter_sub` - Apply the language filter to subtitle selection. Default: `False`
+ - `lang_filter_audio` - Apply the language filter to audio selection. Default: `False`
+ - `screenshot_dir` - Sets where screenshots go.
+    - Default is the desktop on Windows and unset (current directory) on other platforms.
+ - `force_set_played` - This forcibly sets items as played when MPV playback finished.
+    - If you have files with malformed timestamps that don't get marked as played, enable this.
+ - `raise_mpv` - Windows only. Disable this if you are fine with MPV sometimes appearing behind other windows when playing.
+ - `health_check_interval` - The number of seconds between each client health check. Null disables it. Default: `300`
+
+### Skip Intro Support
+
+This functionality is considered experimental and requires the third-party [SkipIntro server plugin](https://github.com/ConfusedPolarBear/intro-skipper). It works the same ways as it did on MPV Shim for Plex.
+
+ - `skip_intro_always` - Always skip intros, without asking. Default: `false`
+ - `skip_intro_prompt` - Prompt to skip intro via seeking. Default: `false`
+
+### MPV Configuration
+
+You can configure mpv directly using the `mpv.conf` and `input.conf` files. (It is in the same folder as `conf.json`.)
+This may be useful for customizing video upscaling, keyboard shortcuts, or controlling the application
+via the mpv IPC server.
+
+### Authorization
+
+The `cred.json` file contains the authorization information. If you are having problems with the client,
+such as the Now Playing not appearing or want to delete a server, you can delete this file and add the
+servers again.
+
+## Tips and Tricks
+
+Various tips have been found that allow the media player to support special
+functionality, albeit with more configuration required.
+
+### Open on Specific Monitor (#19)
+
+Please note: Edits to the `mpv.conf` will not take effect until you restart the application. You can open the config directory by using the menu option in the system tray icon.
+
+**Option 1**: Select fullscreen output screen through MPV.
+Determine which screen you would like MPV to show up on.
+ - If you are on Windows, right click the desktop and select "Display Settings". Take the monitor number and subtract one.
+ - If you are on Linux, run `xrandr`. The screen number is the number you want. If there is only one proceed to **Option 2**.
+
+Add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration), replacing `0` with the number from the previous step:
+```
+fs=yes
+fs-screen=0
+```
+
+**Option 2**: (Linux Only) If option 1 does not work, both of your monitors are likely configured as a single "screen".
+
+Run `xrandr`. It should look something like this:
+
+```
+Screen 0: minimum 8 x 8, current 3520 x 1080, maximum 16384 x 16384
+VGA-0 connected 1920x1080+0+0 (normal left inverted right x axis y axis) 521mm x 293mm
+   1920x1080     60.00*+
+   1680x1050     59.95
+   1440x900      59.89
+   1280x1024     75.02    60.02
+   1280x960      60.00
+   1280x800      59.81
+   1280x720      60.00
+   1152x864      75.00
+   1024x768      75.03    70.07    60.00
+   800x600       75.00    72.19    60.32    56.25
+   640x480       75.00    59.94
+LVDS-0 connected 1600x900+1920+180 (normal left inverted right x axis y axis) 309mm x 174mm
+   1600x900      59.98*+
+```
+
+If you want MPV to open on VGA-0 for instance, add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration):
+```
+fs=yes
+geometry=1920x1080+0+0
+```
+**Option 3**: (Linux Only) If your window manager supports it, you can tell the window manager to always open on a specific screen.
+
+ - For OpenBox: https://forums.bunsenlabs.org/viewtopic.php?id=1199
+ - For i3: https://unix.stackexchange.com/questions/96798/i3wm-start-applications-on-specific-workspaces-when-i3-starts/363848#363848
+
+### Control Volume with Mouse Wheel (#48)
+
+Add the following to `input.conf`:
+```
+WHEEL_UP add volume 5
+WHEEL_DOWN add volume -5
+```
+
+### MPRIS Plugin (#54)
+
+Set `mpv_ext` to `true` in the config. Add `script=/path/to/mpris.so` to `mpv.conf`.
+
+### Run Multiple Instances (#45)
+
+You can pass `--config /path/to/folder` to run another copy of the player. Please
+note that running multiple copies of the desktop client is currently not supported.
+
+### Audio Passthrough
+
+You can edit `mpv.conf` to support audio passthrough. A [user on Reddit](https://reddit.com/r/jellyfin/comments/fru6xo/new_cross_platform_desktop_client_jellyfin_mpv/fns7vyp) had luck with this config:
+```
+audio-spdif=ac3,dts,eac3 # (to use the passthrough to receiver over hdmi)
+audio-channels=2 # (not sure this is necessary, but i keep it in because it works)
+af=scaletempo,lavcac3enc=yes:640:3 # (for aac 5.1 tracks to the receiver)
+```
+
+### MPV Crashes with "The sub-scale option must be a floating point number or a ratio"
+
+Run the jellyfin-mpv-shim program with LC_NUMERIC=C.
+
+### Use with gnome-mpv/celluloid (#61)
+
+You can use `gnome-mpv` with MPV Shim, but you must launch `gnome-mpv` separately before MPV Shim. (`gnome-mpv` doesn't support the MPV command options directly.)
+
+Configure MPV Shim with the following options (leave the other ones):
+```json
+{
+    "mpv_ext": true,
+    "mpv_ext_ipc": "/tmp/gmpv-socket",
+    "mpv_ext_path": null,
+    "mpv_ext_start": false,
+    "enable_osc": false
+}
+```
+Then within `gnome-mpv`, click the application icon (top left) > Preferences. Configure the following Extra MPV Options:
+```
+--idle --input-ipc-server=/tmp/gmpv-socket
+```
+
+### Heavy Memory Usage
+
+A problem has been identified where MPV can use a ton of RAM after media has been played,
+and this RAM is not always freed when the player goes into idle mode. Some users have
+found that using external MPV lessens the memory leak. To enable external MPV on Windows:
+
+ - [Download a copy of MPV](https://sourceforge.net/projects/mpv-player-windows/files/64bit/)
+ - Unzip it with 7zip.
+ - Configure `mpv_ext` to `true`. (See the config section.)
+ - Configure `mpv_ext_path` to `C:\\replace\\with\\path\\to\\mpv.exe`. (Note usage of two `\\`.)
+ - Run the program and wait. (You'll probably have to use it for a while.)
+ - Let me know if the high memory usage is with `mpv.exe` or the shim itself.
+
+On Linux, the process is similar, except that you don't need to set the `mpv_ext_path` variable.
+On macOS, external MPV is already the default and is the only supported player mode.
+
+In the long term, I may look into a method of terminating MPV when not in use. This will require
+a lot of changes to the software.
+
+### Player Sizing (#91)
+
+MPV by default may force the window size to match the video aspect ratio, instead of allowing
+resizing and centering the video accordingly. Add the following to `mpv.conf` to enable resizing
+of the window freely, if desired:
+```
+no-keepaspect-window
+```
+
+## Development
+
+If you'd like to run the application without installing it, run `./run.py`.
+The project is written entirely in Python 3. There are no closed-source
+components in this project. It is fully hackable.
+
+The project is dependent on `python-mpv`, `python-mpv-jsonipc`, and `jellyfin-apiclient-python`. If you are
+using Windows and would like mpv to be maximize properly, `pywin32` is also needed. The GUI
+component uses `pystray` and `tkinter`, but there is a fallback cli mode. The mirroring dependencies
+are `Jinja2` and `pywebview`, along with platform-specific dependencies. (See the installation and building
+guides for details on platform-specific dependencies for display mirroring.)
+
+This project is based Plex MPV Shim, which is based on https://github.com/wnielson/omplex, which
+is available under the terms of the MIT License. The project was ported to python3, modified to
+use mpv as the player, and updated to allow all features of the remote control api for video playback.
+
+The Jellyfin API client comes from [Jellyfin for Kodi](https://github.com/jellyfin/jellyfin-kodi/tree/master/jellyfin_kodi).
+The API client was originally forked for this project and is now a [separate package](https://github.com/iwalton3/jellyfin-apiclient-python).
+
+The css file for desktop mirroring is from [jellyfin-chromecast](https://github.com/jellyfin/jellyfin-chromecast/tree/5194d2b9f0120e0eb8c7a81fe546cb9e92fcca2b) and is subject to GPL v2.0.
+
+The shaders included in the shader pack are also available under verious open source licenses,
+[which you can read about here](https://github.com/iwalton3/default-shader-pack/blob/master/LICENSE.md).
+
+### Local Dev Installation
+
+If you are on Windows there are additional dependencies. Please see the Windows Build Instructions.
+
+1. Install the dependencies: `pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
+    - If you run `./gen_pkg.sh --install`, it will also fetch these for you.
+    - Note: Recent distributions make pip unusable by default. Consider using conda or add a virtualenv to your user's path.
+2. Clone this repository: `git clone https://github.com/jellyfin/jellyfin-mpv-shim`
+    - You can also download a zip build.
+3. `cd` to the repository: `cd jellyfin-mpv-shim`
+4. Run prepare script: `./gen_pkg.sh`
+    - To do this manually, download the web client, shader pack, and build the language files.
+5. Ensure you have a copy of `libmpv1` or `mpv` available.
+6. Install any platform-specific dependencies from the respective install tutorials.
+7. You should now be able to run the program with `./run.py`. Installation is possible with `sudo pip3 install .`.
+    - You can also install the package with `./gen_pkg.sh --install`.
+
+### Translation
+
+This project uses gettext for translation. The current template language file is `base.pot` in `jellyfin_mpv_shim/messages/`.
+
+To regenerate `base.pot` and update an existing translation with new strings:
+```bash
+./regen_pot.sh
+```
+
+To compile all `*.po` files to `*.mo`:
+```bash
+./gen_pkg.sh --skip-build
+```
+
+## Linux Installation
+
+You can [install the software from flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim). The pip installation is less integrated but takes up less space if you're not already using flatpak.
+
+If you are on Linux, you can install via pip. You'll need [libmpv1](https://github.com/Kagami/mpv.js/blob/master/README.md#get-libmpv) or `mpv` installed.
+```bash
+sudo pip3 install --upgrade jellyfin-mpv-shim
+```
+If you would like the GUI and systray features, also install `pystray` and `tkinter`:
+```bash
+sudo pip3 install pystray
+sudo apt install python3-tk
+```
+If you would like display mirroring support, install the mirroring dependencies:
+```bash
+sudo apt install python3-jinja2 python3-webview
+# -- OR --
+sudo pip3 install jellyfin-mpv-shim[mirror]
+sudo apt install gir1.2-webkit2-4.0
+```
+Discord rich presence support:
+```bash
+sudo pip3 install jellyfin-mpv-shim[discord]
+```
+You can build mpv from source to get better codec support. Execute the following:
+```bash
+sudo pip3 install --upgrade python-mpv
+sudo apt install autoconf automake libtool libharfbuzz-dev libfreetype6-dev libfontconfig1-dev libx11-dev libxrandr-dev libvdpau-dev libva-dev mesa-common-dev libegl1-mesa-dev yasm libasound2-dev libpulse-dev libuchardet-dev zlib1g-dev libfribidi-dev git libgnutls28-dev libgl1-mesa-dev libsdl2-dev cmake wget python g++ libluajit-5.1-dev
+git clone https://github.com/mpv-player/mpv-build.git
+cd mpv-build
+echo --enable-libmpv-shared > mpv_options
+./rebuild -j4
+sudo ./install
+sudo ldconfig
+```
+
+## <h2 id="osx-installation">macOS Installation</h2>
+Currently on macOS only the external MPV backend seems to be working. I cannot test on macOS, so please report any issues you find.
+
+To install the CLI version:
+
+1. Install brew. ([Instructions](https://brew.sh/))
+2. Install python3 and mpv. `brew install python mpv`
+3. Install jellyfin-mpv-shim. `pip3 install --upgrade jellyfin-mpv-shim`
+4. Run `jellyfin-mpv-shim`.
+
+If you'd like to install the GUI version, you need a working copy of tkinter.
+
+1. Install pyenv. ([Instructions](https://medium.com/python-every-day/python-development-on-macos-with-pyenv-2509c694a808))
+2. Install TK and mpv. `brew install tcl-tk mpv`
+3. Install python3 with TK support. `FLAGS="-I$(brew --prefix tcl-tk)/include" pyenv install 3.8.1`
+4. Set this python3 as the default. `pyenv global 3.8.1`
+5. Install jellyfin-mpv-shim and pystray. `pip3 install --upgrade 'jellyfin-mpv-shim[gui]'`
+6. Run `jellyfin-mpv-shim`.
+
+Display mirroring is not tested on macOS, but may be installable with 'pip3 install --upgrade 'jellyfin-mpv-shim[mirror]'`.
+
+## Building on Windows
+
+There is a prebuilt version for Windows in the releases section. When
+following these directions, please take care to ensure both the python
+and libmpv libraries are either 64 or 32 bit. (Don't mismatch them.)
+
+If you'd like to build the installer, please install [Inno Setup](https://jrsoftware.org/isinfo.php) to build
+the installer. If you'd like to build a 32 bit version, download the 32 bit version of mpv-1.dll and
+copy it into a new folder called mpv32. You'll also need [WebBrowserInterop.x86.dll](https://github.com/r0x0r/pywebview/blob/master/webview/lib/WebBrowserInterop.x86.dll?raw=true).
+You may also need to edit the batch file for 32 bit builds to point to the right python executable.
+
+1. Install Git for Windows. Open Git Bash and run `git clone https://github.com/jellyfin/jellyfin-mpv-shim; cd jellyfin-mpv-shim`.
+    - You can update the project later with `git pull`.
+2. Install [Python3](https://www.python.org/downloads/) with PATH enabled. Install [7zip](https://ninite.com/7zip/).
+3. After installing python3, open `cmd` as admin and run `pip install --upgrade pyinstaller python-mpv jellyfin-apiclient-python pywin32 pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
+    - Details: https://github.com/pyinstaller/pyinstaller/issues/4346
+4. Download [libmpv](https://sourceforge.net/projects/mpv-player-windows/files/libmpv/).
+5. Extract the `mpv-2.dll` from the file and move it to the `jellyfin-mpv-shim` folder.
+6. Open a regular `cmd` prompt. Navigate to the `jellyfin-mpv-shim` folder.
+7. Run `get_pywebview_natives.py`.
+8. Run `./gen_pkg.sh --skip-build` using the Git for Windows console.
+    - This builds the translation files and downloads the shader packs.
+9. Run `build-win.bat`.
```

### Comparing `jellyfin-mpv-shim-2.6.0/README.md` & `jellyfin-mpv-shim-2.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
  - Enable and disable SyncPlay.
  - Configure shader packs and SVP profiles.
  - Take screenshots.
 
 On your computer, use the mouse or arrow keys, enter, and escape to navigate.
 On your phone, use the arrow buttons, ok, back, and home to navigate.
 
-### Shader Packs 
+### Shader Packs
 
 Shader packs are a recent feature addition that allows you to easily use advanced video
 shaders and video quality settings. These usually require a lot of configuration to use,
 but MPV Shim's default shader pack comes with [FSRCNNX](https://github.com/igv/FSRCNN-TensorFlow)
 and [Anime4K](https://github.com/bloc97/Anime4K) preconfigured. Try experimenting with video
 profiles! It may greatly improve your experience.
 
@@ -172,14 +172,17 @@
       requirements. There is nothing I can do on my end to disable this, but you can reduce
       the bandwidth setting to force a transcode.
 - `transcode_hdr` - Force transcode HDR videos to SDR. Default: `false`
 - `transcode_dolby_vision` - Force transcode Dolby Vision videos to SDR. Default: `true`
     - If your computer can handle it, you can get tone mapping to work for this using `vo=gpu-next`.
     - Note that `vo=gpu-next` is considered experimental by MPV at this time.
 - `transcode_hi10p` - Force transcode 10 bit color videos to 8 bit color. Default: `false`
+- `transcode_hevc` - Force transcode HEVC videos. Default: `false`
+- `transcode_av1` - Force transcode AV1 videos. Default: `false`
+- `transcode_4k` - Force transcode videos over 1080p. Default: `false`
 - `remote_kbps` - Bandwidth to permit for remote streaming. Default: `10000`
 - `local_kbps` - Bandwidth to permit for local streaming. Default: `2147483`
 - `direct_paths` - Play media files directly from the SMB or NFS source. Default: `false`
     - `remote_direct_paths` - Apply this even when the server is detected as remote. Default: `false`
 - `allow_transcode_to_h265` - Allow the server to transcode media *to* `hevc`. Default: `false`
     - If you enable this, it'll allow remuxing to HEVC but it'll also break force transcoding of Dolby Vision and HDR content if those settings are used. (See [this bug](https://github.com/jellyfin/jellyfin/issues/9313).)
 - `prefer_transcode_to_h265` - Requests the server to transcode media *to* `hevc` as the default. Default: `false`
@@ -206,15 +209,15 @@
  - `use_web_seek` - Use the seek times set in Jellyfin web for arrow key seek. Default: `false`
  - `display_mirroring` - Enable webview-based display mirroring (content preview). Default: `false`
  - `screenshot_menu` - Allow taking screenshots from menu. Default: `true`
  - `check_updates` - Check for updates via GitHub. Default: `true`
     - This requests the GitHub releases page and checks for a new version.
     - Update checks are performed when playing media, once per day.
  - `notify_updates` - Display update notification when playing media. Default: `true`
-    - Notification will only display once until the application is restarted. 
+    - Notification will only display once until the application is restarted.
  - `discord_presence` - Enable Discord rich presence support. Default: `false`
  - `menu_mouse` - Enable mouse support in the menu. Default: `true`
      - This requires MPV to be compiled with lua support.
 
 ### Shell Command Triggers
 
 You can execute shell commands on media state using the config file:
@@ -239,15 +242,16 @@
 
 ### External MPV
 
 The client now supports using an external copy of MPV, including one that is running prior to starting
 the client. This may be useful if your distribution only provides MPV as a binary executable (instead
 of as a shared library), or to connect to MPV-based GUI players. Please note that SMPlayer exhibits
 strange behaviour when controlled in this manner. External MPV is currently the only working backend
-for media playback on macOS.
+for media playback on macOS. Additionally, due to Flatpak sandbox restrictions, external mpv is not
+practical to use in most cases for the Flatpak version.
 
 - `mpv_ext` - Enable usage of the external player by default. Default: `false`
     - The external player may still be used by default if `libmpv1` is not available.
 - `mpv_ext_path` - The path to the `mpv` binary to use. By default it uses the one in the PATH. Default: `null`
     - If you are using Windows, make sure to use two backslashes. Example: `C:\\path\\to\\mpv.exe`
 - `mpv_ext_ipc` - The path to the socket to control MPV. Default: `null`
     - If unset, the socket is a randomly selected temp file.
@@ -305,23 +309,21 @@
  - `shader_pack_remember` - Automatically remember the last used shader profile. (Default: `true`)
  - `shader_pack_profile` - The default profile to use. (Default: `null`)
     - If you use `shader_pack_remember`, this will be updated when you set a profile through the UI.
  - `shader_pack_subtype` - The profile group to use. The default pack contains `lq` and `hq` groups. Use `hq` if you have a fancy graphics card.
 
 ### Trickplay Thumbnails
 
-MPV will automatically display thumbnail previews. By default it uses the Jellyfin chapter images
-but it can also use JellyScrub as the source. Please note that this feature will download and
+MPV will automatically display thumbnail previews. By default it uses the Trickplay images and falls back to chapter images. Please note that this feature will download and
 uncompress all of the chapter images before it becomes available for a video. For a 4 hour movie this
 causes disk usage of about 250 MB, but for the average TV episode it is around 40 MB. It also requires
 overriding the default MPV OSC, which may conflict with some custom user script. Trickplay is compatible
 with any OSC that uses [thumbfast](https://github.com/po5/thumbfast), as I have added a [compatibility layer](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/jellyfin_mpv_shim/thumbfast.lua).
 
  - `thumbnail_enable` - Enable thumbnail feature. (Default: `true`)
- - `thumbnail_jellyscrub` - Use JellyScrub as the thumbnail source instead of chapter images. (Default: `false`)
  - `thumbnail_osc_builtin` - Disable this setting if you want to use your own custom osc but leave trickplay enabled. (Default: `true`)
  - `thumbnail_preferred_size` - The ideal size for thumbnails. (Default: `320`)
 
 ### SVP Integration
 
 To enable SVP integration, set `svp_enable` to `true` and enable "External control via HTTP" within SVP
 under Settings > Control options. Adjust the `svp_url` and `svp_socket` settings if needed.
@@ -438,24 +440,24 @@
 
 Run `xrandr`. It should look something like this:
 
 ```
 Screen 0: minimum 8 x 8, current 3520 x 1080, maximum 16384 x 16384
 VGA-0 connected 1920x1080+0+0 (normal left inverted right x axis y axis) 521mm x 293mm
    1920x1080     60.00*+
-   1680x1050     59.95  
-   1440x900      59.89  
-   1280x1024     75.02    60.02  
-   1280x960      60.00  
-   1280x800      59.81  
-   1280x720      60.00  
-   1152x864      75.00  
-   1024x768      75.03    70.07    60.00  
-   800x600       75.00    72.19    60.32    56.25  
-   640x480       75.00    59.94  
+   1680x1050     59.95
+   1440x900      59.89
+   1280x1024     75.02    60.02
+   1280x960      60.00
+   1280x800      59.81
+   1280x720      60.00
+   1152x864      75.00
+   1024x768      75.03    70.07    60.00
+   800x600       75.00    72.19    60.32    56.25
+   640x480       75.00    59.94
 LVDS-0 connected 1600x900+1920+180 (normal left inverted right x axis y axis) 309mm x 174mm
    1600x900      59.98*+
 ```
 
 If you want MPV to open on VGA-0 for instance, add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration):
 ```
 fs=yes
@@ -476,16 +478,16 @@
 
 ### MPRIS Plugin (#54)
 
 Set `mpv_ext` to `true` in the config. Add `script=/path/to/mpris.so` to `mpv.conf`.
 
 ### Run Multiple Instances (#45)
 
-You can pass `--config /path/to/folder` to run another copy of the player. Please 
-note that running multiple copies of the desktop client is currently not supported. 
+You can pass `--config /path/to/folder` to run another copy of the player. Please
+note that running multiple copies of the desktop client is currently not supported.
 
 ### Audio Passthrough
 
 You can edit `mpv.conf` to support audio passthrough. A [user on Reddit](https://reddit.com/r/jellyfin/comments/fru6xo/new_cross_platform_desktop_client_jellyfin_mpv/fns7vyp) had luck with this config:
 ```
 audio-spdif=ac3,dts,eac3 # (to use the passthrough to receiver over hdmi)
 audio-channels=2 # (not sure this is necessary, but i keep it in because it works)
@@ -528,15 +530,15 @@
  - Run the program and wait. (You'll probably have to use it for a while.)
  - Let me know if the high memory usage is with `mpv.exe` or the shim itself.
 
 On Linux, the process is similar, except that you don't need to set the `mpv_ext_path` variable.
 On macOS, external MPV is already the default and is the only supported player mode.
 
 In the long term, I may look into a method of terminating MPV when not in use. This will require
-a lot of changes to the software. 
+a lot of changes to the software.
 
 ### Player Sizing (#91)
 
 MPV by default may force the window size to match the video aspect ratio, instead of allowing
 resizing and centering the video accordingly. Add the following to `mpv.conf` to enable resizing
 of the window freely, if desired:
 ```
@@ -567,16 +569,17 @@
 The shaders included in the shader pack are also available under verious open source licenses,
 [which you can read about here](https://github.com/iwalton3/default-shader-pack/blob/master/LICENSE.md).
 
 ### Local Dev Installation
 
 If you are on Windows there are additional dependencies. Please see the Windows Build Instructions.
 
-1. Install the dependencies: `sudo pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
+1. Install the dependencies: `pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
     - If you run `./gen_pkg.sh --install`, it will also fetch these for you.
+    - Note: Recent distributions make pip unusable by default. Consider using conda or add a virtualenv to your user's path.
 2. Clone this repository: `git clone https://github.com/jellyfin/jellyfin-mpv-shim`
     - You can also download a zip build.
 3. `cd` to the repository: `cd jellyfin-mpv-shim`
 4. Run prepare script: `./gen_pkg.sh`
     - To do this manually, download the web client, shader pack, and build the language files.
 5. Ensure you have a copy of `libmpv1` or `mpv` available.
 6. Install any platform-specific dependencies from the respective install tutorials.
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/action_thread.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/action_thread.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/bulk_subtitle.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bulk_subtitle.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 def render_message(message, show_text):
     log.info(message)
     messages.append(message)
     text = _("Selecting Tracks...")
     for message in messages[-6:]:
         text += "\n   " + message
-    show_text(text, 2 ** 30, 1)
+    show_text(text, 2**30, 1)
 
 
 def process_series(mode, player: "PlayerManager_type", m_raid=None, m_rsid=None):
     messages.clear()
     media = player.get_video()
     client = media.client
     show_text = player.show_text
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/clients.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 from typing import Optional
 
 
 def expo(max_value: Optional[int] = None):
     n = 0
     while True:
-        a = 2 ** n
+        a = 2**n
         if max_value is None or a < max_value:
             yield a
             n += 1
         else:
             yield max_value
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/conf.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     play_cmd: Optional[str] = None
     idle_cmd_delay: int = 60
     direct_paths: bool = False
     remote_direct_paths: bool = False
     always_transcode: bool = False
     transcode_hi10p: bool = False
     transcode_hdr: bool = False
+    transcode_hevc: bool = False
+    transcode_av1: bool = False
+    transcode_4k: bool = False
     transcode_dolby_vision: bool = True
     allow_transcode_to_h265: bool = False
     prefer_transcode_to_h265: bool = False
     remote_kbps: int = 10000
     local_kbps: int = 2147483
     subtitle_size: int = 100
     subtitle_color: str = "#FFFFFFFF"
@@ -123,15 +126,14 @@
     raise_mpv: bool = True
     force_video_codec: Optional[str] = None
     force_audio_codec: Optional[str] = None
     health_check_interval: Optional[int] = 300
     skip_intro_always: bool = False
     skip_intro_prompt: bool = False
     thumbnail_enable: bool = True
-    thumbnail_jellyscrub: bool = False
     thumbnail_osc_builtin: bool = True
     thumbnail_preferred_size: int = 320
 
     def __get_file(self, path: str, mode: str = "r", create: bool = True):
         created = False
 
         if not os.path.exists(path):
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/conffile.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conffile.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/constants.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 APP_NAME = "jellyfin-mpv-shim"
 USER_APP_NAME = "Jellyfin MPV Shim"
-CLIENT_VERSION = "2.6.0"
+CLIENT_VERSION = "2.7.0"
 USER_AGENT = "Jellyfin-MPV-Shim/%s" % CLIENT_VERSION
 CAPABILITIES = {
     "PlayableMediaTypes": "Video",
     "SupportsMediaControl": True,
     "SupportedCommands": (
         "MoveUp,MoveDown,MoveLeft,MoveRight,Select,"
         "Back,ToggleFullscreen,"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/README.md` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/README.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/pack.json` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/display_mirror/__init__.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/display_mirror/helpers.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # Is this stuff in there already?
 #
 # FIXME: A lot of this could be done so much better with format-strings
 
 
 # noinspection PyPep8Naming,PyPep8Naming
 def getUrl(serverAddress, name):
-
     if not name:
         raise Exception("Url name cannot be empty")
 
     url = serverAddress
     url += "/" if not serverAddress.endswith("/") and not name.startswith("/") else ""
     url += name
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/event_handler.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/event_handler.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/gui_mgr.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/gui_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import logging
 import queue
 
 from .constants import USER_APP_NAME, APP_NAME
 from .conffile import confdir
 from .clients import clientManager
 from .utils import get_resource
-from .log_utils import CustomFormatter
+from .log_utils import CustomFormatter, root_logger
 from .i18n import _
 
 log = logging.getLogger("gui_mgr")
 
 # From https://stackoverflow.com/questions/6631299/
 # This is for opening the config directory.
 
@@ -41,22 +41,20 @@
 
 try:
     show_file = _show_file_func[sys.platform]
 
     def open_config():
         show_file(confdir(APP_NAME))
 
-
 except KeyError:
     open_config = None
     log.warning("Platform does not support opening folders.")
 
 # Setup a log handler for log items.
 log_cache = deque([], 1000)
-root_logger = logging.getLogger("")
 
 
 class GUILogHandler(logging.Handler):
     def __init__(self):
         self.callback = None
         super().__init__()
 
@@ -456,15 +454,15 @@
             MenuItem(_("Configure Servers"), get_wrapper("show_preferences")),
             MenuItem(_("Show Console"), get_wrapper("show_console")),
             MenuItem(_("Application Menu"), get_wrapper("open_player_menu")),
             MenuItem(_("Open Config Folder"), get_wrapper("open_config_brs")),
             MenuItem(_("Quit"), die),
         ]
 
-        icon = Icon(USER_APP_NAME, menu=Menu(*menu_items))
+        icon = Icon(APP_NAME, title=USER_APP_NAME, menu=Menu(*menu_items))
         icon.icon = Image.open(get_resource("systray.png"))
         self.icon_stop = icon.stop
 
         def setup(icon: Icon):
             icon.visible = True
             self.r_queue.put(("ready", None))
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/i18n.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/i18n.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml`

 * *Files 2% similar despite different names*

#### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml`

```diff
@@ -1,16 +1,18 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- Copyright 2020 Ian Walton <ian@iwalton.com> -->
+<!-- Copyright 2020 Izzie Walton <izzie@iwalton.com> -->
 <component type="desktop-application">
   <id>com.github.iwalton3.jellyfin-mpv-shim</id>
   <metadata_license>FSFAP</metadata_license>
   <project_license>GPL-3.0</project_license>
   <name>Jellyfin MPV Shim</name>
   <summary>Cast-only client for Jellyfin Media Server</summary>
-  <developer_name>Ian Walton</developer_name>
+  <developer id="com.github.iwalton3">
+    <name>Izzie Walton</name>
+  </developer>
   <description>
     <p>Jellyfin MPV Shim is a client for the Jellyfin media server which plays media in the
         MPV media player. The application runs in the background and opens MPV only
         when media is cast to the player. The player supports most file formats, allowing you
         to prevent needless transcoding of your media files on the server. The player also has
         advanced features, such as bulk subtitle updates and launching commands on events.</p>
     <p>Please read the detailed instructions on GitHub for more details, including usage
@@ -41,16 +43,26 @@
     </screenshot>
   </screenshots>
   <launchable type="desktop-id">com.github.iwalton3.jellyfin-mpv-shim.desktop</launchable>
   <url type="homepage">https://github.com/jellyfin/jellyfin-mpv-shim</url>
   <provides>
     <binary>jellyfin-mpv-shim</binary>
   </provides>
+  <launchable type="desktop-id">com.github.iwalton3.jellyfin-mpv-shim.desktop</launchable>
   <content_rating type="oars-1.1"/>
   <releases>
+    <release version="2.7.0" date="2024-05-13">
+      <description>
+        <li>Switch to native Jellyfin Trickplay support.</li>
+        <li>Update mpv version to latest git version.</li>
+        <li>Fix support for newer MPV versions. (#377)</li>
+        <li>Make log level configurable. (#379)</li>
+        <li>Fix icon title. (#380)</li>
+      </description>
+    </release>
     <release version="2.6.0" date="2023-03-07">
       <description>
         <p>Disable built-in MPV playback resuming. (#323)</p>
         <p>Support IPv6 addressing with a protocol prefix (#306)</p>
         <p>Switch to mpv build 20230304 362256e with TLS 1.3 support.</p>
         <p>Fix DEL stock MPV shortcut. (#326)</p>
         <p>Fix endless video skipping with auto profiles. (#323)</p>
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-128.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-128.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-16.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-16.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-256.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-256.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-32.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-32.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-48.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-48.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/integration/jellyfin-64.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-64.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/log_utils.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/log_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,25 @@
         "'X-MediaBrowser-Token': 'REDACTED'",
     ),
     (re.compile("'AccessToken': '[a-f0-9]*'"), "'AccessToken': 'REDACTED'"),
 )
 
 sanitize_logs = False
 root_logger = logging.getLogger("")
-root_logger.level = logging.DEBUG
+root_logger.level = logging.INFO
+level_mapping = {
+    "CRITICAL": 50,
+    "FATAL": 50,
+    "ERROR": 40,
+    "WARN": 30,
+    "WARNING": 30,
+    "INFO": 20,
+    "DEBUG": 10,
+    "NOTSET": 0,
+}
 
 
 def sanitize(message):
     if type(message) in (int, float):
         return message
     if message is not str and message is not bytes:
         message = str(message)
@@ -48,18 +58,24 @@
 
 
 def enable_sanitization():
     global sanitize_logs
     sanitize_logs = True
 
 
-def configure_log(destination):
+def configure_log(destination, level: str = "info"):
+    lvl = level_mapping[level.upper()]
+
     handler = logging.StreamHandler(destination)
     handler.setFormatter(CustomFormatter())
+    handler.setLevel(lvl)
     root_logger.addHandler(handler)
 
 
-def configure_log_file(destination: str):
+def configure_log_file(destination: str, level: str = "info"):
+    lvl = level_mapping[level.upper()]
+
     handler = logging.FileHandler(destination, mode="w")
     # Never allow logging API keys to a file.
     handler.setFormatter(CustomFormatter(True))
+    handler.setLevel(lvl)
     root_logger.addHandler(handler)
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/media.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/media.py`

 * *Files 5% similar despite different names*

```diff
@@ -168,15 +168,14 @@
             (
                 self.media_source.get("Protocol") == "Http"
                 or self.media_source["SupportsDirectPlay"]
             )
             and settings.direct_paths
             and (settings.remote_direct_paths or self.parent.is_local)
         ):
-
             if platform.startswith("win32") or platform.startswith("cygwin"):
                 # matches on SMB scheme
                 match = re.search("(?:\\\\).+:.*@(.+)", self.media_source["Path"])
                 if match:
                     # replace forward slash to backward slashes
                     log.debug("cleaned up credentials from path")
                     self.media_source["Path"] = str(
@@ -267,50 +266,39 @@
                 f"Items/{self.item_id}/Images/Chapter/{i}",
                 data,
                 {"tag": item["ImageTag"], "maxWidth": max_width, "quality": quality},
             )
             yield data.getvalue()
 
     def get_hls_tile_images(self, width, count):
-        for i in range(1, count + 1):
+        for i in range(0, count):
             data = BytesIO()
             self.client.jellyfin._get_stream(
-                f"Trickplay/{self.media_source['Id']}/{width}/{i}.jpg", data
+                f"Videos/{self.item['Id']}/Trickplay/{width}/{i}.jpg?MediaSourceId={self.media_source['Id']}",
+                data,
             )
             yield data.getvalue()
 
     def get_bif(self, prefer_width=320):
-        # requires JellyScrub plugin
-        manifest = self.client.jellyfin._get(
-            f"Trickplay/{self.media_source['Id']}/GetManifest"
-        )
+        manifest = self.item.get("Trickplay")
         if (
             manifest is not None
-            and manifest.get("WidthResolutions") is not None
-            and len(manifest["WidthResolutions"]) > 0
+            and manifest.get(self.media_source["Id"]) is not None
+            and len(manifest[self.media_source["Id"]]) > 0
         ):
-            available_widths = manifest["WidthResolutions"]
-            if type(manifest["WidthResolutions"]) is dict:
-                available_widths = [int(x) for x in manifest["WidthResolutions"].keys()]
+            available_widths = [
+                int(x) for x in manifest[self.media_source["Id"]].keys()
+            ]
 
             if prefer_width is not None:
                 width = min(available_widths, key=lambda x: abs(x - prefer_width))
             else:
                 width = max(available_widths)
 
-            if type(manifest["WidthResolutions"]) is dict:
-                return manifest["WidthResolutions"][str(width)]
-            else:
-                data = BytesIO()
-                self.client.jellyfin._get_stream(
-                    f"Trickplay/{self.media_source['Id']}/{width}/GetBIF", data
-                )
-
-                data.seek(0)
-                return data
+            return manifest[self.media_source["Id"]][str(width)]
         else:
             return None
 
     def get_playback_url(
         self,
         video_bitrate: Optional[int] = None,
         force_transcode: Optional[int] = False,
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/menu.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             menu_text = self.menu_title
         for i, item in enumerate(items):
             fmt = "\n   {0}"
             if i == selected_item and not self.mouse_back:
                 fmt = "\n   **{0}**"
             menu_text += fmt.format(item[0])
 
-        self.playerManager.show_text(menu_text, 2 ** 30, 1)
+        self.playerManager.show_text(menu_text, 2**30, 1)
 
     def mouse_select(self, idx: int):
         if idx < 0 or idx > len(self.menu_list):
             return
         if idx == 0:
             self.mouse_back = True
         else:
@@ -554,16 +554,13 @@
                     _("Discord Rich Presence"), "discord_presence"
                 ),
                 self.get_settings_toggle(_("Always Skip Intros"), "skip_intro_always"),
                 self.get_settings_toggle(_("Ask to Skip Intros"), "skip_intro_prompt"),
                 self.get_settings_toggle(
                     _("Enable thumbnail previews"), "thumbnail_enable"
                 ),
-                self.get_settings_toggle(
-                    _("Use JellyScrub thumbnails"), "thumbnail_jellyscrub"
-                ),
             ],
         )
 
     def unwatched_menu_handle(self):
         self.playerManager.put_task(self.playerManager.unwatched_quit)
         self.playerManager.timeline_handle()
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-01-09 16:51+0000\n"
-"Last-Translator: Stephen Cox <stephencoxmail@gmail.com>\n"
+"PO-Revision-Date: 2023-11-30 09:30+0000\n"
+"Last-Translator: Bryan T <weblate@bryanturner.co.za>\n"
 "Language-Team: Afrikaans <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/af/>\n"
 "Language: af\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -36,14 +36,17 @@
 
 msgid "Black"
 msgstr "Swart"
 
 msgid "Blue"
 msgstr "Blou"
 
+msgid "Bottom"
+msgstr "Onderkant"
+
 msgid "Change Audio"
 msgstr "Verander Klank"
 
 msgid "Change Subtitles"
 msgstr "Verander Onderskrifte"
 
 msgid "Change Video Playback Profile"
@@ -67,14 +70,17 @@
 msgstr ""
 "Kon nie server byvoeg nie.\n"
 "Gaan u na verbindingsinligting toe."
 
 msgid "Cyan"
 msgstr "Siaan"
 
+msgid "English Audio"
+msgstr "Engelse Klank"
+
 msgid "Fail"
 msgstr "Misluk"
 
 msgid "Gray"
 msgstr "Grys"
 
 msgid "Green"
@@ -94,20 +100,26 @@
 
 msgid "Magenta"
 msgstr "Magenta"
 
 msgid "Main Menu"
 msgstr "Hoof Kieslys"
 
+msgid "Manual by Track Index (Less Reliable)"
+msgstr "Handleiding volgens Snitindeks (Minder Betroubaar)"
+
 msgid "Manual: {0} ok, {1} fail"
 msgstr "Handleiding: {0} ok, {1} misluk"
 
 msgid "Maximum"
 msgstr "Maksimum"
 
+msgid "Middle"
+msgstr "Middelkant"
+
 msgid "No Transcode"
 msgstr "Geen transkodering"
 
 msgid "None"
 msgstr "Geen"
 
 msgid "Normal"
@@ -151,14 +163,26 @@
 
 msgid "Select Audio Track"
 msgstr "Kies Klankbaan"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Kies Klank/Sub-titels vir Reeks"
 
+msgid "Select Default Transcode Profile"
+msgstr "Kies Verstek Transkodeerprofiel"
+
+msgid "Select Subtitle Color"
+msgstr "Kies Sub-titel Kleur"
+
+msgid "Select Subtitle Position"
+msgstr "Kies Sub-titel Posisie"
+
+msgid "Select Subtitle Size"
+msgstr "Kies Sub-titel Grootte"
+
 msgid "Select Subtitle Track"
 msgstr "Kies sub titels"
 
 msgid "Select Transcode Quality"
 msgstr "Kies transkodeer kwaliteit"
 
 msgid "Select your media in Jellyfin and play it here"
@@ -196,14 +220,20 @@
 
 msgid "SyncPlay"
 msgstr "SyncPlay"
 
 msgid "Tiny"
 msgstr "Baie klein"
 
+msgid "Top"
+msgstr "Bokant"
+
+msgid "Transcode HDR"
+msgstr "Transkodeer HDR"
+
 msgid "Username:"
 msgstr "Verbruikersnaam:"
 
 msgid "Username: "
 msgstr "Naam: "
 
 msgid "Video Playback Profiles"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-12-27 09:51+0000\n"
-"Last-Translator: 0TTA <osamh735@gmail.com>\n"
+"PO-Revision-Date: 2023-04-04 21:39+0000\n"
+"Last-Translator: AmmarAlhawsawi <ammaralhawsawi@outlook.com>\n"
 "Language-Team: Arabic <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/ar/>\n"
 "Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
@@ -28,14 +28,17 @@
 
 msgid "Add another server?"
 msgstr "إضافة خادم آخر؟"
 
 msgid "Adding server failed."
 msgstr "فشل إضافة الخادم."
 
+msgid "Always Skip Intros"
+msgstr "تخطى المقدمات دائما"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (ل HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (ل HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "سجل التطبيق"
 
 msgid "Application Menu"
 msgstr "قائمة التطبيق"
 
+msgid "Ask to Skip Intros"
+msgstr "اسأل لتخطي المقدمات"
+
 msgid "Auto Fullscreen"
 msgstr "تكبير الشاشة تلقائي"
 
 msgid "Auto Play"
 msgstr "التشغيل التلقائي"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -131,14 +137,17 @@
 
 msgid "Display Mirroring"
 msgstr "انعكاس الشاشة"
 
 msgid "Enable SVP"
 msgstr "تفعيل SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "تمكين الصور المصغرة للمعاينة"
+
 msgid "English Audio"
 msgstr "صوت إنجليزي"
 
 msgid "Fail"
 msgstr "فشل"
 
 msgid "Generic (FSRCNNX)"
@@ -255,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "لقطة الشاشة"
 
 msgid "Season {0} - Episode {1}"
 msgstr "الموسم {0} - الحلقة {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "قم بالتنقل لتتخطى المقدمة"
+
 msgid "Select Audio Track"
 msgstr "تحديد مقطع الصوت"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "تحديد الصوت/الترجمة للمسلسلات"
 
 msgid "Select Default Transcode Profile"
@@ -315,14 +327,17 @@
 
 msgid "Show Console"
 msgstr "إظهار وحدة التحكم"
 
 msgid "SkipToSync (x{0})"
 msgstr "تخطي للمزامنة (x{0})"
 
+msgid "Skipped Intro"
+msgstr "تم تخطي المقدمة"
+
 msgid "Small"
 msgstr "صغير"
 
 msgid "SpeedToSync (x{0})"
 msgstr "سرعة المزامنة (×{0})"
 
 msgid "Subtitle Color: {0}"
@@ -357,14 +372,17 @@
 
 msgid "Tiny"
 msgstr "صغير جدا"
 
 msgid "Top"
 msgstr "الأعلى"
 
+msgid "Transcode HDR"
+msgstr "رمز إلى H265"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "رمز Hi10p إلى 8bit"
 
 msgid "Unkn"
 msgstr "غير معروف"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -381,17 +381,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Перакадзіраваць Hi10p у 8біт"
 
 msgid "Unkn"
 msgstr "Невядомы"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Выкарыстоўваць JellyScrub мініацюры"
-
 msgid "Use Web Seek Pref"
 msgstr "Выкарыстоўвайце функцыю Web Seek Pref"
 
 msgid "Username:"
 msgstr "Імя карыстальніка:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-01-19 13:24+0000\n"
-"Last-Translator: marcus2799 <marcus@mail.bg>\n"
+"PO-Revision-Date: 2023-08-15 18:34+0000\n"
+"Last-Translator: Stefan <starchasmnyx@abv.bg>\n"
 "Language-Team: Bulgarian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/bg/>\n"
 "Language: bg\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -28,14 +28,17 @@
 
 msgid "Add another server?"
 msgstr "Добавяне на друг сървър?"
 
 msgid "Adding server failed."
 msgstr "Добавянето на сървъра е неуспешно."
 
+msgid "Always Skip Intros"
+msgstr "Винаги пропускай въведенията"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Надеждно (за ВК)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Перцептивно (за ВК)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Лог на програмата"
 
 msgid "Application Menu"
 msgstr "Меню на приложението"
 
+msgid "Ask to Skip Intros"
+msgstr "Питай за пропуск на въведенията"
+
 msgid "Auto Fullscreen"
 msgstr "Автоматично на цял екран"
 
 msgid "Auto Play"
 msgstr "Автоматично стартиране"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -109,15 +115,15 @@
 "Моля,проверете информацията за връзката."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr ""
 "Създаването на група за \"синхронизирано възпроизвеждане\" не е позволено."
 
 msgid "Cyan"
-msgstr "Синьо-зелен"
+msgstr "Светлосиньо"
 
 msgid "Direct Paths"
 msgstr "Директни пътища"
 
 msgid "Disable"
 msgstr "Изключи"
 
@@ -132,14 +138,17 @@
 
 msgid "Display Mirroring"
 msgstr "Дублиране на дисплея"
 
 msgid "Enable SVP"
 msgstr "Включи SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Активиране преглед на миниатюрни визуализации"
+
 msgid "English Audio"
 msgstr "Английско аудио"
 
 msgid "Fail"
 msgstr "Грешка"
 
 msgid "Generic (FSRCNNX)"
@@ -154,15 +163,15 @@
 msgid "Green"
 msgstr "Зелен"
 
 msgid "Huge"
 msgstr "Огромен"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "Японско аудио със /Английски субтитри"
+msgstr "Японско аудио с /Английски субтитри"
 
 msgid "Large"
 msgstr "Голям"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} Информация за версия/Свали"
 
@@ -256,14 +265,17 @@
 
 msgid "Screenshot"
 msgstr "Снимка на екрана"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Сезон {0} - Епизод {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Търсене за пропускане на въведението"
+
 msgid "Select Audio Track"
 msgstr "Избери аудио пътека"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Избери Аудио/Субтитри за сезона"
 
 msgid "Select Default Transcode Profile"
@@ -316,14 +328,17 @@
 
 msgid "Show Console"
 msgstr "Покажи конзола"
 
 msgid "SkipToSync (x{0})"
 msgstr "Забавяне до синхронизиране (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Пропуснато въведение"
+
 msgid "Small"
 msgstr "Малък"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Скорост до синхронизация (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -359,14 +374,17 @@
 
 msgid "Tiny"
 msgstr "Много малък"
 
 msgid "Top"
 msgstr "Горе"
 
+msgid "Transcode HDR"
+msgstr "Транскодирай HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Транскодирай Hi10p до 8bit"
 
 msgid "Unkn"
 msgstr "Непознат"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,17 +1,17 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "PO-Revision-Date: 2022-08-06 12:22+0000\n"
 "Last-Translator: Daniel Papasergio <daniel.papasergio@outlook.com>\n"
-"Language-Team: Bengali <https://translate.jellyfin.org/projects/jellyfin/"
-"jellyfin-desktop/bn/>\n"
-"Language: bn\n"
+"Language-Team: Malayalam <https://translate.jellyfin.org/projects/jellyfin/"
+"jellyfin-desktop/ml/>\n"
+"Language: ml\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.10.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid "Small"
-msgstr "ছোট"
+msgstr "ചെറിയ"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -380,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Překódovat Hi10p na 8bit"
 
 msgid "Unkn"
 msgstr "Nezn"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Zobrazit náhledy na časové ose JellyScrub"
-
 msgid "Use Web Seek Pref"
 msgstr "Použít nastavení posouvání na webu"
 
 msgid "Username:"
 msgstr "Uživatelské jméno:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-03-28 00:28+0000\n"
-"Last-Translator: Rhodri <rhodrilld@gmail.com>\n"
+"PO-Revision-Date: 2023-05-07 21:39+0000\n"
+"Last-Translator: Brett Healey <Bearach.goll@gmail.com>\n"
 "Language-Team: Welsh <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/cy/>\n"
 "Language: cy\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=6; plural=(n==0) ? 0 : (n==1) ? 1 : (n==2) ? 2 : "
 "(n==3) ? 3 :(n==6) ? 4 : 5;\n"
-"X-Generator: Weblate 4.10.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Trawsgodio)"
 
 msgid " Forced"
 msgstr " Gorfodol"
@@ -28,35 +28,44 @@
 
 msgid "Add another server?"
 msgstr "Ychwanegu gweinydd arall?"
 
 msgid "Adding server failed."
 msgstr "Methwyd ychwanegu gweinydd."
 
+msgid "Always Skip Intros"
+msgstr "Hepgor Rhagarweiniadau bob amser"
+
 msgid "Anime4K x2 Faithful (For HD)"
-msgstr "Anime4K x2 Faithful (For HD)"
+msgstr "Anime4K x2 Ffyddlon (Ar gyfer HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
-msgstr "Anime4K x2 Perceptual (For HD)"
+msgstr "Anime4K x2 Canfyddiadol (Ar gyfer HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
-msgstr "Anime4K x2 Perceptual + Deblur (For HD)"
+msgstr "Anime4K x2 Canfyddiadol + Deblur (Ar gyfer HD)"
 
 msgid "Anime4K x4 Faithful (For SD)"
-msgstr "Anime4K x4 Faithful (For SD)"
+msgstr "Anime4K x4 Ffyddlon (Ar gyfer SD)"
+
+msgid "Anime4K x4 Perceptual (For SD)"
+msgstr "Anime4K x4 Canfyddiadol (Ar gyfer SD)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
-msgstr "Anime4K x4 Perceptual + Deblur (For SD)"
+msgstr "Anime4K x4 Canfyddiadol + Deblur (Ar gyfer SD)"
 
 msgid "Application Log"
 msgstr "Log Rhaglen"
 
 msgid "Application Menu"
 msgstr "Dewislen Rhaglen"
 
+msgid "Ask to Skip Intros"
+msgstr "Gofynnwch i Hepgor Intros"
+
 msgid "Auto Fullscreen"
 msgstr "Sgrîn Lawn Awtomatig"
 
 msgid "Auto Play"
 msgstr "Awto-Chwarae"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -120,22 +129,25 @@
 msgid "Disable Direct Play"
 msgstr "Diffodd Direct Play"
 
 msgid "Disabled"
 msgstr "Wedi'i ddiffodd"
 
 msgid "Discord Rich Presence"
-msgstr "Discord Rich Presence"
+msgstr "Presenoldeb Cyfoethog Discord"
 
 msgid "Display Mirroring"
 msgstr "Efelychu Dangosydd"
 
 msgid "Enable SVP"
 msgstr "Dechrau SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Galluogi rhagolwg mân-luniau"
+
 msgid "English Audio"
 msgstr "Sain Saesneg"
 
 msgid "Fail"
 msgstr "Methu"
 
 msgid "Generic (FSRCNNX)"
@@ -171,17 +183,26 @@
 
 msgid "Magenta"
 msgstr "Magenta"
 
 msgid "Main Menu"
 msgstr "Prif ddewislen"
 
+msgid "Manual by Track Index (Less Reliable)"
+msgstr "Llawlyfr yn ôl Mynegai Trac (Llai Dibynadwy)"
+
+msgid "Manual: {0} ok, {1} fail"
+msgstr "Llawlyfr: {0} iawn, {1} methu"
+
 msgid "Maximum"
 msgstr "Macsimwm"
 
+msgid "Media Key Seek"
+msgstr "Ceisio Allwedd Cyfryngau"
+
 msgid "Middle"
 msgstr "Canol"
 
 msgid "New Group"
 msgstr "Grwp Newydd"
 
 msgid "No Transcode"
@@ -243,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "Sgrinlun"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Cyfres {0} - Pennod {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Ceisio Hepgor y Cyflwyniad"
+
 msgid "Select Audio Track"
 msgstr "Dewiswch Trac Sain"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Dewis Sain/Is-deitl ar gyfer Cyfres"
 
 msgid "Select Default Transcode Profile"
@@ -294,20 +318,26 @@
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "Gosod Dwbio: {0} iawn, {1} sain yn unig, {2} methu"
 
 msgid "Set Subbed: {0} ok, {1} fail"
 msgstr "Gosod is-deitlau: {0} iawn, {1} methu"
 
+msgid "Setting Current..."
+msgstr "Gosod Cyfredol..."
+
 msgid "Show Console"
 msgstr "Dangos Console"
 
 msgid "SkipToSync (x{0})"
 msgstr "SgipioIGydweddu (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Wedi hepgor y Cyflwyniad"
+
 msgid "Small"
 msgstr "Bach"
 
 msgid "SpeedToSync (x{0})"
 msgstr "CyflymuIGydweddu (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -322,15 +352,15 @@
 msgid "Successfully added server."
 msgstr "Ychwanegwyd gweinydd yn llwyddiannus."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Cydweddu wedi'i Diffodd (Gormod o Geisiadau)"
 
 msgid "SyncPlay"
-msgstr "SyncPlay"
+msgstr "ChwaraeCysoni"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay wedi'i ddiffodd."
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay wedi'i ddechrau."
 
@@ -342,32 +372,44 @@
 
 msgid "Tiny"
 msgstr "Bychan"
 
 msgid "Top"
 msgstr "Top"
 
+msgid "Transcode HDR"
+msgstr "Trawsgodio HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Trawsgodio o Hi10p i 8bit"
 
 msgid "Unkn"
 msgstr "Anhysbys"
 
+msgid "Use Web Seek Pref"
+msgstr "Defnyddiwch Web Seek Pref"
+
 msgid "Username:"
 msgstr "Enw defnyddiwr:"
 
 msgid "Username: "
 msgstr "Enw defnyddiwr: "
 
 msgid "Video Playback Profiles"
 msgstr "Proffiliau Chwarae"
 
 msgid "Video Preferences"
 msgstr "Dewisiadau Fideo"
 
+msgid "Video Profile Subtype"
+msgstr "Is-deip Proffil Fideo"
+
+msgid "Video Profile Subtype: {0}"
+msgstr "Is-fath Proffil Fideo: {0}"
+
 msgid "White"
 msgstr "Gwyn"
 
 msgid "Write Logs to File"
 msgstr "Ysgrifennu Logiau i Ffeil"
 
 msgid "Yellow"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-04 09:51+0000\n"
-"Last-Translator: Max <madstk1@pm.me>\n"
+"PO-Revision-Date: 2023-03-28 22:39+0000\n"
+"Last-Translator: heim3x <heim3x@proton.me>\n"
 "Language-Team: Danish <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/da/>\n"
 "Language: da\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -27,38 +27,44 @@
 
 msgid "Add another server?"
 msgstr "Tilføj en anden server?"
 
 msgid "Adding server failed."
 msgstr "Tilføjelse af serveren fejlede."
 
+msgid "Always Skip Intros"
+msgstr "Altid spring over introer"
+
 msgid "Anime4K x2 Faithful (For HD)"
-msgstr "Anime4K x2 Faithful (For HD)"
+msgstr "Anime4K x2 Faithful (Til HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
-msgstr "Anime4K x2 Perceptual (For HD)"
+msgstr "Anime4K x2 Perceptual (Til HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
-msgstr "Anime4K x2 Perceptual + Deblur (For HD)"
+msgstr "Anime4K x2 Perceptual + anti-sløring (til HD)"
 
 msgid "Anime4K x4 Faithful (For SD)"
-msgstr "Anime4K x4 Faithful (For SD)"
+msgstr "Anime4K x4 Faithful (Til SD)"
 
 msgid "Anime4K x4 Perceptual (For SD)"
-msgstr "Anime4K x4 Perceptual (For SD)"
+msgstr "Anime4K x4 Perceptual (Til SD)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
-msgstr "Anime4K x4 Perceptual + Deblur (For SD)"
+msgstr "Anime4K x4 Perceptual + anti-sløring (Til SD)"
 
 msgid "Application Log"
 msgstr "Applikationslog"
 
 msgid "Application Menu"
 msgstr "Applikation menu"
 
+msgid "Ask to Skip Intros"
+msgstr "Spørg om at spring over introer"
+
 msgid "Auto Fullscreen"
 msgstr "Automatisk fuldskærm"
 
 msgid "Auto Play"
 msgstr "Automatisk afspilning"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -107,15 +113,15 @@
 "Kunne ikke tilføje serveren.\n"
 "Venligst undersøg din internet forbindelse."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Oprettelse af SyncPlay gruppe er ikke tilladt."
 
 msgid "Cyan"
-msgstr "Turkisblå"
+msgstr "Cyan"
 
 msgid "Direct Paths"
 msgstr "Direkte stier"
 
 msgid "Disable"
 msgstr "Deaktiver"
 
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "Vis spejling"
 
 msgid "Enable SVP"
 msgstr "Aktiver SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Aktiver forhåndsvisning af thumbnails"
+
 msgid "English Audio"
 msgstr "Engelsk lyd"
 
 msgid "Fail"
 msgstr "Fejl"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Skærmbillede"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sæson {0} - Afsnit {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Søg til Spring over Intro"
+
 msgid "Select Audio Track"
 msgstr "Skift lyd spor"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Skift lyd/undertekster for serier"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Vis konsol"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Introer sprunget over"
+
 msgid "Small"
 msgstr "Lille"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Meget lille"
 
 msgid "Top"
 msgstr "Top"
 
+msgid "Transcode HDR"
+msgstr "Omkod til HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Omkod Hi10p til 8bit"
 
 msgid "Unkn"
 msgstr "Ukendt"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-03-07 10:39+0000\n"
-"Last-Translator: mweylandt <mweylandt@gmail.com>\n"
+"PO-Revision-Date: 2023-07-13 11:41+0000\n"
+"Last-Translator: Achim Walz <achim@aalso-walz.de>\n"
 "Language-Team: German <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -55,15 +55,15 @@
 msgid "Application Log"
 msgstr "Anwendungslogs"
 
 msgid "Application Menu"
 msgstr "Applikationsmenü"
 
 msgid "Ask to Skip Intros"
-msgstr "Nachfragen ob Intros übersprungen werden sollen"
+msgstr "Nachfragen, ob Intros übersprungen werden sollen"
 
 msgid "Auto Fullscreen"
 msgstr "Automatisch Vollbild"
 
 msgid "Auto Play"
 msgstr "Automatisch Abspielen"
 
@@ -137,15 +137,15 @@
 msgid "Display Mirroring"
 msgstr "Bildschirmspiegelung"
 
 msgid "Enable SVP"
 msgstr "SVP aktivieren"
 
 msgid "Enable thumbnail previews"
-msgstr "Aktiviere Thumbnail Vorschau"
+msgstr "Miniaturvorschauen aktivieren"
 
 msgid "English Audio"
 msgstr "Englische Tonspur"
 
 msgid "Fail"
 msgstr "Fehler"
 
@@ -192,15 +192,15 @@
 msgid "Manual: {0} ok, {1} fail"
 msgstr "Manuell: {0} Ok, {1} Fehler"
 
 msgid "Maximum"
 msgstr "Maximum"
 
 msgid "Media Key Seek"
-msgstr "Medien Spultaste"
+msgstr "Medienspultaste"
 
 msgid "Middle"
 msgstr "Mitte"
 
 msgid "New Group"
 msgstr "Neue Gruppe"
 
@@ -240,15 +240,15 @@
 msgid "Ready to cast"
 msgstr "Bereit für Übertragung"
 
 msgid "Red"
 msgstr "Rot"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
-msgstr "Remote Transkodierungsqualität: {0:0.1f} Mbps"
+msgstr "Remote-Transkodierungsqualität: {0:0.1f} Mbps"
 
 msgid "Remove Server"
 msgstr "Server entfernen"
 
 msgid "Retry"
 msgstr "Wiederholen"
 
@@ -264,15 +264,15 @@
 msgid "Screenshot"
 msgstr "Bildschirmfoto"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Staffel {0} - Folge {1}"
 
 msgid "Seek to Skip Intro"
-msgstr "Versuche Intro zu überspringen"
+msgstr "Versuche, Intro zu überspringen"
 
 msgid "Select Audio Track"
 msgstr "Audiospur wählen"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Audio/Untertitel für Serie wählen"
 
@@ -324,24 +324,24 @@
 msgid "Setting Current..."
 msgstr "Setze aktuelle Einstellung..."
 
 msgid "Show Console"
 msgstr "Konsole anzeigen"
 
 msgid "SkipToSync (x{0})"
-msgstr "SkipToSync (x{0})"
+msgstr "Springe zum Synchronisieren (x{0})"
 
 msgid "Skipped Intro"
 msgstr "Intro übersprungen"
 
 msgid "Small"
 msgstr "Klein"
 
 msgid "SpeedToSync (x{0})"
-msgstr "SpeedToSync (x{0})"
+msgstr "Geschwindigkeit zum Synchronisieren (x{0})"
 
 msgid "Subtitle Color: {0}"
 msgstr "Untertitelfarbe: {0}"
 
 msgid "Subtitle Position: {0}"
 msgstr "Untertitelposition: {0}"
 
@@ -380,28 +380,25 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkodiere Hi10p zu 8bit"
 
 msgid "Unkn"
 msgstr "Unbekannt"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Verwände JellyScrub Thumbnails"
-
 msgid "Use Web Seek Pref"
 msgstr "Verwende Spul-Einstellungen aus dem Internet"
 
 msgid "Username:"
 msgstr "Benutzername:"
 
 msgid "Username: "
 msgstr "Benutzername: "
 
 msgid "Video Playback Profiles"
-msgstr "Video Abspielprofile"
+msgstr "Videowiedergabeprofile"
 
 msgid "Video Preferences"
 msgstr "Videoeinstellungen"
 
 msgid "Video Profile Subtype"
 msgstr "Videoprofil-Subtyp"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-01-09 16:51+0000\n"
-"Last-Translator: Retrial <giwrgosmant@gmail.com>\n"
+"PO-Revision-Date: 2023-10-06 07:31+0000\n"
+"Last-Translator: [   ] <christiangrece45@gmail.com>\n"
 "Language-Team: Greek <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/el/>\n"
 "Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "Προσθήκη άλλου διακομιστή;"
 
 msgid "Adding server failed."
 msgstr "Η προσθήκη διακομιστή απέτυχε."
 
+msgid "Always Skip Intros"
+msgstr "Πάντα να παραλείπονται οι εισαγωγές"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (για HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (για HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Αρχείο καταγραφής Εφαρμογής"
 
 msgid "Application Menu"
 msgstr "Μενού Εφαρμογής"
 
+msgid "Ask to Skip Intros"
+msgstr "Να γίνεται ερώτηση για να παραλείπονται οι εισαγωγές"
+
 msgid "Auto Fullscreen"
 msgstr "Αυτόματη Πλήρης οθόνη"
 
 msgid "Auto Play"
 msgstr "Αυτόματη Αναπαραγωγή"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "Κατοπτρισμός Οθόνης"
 
 msgid "Enable SVP"
 msgstr "Ενεργοποίηση SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Προεπισκόπηση μικρογραφίας ενεργή"
+
 msgid "English Audio"
 msgstr "Αγγλικός Ήχος"
 
 msgid "Fail"
 msgstr "Αποτυχία"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Στιγμιότυπο οθόνης"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Κύκλος {0} - Επεισόδιο {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Επιδιώξτε να παραλείψετε την εισαγωγή"
+
 msgid "Select Audio Track"
 msgstr "Επιλέξτε Κομμάτι Ήχου"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Επιλέξτε Ήχο/Υπότιτλο για Σειρές"
 
 msgid "Select Default Transcode Profile"
@@ -303,25 +315,28 @@
 msgid "Server:"
 msgstr "Διακομιστής:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "Ορισμός Μεταγλώττισης: {0} εντάξει, {1} μόνο ήχος, {2} αποτυχία"
 
 msgid "Set Subbed: {0} ok, {1} fail"
-msgstr "Ορισμός Υπότιτλου: {0} εντάξει, {1} αποτυχία"
+msgstr "Ορισμός ως υποτιτλισμένο: {0} εντάξει, {1} αποτυχία"
 
 msgid "Setting Current..."
 msgstr "Τρέχον Ρύθμιση..."
 
 msgid "Show Console"
 msgstr "Εμφάνιση Κονσόλας"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Παράλειψη Εισαγωγής"
+
 msgid "Small"
 msgstr "Μικρό"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Μικροσκοπικό"
 
 msgid "Top"
 msgstr "Πάνω"
 
+msgid "Transcode HDR"
+msgstr "Διακωδικοποίηση σε HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Διακωδικοποίηση Hi10p σε 8bit"
 
 msgid "Unkn"
 msgstr "Unkn"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -380,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcode Hi10p to 8bit"
 
 msgid "Unkn"
 msgstr "Unknown"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Use JellyScrub thumbnails"
-
 msgid "Use Web Seek Pref"
 msgstr "Use Web Seek Pref"
 
 msgid "Username:"
 msgstr "Username:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,39 +1,39 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-08 20:51+0000\n"
-"Last-Translator: ManuXD32 <manuelgm344@gmail.com>\n"
-"Language-Team: Spanish <https://translate.jellyfin.org/projects/jellyfin/"
-"jellyfin-desktop/es/>\n"
-"Language: es\n"
+"PO-Revision-Date: 2023-07-08 13:41+0000\n"
+"Last-Translator: D <dln0@proton.me>\n"
+"Language-Team: Galician <https://translate.jellyfin.org/projects/jellyfin/"
+"jellyfin-desktop/gl/>\n"
+"Language: gl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
-msgid " (Transcode)"
-msgstr " (Transcodificar)"
-
 msgid " Forced"
 msgstr " Forzado"
 
 msgid "Access to the SyncPlay library was denied."
-msgstr "Se denegó el acceso a la biblioteca SyncPlay."
+msgstr "O acceso á biblioteca SyncPlay foi denegado."
 
 msgid "Add Server"
-msgstr "Añadir Servidor"
+msgstr "Engadir servidor"
 
 msgid "Add another server?"
-msgstr "¿Añadir otro servidor?"
+msgstr "Engadir outro servidor?"
 
 msgid "Adding server failed."
-msgstr "No se pudo añadir el servidor."
+msgstr "Non foi posíbel engadir o servidor."
+
+msgid "Always Skip Intros"
+msgstr "Saltar introdución sempre"
 
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (para HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (para HD)"
 
@@ -46,378 +46,374 @@
 msgid "Anime4K x4 Perceptual (For SD)"
 msgstr "Anime4K x4 Perceptual (para SD)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
 msgstr "Anime4K x4 Perceptual + Deblur (para SD)"
 
 msgid "Application Log"
-msgstr "Registro de la aplicación"
+msgstr "Rexistros da aplicación"
 
 msgid "Application Menu"
-msgstr "Menú de la aplicación"
+msgstr "Menú da aplicación"
+
+msgid "Ask to Skip Intros"
+msgstr "Solicitar saltar as introduccións"
 
 msgid "Auto Fullscreen"
 msgstr "Pantalla Completa Automática"
 
 msgid "Auto Play"
-msgstr "Auto-Reproducción"
+msgstr "Auto-Reprodución"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
-msgstr "Ajuste Automático de Audio/Subtítulos (Serie Completa)"
+msgstr "Axuste automático de Audio/Subtítulos (Todas as series)"
 
 msgid "Automatic"
 msgstr "Automático"
 
 msgid "Black"
 msgstr "Negro"
 
 msgid "Blue"
 msgstr "Azul"
 
-msgid "Bottom"
-msgstr "Inferior"
-
 msgid "Change Audio"
 msgstr "Cambiar Audio"
 
 msgid "Change Subtitles"
-msgstr "Cambiar subtítulos"
+msgstr "Cambiar Subtítulos"
 
 msgid "Change Video Playback Profile"
-msgstr "Cambiar el Perfil de Reproducción de Video"
+msgstr "Cambiar Perfil de Reprodución de Vídeo"
 
 msgid "Change Video Quality"
-msgstr "Cambiar Calidad de Video"
+msgstr "Cambiar Calidade de Vídeo"
 
 msgid "Check for Updates"
-msgstr "Buscar Actualizaciones"
+msgstr "Buscar Actualizacións"
 
 msgid "Close"
-msgstr "Cerrar"
+msgstr "Fechar"
 
 msgid "Close Menu"
-msgstr "Cerrar Menú"
+msgstr "Fechar Menú"
 
 msgid "Configure Servers"
-msgstr "Configurar servidores"
+msgstr "Configurar Servidores"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
-"No se pudo agregar el servidor.\n"
-"Compruebe la información de su conexión."
+"Non foi posíbel engadir o servidor.\n"
+"Por favor, revise os parámetros de conexión."
 
 msgid "Creating SyncPlay groups is not allowed."
-msgstr "No se permite la creación de grupos SyncPlay."
+msgstr "Non se permite a creación de grupos SyncPlay."
 
 msgid "Cyan"
 msgstr "Cian"
 
 msgid "Direct Paths"
-msgstr "Rutas Directas"
+msgstr "Localizacións Directas"
 
 msgid "Disable"
 msgstr "Deshabilitar"
 
 msgid "Disable Direct Play"
-msgstr "Desactivar la Reproducción Directa"
+msgstr "Deshabilitar a Reprodución Directa"
 
 msgid "Disabled"
 msgstr "Deshabilitado"
 
 msgid "Discord Rich Presence"
-msgstr "Presencia en Discord"
+msgstr "Discord Rich Presence"
 
 msgid "Display Mirroring"
 msgstr "Duplicación de Pantalla"
 
 msgid "Enable SVP"
 msgstr "Habilitar SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Activar vistas previas na miniatura"
+
 msgid "English Audio"
 msgstr "Audio en Inglés"
 
 msgid "Fail"
-msgstr "Falla"
+msgstr "Fallo"
 
 msgid "Generic (FSRCNNX)"
-msgstr "Genérica (FSRCNNX)"
+msgstr "Xenérica (FSRCNNX)"
 
 msgid "Generic High (FSRCNNX x16)"
-msgstr "Genérica Alta (FSRCNNX x16)"
+msgstr "Xenérica Alta (FSRCNNX x16)"
 
 msgid "Gray"
 msgstr "Gris"
 
 msgid "Green"
 msgstr "Verde"
 
 msgid "Huge"
 msgstr "Enorme"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "Audio en Japonés con Subtítulos en Inglés"
+msgstr "Audio en Xaponés con Subtítulos en Inglés"
 
 msgid "Large"
 msgstr "Grande"
 
 msgid "MPV Shim v{0} Release Info/Download"
-msgstr "MPV Shim v {0} Información de Versión/Descarga"
+msgstr "MPV Shim v{0} Información de Versión/Descarga"
 
 msgid ""
 "MPV Shim v{0} Update Available\n"
 "Open menu (press c) for details."
 msgstr ""
-"MPV Shim v {0} Actualización Disponible\n"
-"Abra el menú (presione c) para obtener detalles."
+"MPV Shim v{0} Actualización dispoñíbel \n"
+"Abra o menú (prema c) para obter detalles."
 
 msgid "Magenta"
-msgstr "Magenta"
+msgstr "Maxenta"
 
 msgid "Main Menu"
 msgstr "Menú principal"
 
 msgid "Manual by Track Index (Less Reliable)"
-msgstr "Manual por índice de pista (menos confiable)"
+msgstr "Manual por índice de pista (menos confiábel)"
 
 msgid "Manual: {0} ok, {1} fail"
-msgstr "Manual: {0} ok, {1} falló"
-
-msgid "Maximum"
-msgstr "Máxima"
+msgstr "Manual: {0} ok, {1} fallo"
 
 msgid "Media Key Seek"
-msgstr "Búsqueda de Tecla Multimedia"
+msgstr "Busca de Tecla Multimedia"
 
 msgid "Middle"
 msgstr "Medio"
 
 msgid "New Group"
-msgstr "Nuevo Grupo"
+msgstr "Novo Grupo"
 
 msgid "No Transcode"
-msgstr "Sin Transcodificación"
+msgstr "Sen Transcodificación"
 
 msgid "None"
-msgstr "Nada"
+msgstr "Ningún"
 
 msgid "None (Disabled)"
-msgstr "Ninguna (Deshabilitada)"
+msgstr "Ningunha (Deshabilitada)"
 
 msgid "Normal"
 msgstr "Normal"
 
 msgid "Ok"
 msgstr "Ok"
 
 msgid "Open Config Folder"
-msgstr "Abrir carpeta de configuración"
+msgstr "Abrir o cartafol de configuración"
 
 msgid "Password:"
-msgstr "Contraseña:"
+msgstr "Contrasinal:"
 
 msgid "Password: "
-msgstr "Contraseña: "
+msgstr "Contrasinal: "
 
 msgid "Player Preferences"
-msgstr "Preferencias Reproductor"
+msgstr "Preferencias do Reprodutor"
 
 msgid "Quit"
-msgstr "Salir"
+msgstr "Saír"
 
 msgid "Quit and Mark Unwatched"
-msgstr "Salir y Marcar como No Visto"
-
-msgid "Ready to cast"
-msgstr "Listo para cast"
+msgstr "Saír e Marcar como Non visto"
 
 msgid "Red"
-msgstr "Rojo"
+msgstr "Vermello"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
 msgstr "Calidad de Transcodificación Remota: {0: 0.1f} Mbps"
 
 msgid "Remove Server"
-msgstr "Eliminar servidor"
+msgstr "Eliminar Servidor"
 
 msgid "Retry"
 msgstr "Reintentar"
 
 msgid "SVP Settings"
 msgstr "Configuración de SVP"
 
 msgid "SVP is Disabled"
-msgstr "SVP está Deshabilitada"
+msgstr "SVP está Deshabilitado"
 
 msgid "SVP is Not Active"
-msgstr "SVP no está activa"
+msgstr "SVP non está activo"
 
 msgid "Screenshot"
 msgstr "Captura de pantalla"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Temporada {0} - Episodio {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Intentar saltar a introdución"
+
 msgid "Select Audio Track"
-msgstr "Seleccionar Pista de Audio"
+msgstr "Selecionar Faixa de Audio"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "Seleccionar Audio/Subtítulo de la serie"
+msgstr "Seleccionar Audio/Subtítulo da serie"
 
 msgid "Select Default Transcode Profile"
 msgstr "Seleccionar perfil de transcodificación predeterminado"
 
 msgid "Select SVP Profile"
 msgstr "Seleccionar Perfil de SVP"
 
 msgid "Select Shader Profile"
 msgstr "Seleccionar Perfil de Sombras"
 
 msgid "Select Subtitle Color"
-msgstr "Seleccionar Color de Subtítulos"
+msgstr "Selecione a Cor dos Subtítulos"
 
 msgid "Select Subtitle Position"
-msgstr "Seleccionar Posición de Subtítulo"
+msgstr "Seleccione Posición de Subtítulo"
 
 msgid "Select Subtitle Size"
-msgstr "Seleccione el Tamaño de los Subtítulos"
+msgstr "Seleccione o Tamaño dos Subtítulos"
 
 msgid "Select Subtitle Track"
-msgstr "Seleccionar Pista de Subtítulos"
+msgstr "Selecionar Faixa de Subtítulos"
 
 msgid "Select Transcode Quality"
-msgstr "Seleccionar Calidad de Transcodificación"
+msgstr "Seleccionar Calidade de Transcodificación"
 
 msgid "Select your media in Jellyfin and play it here"
-msgstr "Seleccione su contenido multimedia en Jellyfin y reprodúzcalo aquí"
+msgstr "Seleccione a súa multimedia en Jellyfin e reprodúzaa aquí"
 
 msgid "Selecting Tracks..."
-msgstr "Seleccionando Pistas..."
+msgstr "A seleccionar Faixas..."
 
 msgid "Server Configuration"
-msgstr "Configuración del servidor"
+msgstr "Configuración do Servidor"
 
 msgid "Server URL: "
-msgstr "URL del Servidor: "
+msgstr "URL do servidor: "
 
 msgid "Server:"
 msgstr "Servidor:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
-msgstr "Establecer doblaje: {0} ok, {1} solo audio, {2} falló"
+msgstr "Definir como dobrado: {0} ok, {1} só audio, {2} fallo"
 
 msgid "Set Subbed: {0} ok, {1} fail"
-msgstr "Establecer subtitulado: {0} ok, {1} falló"
+msgstr "Definir como subtítulo: {0} ok, {1} fallo"
 
 msgid "Setting Current..."
 msgstr "Configuración actual..."
 
 msgid "Show Console"
-msgstr "Muestra la consola"
+msgstr "Ver Consola"
 
 msgid "SkipToSync (x{0})"
-msgstr "Saltar a la Sincronización (x{0})"
+msgstr "Saltar a Sincronización (x{0})"
+
+msgid "Skipped Intro"
+msgstr "Introdución Saltada"
 
 msgid "Small"
-msgstr "Pequeño"
+msgstr "Pequeno"
 
 msgid "SpeedToSync (x{0})"
-msgstr "Velocidad para la Sincronización(x{0})"
+msgstr "Velocidade para a Sincronización(x{0})"
 
 msgid "Subtitle Color: {0}"
-msgstr "Color de Subtítulos: {0}"
+msgstr "Cor de Subtítulos: {0}"
 
 msgid "Subtitle Position: {0}"
-msgstr "Posición de los Subtítulos: {0}"
+msgstr "Posición dos Subtítulos: {0}"
 
 msgid "Subtitle Size: {0}"
 msgstr "Tamaño de Subtítulo: {0}"
 
 msgid "Successfully added server."
-msgstr "Servidor añadido exitosamente."
+msgstr "Servidor engadido existosamente."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sincronización Desactivada (Demasiados Intentos)"
 
 msgid "SyncPlay"
 msgstr "SyncPlay"
 
 msgid "SyncPlay disabled."
-msgstr "SyncPlay Deshabilitada."
+msgstr "SyncPlay deshabilitado."
 
 msgid "SyncPlay enabled."
-msgstr "SyncPlay Habilitado."
+msgstr "SyncPlay habilitado."
 
 msgid "SyncPlay group access was denied."
-msgstr "Se denegó el acceso al grupo SyncPlay."
+msgstr "O acceso ao grupo SyncPlay foi denegado."
 
 msgid "The specified SyncPlay group does not exist."
-msgstr "El grupo SyncPlay especificado no existe."
+msgstr "O grupo SyncPlay especificado non existe."
 
 msgid "Tiny"
-msgstr "Minúscula"
-
-msgid "Top"
-msgstr "Superior"
+msgstr "Minúsculo"
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcodificar Hi10p a 8bit"
 
 msgid "Unkn"
-msgstr "Desconocido"
-
-msgid "Use Web Seek Pref"
-msgstr "Usar pref. de búsqueda web"
+msgstr "Descoñecido"
 
 msgid "Username:"
 msgstr "Usuario:"
 
 msgid "Username: "
 msgstr "Usuario: "
 
 msgid "Video Playback Profiles"
-msgstr "Perfiles de Reproducción de Video"
+msgstr "Perfís de Reprodución de Vídeo"
 
 msgid "Video Preferences"
-msgstr "Preferencias de Video"
+msgstr "Preferencias de Vídeo"
 
 msgid "Video Profile Subtype"
 msgstr "Subtipo de Perfil de Vídeo"
 
 msgid "Video Profile Subtype: {0}"
 msgstr "Subtipo de Perfil de Vídeo: {0}"
 
 msgid "White"
-msgstr "Blanco"
+msgstr "Branco"
 
 msgid "Write Logs to File"
-msgstr "Escribir Registros en Archivo"
+msgstr "Escribir Rexistros en Arquivo"
 
 msgid "Yellow"
-msgstr "Amarillo"
+msgstr "Amarelo"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
-"¡El video remoto se está transcodificando!\n"
-"Si esto no es necesario presionar c para ajustar la configuración del ancho "
-"de banda."
+"O seu vídeo remoto está a se transcodificar \n"
+"Se non for necesario, prema c para axustar a largura de banda."
 
 msgid "{0} has joined."
-msgstr "{0} se ha unido."
+msgstr "{0} xuntouse."
 
 msgid "{0} has left."
-msgstr "{0} se ha ido."
+msgstr "{0} foise."
 
 msgid "{0} is buffering."
-msgstr "{0} está almacenando en búfer."
+msgstr "{0} está almacenado no búfer."
 
 msgid "{0}'s Group"
 msgstr "Grupo de {0}"
 
 msgid "{0}: Fail"
-msgstr "{0}: Falló"
+msgstr "{0}: Fallo"
 
 msgid "{0}: No Subtitles"
-msgstr "{0}: Sin Subtítulos"
+msgstr "{0}: Sen Subtítulos"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-08-25 22:11+0000\n"
-"Last-Translator: Asadito Familiar <asaditofamiliarremix@gmail.com>\n"
+"PO-Revision-Date: 2023-05-23 16:21+0000\n"
+"Last-Translator: Oswaldo Arias <github@arias.pw>\n"
 "Language-Team: Spanish (Latin America) <https://translate.jellyfin.org/"
 "projects/jellyfin/jellyfin-desktop/es_419/>\n"
 "Language: es_419\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transcodificar)"
 
 msgid " Forced"
 msgstr " Forzado"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "¿Agregar otro servidor?"
 
 msgid "Adding server failed."
 msgstr "Error al agregar el servidor."
 
+msgid "Always Skip Intros"
+msgstr "Siempre omitir intro"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Constante (Para HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (Para HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Registro de la aplicación"
 
 msgid "Application Menu"
 msgstr "Menú de la Aplicación"
 
+msgid "Ask to Skip Intros"
+msgstr "Preguntar para saltar intro"
+
 msgid "Auto Fullscreen"
 msgstr "Pantalla Completa Automáticamente"
 
 msgid "Auto Play"
 msgstr "Reproducir Automáticamente"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "Duplicar Pantalla"
 
 msgid "Enable SVP"
 msgstr "Habilitar SVP (Conversión de Velocidad de Fotogramas)"
 
+msgid "Enable thumbnail previews"
+msgstr "Activar vista previa de miniaturas"
+
 msgid "English Audio"
 msgstr "Audio en Inglés"
 
 msgid "Fail"
 msgstr "Error"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Captura de pantalla"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Temporada {0} - Episodio {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Intentar omitir intro"
+
 msgid "Select Audio Track"
 msgstr "Seleccionar Pista de Audio"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Seleccionar el Audio/Subtítulo para las Series"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Mostrar consola"
 
 msgid "SkipToSync (x{0})"
 msgstr "Saltar para Sincronizar (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Intro omitida"
+
 msgid "Small"
 msgstr "Pequeño"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Velocidad para Sincronizar (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Minúsculo"
 
 msgid "Top"
 msgstr "Arriba"
 
+msgid "Transcode HDR"
+msgstr "Transcodificar a HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcodificar Hi10p a 8bit"
 
 msgid "Unkn"
 msgstr "Desconocido"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,432 +1,440 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-07-19 22:22+0000\n"
-"Last-Translator: Franco Castillo <castillofrancodamian@gmail.com>\n"
-"Language-Team: Spanish (Argentina) <https://translate.jellyfin.org/projects/"
-"jellyfin/jellyfin-desktop/es_AR/>\n"
-"Language: es_AR\n"
+"PO-Revision-Date: 2023-04-23 01:39+0000\n"
+"Last-Translator: MrOscarvs <oscarvilluendas7@gmail.com>\n"
+"Language-Team: Catalan <https://translate.jellyfin.org/projects/jellyfin/"
+"jellyfin-desktop/ca/>\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.10.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transcodificar)"
 
 msgid " Forced"
-msgstr " Forzado"
+msgstr " Forçat"
 
 msgid "Access to the SyncPlay library was denied."
-msgstr "Se denegó el acceso a la biblioteca SyncPlay."
+msgstr "S'ha denegat l'accés a la llibreria de SyncPlay."
 
 msgid "Add Server"
-msgstr "Añadir Servidor"
+msgstr "Afegir Servidor"
 
 msgid "Add another server?"
-msgstr "¿Agregar otro servidor?"
+msgstr "Afegir un altre servidor?"
 
 msgid "Adding server failed."
-msgstr "Error al agregar el servidor."
+msgstr "Error a l'afegir el servidor."
 
 msgid "Always Skip Intros"
-msgstr "Omitir siempre las intros"
+msgstr "Saltar introduccions sempre"
 
 msgid "Anime4K x2 Faithful (For HD)"
-msgstr "Anime4K x2 Fiel (para HD)"
+msgstr "Anime4K x2 Faithful (Per a alta resolució)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
-msgstr "Anime4K x2 Perceptual (para HD)"
+msgstr "Anime4K x2 Perceptual (Per a alta resolució)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
-msgstr "Anime4K x2 Perceptual + Deblur (para HD)"
+msgstr "Anime4K x2 Perceptual + Deblur (Per a alta resolució)"
 
 msgid "Anime4K x4 Faithful (For SD)"
-msgstr "Anime4K x4 Fiel (para SD)"
+msgstr "Anime4K x4 Faithful (Per a resolució estàndar)"
 
 msgid "Anime4K x4 Perceptual (For SD)"
-msgstr "Anime4K x4 Perceptual (para SD)"
+msgstr "Anime4K x4 Perceptual (Per a resolució estàndar)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
-msgstr "Anime4K x4 Perceptual + Deblur (para SD)"
+msgstr "Anime4K x4 Perceptual + Deblur (Per a resolució estàndar)"
 
 msgid "Application Log"
-msgstr "Registro de la aplicación"
+msgstr "Registre de l'aplicació"
 
 msgid "Application Menu"
-msgstr "Menú de Aplicación"
+msgstr "Menú de l'aplicació"
 
 msgid "Ask to Skip Intros"
-msgstr "Preguntar para saltar las intros"
+msgstr "Demanar saltar introduccions"
 
 msgid "Auto Fullscreen"
-msgstr "Pantalla completa automática"
+msgstr "Pantalla Completa Automàtica"
 
 msgid "Auto Play"
-msgstr "Auto-reproducción"
+msgstr "Reproducció Automàtica"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
-msgstr "Ajuste automático de audio/subtítulos (serie completa)"
+msgstr "Configuració Automàtica d'Àudio/Subtítols (Serie Completa)"
 
 msgid "Automatic"
-msgstr "Automático"
+msgstr "Automàtic"
 
 msgid "Black"
-msgstr "Negro"
+msgstr "Negre"
 
 msgid "Blue"
-msgstr "Azul"
+msgstr "Blau"
 
 msgid "Bottom"
-msgstr "Fondo"
+msgstr "Inferior"
 
 msgid "Change Audio"
-msgstr "Cambiar Audio"
+msgstr "Canviar l'àudio"
 
 msgid "Change Subtitles"
-msgstr "Cambiar Subtítulos"
+msgstr "Canviar els subtítols"
 
 msgid "Change Video Playback Profile"
-msgstr "Cambiar el perfil de reproducción de vídeo"
+msgstr "Canviar el Perfil de Reproducció de Vídeo"
 
 msgid "Change Video Quality"
-msgstr "Cambiar Calidad del Vídeo"
+msgstr "Canviar la Qualitat del Vídeo"
 
 msgid "Check for Updates"
-msgstr "Buscar actualizaciones"
+msgstr "Buscar actualitzacions"
 
 msgid "Close"
-msgstr "Cerrar"
+msgstr "Tancar"
 
 msgid "Close Menu"
-msgstr "Cerrar Menú"
+msgstr "Tancar el Menú"
 
 msgid "Configure Servers"
-msgstr "Configurar Servidores"
+msgstr "Configurar Servidors"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
-"No se pudo agregar el servidor.\n"
-"Compruebe la información de conexión."
+"No s'ha pogut afegir el servidor.\n"
+"Si us plau, comprova la informació de la connexió."
 
 msgid "Creating SyncPlay groups is not allowed."
-msgstr "No se permite la creación de grupos SyncPlay."
+msgstr "Crear grups de SyncPlay no està activat."
 
 msgid "Cyan"
 msgstr "Cian"
 
 msgid "Direct Paths"
-msgstr "Rutas directas"
+msgstr "Rutes Directes"
 
 msgid "Disable"
-msgstr "Deshabilitar"
+msgstr "Desactivar"
 
 msgid "Disable Direct Play"
-msgstr "Deshabilitar reproducción directa"
+msgstr "Desactivar la Reproducció Directa"
 
 msgid "Disabled"
-msgstr "Deshabilitado"
+msgstr "Desactivat"
 
 msgid "Discord Rich Presence"
-msgstr "Presencia rica en Discord"
+msgstr "Rich Presence de Discord"
 
 msgid "Display Mirroring"
-msgstr "Duplicación de pantalla"
+msgstr "Duplicació de pantalla"
 
 msgid "Enable SVP"
-msgstr "Habilitar SVP"
+msgstr "Activar SVP"
+
+msgid "Enable thumbnail previews"
+msgstr "Activar la vista prèvia de les miniatures"
 
 msgid "English Audio"
-msgstr "Audio en Inglés"
+msgstr "Àudio en Anglès"
 
 msgid "Fail"
-msgstr "Falló"
+msgstr "Fallada"
 
 msgid "Generic (FSRCNNX)"
-msgstr "Genérico (FSRCNNX)"
+msgstr "Genèric (FSRCNNX)"
 
 msgid "Generic High (FSRCNNX x16)"
-msgstr "Genérico alto (FSRCNNX x16)"
+msgstr "Genèric alt (FSRCNNX x16)"
 
 msgid "Gray"
 msgstr "Gris"
 
 msgid "Green"
-msgstr "Verde"
+msgstr "Verd"
 
 msgid "Huge"
 msgstr "Enorme"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "Audio Japonés con subtítulos en Inglés"
+msgstr "Àudio en Japonés amb Subtítols en Anglès"
 
 msgid "Large"
-msgstr "Grande"
+msgstr "Gran"
 
 msgid "MPV Shim v{0} Release Info/Download"
-msgstr "MPV Shim v{0} Información de versión/descarga"
+msgstr "MPV Shim v{0} Informació de Versió/Descàrrega"
 
 msgid ""
 "MPV Shim v{0} Update Available\n"
 "Open menu (press c) for details."
 msgstr ""
-"MPV Shim v {0} Actualización disponible\n"
-"Abra el menú (presione c) para obtener detalles."
+"Actualització de MPV Shim v{0} disponible\n"
+"Premeu c per obtenir més informació."
 
 msgid "Magenta"
 msgstr "Magenta"
 
 msgid "Main Menu"
 msgstr "Menú Principal"
 
 msgid "Manual by Track Index (Less Reliable)"
-msgstr "Manual por índice de pista (Menos confiable)"
+msgstr "Manual per índex de pista (poc fiable)"
 
 msgid "Manual: {0} ok, {1} fail"
-msgstr "Manual: {0} OK, {1} Fallaron"
+msgstr "Manual: {0} ok, {1} error"
 
 msgid "Maximum"
-msgstr "Máximo"
+msgstr "Màxim"
 
 msgid "Media Key Seek"
-msgstr "Búsqueda de clave multimedia"
+msgstr "Cerca de la Tecla Multimèdia"
 
 msgid "Middle"
-msgstr "Medio"
+msgstr "Mig"
 
 msgid "New Group"
-msgstr "Nuevo grupo"
+msgstr "Grup nou"
 
 msgid "No Transcode"
-msgstr "Sin transcodificación"
+msgstr "No transcodificar"
 
 msgid "None"
-msgstr "Ninguno"
+msgstr "Cap"
 
 msgid "None (Disabled)"
-msgstr "Ninguno (Deshabilitado)"
+msgstr "Cap (desactivat)"
 
 msgid "Normal"
 msgstr "Normal"
 
 msgid "Ok"
-msgstr "OK"
+msgstr "D'acord"
 
 msgid "Open Config Folder"
-msgstr "Abrir carpeta de configuraciones"
+msgstr "Obrir carpeta de configuració"
 
 msgid "Password:"
-msgstr "Contraseña:"
+msgstr "Contrassenya:"
 
 msgid "Password: "
-msgstr "Contraseña: "
+msgstr "Contrasenya: "
 
 msgid "Player Preferences"
-msgstr "Preferencias del reproductor"
+msgstr "Preferències del Reproductor"
 
 msgid "Quit"
-msgstr "Salir"
+msgstr "Sortir"
 
 msgid "Quit and Mark Unwatched"
-msgstr "Salir y marcar como no visto"
+msgstr "Sortir i Marcar com a No Vist"
 
 msgid "Ready to cast"
-msgstr "Listo para transmitir"
+msgstr "Preparat per a cast"
 
 msgid "Red"
-msgstr "Rojo"
+msgstr "Vermell"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
-msgstr "Calidad de transcodificación remota: {0:0.1f} Mbps"
+msgstr "Qualitat de transcodificació remota: {0: 0.1f} Mbps"
 
 msgid "Remove Server"
-msgstr "Remover servidor"
+msgstr "Eliminar Servidor"
 
 msgid "Retry"
 msgstr "Reintentar"
 
 msgid "SVP Settings"
-msgstr "Configuraciones SVP"
+msgstr "Configuració de SVP"
 
 msgid "SVP is Disabled"
-msgstr "SVP está deshabilitado"
+msgstr "SVP està desactivat"
 
 msgid "SVP is Not Active"
-msgstr "SVP no está activo"
+msgstr "SVP no està actiu"
 
 msgid "Screenshot"
 msgstr "Captura de pantalla"
 
 msgid "Season {0} - Episode {1}"
-msgstr "Temporada {0} - Episodio {1}"
+msgstr "Temporada {0} - Episodi {1}"
+
+msgid "Seek to Skip Intro"
+msgstr "Intenta saltar la Introducció"
 
 msgid "Select Audio Track"
-msgstr "Seleccionar pista de audio"
+msgstr "Seleccionar Pista d'Àudio"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "Seleccione audio/subtítulo para Series"
+msgstr "Seleccionar Àudio/Subtítols per a la Sèrie"
 
 msgid "Select Default Transcode Profile"
-msgstr "Seleccione el perfil de transcodificación predeterminado"
+msgstr "Seleccionar el perfil de transcodificació per defecte"
 
 msgid "Select SVP Profile"
 msgstr "Seleccionar perfil SVP"
 
 msgid "Select Shader Profile"
-msgstr "Seleccionar perfil de sombreador"
+msgstr "Seleccionar perfil de shader"
 
 msgid "Select Subtitle Color"
-msgstr "Seleccionar color de subtítulos"
+msgstr "Seleccionar color de Subtítols"
 
 msgid "Select Subtitle Position"
-msgstr "Seleccione la posición de los subtítulos"
+msgstr "Seleccionar posició de Subtítols"
 
 msgid "Select Subtitle Size"
-msgstr "Seleccione el tamaño de los subtítulos"
+msgstr "Seleccionar tamany de Subtítols"
 
 msgid "Select Subtitle Track"
-msgstr "Seleccionar pista de subtítulos"
+msgstr "Seleccionar Pista de Subtítols"
 
 msgid "Select Transcode Quality"
-msgstr "Seleccione la calidad de transcodificación"
+msgstr "Seleccionar la qualitat de transcodificació"
 
 msgid "Select your media in Jellyfin and play it here"
-msgstr "Seleccione su contenido multimedia en Jellyfin y reprodúzcalo aquí"
+msgstr "Selecciona el teu contingut multimèdia a Jellyfin i reprodueix-ho aquí"
 
 msgid "Selecting Tracks..."
-msgstr "Selección de pistas..."
+msgstr "Seleccionant pistes..."
 
 msgid "Server Configuration"
-msgstr "Configuración del Servidor"
+msgstr "Configuració del servidor"
 
 msgid "Server URL: "
-msgstr "URL del Servidor: "
+msgstr "URL del servidor: "
 
 msgid "Server:"
 msgstr "Servidor:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
-msgstr "Establecer doblaje: {0} ok, {1} solo audio, {2} falla"
+msgstr "Establir doblat: {0} ok, {1} només àudio, {2} error"
 
 msgid "Set Subbed: {0} ok, {1} fail"
-msgstr "Establecer subtitulado: {0} ok, {1} falla"
+msgstr "Establir subtitulat: {0} ok, {1} error"
 
 msgid "Setting Current..."
-msgstr "Configuración actual..."
+msgstr "Configuració actual..."
 
 msgid "Show Console"
-msgstr "Mostrar Consola"
+msgstr "Mostrar la consola"
 
 msgid "SkipToSync (x{0})"
-msgstr "SaltarParaSincronizar (x{0})"
+msgstr "Saltar a la Sincronizació (x{0})"
 
 msgid "Skipped Intro"
-msgstr "Intro omitida"
+msgstr "Introducció saltada"
 
 msgid "Small"
-msgstr "Pequeño"
+msgstr "Petit"
 
 msgid "SpeedToSync (x{0})"
-msgstr "SpeedToSync (x{0})"
+msgstr "Velocitat per la Sincronització (x{0})"
 
 msgid "Subtitle Color: {0}"
-msgstr "Color de subtítulos: {0}"
+msgstr "Color de Subtítols: {0}"
 
 msgid "Subtitle Position: {0}"
-msgstr "Posición de los subtítulos: {0}"
+msgstr "Posició de Subtítols: {0}"
 
 msgid "Subtitle Size: {0}"
-msgstr "Tamaño de subtítulo: {0}"
+msgstr "Mida de Subtítols: {0}"
 
 msgid "Successfully added server."
-msgstr "Se ha añadido correctamente el servidor."
+msgstr "Servidor afegit correctament."
 
 msgid "Sync Disabled (Too Many Attempts)"
-msgstr "Sincronización deshabilitada (demasiados intentos)"
+msgstr "Sincronització desactivada (Masses intents)"
 
 msgid "SyncPlay"
-msgstr "SyncPlay"
+msgstr "Reproducció Sincronitzada"
 
 msgid "SyncPlay disabled."
-msgstr "SyncPlay deshabilitado."
+msgstr "SyncPlay desactivat."
 
 msgid "SyncPlay enabled."
-msgstr "SyncPlay habilitado."
+msgstr "SyncPlay activat."
 
 msgid "SyncPlay group access was denied."
-msgstr "Se denegó el acceso al grupo SyncPlay."
+msgstr "S'ha denegat l'accés al grup de SyncPlay."
 
 msgid "The specified SyncPlay group does not exist."
-msgstr "El grupo SyncPlay especificado no existe."
+msgstr "El grup de SyncPlay especificat no existeix."
 
 msgid "Tiny"
-msgstr "Minúsculo"
+msgstr "Diminut"
 
 msgid "Top"
 msgstr "Superior"
 
+msgid "Transcode HDR"
+msgstr "Transcodificar l'HDR"
+
 msgid "Transcode Hi10p to 8bit"
-msgstr "Transcodificar Hi10p a 8bit"
+msgstr "Transcodificació d'Hi10p a 8bit"
 
 msgid "Unkn"
-msgstr "Desconocido"
+msgstr "Desconegut"
 
 msgid "Use Web Seek Pref"
-msgstr "Usar Web Seek Pref"
+msgstr "Utilitzar pref. de cerca web"
 
 msgid "Username:"
-msgstr "Usuario:"
+msgstr "Nom d'usuari:"
 
 msgid "Username: "
-msgstr "Usuario: "
+msgstr "Nom d'usuari: "
 
 msgid "Video Playback Profiles"
-msgstr "Perfiles de reproducción de vídeo"
+msgstr "Perfils de Reproducció de Vídeo"
 
 msgid "Video Preferences"
-msgstr "Preferencias de Vídeo"
+msgstr "Preferències de Vídeo"
 
 msgid "Video Profile Subtype"
-msgstr "Subtipo de perfil de video"
+msgstr "Subtip de Perfil de Vídeo"
 
 msgid "Video Profile Subtype: {0}"
-msgstr "Subtipo de perfil de video: {0}"
+msgstr "Subtip de Perfil de Vídeo: {0}"
 
 msgid "White"
-msgstr "Blanco"
+msgstr "Blanc"
 
 msgid "Write Logs to File"
-msgstr "Escribir registros en archivo"
+msgstr "Escriure registres a l'arxiu"
 
 msgid "Yellow"
-msgstr "Amarillo"
+msgstr "Groc"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
-"¡Tu video remoto se está transcodificando!\n"
-"Presione C para ajustar la configuración del ancho de banda si no es "
-"necesario."
+"El seu vídeo remot s'està transcodificant!\n"
+"Premeu c per ajustar la configuració de l'ample de banda si no és necessari."
 
 msgid "{0} has joined."
-msgstr "{0} se ha unido."
+msgstr "{0} s'ha unit."
 
 msgid "{0} has left."
-msgstr "{0} se ha ido."
+msgstr "{0} ha marxat."
 
 msgid "{0} is buffering."
-msgstr "{0} se está almacenando en búfer."
+msgstr "{0} està en buffer."
 
 msgid "{0}'s Group"
-msgstr "{0} Grupos"
+msgstr "Grup de {0}"
 
 msgid "{0}: Fail"
-msgstr "{0}: Falló"
+msgstr "{0}: Error"
 
 msgid "{0}: No Subtitles"
-msgstr "{0}: Sin subtítulos"
+msgstr "{0}: Sense subtítols"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-12-02 09:10+0000\n"
-"Last-Translator: rimasx <riks_12@hot.ee>\n"
+"PO-Revision-Date: 2024-01-30 14:30+0000\n"
+"Last-Translator: antti202 <anttipel@gmail.com>\n"
 "Language-Team: Estonian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/et/>\n"
 "Language: et\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "Kas lisada teine server?"
 
 msgid "Adding server failed."
 msgstr "Serveri lisamine nurjus."
 
+msgid "Always Skip Intros"
+msgstr "Alati jäta sissejuhatus vahele"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Rakenduse logi"
 
 msgid "Application Menu"
 msgstr "Rakenduse menüü"
 
+msgid "Ask to Skip Intros"
+msgstr "Küsi sissejuhatuse vahelejätmist"
+
 msgid "Auto Fullscreen"
 msgstr "Automaatne täisekraan"
 
 msgid "Auto Play"
 msgstr "Automaatne esitus"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -121,20 +127,26 @@
 
 msgid "Disable Direct Play"
 msgstr "Keela otsene esitus"
 
 msgid "Disabled"
 msgstr "Keelatud"
 
+msgid "Discord Rich Presence"
+msgstr "Discordi Rikas Kohalolek"
+
 msgid "Display Mirroring"
 msgstr "Ekraani peegeldamine"
 
 msgid "Enable SVP"
 msgstr "Luba SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Luba pisipiltide eelvaade"
+
 msgid "English Audio"
 msgstr "Inglise keelne heli"
 
 msgid "Fail"
 msgstr "Nurjumine"
 
 msgid "Generic (FSRCNNX)"
@@ -251,26 +263,32 @@
 
 msgid "Screenshot"
 msgstr "Ekraanipilt"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Hooaeg {0} - episood {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Küsi sissejuhatuse vahelejätmist"
+
 msgid "Select Audio Track"
 msgstr "Vali heliriba"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Vali seriaalile heli/subtiitrid"
 
 msgid "Select Default Transcode Profile"
 msgstr "Vali transkoodimise vaikeprofiil"
 
 msgid "Select SVP Profile"
 msgstr "Vali SVP profiil"
 
+msgid "Select Shader Profile"
+msgstr "Vali Varjutaja Profiil"
+
 msgid "Select Subtitle Color"
 msgstr "Vali subtiitrite värv"
 
 msgid "Select Subtitle Position"
 msgstr "Vali subtiitrite asukoht"
 
 msgid "Select Subtitle Size"
@@ -308,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Kuva konsool"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Sissejuhatus vahele jäetud"
+
 msgid "Small"
 msgstr "Väike"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -350,20 +371,26 @@
 
 msgid "Tiny"
 msgstr "Pisike"
 
 msgid "Top"
 msgstr "Üleval"
 
+msgid "Transcode HDR"
+msgstr "Transkood HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkoodi Hi10p > 8bit"
 
 msgid "Unkn"
 msgstr "Tundmatu"
 
+msgid "Use Web Seek Pref"
+msgstr "Kasuta veebiotsingu eelistust"
+
 msgid "Username:"
 msgstr "Kasutajanimi:"
 
 msgid "Username: "
 msgstr "Kasutajanimi: "
 
 msgid "Video Playback Profiles"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-02 00:51+0000\n"
-"Last-Translator: Peyman M. <peymanr34@outlook.com>\n"
+"PO-Revision-Date: 2024-04-17 01:11+0000\n"
+"Last-Translator: blackcharon <blackcharon142@gmail.com>\n"
 "Language-Team: Persian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/fa/>\n"
 "Language: fa\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (کد رمز)"
 
 msgid " Forced"
 msgstr " اجباری"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "سرور دیگری اضافه شود؟"
 
 msgid "Adding server failed."
 msgstr "افزودن سرور ناموفق بود."
 
+msgid "Always Skip Intros"
+msgstr "رد کردن همیشگی تیتراژ"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "انیمه4K x2 با ایمان (برای HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "انیمه4K x2 ادراکی (برای HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "گزارش برنامه"
 
 msgid "Application Menu"
 msgstr "منوی برنامه"
 
+msgid "Ask to Skip Intros"
+msgstr "برای رد کردن تیتراژ سوال بپرس"
+
 msgid "Auto Fullscreen"
 msgstr "تمام صفحه خودکار"
 
 msgid "Auto Play"
 msgstr "پخش خودکار"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -107,15 +113,15 @@
 "سرور اضافه نشد\n"
 "لطفاً اطلاعات اتصال خود را بررسی کنید."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "ایجاد گروه های همگام سازی پخش مجاز نیست."
 
 msgid "Cyan"
-msgstr "فیروزه ای"
+msgstr "یشمی"
 
 msgid "Direct Paths"
 msgstr "مسیرهای مستقیم"
 
 msgid "Disable"
 msgstr "غیرفعال"
 
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "نمایش آینه"
 
 msgid "Enable SVP"
 msgstr "SVP را فعال کنید"
 
+msgid "Enable thumbnail previews"
+msgstr "فعال کردن پیش‌نمایش های بندانگشتی"
+
 msgid "English Audio"
 msgstr "صوت انگلیسی"
 
 msgid "Fail"
 msgstr "شکست"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "عکس صفحه"
 
 msgid "Season {0} - Episode {1}"
 msgstr "فصل {0} - قسمت {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "پرش برای رد کردن تیتراژ"
+
 msgid "Select Audio Track"
 msgstr "آهنگ صوتی را انتخاب کنید"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "صوتی / زیرنویس را برای سریال انتخاب کنید"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "نمایش کنسول"
 
 msgid "SkipToSync (x{0})"
 msgstr "پرش همگام سازی(x{0})"
 
+msgid "Skipped Intro"
+msgstr "تیتراژ رد شده"
+
 msgid "Small"
 msgstr "کوچک"
 
 msgid "SpeedToSync (x{0})"
 msgstr "سرعت همگام سازی (x {0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "ریز"
 
 msgid "Top"
 msgstr "بالا"
 
+msgid "Transcode HDR"
+msgstr "پردازش و تبدیل HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "کد Hi10p را به 8 بیت تبدیل کنید"
 
 msgid "Unkn"
 msgstr "باز کردن"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-19 13:29+0000\n"
+"PO-Revision-Date: 2023-05-18 17:21+0000\n"
 "Last-Translator: Oskari Lavinto <olavinto@protonmail.com>\n"
 "Language-Team: Finnish <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/fi/>\n"
 "Language: fi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -380,16 +380,16 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkoodaa Hi10p 8bit"
 
 msgid "Unkn"
 msgstr "Tuntematon"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Käytä JellyScrub-pienoiskuvia"
+msgid "Use Web Seek Pref"
+msgstr "Käytä verkkohaun mieltymyksiä"
 
 msgid "Username:"
 msgstr "Käyttäjätunnus:"
 
 msgid "Username: "
 msgstr "Käyttäjätunnus: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2021-12-26 14:05+0000\n"
-"Last-Translator: WWWesten <wwwesten@gmail.com>\n"
+"PO-Revision-Date: 2024-02-10 16:30+0000\n"
+"Last-Translator: hatsiko panado <dedioskimoy96@gmail.com>\n"
 "Language-Team: Filipino <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/fil/>\n"
 "Language: fil\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1 && n != 2 && n != 3 && (n % 10 == 4 "
 "|| n % 10 == 6 || n % 10 == 9);\n"
-"X-Generator: Weblate 4.5.2\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transcode)"
 
 msgid " Forced"
 msgstr " Pilit"
@@ -28,14 +28,17 @@
 
 msgid "Add another server?"
 msgstr "Magdagdag ng isa pang server?"
 
 msgid "Adding server failed."
 msgstr "Nag-fail ang pagdaragdag ng server."
 
+msgid "Always Skip Intros"
+msgstr "I-skip palagi ang mga intro"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (For HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (For HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Log ng Application"
 
 msgid "Application Menu"
 msgstr "Menu ng Application"
 
+msgid "Ask to Skip Intros"
+msgstr "Magtanong muna bago magskip ng intro"
+
 msgid "Auto Fullscreen"
 msgstr "Auto Fullscreen"
 
 msgid "Auto Play"
 msgstr "Auto Play"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -131,14 +137,17 @@
 
 msgid "Display Mirroring"
 msgstr "Display Mirroring"
 
 msgid "Enable SVP"
 msgstr "I-enable ang SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Magpakita ng thumbnail"
+
 msgid "English Audio"
 msgstr "Ingles na Audio"
 
 msgid "Fail"
 msgstr "Nag-fail"
 
 msgid "Generic (FSRCNNX)"
@@ -255,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "Screenshot"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Season {0} - Episode {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Iskip ang intro"
+
 msgid "Select Audio Track"
 msgstr "Piliin ang Audio Track"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Piliin ang Audio/Subtitle para sa Serye"
 
 msgid "Select Default Transcode Profile"
@@ -315,14 +327,17 @@
 
 msgid "Show Console"
 msgstr "Ipakita ang Console"
 
 msgid "SkipToSync (x{0})"
 msgstr "Hindi Pinagana ang Pag-sync (Napakaraming Pagsubok)"
 
+msgid "Skipped Intro"
+msgstr "Skinip ang intro"
+
 msgid "Small"
 msgstr "Maliit"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -357,14 +372,17 @@
 
 msgid "Tiny"
 msgstr "Mas maliit"
 
 msgid "Top"
 msgstr "Itaas"
 
+msgid "Transcode HDR"
+msgstr "I-transcode sa HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "I-transcode ang Hi10p sa 8bit"
 
 msgid "Unkn"
 msgstr "Hindi alam"
 
 msgid "Use Web Seek Pref"
@@ -378,14 +396,20 @@
 
 msgid "Video Playback Profiles"
 msgstr "Mga Profile sa Pag-playback ng Video"
 
 msgid "Video Preferences"
 msgstr "Mga Kagustuhan sa Video"
 
+msgid "Video Profile Subtype"
+msgstr "Uri ng bidyo profile"
+
+msgid "Video Profile Subtype: {0}"
+msgstr "Uri ng bidyo profile: {0}"
+
 msgid "White"
 msgstr "Puti"
 
 msgid "Write Logs to File"
 msgstr "I-write ng mga Log sa File"
 
 msgid "Yellow"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-25 05:39+0000\n"
-"Last-Translator: Valentin COMTE <angenoir71880@gmail.com>\n"
+"PO-Revision-Date: 2023-07-03 17:41+0000\n"
+"Last-Translator: Nicolas Viviani <nicolas.viviani01@gmail.com>\n"
 "Language-Team: French <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
@@ -28,15 +28,15 @@
 msgid "Add another server?"
 msgstr "Ajouter un autre serveur ?"
 
 msgid "Adding server failed."
 msgstr "Échec d'ajout du serveur."
 
 msgid "Always Skip Intros"
-msgstr "Toujours passer l'introduction"
+msgstr "Toujours passer les introductions"
 
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (Pour HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (Pour HD)"
 
@@ -264,15 +264,15 @@
 msgid "Screenshot"
 msgstr "Capture d'écran"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Saison {0} - Épisode {1}"
 
 msgid "Seek to Skip Intro"
-msgstr "Avancer jusqu'après l'introduction"
+msgstr "Avancer pour passer l'introduction"
 
 msgid "Select Audio Track"
 msgstr "Choisir une piste audio"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Choisir l'audio / les sous-titres pour les séries"
 
@@ -327,15 +327,15 @@
 msgid "Show Console"
 msgstr "Afficher la console"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
 msgid "Skipped Intro"
-msgstr "Introduction sautée"
+msgstr "Introduction ignorée"
 
 msgid "Small"
 msgstr "Petit"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
@@ -372,25 +372,22 @@
 msgid "Tiny"
 msgstr "Très petit"
 
 msgid "Top"
 msgstr "Haut"
 
 msgid "Transcode HDR"
-msgstr "Transcoder en H265"
+msgstr "Transcoder le HDR"
 
 msgid "Transcode Hi10p to 8bit"
-msgstr "Transcoder Hi10p vers 8bit"
+msgstr "Transcoder le Hi10p en 8bit"
 
 msgid "Unkn"
 msgstr "Inconnu"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Utiliser les miniatures JellyScrub"
-
 msgid "Use Web Seek Pref"
 msgstr "Utiliser la préf. de recherche web"
 
 msgid "Username:"
 msgstr "Nom d'utilisateur :"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,47 +1,71 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-01-27 08:51+0000\n"
-"Last-Translator: moshiko kar <moshikokar@gmail.com>\n"
+"PO-Revision-Date: 2024-05-06 13:01+0000\n"
+"Last-Translator: Arielnoder <arielnoder@gmail.com>\n"
 "Language-Team: Hebrew <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/he/>\n"
 "Language: he\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1) ? 0 : ((n == 2) ? 1 : ((n > 10 && "
 "n % 10 == 0) ? 2 : 3));\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
-msgstr " (קידוד)"
+msgstr " (המרת קידוד)"
 
 msgid " Forced"
 msgstr " כפוי"
 
 msgid "Access to the SyncPlay library was denied."
-msgstr "SyncPlay"
+msgstr "הגישה לספריית SyncPlay נדחתה."
 
 msgid "Add Server"
 msgstr "הוסף שרת"
 
 msgid "Add another server?"
 msgstr "להוסיף שרת נוסף?"
 
 msgid "Adding server failed."
 msgstr "הוספת השרת כשלה."
 
+msgid "Always Skip Intros"
+msgstr "דלג תמיד על הפתיח"
+
+msgid "Anime4K x2 Faithful (For HD)"
+msgstr "Anime4K x2 Faithful (ל־HD)"
+
+msgid "Anime4K x2 Perceptual (For HD)"
+msgstr "Anime4K x2 Perceptual (ל־HD)"
+
+msgid "Anime4K x2 Perceptual + Deblur (For HD)"
+msgstr "Anime4K x2 Perceptual + Deblur (ל־HD)"
+
+msgid "Anime4K x4 Faithful (For SD)"
+msgstr "Anime4K x4 Faithful (ל־SD)"
+
+msgid "Anime4K x4 Perceptual (For SD)"
+msgstr "Anime4K x4 Perceptual (ל־SD)"
+
+msgid "Anime4K x4 Perceptual + Deblur (For SD)"
+msgstr "Anime4K x4 Perceptual + Deblur (ל־SD)"
+
 msgid "Application Log"
 msgstr "יומן מערכת"
 
 msgid "Application Menu"
 msgstr "תפריט תוכנה"
 
+msgid "Ask to Skip Intros"
+msgstr "בקש לדלג על הפתיח"
+
 msgid "Auto Fullscreen"
 msgstr "מסך מלא אוטומטי"
 
 msgid "Auto Play"
 msgstr "הפעלה אוטומטית"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -113,23 +137,29 @@
 
 msgid "Display Mirroring"
 msgstr "שכפול מסכים"
 
 msgid "Enable SVP"
 msgstr "הפעל SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "הפעל תצוגה מקדימה של תמונות קטנות"
+
 msgid "English Audio"
 msgstr "אדויו באנגלית"
 
 msgid "Fail"
 msgstr "נכשל"
 
 msgid "Generic (FSRCNNX)"
 msgstr "כללי (FSRCNNX)"
 
+msgid "Generic High (FSRCNNX x16)"
+msgstr "גנרי גבוה (FSRCNNX x16)"
+
 msgid "Gray"
 msgstr "אפור"
 
 msgid "Green"
 msgstr "ירוק"
 
 msgid "Huge"
@@ -234,26 +264,32 @@
 
 msgid "Screenshot"
 msgstr "צילום מסך"
 
 msgid "Season {0} - Episode {1}"
 msgstr "עונה {0} - פרק {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "דילוג על ההקדמה"
+
 msgid "Select Audio Track"
 msgstr "בחר פס שמע"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "בחר אודיו/כתוביות עבור סדרה"
 
 msgid "Select Default Transcode Profile"
 msgstr "בחר פרופיל ברירת מחדל עבור קידוד"
 
 msgid "Select SVP Profile"
 msgstr "בחר פרופיל SVP"
 
+msgid "Select Shader Profile"
+msgstr "נא לבחור פרופיל שיידר (Shader)"
+
 msgid "Select Subtitle Color"
 msgstr "בחר צבע כתוביות"
 
 msgid "Select Subtitle Position"
 msgstr "בחר מיקום כתוביות"
 
 msgid "Select Subtitle Size"
@@ -291,14 +327,17 @@
 
 msgid "Show Console"
 msgstr "הצג קונסולה"
 
 msgid "SkipToSync (x{0})"
 msgstr "דלג כדי לתאם (x{0})"
 
+msgid "Skipped Intro"
+msgstr "דילג פתיח"
+
 msgid "Small"
 msgstr "קטן"
 
 msgid "SpeedToSync (x{0})"
 msgstr "האץ כדי לתאם (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -313,34 +352,37 @@
 msgid "Successfully added server."
 msgstr "שרת נוסף בהצלחה."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "סנכרון מושבת (יותר מדי ניסיונות)"
 
 msgid "SyncPlay"
-msgstr "SyncPlay"
+msgstr "צפייה מסונכרנת"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay מושבת."
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay מופעל."
 
 msgid "SyncPlay group access was denied."
-msgstr "SyncPlay"
+msgstr "הגישה לקבוצת SyncPlay נדחתה."
 
 msgid "The specified SyncPlay group does not exist."
 msgstr "קבוצת ה-SyncPlay שצויינה אינה קיימת."
 
 msgid "Tiny"
 msgstr "קטנטן"
 
 msgid "Top"
 msgstr "ראש"
 
+msgid "Transcode HDR"
+msgstr "התמרת HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "קדד Hi10p ל 8bit"
 
 msgid "Unkn"
 msgstr "לא ידוע"
 
 msgid "Use Web Seek Pref"
@@ -383,15 +425,15 @@
 msgid "{0} has joined."
 msgstr "{0} הצטרף."
 
 msgid "{0} has left."
 msgstr "{0} עזב."
 
 msgid "{0} is buffering."
-msgstr "{0} נטען למתמון."
+msgstr "{0} טוען."
 
 msgid "{0}'s Group"
 msgstr "הקבוצה של {0}"
 
 msgid "{0}: Fail"
 msgstr "{0}: כשל"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-11-21 07:33+0000\n"
-"Last-Translator: lukapiplica <github163007297@protonmail.com>\n"
+"PO-Revision-Date: 2024-03-29 06:07+0000\n"
+"Last-Translator: Stjepan Mrgnaić <stjepan.mrganic@gmail.com>\n"
 "Language-Team: Croatian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/hr/>\n"
 "Language: hr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Konverzija formata)"
 
 msgid " Forced"
 msgstr " Prisilno"
@@ -23,19 +23,22 @@
 msgid "Access to the SyncPlay library was denied."
 msgstr "Pristup biblioteci SyncPlay je odbijen."
 
 msgid "Add Server"
 msgstr "Dodaj server"
 
 msgid "Add another server?"
-msgstr "Dodavanje novog servera?"
+msgstr "Želite li dodati drugi server?"
 
 msgid "Adding server failed."
 msgstr "Dodavanje servera neuspješno."
 
+msgid "Always Skip Intros"
+msgstr "Uvijek preskoči najave (intros)"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (za HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (za HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Zapisnik aplikacije"
 
 msgid "Application Menu"
 msgstr "Izbornik aplikacije"
 
+msgid "Ask to Skip Intros"
+msgstr "Pitaj za preskakanje najava (intros)"
+
 msgid "Auto Fullscreen"
 msgstr "Automatski cijeli zaslon"
 
 msgid "Auto Play"
 msgstr "Automatska reprodukcija"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -74,68 +80,74 @@
 msgid "Blue"
 msgstr "Plava"
 
 msgid "Bottom"
 msgstr "Donji rub"
 
 msgid "Change Audio"
-msgstr "Promijenite audio"
+msgstr "Promijenite zapis zvuka"
 
 msgid "Change Subtitles"
 msgstr "Promjena podnaslova"
 
 msgid "Change Video Playback Profile"
 msgstr "Promijeni profil video reprodukcije"
 
 msgid "Change Video Quality"
 msgstr "Promjena kvalitete videozapisa"
 
 msgid "Check for Updates"
-msgstr "Provjeri ažuriranja"
+msgstr "Provjeri za ažuriranja"
 
 msgid "Close"
 msgstr "Zatvori"
 
 msgid "Close Menu"
 msgstr "Zatvori izbornik"
 
 msgid "Configure Servers"
-msgstr "Konfiguriraj poslužitelja"
+msgstr "Konfiguriraj servere"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
 "Nije moguće dodati server.\n"
 "Molimo provjerite postavke veze."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Stvaranje SyncPlay grupa nije dopušteno."
 
 msgid "Cyan"
-msgstr "Cijan"
+msgstr "Tirkizna"
+
+msgid "Direct Paths"
+msgstr "Direktne putanje"
 
 msgid "Disable"
 msgstr "Onemogući"
 
 msgid "Disable Direct Play"
 msgstr "Onemogući Direct Play"
 
 msgid "Disabled"
 msgstr "Onemogućeno"
 
 msgid "Discord Rich Presence"
-msgstr "Discord bogata prisutnost"
+msgstr "Status na aplikaciji Discord"
 
 msgid "Display Mirroring"
-msgstr "Zrcaljenje zaslona"
+msgstr "Dijeljenje zaslona"
 
 msgid "Enable SVP"
 msgstr "Omogući SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Omogući pregled sličica"
+
 msgid "English Audio"
 msgstr "Engleski zvuk"
 
 msgid "Fail"
 msgstr "Greška"
 
 msgid "Generic (FSRCNNX)"
@@ -153,15 +165,15 @@
 msgid "Huge"
 msgstr "Ogromno"
 
 msgid "Japanese Audio w/ English Subtitles"
 msgstr "Japanski zvuk sa engleskim titlovima"
 
 msgid "Large"
-msgstr "Veliki"
+msgstr "Veliko"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} Informacije o izdanju/Preuzimanje"
 
 msgid ""
 "MPV Shim v{0} Update Available\n"
 "Open menu (press c) for details."
@@ -190,15 +202,15 @@
 msgid "Middle"
 msgstr "Sredina"
 
 msgid "New Group"
 msgstr "Nova grupa"
 
 msgid "No Transcode"
-msgstr "Nema pretvorbe formata"
+msgstr "Nema konverzije formata"
 
 msgid "None"
 msgstr "Ništa"
 
 msgid "None (Disabled)"
 msgstr "Ništa (onemogućeno)"
 
@@ -229,18 +241,18 @@
 msgid "Ready to cast"
 msgstr "Spreman za prijenos"
 
 msgid "Red"
 msgstr "Crvena"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
-msgstr "Kvaliteta pretvorbe formta udaljenog zapisa: {0:0.f} Mbps"
+msgstr "Kvaliteta pretvorbe formata udaljenog zapisa: {0:0.f} Mbps"
 
 msgid "Remove Server"
-msgstr "Ukloni poslužitelja"
+msgstr "Ukloni server"
 
 msgid "Retry"
 msgstr "Pokušaj ponovno"
 
 msgid "SVP Settings"
 msgstr "SVP postavke"
 
@@ -252,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "Snimka zaslona"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sezona {0} - Epizoda {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Traži za preskakanje uvoda (intro)"
+
 msgid "Select Audio Track"
 msgstr "Odaberi zapis zvuka"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Odaberi audio/titlove za cijelu sezonu"
 
 msgid "Select Default Transcode Profile"
@@ -291,42 +306,45 @@
 "Odaberite svoje medijske datoteke unutar Jellyfin sučelja i reproducirajte "
 "ih ovdje"
 
 msgid "Selecting Tracks..."
 msgstr "Odabir pjesama..."
 
 msgid "Server Configuration"
-msgstr "Konfiguracija poslužitelja"
+msgstr "Konfiguracija servera"
 
 msgid "Server URL: "
 msgstr "Poveznica poslužitelja: "
 
 msgid "Server:"
-msgstr "Poslužitelj:"
+msgstr "Server:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "Postavi zvučni zapis: {0} uspjeh, {1} samo zvuk, {2} greška"
 
 msgid "Set Subbed: {0} ok, {1} fail"
 msgstr "Postavi titlove: {0} uspjeh, {1} greška"
 
 msgid "Setting Current..."
 msgstr "Postavljanje trenutnog..."
 
 msgid "Show Console"
 msgstr "Prikaži konzolu"
 
 msgid "SkipToSync (x{0})"
-msgstr "SkipToSync (x{0})"
+msgstr "Preskok do sinkroniziranja (x{0})"
+
+msgid "Skipped Intro"
+msgstr "Preskočena najava (intro)"
 
 msgid "Small"
-msgstr "Mali"
+msgstr "Malo"
 
 msgid "SpeedToSync (x{0})"
-msgstr "SpeedToSync (x{0})"
+msgstr "Brzina do sinkroniziranja (x{0})"
 
 msgid "Subtitle Color: {0}"
 msgstr "Boja titlova: {0}"
 
 msgid "Subtitle Position: {0}"
 msgstr "Pozicija titlova: {0}"
 
@@ -336,15 +354,15 @@
 msgid "Successfully added server."
 msgstr "Server je uspješno dodan."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sinkronizacija onemogućena (previše pokušaja)"
 
 msgid "SyncPlay"
-msgstr "Sinkronizirana reprodukcija"
+msgstr "Sinkronizirana reprodukcija (SyncPlay)"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay onemogućen."
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay omogućen."
 
@@ -356,22 +374,25 @@
 
 msgid "Tiny"
 msgstr "Sitno"
 
 msgid "Top"
 msgstr "Gornji rub"
 
+msgid "Transcode HDR"
+msgstr "Transkodiranje u HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkodiranje Hi10p u 8bit"
 
 msgid "Unkn"
 msgstr "Nepoznato"
 
 msgid "Use Web Seek Pref"
-msgstr "Koristite Web Seek Pref"
+msgstr "Koristite Web Seek preferencije"
 
 msgid "Username:"
 msgstr "Korisničko ime:"
 
 msgid "Username: "
 msgstr "Korisničko ime: "
 
@@ -386,23 +407,36 @@
 
 msgid "Video Profile Subtype: {0}"
 msgstr "Podvrsta video profila: {0}"
 
 msgid "White"
 msgstr "Bijela"
 
+msgid "Write Logs to File"
+msgstr "Zapisuj logove u datoteku"
+
 msgid "Yellow"
 msgstr "Žuta"
 
+msgid ""
+"Your remote video is transcoding!\n"
+"Press c to adjust bandwidth settings if this is not needed."
+msgstr ""
+"Vaš se video transkodira!\n"
+"Pritisni \"c\" za prilagodbu postavki propusnosti veze."
+
 msgid "{0} has joined."
 msgstr "{0} se pridružio."
 
 msgid "{0} has left."
 msgstr "{0} je otišao."
 
+msgid "{0} is buffering."
+msgstr "{0} učitava."
+
 msgid "{0}'s Group"
 msgstr "Grupa korisnika {0}"
 
 msgid "{0}: Fail"
 msgstr "{0}: Greška"
 
 msgid "{0}: No Subtitles"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -380,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Átkódolás Hi10p-ről 8bit-re"
 
 msgid "Unkn"
 msgstr "Ismeretlen"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "JellyScrub indexképek használata"
-
 msgid "Use Web Seek Pref"
 msgstr "Használja a Web Seek Pref alkalmazást"
 
 msgid "Username:"
 msgstr "Felhasználónév:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-08-15 13:40+0000\n"
-"Last-Translator: Arief Hidayat <kekesed97@gmail.com>\n"
+"PO-Revision-Date: 2023-10-02 14:09+0000\n"
+"Last-Translator: MAhoyo <welya_skullboy@yahoo.co.id>\n"
 "Language-Team: Indonesian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/id/>\n"
 "Language: id\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transkode)"
 
 msgid " Forced"
 msgstr " Dipaksakan"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "Tambahkan server lain?"
 
 msgid "Adding server failed."
 msgstr "Penambahan server gagal."
 
+msgid "Always Skip Intros"
+msgstr "Selalu lewatkan pembuka"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (Untuk HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (Untuk HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Rekap Aplikasi"
 
 msgid "Application Menu"
 msgstr "Menu Aplikasi"
 
+msgid "Ask to Skip Intros"
+msgstr "Tanya untuk lewatkan pembuka"
+
 msgid "Auto Fullscreen"
 msgstr "Layar Penuh Otomatis"
 
 msgid "Auto Play"
 msgstr "Putar Otomatis"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -122,22 +128,25 @@
 msgid "Disable Direct Play"
 msgstr "Matikan Pemutaran Langsung"
 
 msgid "Disabled"
 msgstr "Dimatikan"
 
 msgid "Discord Rich Presence"
-msgstr "Kehadiran Kaya Discord"
+msgstr "Discord Rich Presence"
 
 msgid "Display Mirroring"
 msgstr "Tampilan mirroring"
 
 msgid "Enable SVP"
 msgstr "Aktifkan SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Aktifkan tampilan gambar mini"
+
 msgid "English Audio"
 msgstr "Audio Inggris"
 
 msgid "Fail"
 msgstr "Gagal"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Tangkapan Layar"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Musim {0} - Episode {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Loncat untuk lewatkan pembuka"
+
 msgid "Select Audio Track"
 msgstr "Pilih Trek Audio"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Pilih Audio/Subtitle untuk Seri"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Tampilkan Console"
 
 msgid "SkipToSync (x{0})"
 msgstr "Lewati Sinkronisasi (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Pembuka terlewati"
+
 msgid "Small"
 msgstr "Kecil"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Kecepatan Sinkronisasi (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Sangat Kecil"
 
 msgid "Top"
 msgstr "Atas"
 
+msgid "Transcode HDR"
+msgstr "Transkode HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkode Hi10p ke 8bit"
 
 msgid "Unkn"
 msgstr "Tidak Diketahui"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-27 20:43+0000\n"
-"Last-Translator: CarlBishop <peppino@galad.it>\n"
+"PO-Revision-Date: 2024-03-22 05:48+0000\n"
+"Last-Translator: VitoFe <vito-7@hotmail.it>\n"
 "Language-Team: Italian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transcodifica)"
 
 msgid " Forced"
 msgstr " Forzato"
@@ -128,15 +128,15 @@
 msgid "Disable Direct Play"
 msgstr "Disabilita Streaming Diretto"
 
 msgid "Disabled"
 msgstr "Disattivo"
 
 msgid "Discord Rich Presence"
-msgstr "Discord Rich Presence"
+msgstr "Stato Dettagliato Discord"
 
 msgid "Display Mirroring"
 msgstr "Mirroring schermo"
 
 msgid "Enable SVP"
 msgstr "Attiva SVP"
 
@@ -380,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcodifica Hi10p a 8bit"
 
 msgid "Unkn"
 msgstr "Sconosciuto"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Usa le miniature JellyScrub"
-
 msgid "Use Web Seek Pref"
 msgstr "Utilizza preferenza ricerca web"
 
 msgid "Username:"
 msgstr "Nome utente:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-12-25 23:51+0000\n"
-"Last-Translator: DuaLee <cony.j.lee@gmail.com>\n"
+"PO-Revision-Date: 2023-10-11 15:25+0000\n"
+"Last-Translator: HiSkyZen <mchan030704@gmail.com>\n"
 "Language-Team: Korean <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -22,19 +22,22 @@
 msgid "Access to the SyncPlay library was denied."
 msgstr "SyncPlay 라이브러리에 거부되었습니다."
 
 msgid "Add Server"
 msgstr "서버 추가"
 
 msgid "Add another server?"
-msgstr "다른 서버를 추가 하시겠습니까?"
+msgstr "다른 서버를 추가하시겠습니까?"
 
 msgid "Adding server failed."
 msgstr "서버 추가 실패 했습니다."
 
+msgid "Always Skip Intros"
+msgstr "항상 인트로를 건너뛰기"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 충실함 (HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 해석 (HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "애플리케이션 로그"
 
 msgid "Application Menu"
 msgstr "어플 메뉴"
 
+msgid "Ask to Skip Intros"
+msgstr "인트로 건너뛰기전에 항상 물어보기"
+
 msgid "Auto Fullscreen"
 msgstr "자동 전체 화면"
 
 msgid "Auto Play"
 msgstr "자동 재생"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "디스플레이 미러링"
 
 msgid "Enable SVP"
 msgstr "SVP 켠다"
 
+msgid "Enable thumbnail previews"
+msgstr "섬네일 미리보기 활성화하기"
+
 msgid "English Audio"
 msgstr "영어 오디오"
 
 msgid "Fail"
 msgstr "실패"
 
 msgid "Generic (FSRCNNX)"
@@ -149,15 +158,15 @@
 msgid "Gray"
 msgstr "회색"
 
 msgid "Green"
 msgstr "녹색"
 
 msgid "Huge"
-msgstr "거대한"
+msgstr "매우 크게"
 
 msgid "Japanese Audio w/ English Subtitles"
 msgstr "일본어 오디오에 영어 자막"
 
 msgid "Large"
 msgstr "크게"
 
@@ -201,27 +210,27 @@
 msgid "None"
 msgstr "없음"
 
 msgid "None (Disabled)"
 msgstr "없음 (꺼저있다)"
 
 msgid "Normal"
-msgstr "일반"
+msgstr "보통"
 
 msgid "Ok"
 msgstr "오케이"
 
 msgid "Open Config Folder"
 msgstr "설정 폴더 열기"
 
 msgid "Password:"
 msgstr "암호:"
 
 msgid "Password: "
-msgstr "암호 "
+msgstr "암호: "
 
 msgid "Player Preferences"
 msgstr "플레이어 기본 설정"
 
 msgid "Quit"
 msgstr "중지"
 
@@ -243,25 +252,28 @@
 msgid "Retry"
 msgstr "다시 하다"
 
 msgid "SVP Settings"
 msgstr "SVP 설정"
 
 msgid "SVP is Disabled"
-msgstr "SVP 꺼저있다"
+msgstr "SVP 꺼져있다"
 
 msgid "SVP is Not Active"
 msgstr "SVP가 꺼저있다"
 
 msgid "Screenshot"
 msgstr "스크린샷"
 
 msgid "Season {0} - Episode {1}"
 msgstr "시즌 {0} - {1}화"
 
+msgid "Seek to Skip Intro"
+msgstr "인트로 건너뛰기"
+
 msgid "Select Audio Track"
 msgstr "오디오 트랙 선택"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "시리즈 오디오/자막 선택"
 
 msgid "Select Default Transcode Profile"
@@ -288,21 +300,21 @@
 msgid "Select Transcode Quality"
 msgstr "코덱변경 품질 선택"
 
 msgid "Select your media in Jellyfin and play it here"
 msgstr "젤리핀에서 미디어를 선택하고 재생"
 
 msgid "Selecting Tracks..."
-msgstr "트랙 선택 중..."
+msgstr "트랙 선택..."
 
 msgid "Server Configuration"
 msgstr "서버 설정"
 
 msgid "Server URL: "
-msgstr "서버 URL "
+msgstr "서버 주소: "
 
 msgid "Server:"
 msgstr "서버:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "더빙 설정: {0} 확인, {1} 단지 오디오, {2} 실패"
 
@@ -314,31 +326,34 @@
 
 msgid "Show Console"
 msgstr "콘솔 보이기"
 
 msgid "SkipToSync (x{0})"
 msgstr "Sync 건너뛰기 (x{0})"
 
+msgid "Skipped Intro"
+msgstr "인트로 건너뜀"
+
 msgid "Small"
-msgstr "작은"
+msgstr "작게"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Sync 속도 (x{0})"
 
 msgid "Subtitle Color: {0}"
 msgstr "자막 색깔: {0}"
 
 msgid "Subtitle Position: {0}"
 msgstr "자막 위치: {0}"
 
 msgid "Subtitle Size: {0}"
 msgstr "자막 크기: {0}"
 
 msgid "Successfully added server."
-msgstr "서버를 성공적으로 추가했습니다."
+msgstr "서버가 성공적으로 추가되었습니다."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sync 꺼짐 (너무 많은 시도)"
 
 msgid "SyncPlay"
 msgstr "Sync 플레이"
 
@@ -351,19 +366,22 @@
 msgid "SyncPlay group access was denied."
 msgstr "SyncPlay 모임 액세스가 거부되었습니다."
 
 msgid "The specified SyncPlay group does not exist."
 msgstr "그 SyncPlay 모임이 존재하지 않습니다."
 
 msgid "Tiny"
-msgstr "매우 작은"
+msgstr "매우 작게"
 
 msgid "Top"
 msgstr "위"
 
+msgid "Transcode HDR"
+msgstr "HDR 트랜스코드"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Hi10p를 8bit 코덱변환"
 
 msgid "Unkn"
 msgstr "알 수 없는"
 
 msgid "Use Web Seek Pref"
@@ -396,16 +414,16 @@
 msgid "Yellow"
 msgstr "황색"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
-"외부 비디오 코덱변화 중입니다!\n"
-"필요하지 않은 경우 c를 눌러 인터넷 설정을 조정하시오."
+"외부 비디오 코덱 변환 중입니다!\n"
+"필요하지 않은 경우 c를 눌러 인터넷 설정을 조정하세요."
 
 msgid "{0} has joined."
 msgstr "{0}님이 들어왔습니다."
 
 msgid "{0} has left."
 msgstr "{0}님이 나갔습니다."
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-22 15:39+0000\n"
-"Last-Translator: Cyteon <pkristian1@outlook.com>\n"
+"PO-Revision-Date: 2024-01-20 21:30+0000\n"
+"Last-Translator: hulkhaugen <borre.haugen@gmail.com>\n"
 "Language-Team: Norwegian Bokmål <https://translate.jellyfin.org/projects/"
 "jellyfin/jellyfin-desktop/nb_NO/>\n"
 "Language: nb_NO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -19,21 +19,24 @@
 msgid " Forced"
 msgstr " Tvungen"
 
 msgid "Access to the SyncPlay library was denied."
 msgstr "Tilgang til SyncPlay-biblioteket ble avvist."
 
 msgid "Add Server"
-msgstr "Legg til tjener"
+msgstr "Legg til server"
 
 msgid "Add another server?"
-msgstr "Vil du legge til en tjener til?"
+msgstr "Legge til enda en server?"
 
 msgid "Adding server failed."
-msgstr "Kunne ikke legge til tjeneren."
+msgstr "Kunne ikke legge til serveren."
+
+msgid "Always Skip Intros"
+msgstr "Hopp alltid over introduksjoner"
 
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (for HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (for HD)"
 
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Programlogg"
 
 msgid "Application Menu"
 msgstr "Applikasjonsmeny"
 
+msgid "Ask to Skip Intros"
+msgstr "Spør om å hoppe over introduksjoner"
+
 msgid "Auto Fullscreen"
 msgstr "Automatisk fullskjerm"
 
 msgid "Auto Play"
 msgstr "Spill automatisk"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -94,28 +100,28 @@
 msgid "Close"
 msgstr "Lukk"
 
 msgid "Close Menu"
 msgstr "Lukk meny"
 
 msgid "Configure Servers"
-msgstr "Konfigurer tjenere"
+msgstr "Konfigurer servere"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
-"Kunne ikke legge til tjener.\n"
+"Kunne ikke legge til server.\n"
 "Vennligst sjekk tilkoblingsinformasjonen din."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Opprettelse av SyncPlay-grupper er ikke tillatt."
 
 msgid "Cyan"
-msgstr "Cyan"
+msgstr "Turkis"
 
 msgid "Direct Paths"
 msgstr "Direkte baner"
 
 msgid "Disable"
 msgstr "Deaktiver"
 
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "Skjermkloning"
 
 msgid "Enable SVP"
 msgstr "Aktiver SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Aktiver forhåndsvisning av miniatyrbilder"
+
 msgid "English Audio"
 msgstr "Engelsk lyd"
 
 msgid "Fail"
 msgstr "Feil"
 
 msgid "Generic (FSRCNNX)"
@@ -152,15 +161,15 @@
 msgid "Green"
 msgstr "Grønn"
 
 msgid "Huge"
 msgstr "Gigantisk"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "Japansk lyd med engelsk teksting"
+msgstr "Japansk lyd m/engelsk teksting"
 
 msgid "Large"
 msgstr "Stor"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} versjonsinfo/nedlastning"
 
@@ -234,15 +243,15 @@
 msgid "Red"
 msgstr "Rød"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
 msgstr "Fjernomkodingskvalitet: {0:0.1f} Mbps"
 
 msgid "Remove Server"
-msgstr "Fjern tjener"
+msgstr "Fjern server"
 
 msgid "Retry"
 msgstr "Prøv igjen"
 
 msgid "SVP Settings"
 msgstr "SVP-innstillinger"
 
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Skjermdump"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sesong {0} - Episode {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Søk for å hoppe over intro"
+
 msgid "Select Audio Track"
 msgstr "Velg lydspor"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Velg lyd/teksting for serie"
 
 msgid "Select Default Transcode Profile"
@@ -291,21 +303,21 @@
 msgid "Select your media in Jellyfin and play it here"
 msgstr "Velg mediet i Jellyfin og spill det av her"
 
 msgid "Selecting Tracks..."
 msgstr "Velger spor..."
 
 msgid "Server Configuration"
-msgstr "Tjenerkonfigurasjon"
+msgstr "Serverkonfigurasjon"
 
 msgid "Server URL: "
-msgstr "Tjenernettadresse: "
+msgstr "Serveradresse: "
 
 msgid "Server:"
-msgstr "Tjener:"
+msgstr "Server:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "Sett dubbing: {0} ok, {1} kun lyd, {2} feil"
 
 msgid "Set Subbed: {0} ok, {1} fail"
 msgstr "Sett undertekst: {0} ok, {1} feil"
 
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Vis konsoll"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Hoppet over introen"
+
 msgid "Small"
 msgstr "Liten"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -330,15 +345,15 @@
 msgid "Subtitle Position: {0}"
 msgstr "Tekstplassering: {0}"
 
 msgid "Subtitle Size: {0}"
 msgstr "Tekststørrelse: {0}"
 
 msgid "Successfully added server."
-msgstr "Tjeneren ble lagt til."
+msgstr "Serveren ble lagt til."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sync deaktivert (for mange forsøk)"
 
 msgid "SyncPlay"
 msgstr "SynkAvspilling"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-03-01 21:39+0000\n"
+"PO-Revision-Date: 2023-10-06 07:31+0000\n"
 "Last-Translator: Bas <weblate@hanka.mp>\n"
 "Language-Team: Dutch <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/nl/>\n"
 "Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -28,15 +28,15 @@
 msgid "Add another server?"
 msgstr "Nog een server toevoegen?"
 
 msgid "Adding server failed."
 msgstr "Server toevoegen mislukt."
 
 msgid "Always Skip Intros"
-msgstr "Altijd intro's overslaan"
+msgstr "Intro's altijd overslaan"
 
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (voor HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (voor HD)"
 
@@ -128,22 +128,25 @@
 msgid "Disable Direct Play"
 msgstr "Direct Play deactiveren"
 
 msgid "Disabled"
 msgstr "Uitgeschakeld"
 
 msgid "Discord Rich Presence"
-msgstr "Discord Rich Presence"
+msgstr "Discord-Rich Presence"
 
 msgid "Display Mirroring"
 msgstr "Beeld spiegelen"
 
 msgid "Enable SVP"
 msgstr "SVP activeren"
 
+msgid "Enable thumbnail previews"
+msgstr "Miniatuurvoorbeelden inschakelen"
+
 msgid "English Audio"
 msgstr "Engelse Audio"
 
 msgid "Fail"
 msgstr "Mislukt"
 
 msgid "Generic (FSRCNNX)"
@@ -260,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Schermafbeelding"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Seizoen {0} - Aflevering {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Terug- of vooruitspoelen om intro over te slaan"
+
 msgid "Select Audio Track"
 msgstr "Audiospoor selecteren"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Selecteer Audio/Ondertiteling voor Serie"
 
 msgid "Select Default Transcode Profile"
@@ -374,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcode Hi10p naar 8bit"
 
 msgid "Unkn"
 msgstr "Onbekend"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "JellyScrub-thumbnails gebruiken"
-
 msgid "Use Web Seek Pref"
 msgstr "Web zoek voorkeur gebruiken"
 
 msgid "Username:"
 msgstr "Gebruikersnaam:"
 
 msgid "Username: "
@@ -412,15 +415,15 @@
 msgstr "Geel"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
 "Uw remote video wordt omgezet!\n"
-"Druk C om de bandwijdte-instellingen aan te passen als dit niet gewenst is."
+"Druk C om de bandbreedte-instellingen aan te passen als dit niet gewenst is."
 
 msgid "{0} has joined."
 msgstr "{0} heeft toegetreden."
 
 msgid "{0} has left."
 msgstr "{0} heeft verlaten."
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,34 +1,34 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-03-05 10:39+0000\n"
-"Last-Translator: kaypiff <kpiff@proton.me>\n"
+"PO-Revision-Date: 2024-03-25 13:38+0000\n"
+"Last-Translator: Kityn <kitynska@gmail.com>\n"
 "Language-Team: Polish <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transkoduj)"
 
 msgid " Forced"
 msgstr " Wymuszone"
 
 msgid "Access to the SyncPlay library was denied."
 msgstr "Odmówiono dostępu do biblioteki SyncPlay."
 
 msgid "Add Server"
-msgstr "Dodaj Serwer"
+msgstr "Dodaj serwer"
 
 msgid "Add another server?"
 msgstr "Dodać kolejny serwer?"
 
 msgid "Adding server failed."
 msgstr "Dodawanie serwera nie powiodło się."
 
@@ -50,66 +50,66 @@
 msgid "Anime4K x4 Perceptual (For SD)"
 msgstr "Anime4K x4 percepcyjne (dla SD)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
 msgstr "Anime4K x4 percepcyjne + deblur (dla SD)"
 
 msgid "Application Log"
-msgstr "Dziennik Aplikacji"
+msgstr "Dziennik aplikacji"
 
 msgid "Application Menu"
 msgstr "Menu aplikacji"
 
 msgid "Ask to Skip Intros"
 msgstr "Pytaj o pominięcie wstępów"
 
 msgid "Auto Fullscreen"
-msgstr "Automatyczny Pełny Ekran"
+msgstr "Automatyczny pełny ekran"
 
 msgid "Auto Play"
-msgstr "Automatyczne Odtwarzanie"
+msgstr "Automatyczne odtwarzanie"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
-msgstr "Automatyczne Ustawianie Dźwięku/Napisów (Cała Seria)"
+msgstr "Automatyczne ustawianie dźwięku/napisów (cały serial)"
 
 msgid "Automatic"
 msgstr "Automatycznie"
 
 msgid "Black"
 msgstr "Czarny"
 
 msgid "Blue"
 msgstr "Niebieski"
 
 msgid "Bottom"
-msgstr "Na Dole"
+msgstr "Na dole"
 
 msgid "Change Audio"
-msgstr "Zmiana Dźwięku"
+msgstr "Zmiana dźwięku"
 
 msgid "Change Subtitles"
-msgstr "Zmień Napisy"
+msgstr "Zmień napisy"
 
 msgid "Change Video Playback Profile"
 msgstr "Zmiana profilu odtwarzania wideo"
 
 msgid "Change Video Quality"
-msgstr "Zmień Jakość Wideo"
+msgstr "Zmień jakość wideo"
 
 msgid "Check for Updates"
-msgstr "Sprawdź Aktualizacje"
+msgstr "Sprawdź aktualizacje"
 
 msgid "Close"
 msgstr "Zamknij"
 
 msgid "Close Menu"
-msgstr "Zamknij Menu"
+msgstr "Zamknij menu"
 
 msgid "Configure Servers"
-msgstr "Konfiguruj Serwery"
+msgstr "Konfiguruj serwery"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
 "Nie można dodać serwera.\n"
 "Proszę sprawdzić informacje o połączeniu."
@@ -117,60 +117,60 @@
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Tworzenie grup SyncPlay nie jest dozwolone."
 
 msgid "Cyan"
 msgstr "Cyjan"
 
 msgid "Direct Paths"
-msgstr "Ścieżki Bezpośrednie"
+msgstr "Ścieżki bezpośrednie"
 
 msgid "Disable"
 msgstr "Wyłącz"
 
 msgid "Disable Direct Play"
-msgstr "Wyłącz Odtwarzanie Bezpośrednie"
+msgstr "Wyłącz odtwarzanie bezpośrednie"
 
 msgid "Disabled"
 msgstr "Wyłączone"
 
 msgid "Discord Rich Presence"
-msgstr "Bogata obecność na Discordzie"
+msgstr "Discord Rich Presence"
 
 msgid "Display Mirroring"
-msgstr "Wyświetlanie Lustrzane"
+msgstr "Wyświetlanie lustrzane"
 
 msgid "Enable SVP"
 msgstr "Włącz SVP"
 
 msgid "Enable thumbnail previews"
 msgstr "Włącz podgląd miniatur"
 
 msgid "English Audio"
-msgstr "Dźwięk Angielski"
+msgstr "Dźwięk angielski"
 
 msgid "Fail"
 msgstr "Błąd"
 
 msgid "Generic (FSRCNNX)"
 msgstr "Ogólny (FSRCNNX)"
 
 msgid "Generic High (FSRCNNX x16)"
-msgstr "Ogólny Wysoki (FSRCNNX x16)"
+msgstr "Ogólny wysoki (FSRCNNX x16)"
 
 msgid "Gray"
 msgstr "Szary"
 
 msgid "Green"
 msgstr "Zielony"
 
 msgid "Huge"
 msgstr "Wielki"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "Dźwięk Japoński w/ Angielskie Napisy"
+msgstr "Dźwięk japoński z angielskimi napisami"
 
 msgid "Large"
 msgstr "Duży"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} Informacje o wydaniu/Pobieranie"
 
@@ -181,183 +181,183 @@
 "MPV Shim v{0} Aktualizacja Dostępna\n"
 "Otwórz menu (naciśnij c), aby uzyskać szczegółowe informacje."
 
 msgid "Magenta"
 msgstr "Magenta"
 
 msgid "Main Menu"
-msgstr "Menu Główne"
+msgstr "Menu główne"
 
 msgid "Manual by Track Index (Less Reliable)"
 msgstr "Ręczny według indeksu ścieżek (mniej wiarygodny)"
 
 msgid "Manual: {0} ok, {1} fail"
 msgstr "Ręczne: {0} ok, {1} nieudane"
 
 msgid "Maximum"
 msgstr "Maksimum"
 
 msgid "Media Key Seek"
-msgstr "Klawisz Do Szukania Multimediów"
+msgstr "Klawisz przewijania multimediów"
 
 msgid "Middle"
-msgstr "Po Środku"
+msgstr "Po środku"
 
 msgid "New Group"
-msgstr "Nowa Grupa"
+msgstr "Nowa grupa"
 
 msgid "No Transcode"
-msgstr "Nie Transkoduj"
+msgstr "Nie transkoduj"
 
 msgid "None"
-msgstr "Żadne"
+msgstr "Brak"
 
 msgid "None (Disabled)"
-msgstr "Brak (Wyłączone)"
+msgstr "Brak (wyłączone)"
 
 msgid "Normal"
 msgstr "Normalny"
 
 msgid "Ok"
 msgstr "Ok"
 
 msgid "Open Config Folder"
-msgstr "Otwórz Folder Konfiguracji"
+msgstr "Otwórz folder konfiguracji"
 
 msgid "Password:"
 msgstr "Hasło:"
 
 msgid "Password: "
 msgstr "Hasło: "
 
 msgid "Player Preferences"
-msgstr "Preferencje Odtwarzacza"
+msgstr "Preferencje odtwarzacza"
 
 msgid "Quit"
 msgstr "Wyjdź"
 
 msgid "Quit and Mark Unwatched"
-msgstr "Zakończ i zaznacz jako Nie oglądane"
+msgstr "Zakończ i zaznacz jako nieobejrzane"
 
 msgid "Ready to cast"
 msgstr "Gotowy do castowania"
 
 msgid "Red"
 msgstr "Czerwony"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
-msgstr "Jakość Zdalnego Transkodowania: {0:0.1f}. Mbps"
+msgstr "Jakość zdalnego transkodowania: {0:0.1f} Mbps"
 
 msgid "Remove Server"
-msgstr "Usuń Serwer"
+msgstr "Usuń serwer"
 
 msgid "Retry"
-msgstr "Ponów Próbę"
+msgstr "Ponów próbę"
 
 msgid "SVP Settings"
 msgstr "Ustawienia SVP"
 
 msgid "SVP is Disabled"
-msgstr "SVP jest Wyłączone"
+msgstr "SVP jest wyłączone"
 
 msgid "SVP is Not Active"
-msgstr "SVP jest Nie Aktywne"
+msgstr "SVP jest nieaktywne"
 
 msgid "Screenshot"
 msgstr "Zrzut ekranu"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sezon {0} - Odcinek {1}"
 
 msgid "Seek to Skip Intro"
 msgstr "Przewiń, aby pominąć wstęp"
 
 msgid "Select Audio Track"
-msgstr "Wybierz Ścieżkę Dźwiękową"
+msgstr "Wybierz ścieżkę dźwiękową"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "Wybierz Dźwięk/Napisy dla Serii"
+msgstr "Wybierz dźwięk/napisy dla serialu"
 
 msgid "Select Default Transcode Profile"
-msgstr "Wybierz Domyślny Profil Transkodowania"
+msgstr "Wybierz domyślny profil transkodowania"
 
 msgid "Select SVP Profile"
-msgstr "Wybierz Profil SVP"
+msgstr "Wybierz profil SVP"
 
 msgid "Select Shader Profile"
-msgstr "Wybierz Profil Shadera"
+msgstr "Wybierz profil shadera"
 
 msgid "Select Subtitle Color"
-msgstr "Wybierz Kolor Napisów"
+msgstr "Wybierz kolor napisów"
 
 msgid "Select Subtitle Position"
-msgstr "Wybierz Pozycję Napisów"
+msgstr "Wybierz pozycję napisów"
 
 msgid "Select Subtitle Size"
-msgstr "Wybierz Wielkość Napisów"
+msgstr "Wybierz wielkość napisów"
 
 msgid "Select Subtitle Track"
-msgstr "Wybierz Ścieżkę Napisów"
+msgstr "Wybierz ścieżkę napisów"
 
 msgid "Select Transcode Quality"
-msgstr "Wybierz Jakość Transkodowania"
+msgstr "Wybierz jakość transkodowania"
 
 msgid "Select your media in Jellyfin and play it here"
 msgstr "Wybierz swoje multimedia w Jellyfin i odtwarzaj je tutaj"
 
 msgid "Selecting Tracks..."
 msgstr "Wybieranie ścieżki..."
 
 msgid "Server Configuration"
-msgstr "Konfiguracja Serwera"
+msgstr "Konfiguracja serwera"
 
 msgid "Server URL: "
 msgstr "Serwer URL: "
 
 msgid "Server:"
 msgstr "Serwer:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
-msgstr "Ustaw Dubbing: {0} ok, {1} tylko dźwięk,{2} nieudane"
+msgstr "Ustaw dubbing: {0} ok, {1} tylko dźwięk, {2} nieudane"
 
 msgid "Set Subbed: {0} ok, {1} fail"
-msgstr "Napisy: {0} ok, {1} nieudane"
+msgstr "Ustaw napisy: {0} ok, {1} nieudane"
 
 msgid "Setting Current..."
-msgstr "Ustawianie Bieżącego..."
+msgstr "Ustawianie bieżącego..."
 
 msgid "Show Console"
-msgstr "Pokaż Konsolę"
+msgstr "Pokaż konsolę"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
 msgid "Skipped Intro"
 msgstr "Pominięte wprowadzenie"
 
 msgid "Small"
 msgstr "Mały"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Szybkość synchronizacji (x{0})"
 
 msgid "Subtitle Color: {0}"
-msgstr "Kolor Napisów: {0}"
+msgstr "Kolor napisów: {0}"
 
 msgid "Subtitle Position: {0}"
-msgstr "Pozycja Napisów: {0}"
+msgstr "Pozycja napisów: {0}"
 
 msgid "Subtitle Size: {0}"
-msgstr "Rozmiar Napisów: {0}"
+msgstr "Rozmiar napisów: {0}"
 
 msgid "Successfully added server."
 msgstr "Serwer został pomyślnie dodany."
 
 msgid "Sync Disabled (Too Many Attempts)"
-msgstr "Synchronizacja Wyłączona (Zbyt Wiele Prób)"
+msgstr "Synchronizacja wyłączona (zbyt wiele prób)"
 
 msgid "SyncPlay"
 msgstr "SyncPlay"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay wyłączone."
 
@@ -370,42 +370,39 @@
 msgid "The specified SyncPlay group does not exist."
 msgstr "Podana grupa SyncPlay nie istnieje."
 
 msgid "Tiny"
 msgstr "Malutki"
 
 msgid "Top"
-msgstr "Na Górze"
+msgstr "Na górze"
 
 msgid "Transcode HDR"
 msgstr "Transkoduj do HDR"
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transkoduj Hi10p do 8bit"
 
 msgid "Unkn"
 msgstr "Niezn"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Użyj miniatur JellyScrub"
-
 msgid "Use Web Seek Pref"
 msgstr "Użyj funkcji Web Seek Pref"
 
 msgid "Username:"
 msgstr "Nazwa użytkownika:"
 
 msgid "Username: "
 msgstr "Nazwa użytkownika: "
 
 msgid "Video Playback Profiles"
-msgstr "Profile Odtwarzania Wideo"
+msgstr "Profile odtwarzania wideo"
 
 msgid "Video Preferences"
-msgstr "Preferencje Wideo"
+msgstr "Preferencje wideo"
 
 msgid "Video Profile Subtype"
 msgstr "Podtyp profilu wideo"
 
 msgid "Video Profile Subtype: {0}"
 msgstr "Podtyp profilu wideo: {0}"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,40 +1,43 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-08-28 04:11+0000\n"
-"Last-Translator: Giuliano Chimatti Berna <giucberna@gmail.com>\n"
+"PO-Revision-Date: 2023-11-18 10:13+0000\n"
+"Last-Translator: Lucas Fogolin <lucasfogolin@gmail.com>\n"
 "Language-Team: Portuguese (Brazil) <https://translate.jellyfin.org/projects/"
 "jellyfin/jellyfin-desktop/pt_BR/>\n"
 "Language: pt_BR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Transcodificar)"
 
 msgid " Forced"
 msgstr " Forçado"
 
 msgid "Access to the SyncPlay library was denied."
-msgstr "O acesso a biblioteca SyncPlay foi negado."
+msgstr "O acesso à biblioteca SyncPlay foi negado."
 
 msgid "Add Server"
 msgstr "Adicionar servidor"
 
 msgid "Add another server?"
 msgstr "Adicionar outro servidor?"
 
 msgid "Adding server failed."
 msgstr "Erro ao adicionar servidor."
 
+msgid "Always Skip Intros"
+msgstr "Sempre Pular Abertura"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Fiel (para HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (para HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Logs do programa"
 
 msgid "Application Menu"
 msgstr "Menu do programa"
 
+msgid "Ask to Skip Intros"
+msgstr "Pergunte Sobre Pular Abertura"
+
 msgid "Auto Fullscreen"
 msgstr "Modo tela cheia automático"
 
 msgid "Auto Play"
 msgstr "Auto-reprodução"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -122,22 +128,25 @@
 msgid "Disable Direct Play"
 msgstr "Desabilitar Direct Play (reprodução direta)"
 
 msgid "Disabled"
 msgstr "Desabilitado"
 
 msgid "Discord Rich Presence"
-msgstr "Discordar rica presença"
+msgstr "Status de Atividade no Discord"
 
 msgid "Display Mirroring"
 msgstr "Espelhamento de tela"
 
 msgid "Enable SVP"
 msgstr "Habilitar SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Habilitar miniaturas de imagens"
+
 msgid "English Audio"
 msgstr "Áudio em inglês"
 
 msgid "Fail"
 msgstr "Falhou"
 
 msgid "Generic (FSRCNNX)"
@@ -254,19 +263,22 @@
 
 msgid "Screenshot"
 msgstr "Captura de tela"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Temporada {0} - Episódio {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Tentar pular introdução"
+
 msgid "Select Audio Track"
 msgstr "Selecionar faixa de áudio"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "Selecione Áudio/Legenda para Series"
+msgstr "Selecione Áudio/Legenda para Séries"
 
 msgid "Select Default Transcode Profile"
 msgstr "Selecione o perfil de transcodificação padrão"
 
 msgid "Select SVP Profile"
 msgstr "Selecionar perfil SVP"
 
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Mostrar console"
 
 msgid "SkipToSync (x{0})"
 msgstr "PularParaSincronizar (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Introdução pulada"
+
 msgid "Small"
 msgstr "Pequeno"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Velocidade de sincronização (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Minúsculo"
 
 msgid "Top"
 msgstr "Topo"
 
+msgid "Transcode HDR"
+msgstr "Transcodificar HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcodificar Hi10p para 8bit"
 
 msgid "Unkn"
 msgstr "Desconhecido"
 
 msgid "Use Web Seek Pref"
@@ -387,15 +405,15 @@
 msgid "Video Profile Subtype: {0}"
 msgstr "Subtipo de perfil de vídeo: {0}"
 
 msgid "White"
 msgstr "Branco"
 
 msgid "Write Logs to File"
-msgstr "Escrever logs ao arquivo"
+msgstr "Escrever logs para arquivo"
 
 msgid "Yellow"
 msgstr "Amarelo"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,40 +1,43 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-01-09 16:51+0000\n"
-"Last-Translator: pedropereira98 <pedromlmpereira98@gmail.com>\n"
+"PO-Revision-Date: 2024-04-16 11:04+0000\n"
+"Last-Translator: Blackspirits <blackspirits@gmail.com>\n"
 "Language-Team: Portuguese (Portugal) <https://translate.jellyfin.org/"
 "projects/jellyfin/jellyfin-desktop/pt_PT/>\n"
 "Language: pt_PT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " ·(Transcodificar)"
 
 msgid " Forced"
 msgstr " ·Forçado"
 
 msgid "Access to the SyncPlay library was denied."
 msgstr "Acesso à biblioteca SyncPlay foi negado."
 
 msgid "Add Server"
-msgstr "Adicionar Servidor"
+msgstr "Adicionar servidor"
 
 msgid "Add another server?"
 msgstr "Adicionar outro servidor?"
 
 msgid "Adding server failed."
 msgstr "Não foi possível adicionar o servidor."
 
+msgid "Always Skip Intros"
+msgstr "Saltar sempre as introduções"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime 4K x2 Faithful (para HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (para HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -46,18 +49,21 @@
 msgid "Anime4K x4 Perceptual (For SD)"
 msgstr "Anime4K x4 Perceptual (Para SD)"
 
 msgid "Anime4K x4 Perceptual + Deblur (For SD)"
 msgstr "Anime4K x4 Perceptual + Nitidez (para SD)"
 
 msgid "Application Log"
-msgstr "Registo da Aplicação"
+msgstr "Registo da aplicação"
 
 msgid "Application Menu"
-msgstr "Menu da Aplicação"
+msgstr "Menu da aplicação"
+
+msgid "Ask to Skip Intros"
+msgstr "Perguntar para saltar as introduções"
 
 msgid "Auto Fullscreen"
 msgstr "Ecrã Completo Automático"
 
 msgid "Auto Play"
 msgstr "Reprodução Automática"
 
@@ -73,52 +79,52 @@
 msgid "Blue"
 msgstr "Azul"
 
 msgid "Bottom"
 msgstr "Fundo"
 
 msgid "Change Audio"
-msgstr "Mudar Àudio"
+msgstr "Mudar áudio"
 
 msgid "Change Subtitles"
-msgstr "Mudar Legendas"
+msgstr "Mudar legendas"
 
 msgid "Change Video Playback Profile"
 msgstr "Mudar Perfil da Reprodução do Vídeo"
 
 msgid "Change Video Quality"
-msgstr "Mudar Qualidade do Vídeo"
+msgstr "Mudar qualidade do vídeo"
 
 msgid "Check for Updates"
 msgstr "Procurar Atualizações"
 
 msgid "Close"
 msgstr "Fechar"
 
 msgid "Close Menu"
 msgstr "Fechar Menu"
 
 msgid "Configure Servers"
-msgstr "Configurar Servidores"
+msgstr "Configurar servidores"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
 "Não foi possível adicionar o servidor.\n"
-"Por favor verifique as detalhes da sua ligação."
+"Por favor, verifique as suas informações de ligação."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "A criação de novos grupos SyncPlay não é permitido."
 
 msgid "Cyan"
 msgstr "Ciano"
 
 msgid "Direct Paths"
-msgstr "Caminhos Diretos"
+msgstr "Caminhos diretos"
 
 msgid "Disable"
 msgstr "Desativar"
 
 msgid "Disable Direct Play"
 msgstr "Desabilitar a Reprodução Direta"
 
@@ -130,14 +136,17 @@
 
 msgid "Display Mirroring"
 msgstr "Duplicação de Ecrã"
 
 msgid "Enable SVP"
 msgstr "Ativar SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Activar previsão de miniatura"
+
 msgid "English Audio"
 msgstr "Àudio em Inglês"
 
 msgid "Fail"
 msgstr "Falhou"
 
 msgid "Generic (FSRCNNX)"
@@ -171,15 +180,15 @@
 "MPV Shim v{0} Atualização Disponível↵\n"
 "Abre o menu (pressione c) para detalhes."
 
 msgid "Magenta"
 msgstr "Magenta"
 
 msgid "Main Menu"
-msgstr "Menu Príncipal"
+msgstr "Menu principal"
 
 msgid "Manual by Track Index (Less Reliable)"
 msgstr "Manualmente por Ìndice de Faixas (Menos Confiável)"
 
 msgid "Manual: {0} ok, {1} fail"
 msgstr "Manual: {0} ok, {1} falhou"
 
@@ -204,64 +213,67 @@
 msgid "None (Disabled)"
 msgstr "Nenhum (Desativado)"
 
 msgid "Normal"
 msgstr "Normal"
 
 msgid "Ok"
-msgstr "OK"
+msgstr "Ok"
 
 msgid "Open Config Folder"
-msgstr "Abrir Pasta das Configurações"
+msgstr "Abrir pasta de configurações"
 
 msgid "Password:"
 msgstr "Palavra-passe:"
 
 msgid "Password: "
 msgstr "Palavra-passe: "
 
 msgid "Player Preferences"
 msgstr "Preferências de Reprodutor"
 
 msgid "Quit"
-msgstr "Sair"
+msgstr "Terminar sessão"
 
 msgid "Quit and Mark Unwatched"
 msgstr "Sair e Definir como Não Visto"
 
 msgid "Ready to cast"
 msgstr "Pronto para transmitir"
 
 msgid "Red"
 msgstr "Vermelho"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
 msgstr "Qualidade da Transcodificação Remota: {0:0.1f} Mbps"
 
 msgid "Remove Server"
-msgstr "Eliminar Servidor"
+msgstr "Eliminar servidor"
 
 msgid "Retry"
 msgstr "Tentar de novo"
 
 msgid "SVP Settings"
-msgstr "Opções de SVP"
+msgstr "Definições de SVP"
 
 msgid "SVP is Disabled"
 msgstr "SVP está desativado"
 
 msgid "SVP is Not Active"
 msgstr "SVP não está ativo"
 
 msgid "Screenshot"
-msgstr "Captura de Ecrã"
+msgstr "Captura de ecrã"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Temporada {0} - Episódio {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Tentar saltar introdução"
+
 msgid "Select Audio Track"
 msgstr "Selecionar Faixa de Àudio"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Selecionar Àudio/Legendas para Série"
 
 msgid "Select Default Transcode Profile"
@@ -270,58 +282,61 @@
 msgid "Select SVP Profile"
 msgstr "Selecionar Perfil SVP"
 
 msgid "Select Shader Profile"
 msgstr "Selecionar Perfil do Sombreador"
 
 msgid "Select Subtitle Color"
-msgstr "Selecionar a Cor das Legendas"
+msgstr "Selecionar Cor das Legendas"
 
 msgid "Select Subtitle Position"
-msgstr "Selecionar a Posição das Legendas"
+msgstr "Selecionar Posição das Legendas"
 
 msgid "Select Subtitle Size"
 msgstr "Selecionar Tamanho das Legendas"
 
 msgid "Select Subtitle Track"
 msgstr "Selecionar Faixa de Legendas"
 
 msgid "Select Transcode Quality"
 msgstr "Selecionar Qualidade de Transcodificação"
 
 msgid "Select your media in Jellyfin and play it here"
 msgstr "Selecione o seu conteúdo no Jellyfin e reproduza-o aqui"
 
 msgid "Selecting Tracks..."
-msgstr "A Selecionar Faixas..."
+msgstr "A selecionar faixas..."
 
 msgid "Server Configuration"
-msgstr "Configuração do Servidor"
+msgstr "Configurações do servidor"
 
 msgid "Server URL: "
 msgstr "URL do Servidor: "
 
 msgid "Server:"
 msgstr "Servidor:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
-msgstr "Definir Dublado: {0} ok, {1} apenas aúdio, {2} falhou"
+msgstr "Definir como dobrado: {0} ok, {1} áudio apenas, {2} falhou"
 
 msgid "Set Subbed: {0} ok, {1} fail"
-msgstr "Definir Legendado: {0} ok, {1} falhou"
+msgstr "Definir como legendado: {0} ok, {1} falhou"
 
 msgid "Setting Current..."
-msgstr "A definir Atual..."
+msgstr "Configuração atual..."
 
 msgid "Show Console"
-msgstr "Mostrar Consola"
+msgstr "Mostrar consola"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Introdução ignorada"
+
 msgid "Small"
 msgstr "Pequeno"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -330,15 +345,15 @@
 msgid "Subtitle Position: {0}"
 msgstr "Posição das Legendas: {0}"
 
 msgid "Subtitle Size: {0}"
 msgstr "Tamanho das Legendas: {0}"
 
 msgid "Successfully added server."
-msgstr "Servidor adicionado com êxito."
+msgstr "Servidor adicionado com sucesso."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sincronização Desativada (Demasiadas Tentativas)"
 
 msgid "SyncPlay"
 msgstr "SyncPlay"
 
@@ -356,56 +371,59 @@
 
 msgid "Tiny"
 msgstr "Minúsculo"
 
 msgid "Top"
 msgstr "Cimo"
 
+msgid "Transcode HDR"
+msgstr "Transcodificar HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Transcodificar Hi10p para 8bit"
 
 msgid "Unkn"
 msgstr "Desconhecido"
 
 msgid "Use Web Seek Pref"
 msgstr "Utilizar as Prefs da Procuração de Jellyfin Web"
 
 msgid "Username:"
-msgstr "Nome de Usuário:"
+msgstr "Nome de utilizador:"
 
 msgid "Username: "
-msgstr "Nome de Usuário: "
+msgstr "Nome de utilizador: "
 
 msgid "Video Playback Profiles"
 msgstr "Perfis de Reprodução de Vídeo"
 
 msgid "Video Preferences"
 msgstr "Preferências de Vídeo"
 
 msgid "Video Profile Subtype"
-msgstr "Subtipo do Perfil de Vídeo"
+msgstr "Perfil de Video Subtipo: {0}"
 
 msgid "Video Profile Subtype: {0}"
-msgstr "Subtipo do Perfil de Vídeo: {0}"
+msgstr "Perfil de Video Subtipo: {0}"
 
 msgid "White"
 msgstr "Branco"
 
 msgid "Write Logs to File"
-msgstr "Escrever Registos para um Ficheiro"
+msgstr "Escrever registos em ficheiro"
 
 msgid "Yellow"
 msgstr "Amarelo"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
 "O seu vídeo remoto esta a ser transcodificado!↵\n"
-"Pressione c para ajustar as configurações da largura de banda se não é "
+"Pressione c para ajustar as configurações da largura de banda se tal não for "
 "necessário."
 
 msgid "{0} has joined."
 msgstr "{0} juntou-se."
 
 msgid "{0} has left."
 msgstr "{0} saiu."
@@ -416,8 +434,8 @@
 msgid "{0}'s Group"
 msgstr "Grupo de {0}"
 
 msgid "{0}: Fail"
 msgstr "{0}: Falhou"
 
 msgid "{0}: No Subtitles"
-msgstr "{0}: Sem Legendas"
+msgstr "{0}: Sem legendas"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-03-06 10:20+0000\n"
-"Last-Translator: sand14 <sand.avrigeanu@yahoo.com>\n"
+"PO-Revision-Date: 2023-10-20 12:11+0000\n"
+"Last-Translator: Acrotos <alexandrufly@gmail.com>\n"
 "Language-Team: Romanian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/ro/>\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : (n==0 || (n%100 > 0 && n%100 < "
@@ -28,14 +28,17 @@
 
 msgid "Add another server?"
 msgstr "Adăugați alt server?"
 
 msgid "Adding server failed."
 msgstr "Adăugarea serverului a eșuat."
 
+msgid "Always Skip Intros"
+msgstr "Treci mereu peste introducere"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (For HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (For HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Jurnalul Aplicației"
 
 msgid "Application Menu"
 msgstr "Meniul Aplicației"
 
+msgid "Ask to Skip Intros"
+msgstr "Întreabă înainte să treci peste introducere"
+
 msgid "Auto Fullscreen"
 msgstr "Ecran complet automat"
 
 msgid "Auto Play"
 msgstr "Redare automată"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -108,15 +114,15 @@
 "Nu s-a putut adăuga serverul.\n"
 "Vă rugăm să verificați informațiile conexiunii."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Crearea unui grup SyncPlay nu este permisă."
 
 msgid "Cyan"
-msgstr "Cian"
+msgstr "verde-albastrui"
 
 msgid "Direct Paths"
 msgstr "Calea directă"
 
 msgid "Disable"
 msgstr "Dezactivează"
 
@@ -131,14 +137,17 @@
 
 msgid "Display Mirroring"
 msgstr "Oglindirea ecranului"
 
 msgid "Enable SVP"
 msgstr "Activează SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Activați previzualizările în miniatură"
+
 msgid "English Audio"
 msgstr "Audio în engleză"
 
 msgid "Fail"
 msgstr "Eșuat"
 
 msgid "Generic (FSRCNNX)"
@@ -208,21 +217,21 @@
 msgid "Normal"
 msgstr "Normal"
 
 msgid "Ok"
 msgstr "Ok"
 
 msgid "Open Config Folder"
-msgstr "Deschideți dosarul de configurare"
+msgstr "Deschideți fișierul de configurare"
 
 msgid "Password:"
 msgstr "Parolă:"
 
 msgid "Password: "
-msgstr "Parola: "
+msgstr "Parolă: "
 
 msgid "Player Preferences"
 msgstr "Preferințe Redare"
 
 msgid "Quit"
 msgstr "Ieșire"
 
@@ -241,28 +250,31 @@
 msgid "Remove Server"
 msgstr "Eliminați Serverul"
 
 msgid "Retry"
 msgstr "Reîncearcă"
 
 msgid "SVP Settings"
-msgstr "SVP Setări"
+msgstr "Setări SVP"
 
 msgid "SVP is Disabled"
 msgstr "SVP este dezactivat"
 
 msgid "SVP is Not Active"
 msgstr "SVP nu e activ"
 
 msgid "Screenshot"
 msgstr "Captură de ecran"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sezonul {0} - Episodul {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Încearcă să sari peste introducere"
+
 msgid "Select Audio Track"
 msgstr "Selectați Pista Audio"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Selectează Audio/Subtitrare pentru Serie"
 
 msgid "Select Default Transcode Profile"
@@ -289,15 +301,15 @@
 msgid "Select Transcode Quality"
 msgstr "Selectați Calitatea Transcodării"
 
 msgid "Select your media in Jellyfin and play it here"
 msgstr "Selectați-vă media în Jellyfin și redați-o aici"
 
 msgid "Selecting Tracks..."
-msgstr "Se selectează melodiile ..."
+msgstr "Se selectează melodiile..."
 
 msgid "Server Configuration"
 msgstr "Configurare Server"
 
 msgid "Server URL: "
 msgstr "URL Server: "
 
@@ -315,14 +327,17 @@
 
 msgid "Show Console"
 msgstr "Afișați Consola"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Sari peste introducere"
+
 msgid "Small"
 msgstr "Mic"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -400,16 +415,16 @@
 msgid "Yellow"
 msgstr "Galben"
 
 msgid ""
 "Your remote video is transcoding!\n"
 "Press c to adjust bandwidth settings if this is not needed."
 msgstr ""
-"Videoul dvs se convertește\n"
-"Apăsați c pentru ajustarea setării lățimii de bandă dacă nu e nevoie."
+"Videoclipul tău se transcodează!\n"
+"Apasă C pentru a ajusta setările lățimii de bandă dacă nu e nevoie."
 
 msgid "{0} has joined."
 msgstr "{0} s-a alăturat."
 
 msgid "{0} has left."
 msgstr "{0} a plecat."
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-12-05 15:51+0000\n"
-"Last-Translator: Kirill Tyurin <1337soundwave1337@gmail.com>\n"
+"PO-Revision-Date: 2023-10-15 15:25+0000\n"
+"Last-Translator: Spuffio <spuffioworks@gmail.com>\n"
 "Language-Team: Russian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
@@ -26,15 +26,18 @@
 msgid "Add Server"
 msgstr "Добавить сервер"
 
 msgid "Add another server?"
 msgstr "Добавить ещё сервер?"
 
 msgid "Adding server failed."
-msgstr "Добавление сервера неудачно."
+msgstr "Не удалось добавить сервер."
+
+msgid "Always Skip Intros"
+msgstr "Всегда пропускать вступительные ролики"
 
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Достоверный (для HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Перцептивный (для HD)"
 
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Журнал приложения"
 
 msgid "Application Menu"
 msgstr "Меню приложения"
 
+msgid "Ask to Skip Intros"
+msgstr "Спрашивать, пропускать ли вступительные ролики"
+
 msgid "Auto Fullscreen"
 msgstr "Автоматический полный экран"
 
 msgid "Auto Play"
 msgstr "Автоматическое воспроизведение"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -95,15 +101,15 @@
 msgid "Close"
 msgstr "Закрыть"
 
 msgid "Close Menu"
 msgstr "Закрыть меню"
 
 msgid "Configure Servers"
-msgstr "Конфигурировать серверы"
+msgstr "Настроить серверы"
 
 msgid ""
 "Could not add server.\n"
 "Please check your connection information."
 msgstr ""
 "Не удалось добавить сервер.\n"
 "Проверьте информацию о подключении."
@@ -123,22 +129,25 @@
 msgid "Disable Direct Play"
 msgstr "Отключить прямое воспроизведение"
 
 msgid "Disabled"
 msgstr "Отключено"
 
 msgid "Discord Rich Presence"
-msgstr "Rich Presence от Discord"
+msgstr "Статус активности (Rich Presence) в Discord"
 
 msgid "Display Mirroring"
 msgstr "Зеркалирование дисплея"
 
 msgid "Enable SVP"
 msgstr "Включить SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Включить предварительный просмотр миниатюр"
+
 msgid "English Audio"
 msgstr "Английское аудио"
 
 msgid "Fail"
 msgstr "Неудачно"
 
 msgid "Generic (FSRCNNX)"
@@ -235,15 +244,15 @@
 msgid "Red"
 msgstr "Красный"
 
 msgid "Remote Transcode Quality: {0:0.1f} Mbps"
 msgstr "Качество удалённого перекодирования: {0: 0,1f} Мибит/с"
 
 msgid "Remove Server"
-msgstr "Изъять сервер"
+msgstr "Убрать сервер"
 
 msgid "Retry"
 msgstr "Повторить"
 
 msgid "SVP Settings"
 msgstr "Параметры SVP"
 
@@ -255,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "Снимок экрана"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Сезон {0} - Эпизод {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Пропустить вступительный ролик"
+
 msgid "Select Audio Track"
 msgstr "Выбрать аудио дорожку"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Выбрать аудио/субтитры для сериала"
 
 msgid "Select Default Transcode Profile"
@@ -286,63 +298,66 @@
 msgid "Select Subtitle Track"
 msgstr "Выбрать дорожку субтитров"
 
 msgid "Select Transcode Quality"
 msgstr "Выбрать качество перекодирования"
 
 msgid "Select your media in Jellyfin and play it here"
-msgstr "Выберите медиаданные в Jellyfin и воспроизведите их здесь"
+msgstr "Выберите медиафайлы в Jellyfin и воспроизведите их здесь"
 
 msgid "Selecting Tracks..."
 msgstr "Выбираются дорожки…"
 
 msgid "Server Configuration"
 msgstr "Конфигурация сервера"
 
 msgid "Server URL: "
 msgstr "URL сервера: "
 
 msgid "Server:"
 msgstr "Сервер:"
 
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
-msgstr "Задать дубляж: {0} ОК, {1} только аудио, {2} неудачно"
+msgstr "Выбрать дубляж: {0} ОК, {1} только звук, {2} неудачно"
 
 msgid "Set Subbed: {0} ok, {1} fail"
 msgstr "Задать субтитраж: {0} ОК, {1} неудачно"
 
 msgid "Setting Current..."
 msgstr "Задаются текущие..."
 
 msgid "Show Console"
 msgstr "Показать консоль"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync - (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Пропущенное вступление"
+
 msgid "Small"
 msgstr "Мелкий"
 
 msgid "SpeedToSync (x{0})"
-msgstr "SpeedToSync - (x{0})"
+msgstr "Скорость синхронизации (SpeedToSync) - (x{0})"
 
 msgid "Subtitle Color: {0}"
 msgstr "Цвет субтитров: {0}"
 
 msgid "Subtitle Position: {0}"
 msgstr "Позиция субтитров: {0}"
 
 msgid "Subtitle Size: {0}"
 msgstr "Размер субтитров: {0}"
 
 msgid "Successfully added server."
 msgstr "Сервер добавлен успешно."
 
 msgid "Sync Disabled (Too Many Attempts)"
-msgstr "Синхро отключено (Слишком много попыток)"
+msgstr "Синхронизация отключена (слишком много попыток)"
 
 msgid "SyncPlay"
 msgstr "Служба SyncPlay"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay отключен."
 
@@ -357,14 +372,17 @@
 
 msgid "Tiny"
 msgstr "Крошечный"
 
 msgid "Top"
 msgstr "Вверху"
 
+msgid "Transcode HDR"
+msgstr "Перекодирование в HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Перекодирование Hi10p в 8bit"
 
 msgid "Unkn"
 msgstr "Неизвестно"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-27 20:43+0000\n"
-"Last-Translator: MCSifreedsk33 <andrej.melek1121@gmail.com>\n"
+"PO-Revision-Date: 2023-04-20 11:39+0000\n"
+"Last-Translator: nextlooper42 <nextlooper42@protonmail.com>\n"
 "Language-Team: Slovak <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/sk/>\n"
 "Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=(n==1) ? 0 : (n>=2 && n<=4) ? 1 : 2;\n"
@@ -263,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Snímka obrazovky"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Séria {0} - Epizóda {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Preskočiť intro"
+
 msgid "Select Audio Track"
 msgstr "Vybrať zvukovú stopu"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Vybrať zvuk/titulky pre sériu"
 
 msgid "Select Default Transcode Profile"
@@ -377,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Prekódovať Hi10p na 8bit"
 
 msgid "Unkn"
 msgstr "Neznáme"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Použiť JellyScrub miniatúry"
-
 msgid "Use Web Seek Pref"
 msgstr "Použiť webové preferencie pretáčania"
 
 msgid "Username:"
 msgstr "Používateľské meno:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-08-25 22:11+0000\n"
-"Last-Translator: jan <kukovicster@gmail.com>\n"
+"PO-Revision-Date: 2023-10-11 15:25+0000\n"
+"Last-Translator: SaddFox <filip.rutar@gmail.com>\n"
 "Language-Team: Slovenian <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/sl/>\n"
 "Language: sl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n%100==1 ? 0 : n%100==2 ? 1 : n%100==3 || "
 "n%100==4 ? 2 : 3;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 4.14.1\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Prekodiranje)"
 
 msgid " Forced"
 msgstr " Prisiljeno"
@@ -28,14 +28,17 @@
 
 msgid "Add another server?"
 msgstr "Dodaj še en strežnik?"
 
 msgid "Adding server failed."
 msgstr "Napaka pri dodajanju strežnika."
 
+msgid "Always Skip Intros"
+msgstr "Vedno preskoči uvode"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (Za HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (Za HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -52,14 +55,17 @@
 
 msgid "Application Log"
 msgstr "Dnevnik aplikacije"
 
 msgid "Application Menu"
 msgstr "Meni aplikacije"
 
+msgid "Ask to Skip Intros"
+msgstr "Vprašaj za preskok uvoda"
+
 msgid "Auto Fullscreen"
 msgstr "Samodejni celotni zaslon"
 
 msgid "Auto Play"
 msgstr "Samodejno predvajanje"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -108,15 +114,15 @@
 "Strežnika ni bilo mogoče dodati.\n"
 "Preverite vaše nastavitve povezave."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "Ustvarjanje SyncPlay skupin ni dovoljeno."
 
 msgid "Cyan"
-msgstr "Cian"
+msgstr "cian"
 
 msgid "Direct Paths"
 msgstr "Neposredne poti"
 
 msgid "Disable"
 msgstr "Onemogoči"
 
@@ -131,14 +137,17 @@
 
 msgid "Display Mirroring"
 msgstr "Zrcaljenje zaslona"
 
 msgid "Enable SVP"
 msgstr "Omogoči SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Omogoči predogledne sličice"
+
 msgid "English Audio"
 msgstr "Angleški zvok"
 
 msgid "Fail"
 msgstr "Napaka"
 
 msgid "Generic (FSRCNNX)"
@@ -255,14 +264,17 @@
 
 msgid "Screenshot"
 msgstr "Posnetek zaslona"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Sezona {0} - Epizoda {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Premik za preskok uvoda"
+
 msgid "Select Audio Track"
 msgstr "Izberi zvokovno sled"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Izberi zvok/podnapise za serijo"
 
 msgid "Select Default Transcode Profile"
@@ -307,22 +319,25 @@
 msgid "Set Dubbed: {0} ok, {1} audio only, {2} fail"
 msgstr "Nastavi sinhronizacijo: {0} ok, {1} samo zvok, {2} napaka"
 
 msgid "Set Subbed: {0} ok, {1} fail"
 msgstr "Nastavi podnapise: {0} ok, {1} napaka"
 
 msgid "Setting Current..."
-msgstr "Nastavljam trenutne..."
+msgstr "Nastavi trenutno ..."
 
 msgid "Show Console"
 msgstr "Pokaži konzolo"
 
 msgid "SkipToSync (x{0})"
 msgstr "Preskoči na sinhronizacijo (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Uvod je bil preskočen"
+
 msgid "Small"
 msgstr "Majhno"
 
 msgid "SpeedToSync (x{0})"
 msgstr "Hitrost sinhronizacije (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -337,15 +352,15 @@
 msgid "Successfully added server."
 msgstr "Strežnik uspešno dodan."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Sinhronizacija onemogočena (Preveč poskusov)"
 
 msgid "SyncPlay"
-msgstr "SyncPlay"
+msgstr "SinhroniziranoPredvajanja"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay onemogočen."
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay omogočen."
 
@@ -357,14 +372,17 @@
 
 msgid "Tiny"
 msgstr "Najmanjše"
 
 msgid "Top"
 msgstr "Na vrhu"
 
+msgid "Transcode HDR"
+msgstr "Prekodiraj HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Prekodiraj Hi10p v 8bit"
 
 msgid "Unkn"
 msgstr "Neznano"
 
 msgid "Use Web Seek Pref"
@@ -382,15 +400,15 @@
 msgid "Video Preferences"
 msgstr "Nastavitve videa"
 
 msgid "Video Profile Subtype"
 msgstr "Podtip video profila"
 
 msgid "Video Profile Subtype: {0}"
-msgstr "Podtip video profila: {0}"
+msgstr "Podvrsta video profila: {0}"
 
 msgid "White"
 msgstr "Bela"
 
 msgid "Write Logs to File"
 msgstr "Zapiši dnevnike v datoteko"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-08-14 07:27+0000\n"
-"Last-Translator: Arceer <armin.cero@gmail.com>\n"
+"PO-Revision-Date: 2024-03-05 03:38+0000\n"
+"Last-Translator: Alvin <alvinzilverstand@gmail.com>\n"
 "Language-Team: Swedish <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/sv/>\n"
 "Language: sv\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.13.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (Omkoda)"
 
 msgid " Forced"
 msgstr " Tvingad"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "Lägg till en annan server?"
 
 msgid "Adding server failed."
 msgstr "Tilläggande av server misslyckades."
 
+msgid "Always Skip Intros"
+msgstr "Hoppa alltid över introduktioner"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Trogen (För HD)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptuell (För HD)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "Applikationslogg"
 
 msgid "Application Menu"
 msgstr "Applikations meny"
 
+msgid "Ask to Skip Intros"
+msgstr "Fråga om att hoppa över intron"
+
 msgid "Auto Fullscreen"
 msgstr "Automatiskt fullskärm"
 
 msgid "Auto Play"
 msgstr "Automatisk uppspelning"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -122,22 +128,25 @@
 msgid "Disable Direct Play"
 msgstr "Avaktivera Direct Play"
 
 msgid "Disabled"
 msgstr "Inaktiverad"
 
 msgid "Discord Rich Presence"
-msgstr "Discord Rich Presence"
+msgstr "Discord rik närvaro"
 
 msgid "Display Mirroring"
 msgstr "Visa spegling"
 
 msgid "Enable SVP"
 msgstr "Aktivera SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "Använd miniatyr-förhandsvisning"
+
 msgid "English Audio"
 msgstr "Engelskt tal"
 
 msgid "Fail"
 msgstr "Misslyckat"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "Skärmdump"
 
 msgid "Season {0} - Episode {1}"
 msgstr "Säsong {0} - Avsnitt {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "Sök för att hopa över introt"
+
 msgid "Select Audio Track"
 msgstr "Välj ljudfil"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "Välj ljud/undertext för serie"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Visa konsol"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Hoppade över introt"
+
 msgid "Small"
 msgstr "Liten"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "Mycket liten"
 
 msgid "Top"
 msgstr "Längst upp"
 
+msgid "Transcode HDR"
+msgstr "Omkoda HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "Omkoda Hi10p till 8bit"
 
 msgid "Unkn"
 msgstr "Okänd"
 
 msgid "Use Web Seek Pref"
@@ -412,11 +430,11 @@
 msgid "{0} is buffering."
 msgstr "{0} håller på att buffra."
 
 msgid "{0}'s Group"
 msgstr "{0}s grupp"
 
 msgid "{0}: Fail"
-msgstr "{0}: Fel"
+msgstr "{0}: Misslyckat"
 
 msgid "{0}: No Subtitles"
 msgstr "{0}: Inga undertexter"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-09-28 04:54+0000\n"
-"Last-Translator: K.B.Dharun Krishna <kbdharunkrishna@gmail.com>\n"
+"PO-Revision-Date: 2024-04-01 00:05+0000\n"
+"Last-Translator: Oatavandi <oatavandi@gmail.com>\n"
 "Language-Team: Tamil <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/ta/>\n"
 "Language: ta\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 4.14.1\n"
+"X-Generator: Weblate 5.4.2\n"
 "Generated-By: pygettext.py 1.5\n"
 
 msgid " (Transcode)"
 msgstr " (டிரான்ஸ்கோட்)"
 
 msgid " Forced"
 msgstr " கட்டாயப்படுத்தப்பட்டது"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "மற்றொரு சேவையகத்தைச் சேர்க்கவா?"
 
 msgid "Adding server failed."
 msgstr "சேவையகத்தைச் சேர்ப்பது தோல்வியுற்றது."
 
+msgid "Always Skip Intros"
+msgstr "முன்னோட்டங்களை எப்போதும் தவிர்"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "அனிம் 4 கே x2 விசுவாசமான (HD க்கு)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "அனிம் 4 கே x2 புலனுணர்வு (HD க்கு)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "பயன்பாட்டு பதிவு"
 
 msgid "Application Menu"
 msgstr "விண்ணப்ப மெனு"
 
+msgid "Ask to Skip Intros"
+msgstr "முன்னோட்டங்களை தவிர்க்க சொல்லி கேள்"
+
 msgid "Auto Fullscreen"
 msgstr "ஆட்டோ முழுத்திரை"
 
 msgid "Auto Play"
 msgstr "தானியங்கி"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -107,37 +113,40 @@
 "சேவையகத்தைச் சேர்க்க முடியவில்லை.\n"
 "உங்கள் இணைப்பு தகவலை சரிபார்க்கவும்."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "ஒத்திசைவு குழுக்களை உருவாக்குவது அனுமதிக்கப்படாது."
 
 msgid "Cyan"
-msgstr "சியான்"
+msgstr "நீல-பச்சை நிறம்"
 
 msgid "Direct Paths"
 msgstr "நேரடி பாதைகள்"
 
 msgid "Disable"
 msgstr "முடக்கு"
 
 msgid "Disable Direct Play"
 msgstr "நேரடி விளையாட்டை முடக்கு"
 
 msgid "Disabled"
 msgstr "முடக்கப்பட்டது"
 
 msgid "Discord Rich Presence"
-msgstr "இருப்பை நிராகரி"
+msgstr "டிஸ்கார்ட் ரிச் பிரசன்ஸ்"
 
 msgid "Display Mirroring"
 msgstr "காட்சி பிரதிபலிப்பு"
 
 msgid "Enable SVP"
 msgstr "SVP ஐ இயக்கு"
 
+msgid "Enable thumbnail previews"
+msgstr "படங்களின் முன்னோட்டங்களை கான்பி"
+
 msgid "English Audio"
 msgstr "ஆங்கில ஆடியோ"
 
 msgid "Fail"
 msgstr "தோல்வி"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "ஸ்கிரீன்ஷாட்"
 
 msgid "Season {0} - Episode {1}"
 msgstr "பருவம் {0} - அத்தியாயம் {1}"
 
+msgid "Seek to Skip Intro"
+msgstr "முன்னோட்டத்தை தவிர்க்க காணொளியை நகர்த்தவும்"
+
 msgid "Select Audio Track"
 msgstr "ஆடியோ டிராக்கைத் தேர்ந்தெடுக்கவும்"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "தொடருக்கான ஆடியோ / வசனத்தைத் தேர்ந்தெடுக்கவும்"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "கன்சோலைக் காட்டு"
 
 msgid "SkipToSync (x{0})"
 msgstr "SkipToSync (x {0})"
 
+msgid "Skipped Intro"
+msgstr "முன்னோட்டம் தவிர்க்க பட்டது"
+
 msgid "Small"
 msgstr "சிறிய"
 
 msgid "SpeedToSync (x{0})"
 msgstr "SpeedToSync (x {0})"
 
 msgid "Subtitle Color: {0}"
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "சிறிய"
 
 msgid "Top"
 msgstr "மேலே"
 
+msgid "Transcode HDR"
+msgstr "H265 டிரான்ஸ்கோட்"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "டிரான்ஸ்கோட் Hi10p முதல் 8bit வரை"
 
 msgid "Unkn"
 msgstr "தெரியவில்லை"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-09-28 04:54+0000\n"
-"Last-Translator: Burak Meric <mburakmeric22@gmail.com>\n"
+"PO-Revision-Date: 2023-12-19 09:34+0000\n"
+"Last-Translator: queeup <queeup@zoho.com>\n"
 "Language-Team: Turkish <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/tr/>\n"
 "Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
@@ -16,25 +16,28 @@
 msgid " (Transcode)"
 msgstr " (Kod dönüştürme)"
 
 msgid " Forced"
 msgstr " Gömülü"
 
 msgid "Access to the SyncPlay library was denied."
-msgstr "SyncPlay kitaplığına erişim reddedildi."
+msgstr "SyncPlay kütüphanesine erişim reddedildi."
 
 msgid "Add Server"
 msgstr "Sunucu ekle"
 
 msgid "Add another server?"
 msgstr "Başka bir sunucu eklemek ister misiniz?"
 
 msgid "Adding server failed."
 msgstr "Sunucu ekleme başarısız oldu."
 
+msgid "Always Skip Intros"
+msgstr "Her Zaman Girişi Geç"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (HD Kalite)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (HD Kalite)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,22 +54,25 @@
 
 msgid "Application Log"
 msgstr "Uygulama Günlüğü"
 
 msgid "Application Menu"
 msgstr "Uygulama Menüsü"
 
+msgid "Ask to Skip Intros"
+msgstr "Girişi Geçmek için Sor"
+
 msgid "Auto Fullscreen"
 msgstr "Otomatik Tam Ekran"
 
 msgid "Auto Play"
 msgstr "Otomatik oynatma"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
-msgstr "Sesi ve Altyazıları Otomatik Ayarla (Tüm Seri İçin)"
+msgstr "Sesi ve Altyazıları Otomatik Ayarla (Tüm Diziler İçin)"
 
 msgid "Automatic"
 msgstr "Otomatik"
 
 msgid "Black"
 msgstr "Siyah"
 
@@ -107,37 +113,40 @@
 "Sunucu eklenemedi.\n"
 "Lütfen bağlantınızı kontrol ediniz."
 
 msgid "Creating SyncPlay groups is not allowed."
 msgstr "SyncPlay grupları oluşturmaya izin verilmez."
 
 msgid "Cyan"
-msgstr "Açık mavi"
+msgstr "Cam göbeği"
 
 msgid "Direct Paths"
-msgstr "Direkt Yol"
+msgstr "Doğrudan Yollar"
 
 msgid "Disable"
 msgstr "Devre dışı bırak"
 
 msgid "Disable Direct Play"
-msgstr "Direkt Oynatmayı Devre Dışı Bırak"
+msgstr "Doğrudan Oynatmayı Devre Dışı Bırak"
 
 msgid "Disabled"
 msgstr "Devre Dışı"
 
 msgid "Discord Rich Presence"
-msgstr "Discord Rich Presence Özelliği"
+msgstr "Discord"
 
 msgid "Display Mirroring"
 msgstr "Görüntü Yansıtma"
 
 msgid "Enable SVP"
 msgstr "SVP'yi etkinleştir"
 
+msgid "Enable thumbnail previews"
+msgstr "Küçük resim önizlemelerini etkinleştirin"
+
 msgid "English Audio"
 msgstr "İngilizce Ses"
 
 msgid "Fail"
 msgstr "Hata"
 
 msgid "Generic (FSRCNNX)"
@@ -155,15 +164,15 @@
 msgid "Huge"
 msgstr "Kocaman"
 
 msgid "Japanese Audio w/ English Subtitles"
 msgstr "Japonca Ses, İngilizce Altyazılı"
 
 msgid "Large"
-msgstr "Geniş"
+msgstr "Büyük"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} Sürüm Bilgisi/İndir"
 
 msgid ""
 "MPV Shim v{0} Update Available\n"
 "Open menu (press c) for details."
@@ -174,15 +183,15 @@
 msgid "Magenta"
 msgstr "Eflatun"
 
 msgid "Main Menu"
 msgstr "Ana Menü"
 
 msgid "Manual by Track Index (Less Reliable)"
-msgstr "Gömülü Kayıda Göre Kılavuz (Daha Az Güvenilir)"
+msgstr "Sizin Tarafınızdan Parça Dizinine Göre (Daha Az Güvenilir)"
 
 msgid "Manual: {0} ok, {1} fail"
 msgstr "Manuel: {0} tamam, {1} hata"
 
 msgid "Maximum"
 msgstr "Maksimum"
 
@@ -210,27 +219,27 @@
 msgid "Ok"
 msgstr "Tamam"
 
 msgid "Open Config Folder"
 msgstr "Yapılandırma Klasörünü Aç"
 
 msgid "Password:"
-msgstr "Şifre:"
+msgstr "Parola:"
 
 msgid "Password: "
-msgstr "Şifre: "
+msgstr "Parola: "
 
 msgid "Player Preferences"
 msgstr "Kullanıcı Tercihleri"
 
 msgid "Quit"
 msgstr "Çıkış Yap"
 
 msgid "Quit and Mark Unwatched"
-msgstr "Çık ve İzlenmedi Olarak İşaretle"
+msgstr "İzlenmedi Olarak İşaretle ve Çıkış Yap"
 
 msgid "Ready to cast"
 msgstr "Yayınlamaya hazır"
 
 msgid "Red"
 msgstr "Kırmızı"
 
@@ -246,36 +255,39 @@
 msgid "SVP Settings"
 msgstr "SVP Ayarları"
 
 msgid "SVP is Disabled"
 msgstr "SVP Devre Dışı Bırakıldı"
 
 msgid "SVP is Not Active"
-msgstr "SVP Aktif Değil"
+msgstr "SVP Etkin Değil"
 
 msgid "Screenshot"
 msgstr "Ekran Görüntüsü"
 
 msgid "Season {0} - Episode {1}"
-msgstr "Sezon {0} - Bölüm {1}"
+msgstr "{0}. Sezon - {1}. Bölüm"
+
+msgid "Seek to Skip Intro"
+msgstr "Girişi Atlamak için Ara"
 
 msgid "Select Audio Track"
-msgstr "Ses Parçasını Seçin"
+msgstr "Ses Parçası Seçin"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "Dizi için Ses/Altyazı Seçin"
+msgstr "Dizi için Ses ve Altyazı Seçin"
 
 msgid "Select Default Transcode Profile"
 msgstr "Varsayılan Kod Dönüştürme Profilini Seçin"
 
 msgid "Select SVP Profile"
 msgstr "SVP Profilini Seçin"
 
 msgid "Select Shader Profile"
-msgstr "Shader Profili Seç"
+msgstr "Gölgelendirici Profili Seçin"
 
 msgid "Select Subtitle Color"
 msgstr "Altyazı Rengini Seç"
 
 msgid "Select Subtitle Position"
 msgstr "Altyazı Konumunu Seçin"
 
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "Konsolu göster"
 
 msgid "SkipToSync (x{0})"
 msgstr "EşZamanlamayıAtla (x{0})"
 
+msgid "Skipped Intro"
+msgstr "Giriş Geçildi"
+
 msgid "Small"
 msgstr "Küçük"
 
 msgid "SpeedToSync (x{0})"
 msgstr "HızıEşZamanla (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -336,15 +351,15 @@
 msgid "Successfully added server."
 msgstr "Sunucu başarılı bir şekilde eklendi."
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "Eşzamanlama Devre Dışı (Çok Fazla Deneme)"
 
 msgid "SyncPlay"
-msgstr "Aynı Anda Oynatma"
+msgstr "SyncPlay"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay devre dışı."
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay aktif."
 
@@ -356,16 +371,19 @@
 
 msgid "Tiny"
 msgstr "Minik"
 
 msgid "Top"
 msgstr "Üst"
 
+msgid "Transcode HDR"
+msgstr "HDR kod dönüştürme"
+
 msgid "Transcode Hi10p to 8bit"
-msgstr "Hi10p'ten 8bit'e dönüştürün"
+msgstr "Hi10p'ten 8bit'e kod dönüştürün"
 
 msgid "Unkn"
 msgstr "Blnmyr"
 
 msgid "Use Web Seek Pref"
 msgstr "Web Arama Tercihini Kullan"
 
@@ -378,18 +396,18 @@
 msgid "Video Playback Profiles"
 msgstr "Video Oynatma Profilleri"
 
 msgid "Video Preferences"
 msgstr "Video Tercihleri"
 
 msgid "Video Profile Subtype"
-msgstr "Video Profil Alt Tipi"
+msgstr "Video Profili Alt Türü"
 
 msgid "Video Profile Subtype: {0}"
-msgstr "Video Profil Alttipi"
+msgstr "Video Profili Alt Türü: {0}"
 
 msgid "White"
 msgstr "Beyaz"
 
 msgid "Write Logs to File"
 msgstr "Günlükleri Dosyaya Yaz"
 
@@ -416,8 +434,8 @@
 msgid "{0}'s Group"
 msgstr "{0}'ın Grubu"
 
 msgid "{0}: Fail"
 msgstr "{0}: Hata"
 
 msgid "{0}: No Subtitles"
-msgstr "{0}: Altyazı yok"
+msgstr "{0}: Altyazı Yok"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -381,17 +381,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Перекодувати Hi10p на 8біт"
 
 msgid "Unkn"
 msgstr "Невідомо"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Використовувати мініатюри JellyScrub"
-
 msgid "Use Web Seek Pref"
 msgstr "Використовувати Web Seek Pref"
 
 msgid "Username:"
 msgstr "Ім'я користувача:"
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-27 20:43+0000\n"
-"Last-Translator: Toby Cm <newtobycm@gmail.com>\n"
+"PO-Revision-Date: 2024-01-27 18:30+0000\n"
+"Last-Translator: hoanghuy309 <hoanghuy309@gmail.com>\n"
 "Language-Team: Vietnamese <https://translate.jellyfin.org/projects/jellyfin/"
 "jellyfin-desktop/vi/>\n"
 "Language: vi\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -368,29 +368,35 @@
 
 msgid "Transcode HDR"
 msgstr "Chuyển mã HDR"
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "Chuyển mã Hi10p sang 8bit"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "Dùng hình nhỏ JellyScrub"
+msgid "Unkn"
+msgstr "Ko rõ"
 
 msgid "Username:"
 msgstr "Tên đăng nhập:"
 
 msgid "Username: "
 msgstr "Tên đăng nhập: "
 
 msgid "Video Playback Profiles"
 msgstr "Cấu hình phát lại video"
 
 msgid "Video Preferences"
 msgstr "Tùy chọn video"
 
+msgid "Video Profile Subtype"
+msgstr "Loại phụ hồ sơ video"
+
+msgid "Video Profile Subtype: {0}"
+msgstr "Loại phụ hồ sơ video: {0}"
+
 msgid "White"
 msgstr "Trắng"
 
 msgid "Write Logs to File"
 msgstr "Ghi Nhật Ký vào Tệp"
 
 msgid "Yellow"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2023-02-22 15:39+0000\n"
-"Last-Translator: 小造xu_zh <ngc7331@outlook.com>\n"
+"PO-Revision-Date: 2023-05-23 16:21+0000\n"
+"Last-Translator: 皇甫朝云 <hfzy2014@gmail.com>\n"
 "Language-Team: Chinese (Simplified) <https://translate.jellyfin.org/projects/"
 "jellyfin/jellyfin-desktop/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -64,15 +64,15 @@
 msgid "Auto Fullscreen"
 msgstr "自动全屏"
 
 msgid "Auto Play"
 msgstr "自动播放"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
-msgstr "自动设置音频/字幕（整个系列）"
+msgstr "自动设置音频/字幕（整个节目）"
 
 msgid "Automatic"
 msgstr "自动"
 
 msgid "Black"
 msgstr "黑色"
 
@@ -128,15 +128,15 @@
 msgid "Disable Direct Play"
 msgstr "禁用直接播放"
 
 msgid "Disabled"
 msgstr "关闭"
 
 msgid "Discord Rich Presence"
-msgstr "Discord 细节呈现"
+msgstr "Discord丰富状态"
 
 msgid "Display Mirroring"
 msgstr "显示镜像"
 
 msgid "Enable SVP"
 msgstr "启用 SVP"
 
@@ -161,15 +161,15 @@
 msgid "Green"
 msgstr "绿色"
 
 msgid "Huge"
 msgstr "非常大"
 
 msgid "Japanese Audio w/ English Subtitles"
-msgstr "日语音频 / 英语字母"
+msgstr "日语音频 / 英语字幕"
 
 msgid "Large"
 msgstr "大"
 
 msgid "MPV Shim v{0} Release Info/Download"
 msgstr "MPV Shim v{0} 发布信息/下载"
 
@@ -183,15 +183,15 @@
 msgid "Magenta"
 msgstr "紫色"
 
 msgid "Main Menu"
 msgstr "主菜单"
 
 msgid "Manual by Track Index (Less Reliable)"
-msgstr "使用轨道索引手动选择（可靠性更低）"
+msgstr "使用手动选择音轨索引（可靠性更低）"
 
 msgid "Manual: {0} ok, {1} fail"
 msgstr "手动：{0} 成功，{1} 失败"
 
 msgid "Maximum"
 msgstr "最大"
 
@@ -267,18 +267,18 @@
 msgid "Season {0} - Episode {1}"
 msgstr "第 {0} 季第 {1} 集"
 
 msgid "Seek to Skip Intro"
 msgstr "跳过片头"
 
 msgid "Select Audio Track"
-msgstr "选择音频轨道"
+msgstr "选择音频音轨"
 
 msgid "Select Audio/Subtitle for Series"
-msgstr "选择系列的音频/字幕"
+msgstr "选择节目音频/字幕"
 
 msgid "Select Default Transcode Profile"
 msgstr "选择默认转码预设"
 
 msgid "Select SVP Profile"
 msgstr "选择 SVP 配置预设"
 
@@ -291,21 +291,21 @@
 msgid "Select Subtitle Position"
 msgstr "选择字幕位置"
 
 msgid "Select Subtitle Size"
 msgstr "选择字幕大小"
 
 msgid "Select Subtitle Track"
-msgstr "选择字幕轨道"
+msgstr "选择字幕音轨"
 
 msgid "Select Transcode Quality"
 msgstr "选择转码质量"
 
 msgid "Select your media in Jellyfin and play it here"
-msgstr "在Jellyfin中选择您的媒体并在此处播放"
+msgstr "在 Jellyfin 中选择您的媒体并在此处播放"
 
 msgid "Selecting Tracks..."
 msgstr "选择音轨..."
 
 msgid "Server Configuration"
 msgstr "服务器配置"
 
@@ -380,17 +380,14 @@
 
 msgid "Transcode Hi10p to 8bit"
 msgstr "将 Hi10p 转码为 8bit"
 
 msgid "Unkn"
 msgstr "未知"
 
-msgid "Use JellyScrub thumbnails"
-msgstr "使用 JellyScrub 缩略图"
-
 msgid "Use Web Seek Pref"
 msgstr "使用网络搜索偏好"
 
 msgid "Username:"
 msgstr "用户名："
 
 msgid "Username: "
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
-"PO-Revision-Date: 2022-11-21 05:51+0000\n"
-"Last-Translator: Akira Li <akira@irendezvous.net>\n"
+"PO-Revision-Date: 2023-12-26 20:30+0000\n"
+"Last-Translator: 李恩霆 (Lee,EN-TING) <timothylee0802@outlook.com>\n"
 "Language-Team: Chinese (Traditional) <https://translate.jellyfin.org/"
 "projects/jellyfin/jellyfin-desktop/zh_Hant/>\n"
 "Language: zh_Hant\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
@@ -27,14 +27,17 @@
 
 msgid "Add another server?"
 msgstr "新增其他伺服器?"
 
 msgid "Adding server failed."
 msgstr "新增伺服器失敗。"
 
+msgid "Always Skip Intros"
+msgstr "總是跳過片頭"
+
 msgid "Anime4K x2 Faithful (For HD)"
 msgstr "Anime4K x2 Faithful (供高畫質)"
 
 msgid "Anime4K x2 Perceptual (For HD)"
 msgstr "Anime4K x2 Perceptual (供高畫質)"
 
 msgid "Anime4K x2 Perceptual + Deblur (For HD)"
@@ -51,14 +54,17 @@
 
 msgid "Application Log"
 msgstr "應用程式日誌"
 
 msgid "Application Menu"
 msgstr "應用程式選單"
 
+msgid "Ask to Skip Intros"
+msgstr "請跳過序幕"
+
 msgid "Auto Fullscreen"
 msgstr "自動全螢幕"
 
 msgid "Auto Play"
 msgstr "自動播放"
 
 msgid "Auto Set Audio/Subtitles (Entire Series)"
@@ -122,22 +128,25 @@
 msgid "Disable Direct Play"
 msgstr "停用Direct Play"
 
 msgid "Disabled"
 msgstr "停用"
 
 msgid "Discord Rich Presence"
-msgstr "Discord自訂狀態"
+msgstr "Discord 整合"
 
 msgid "Display Mirroring"
 msgstr "螢幕鏡像"
 
 msgid "Enable SVP"
 msgstr "啟用SVP"
 
+msgid "Enable thumbnail previews"
+msgstr "啟用縮圖預覽"
+
 msgid "English Audio"
 msgstr "英文音訊"
 
 msgid "Fail"
 msgstr "連接失敗"
 
 msgid "Generic (FSRCNNX)"
@@ -254,14 +263,17 @@
 
 msgid "Screenshot"
 msgstr "截圖"
 
 msgid "Season {0} - Episode {1}"
 msgstr "第{0}季 - 第{1}集"
 
+msgid "Seek to Skip Intro"
+msgstr "直接進入正片"
+
 msgid "Select Audio Track"
 msgstr "選擇音軌"
 
 msgid "Select Audio/Subtitle for Series"
 msgstr "選擇影集的語音/字幕"
 
 msgid "Select Default Transcode Profile"
@@ -314,14 +326,17 @@
 
 msgid "Show Console"
 msgstr "顯示控制台"
 
 msgid "SkipToSync (x{0})"
 msgstr "跳過至同步 (x{0})"
 
+msgid "Skipped Intro"
+msgstr "已跳過序幕"
+
 msgid "Small"
 msgstr "小"
 
 msgid "SpeedToSync (x{0})"
 msgstr "同步速度 (x{0})"
 
 msgid "Subtitle Color: {0}"
@@ -336,15 +351,15 @@
 msgid "Successfully added server."
 msgstr "成功新增伺服器。"
 
 msgid "Sync Disabled (Too Many Attempts)"
 msgstr "同步已停用 (嘗試次數過多)"
 
 msgid "SyncPlay"
-msgstr "SyncPlay"
+msgstr "SyncPlay 遠端同步播放器"
 
 msgid "SyncPlay disabled."
 msgstr "SyncPlay已停用。"
 
 msgid "SyncPlay enabled."
 msgstr "SyncPlay已啟用。"
 
@@ -356,14 +371,17 @@
 
 msgid "Tiny"
 msgstr "非常小"
 
 msgid "Top"
 msgstr "頂部"
 
+msgid "Transcode HDR"
+msgstr "轉碼至HDR"
+
 msgid "Transcode Hi10p to 8bit"
 msgstr "從Hi10p轉碼至8bit"
 
 msgid "Unkn"
 msgstr "未知"
 
 msgid "Use Web Seek Pref"
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/mouse.lua` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mouse.lua`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/mpv_shim.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mpv_shim.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,32 +6,38 @@
 from threading import Event
 
 from . import conffile
 from . import i18n
 from .conf import settings
 from .clients import clientManager
 from .constants import APP_NAME
-from .log_utils import configure_log, enable_sanitization, configure_log_file
+from .log_utils import (
+    configure_log,
+    configure_log_file,
+    enable_sanitization,
+    root_logger,
+)
 
-configure_log(sys.stdout)
-log = logging.getLogger("")
 logging.getLogger("requests").setLevel(logging.CRITICAL)
 
 
 def main():
     conf_file = conffile.get(APP_NAME, "conf.json")
     load_success = settings.load(conf_file)
     i18n.configure()
 
     if settings.sanitize_output:
         enable_sanitization()
 
+    configure_log(sys.stdout, settings.mpv_log_level)
     if settings.write_logs:
         log_file = conffile.get(APP_NAME, "log.txt")
-        configure_log_file(log_file)
+        configure_log_file(log_file, settings.mpv_log_level)
+
+    log = root_logger
 
     if sys.platform.startswith("darwin"):
         multiprocessing.set_start_method("forkserver")
 
     user_interface = None
     mirror = None
     use_gui = False
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/player.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,14 @@
             and not self.syncplay.is_enabled()
             and self._video is not None
             and self._video.intro_start is not None
             and self._player.playback_time is not None
             and self._player.playback_time > self._video.intro_start
             and self._player.playback_time < self._video.intro_end
         ):
-
             if not self.is_in_intro:
                 if settings.skip_intro_always and not self.intro_has_triggered:
                     self.intro_has_triggered = True
                     self.skip_intro()
                     self._player.show_text(_("Skipped Intro"), 3000, 1)
                 elif settings.skip_intro_prompt:
                     self._player.show_text(_("Seek to Skip Intro"), 3000, 1)
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/rich_presence.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/rich_presence.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/settings_base.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/settings_base.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/svp_integration.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/svp_integration.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/syncplay.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/syncplay.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/systray.png` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/systray.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/thumbfast.lua` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/thumbfast.lua`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/timeline.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/timeline.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/trickplay-osc.lua` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay-osc.lua`

 * *Files 2% similar despite different names*

```diff
@@ -2233,21 +2233,20 @@
                 end
             end
         end
     else
         reset_margins()
     end
 
-    utils.shared_script_property_set("osc-margins",
-        string.format("%f,%f,%f,%f", margins.l, margins.r, margins.t, margins.b))
+    mp.set_property("user-data/osc-margins", string.format("%f,%f,%f,%f", margins.l, margins.r, margins.t, margins.b))
 end
 
 function shutdown()
     reset_margins()
-    utils.shared_script_property_set("osc-margins", nil)
+    mp.set_property("user-data/osc-margins", nil)
 end
 
 --
 -- Other important stuff
 --
 
 
@@ -2903,15 +2902,15 @@
         -- END patch add thumbnails
     else
         msg.warn("Ignoring unknown visibility mode '" .. mode .. "'")
         return
     end
 
     user_opts.visibility = mode
-    utils.shared_script_property_set("osc-visibility", mode)
+    mp.set_property("user-data/osc-visibility", mode)
 
     if not no_osd and tonumber(mp.get_property("osd-level")) >= 1 then
         mp.osd_message("OSC visibility: " .. mode)
     end
 
     -- Reset the input state on a mode change. The input state will be
     -- recalculated on the next render cycle, except in 'never' mode where it
@@ -2935,15 +2934,15 @@
 
     if mode == "yes" then
         user_opts.idlescreen = true
     else
         user_opts.idlescreen = false
     end
 
-    utils.shared_script_property_set("osc-idlescreen", mode)
+    mp.set_property("user-data/osc-idlescreen", mode)
 
     if not no_osd and tonumber(mp.get_property("osd-level")) >= 1 then
         mp.osd_message("OSC logo visibility: " .. tostring(mode))
     end
 
     request_tick()
 end
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/trickplay.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,85 +46,70 @@
             try:
                 log.info("Collecting trickplay images...")
 
                 if not self.player.has_video():
                     continue
 
                 video = self.player.get_video()
-                if settings.thumbnail_jellyscrub:
-                    try:
-                        data = video.get_bif(settings.thumbnail_preferred_size)
+                try:
+                    data = video.get_bif(settings.thumbnail_preferred_size)
+                    if not self.player.has_video() or video != self.player.get_video():
+                        # Video changed while we were getting the bif file
+                        continue
+
+                    if data:
+                        with open(img_file, "wb") as fh:
+                            img_count = math.ceil(
+                                data["ThumbnailCount"]
+                                / data["TileWidth"]
+                                / data["TileHeight"]
+                            )
+                            bifdecode.decompress_tiles(
+                                data["Width"],
+                                data["Height"],
+                                data["TileWidth"],
+                                data["TileHeight"],
+                                data["ThumbnailCount"],
+                                video.get_hls_tile_images(data["Width"], img_count),
+                                fh,
+                            )
+
+                        bif_meta = {
+                            "count": data["ThumbnailCount"],
+                            "multiplier": data["Interval"],
+                            "width": data["Width"],
+                            "height": data["Height"],
+                        }
+
                         if (
                             not self.player.has_video()
                             or video != self.player.get_video()
                         ):
-                            # Video changed while we were getting the bif file
+                            # Video changed while we were decompressing the bif file
                             continue
 
-                        if data:
-                            if type(data) is not dict:
-                                bif = bifdecode.decode(data)
-
-                                with open(img_file, "wb") as fh:
-                                    bif_meta = bifdecode.decompress_bif(
-                                        bif["images"], fh
-                                    )
-                                    bif_meta["multiplier"] = bif["multiplier"]
-                            else:
-                                with open(img_file, "wb") as fh:
-                                    img_count = math.ceil(
-                                        data["TileCount"]
-                                        / data["TileWidth"]
-                                        / data["TileHeight"]
-                                    )
-                                    bifdecode.decompress_tiles(
-                                        data["Width"],
-                                        data["Height"],
-                                        data["TileWidth"],
-                                        data["TileHeight"],
-                                        data["TileCount"],
-                                        video.get_hls_tile_images(
-                                            data["Width"], img_count
-                                        ),
-                                        fh,
-                                    )
-
-                                bif_meta = {
-                                    "count": data["TileCount"],
-                                    "multiplier": data["Interval"],
-                                    "width": data["Width"],
-                                    "height": data["Height"],
-                                }
-
-                            if (
-                                not self.player.has_video()
-                                or video != self.player.get_video()
-                            ):
-                                # Video changed while we were decompressing the bif file
-                                continue
-
-                            self.player.script_message(
-                                "shim-trickplay-bif",
-                                str(bif_meta["count"]),
-                                str(bif_meta["multiplier"]),
-                                str(bif_meta["width"]),
-                                str(bif_meta["height"]),
-                                img_file,
-                            )
-                            log.info(
-                                f"Collected {bif_meta['count']} bif preview images"
-                            )
-                            continue
-                        else:
-                            log.warning("No bif file available")
-                    except:
-                        log.error(
-                            "Could not get bif file. Do you have the plugin installed?",
-                            exc_info=True,
+                        self.player.script_message(
+                            "shim-trickplay-bif",
+                            str(bif_meta["count"]),
+                            str(bif_meta["multiplier"]),
+                            str(bif_meta["width"]),
+                            str(bif_meta["height"]),
+                            img_file,
+                        )
+                        log.info(
+                            f"Collected {bif_meta['count']} trickplay preview images"
                         )
+                        continue
+                    else:
+                        log.warning("No trickplay data available")
+                except:
+                    log.error(
+                        "Could not get trickplay data.",
+                        exc_info=True,
+                    )
 
                 chapter_data = video.get_chapters()
 
                 if chapter_data is None or len(chapter_data) == 0:
                     log.info("No chapters available")
                     continue
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/update_check.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/update_check.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/utils.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -107,17 +107,17 @@
         if is_remote:
             video_bitrate = settings.remote_kbps
         else:
             video_bitrate = settings.local_kbps
 
     if settings.force_video_codec:
         transcode_codecs = settings.force_video_codec
-    elif settings.allow_transcode_to_h265:
+    elif settings.allow_transcode_to_h265 and not settings.transcode_hevc:
         transcode_codecs = "h264,h265,hevc,mpeg4,mpeg2video"
-    elif settings.prefer_transcode_to_h265:
+    elif settings.prefer_transcode_to_h265 and not settings.transcode_hevc:
         transcode_codecs = "h265,hevc,h264,mpeg4,mpeg2video"
     else:
         transcode_codecs = "h264,mpeg4,mpeg2video"
 
     if settings.force_audio_codec:
         audio_transcode_codecs = settings.force_audio_codec
     else:
@@ -214,14 +214,76 @@
                         "Property": "VideoRangeType",
                         "Value": "SDR",
                     }
                 ],
             }
         )
 
+    if settings.transcode_hevc:
+        profile["CodecProfiles"].append(
+            {
+                "Type": "Video",
+                "Codec": "hevc",
+                "Conditions": [
+                    {
+                        "Condition": "Equals",
+                        "Property": "Width",
+                        "Value": "0",
+                    }
+                ],
+            }
+        )
+        profile["CodecProfiles"].append(
+            {
+                "Type": "Video",
+                "Codec": "h265",
+                "Conditions": [
+                    {
+                        "Condition": "Equals",
+                        "Property": "Width",
+                        "Value": "0",
+                    }
+                ],
+            }
+        )
+
+    if settings.transcode_av1:
+        profile["CodecProfiles"].append(
+            {
+                "Type": "Video",
+                "Codec": "av1",
+                "Conditions": [
+                    {
+                        "Condition": "Equals",
+                        "Property": "Width",
+                        "Value": "0",
+                    }
+                ],
+            }
+        )
+
+    if settings.transcode_4k:
+        profile["CodecProfiles"].append(
+            {
+                "Type": "Video",
+                "Conditions": [
+                    {
+                        "Condition": "LessThanEqual",
+                        "Property": "Width",
+                        "Value": "1920",
+                    },
+                    {
+                        "Condition": "LessThanEqual",
+                        "Property": "Height",
+                        "Value": "1080",
+                    },
+                ],
+            }
+        )
+
     if settings.always_transcode or force_transcode:
         profile["DirectPlayProfiles"] = []
 
     if is_tv:
         profile["TranscodingProfiles"].insert(
             0,
             {
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/video_profile.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/video_profile.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim/win_utils.py` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/win_utils.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/PKG-INFO` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,698 +1,701 @@
 Metadata-Version: 2.1
 Name: jellyfin-mpv-shim
-Version: 2.6.0
+Version: 2.7.0
 Summary: Cast media from Jellyfin Mobile and Web apps to MPV.
 Home-page: https://github.com/jellyfin/jellyfin-mpv-shim
-Author: Ian Walton
-Author-email: iwalton3@gmail.com
+Author: Izzie Walton
+Author-email: izzie@iwalton.com
 License: GPLv3
-Description: # Jellyfin MPV Shim
-        
-        [![Current Release](https://img.shields.io/github/release/jellyfin/jellyfin-mpv-shim.svg)](https://github.com/jellyfin/jellyfin-mpv-shim/releases)
-        [![PyPI](https://img.shields.io/pypi/v/jellyfin-mpv-shim)](https://pypi.org/project/jellyfin-mpv-shim/)
-        [![Translation Status](https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-mpv-shim/svg-badge.svg)](https://translate.jellyfin.org/projects/jellyfin/jellyfin-mpv-shim/)
-        [![Code Stype](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        Jellyfin MPV Shim is a cross-platform cast client for Jellyfin.
-        It has support for all your advanced media files without transcoding, as well as tons of
-        features which set it apart from other multimedia clients:
-        
-         - Direct play most media using MPV.
-         - Watch videos with friends using SyncPlay.
-         - Offers a shim mode which runs in the background.
-         - The Jellyfin mobile apps can fully control the client.
-         - [Reconfigure subtitles](https://github.com/jellyfin/jellyfin-mpv-shim#menu) for an entire season at once.
-         - Supports all of the [MPV keyboard shortcuts](https://github.com/jellyfin/jellyfin-mpv-shim#keyboard-shortcuts).
-         - Enhance your video with [Shader Packs](https://github.com/jellyfin/jellyfin-mpv-shim#menu) and [SVP Integration](https://github.com/jellyfin/jellyfin-mpv-shim#svp-integration).
-         - Optionally share your media activity with friends using Discord Rich Presence.
-         - Most features, as well as MPV itself, [can be extensively configured](https://github.com/jellyfin/jellyfin-mpv-shim#configuration).
-         - You can configure the player to use an [external MPV player](https://github.com/jellyfin/jellyfin-mpv-shim#external-mpv) of your choice.
-         - Enable a chromecast-like experience with [Display Mirroring](https://github.com/jellyfin/jellyfin-mpv-shim#display-mirroring).
-         - You can [trigger commands to run](https://github.com/jellyfin/jellyfin-mpv-shim#shell-command-triggers) when certain events happen.
-        
-        To learn more, keep reading. This README explains everything, including [configuration](https://github.com/jellyfin/jellyfin-mpv-shim#configuration), [tips & tricks](https://github.com/jellyfin/jellyfin-mpv-shim#tips-and-tricks), and [development information](https://github.com/jellyfin/jellyfin-mpv-shim#development).
-        
-        ## Getting Started
-        
-        If you are on Windows, simply [download the binary](https://github.com/jellyfin/jellyfin-mpv-shim/releases).
-        If you are using Linux, you can [install via flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim) or [install via pip](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#linux-installation). If you are on macOS, see the [macOS Installation](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#osx-installation)
-        section below.
-        
-        To use the client, simply launch it and log into your Jellyfin server. You’ll need to enter the
-        URL to your server, for example `http://server_ip:8096` or `https://secure_domain`. Make sure to
-        include the subdirectory and port number if applicable. You can then cast your media
-        from another Jellyfin application.
-        
-        The application runs with a notification icon by default. You can use this to edit the server settings,
-        view the application log, open the config folder, and open the application menu. Unlike Plex MPV Shim,
-        authorization tokens for your server are stored on your device, but you are able to cast to the player
-        regardless of location.
-        
-        Note: Due to the huge number of questions and issues that have been submitted about URLs, I now tolerate
-        bare IP addresses and not specifying the port by default. If you want to connect to port 80 instead of
-        8096, you must add the `:80` to the URL because `:8096` is now the default.
-        
-        ## Limitations
-        
-         - Music playback and Live TV are not supported.
-         - The client can’t be shared seamlessly between multiple users on the same server. ([Link to issue.](https://features.jellyfin.org/posts/319/mark-device-as-shared))
-        
-        ### Known Issues
-        
-        Please also note that the on-screen controller for MPV (if available) cannot change the
-        audio and subtitle track configurations for transcoded media. It also cannot load external
-        subtitles. You must either [use the menu](https://github.com/jellyfin/jellyfin-mpv-shim#menu) or the application you casted from.
-        
-        Please note the following issues with controlling SyncPlay:
-         - If you attempt to join a SyncPlay group when casting to MPV Shim, it will play the media but it will not activate SyncPlay.
-             - You can, however, proceed to activate SyncPlay [using the menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
-         - If you would like to create a group or join a group for currently playing media, [use menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
-         - SyncPlay as of 10.7.0 is new and kind of fragile. You may need to rejoin or even restart the client. Please report any issues you find.
-        
-        Music playback sort-of works, but repeat, shuffle, and gapless playback have not been implemented and
-        would require major changes to the application to properly support, as it was built for video.
-        
-        The shader packs feature is sensitive to graphics hardware. It may simply just not work on your computer.
-        You may be able to use the log files to get some more diagnostic information. If you're really unlucky,
-        you'll have to disable the feature by pressing `k` to restore basic functionality.
-        If you find the solution for your case, *please* send me any information you can provide, as every test case helps.
-        
-        ## Advanced Features
-        
-        ### Menu
-        
-        To open the menu, press **c** on your computer or use the navigation controls
-        in the mobile/web app.
-        
-        The menu enables you to:
-         - Adjust video transcoding quality.
-         - Change the default transcoder settings.
-         - Change subtitles or audio, while knowing the track names.
-         - Change subtitles or audio for an entire series at once.
-         - Mark the media as unwatched and quit.
-         - Enable and disable SyncPlay.
-         - Configure shader packs and SVP profiles.
-         - Take screenshots.
-        
-        On your computer, use the mouse or arrow keys, enter, and escape to navigate.
-        On your phone, use the arrow buttons, ok, back, and home to navigate.
-        
-        ### Shader Packs 
-        
-        Shader packs are a recent feature addition that allows you to easily use advanced video
-        shaders and video quality settings. These usually require a lot of configuration to use,
-        but MPV Shim's default shader pack comes with [FSRCNNX](https://github.com/igv/FSRCNN-TensorFlow)
-        and [Anime4K](https://github.com/bloc97/Anime4K) preconfigured. Try experimenting with video
-        profiles! It may greatly improve your experience.
-        
-        Shader Packs are ready to use as of the most recent MPV Shim version. To use, simply
-        navigate to the **Video Playback Profiles** option and select a profile.
-        
-        For details on the shader settings, please see [default-shader-pack](https://github.com/iwalton3/default-shader-pack).
-        If you would like to customize the shader pack, there are details in the configuration section.
-        
-        ### SVP Integration
-        
-        SVP integration allows you to easily configure SVP support, change profiles, and enable/disable
-        SVP without having to exit the player. It is not enabled by default, please see the configuration
-        instructions for instructions on how to enable it.
-        
-        ### Display Mirroring
-        
-        This feature allows media previews to show on your display before you cast the media,
-        similar to Chromecast. It is not enabled by default. To enable it, do one of the following:
-        
-         - Using the systray icon, click "Application Menu". Go to preferences and enable display mirroring.
-             - Use the arrow keys, escape, and enter to navigate the menu.
-         - Cast media to the player and press `c`. Go to preferences and enable display mirroring.
-         - In the config file (see below), change `display_mirroring` to `true`.
-        
-        Then restart the application for the change to take effect. To quit the application on Windows with
-        display mirroring enabled, press Alt+F4.
-        
-        ### Keyboard Shortcuts
-        
-        This program supports most of the [keyboard shortcuts from MPV](https://mpv.io/manual/stable/#interactive-control). The custom keyboard shortcuts are:
-        
-         - < > to skip episodes
-         - q to close player
-         - w to mark watched and skip
-         - u to mark unwatched and quit
-         - c to open the menu
-         - k disable shader packs
-        
-        Here are the notable MPV keyboard shortcuts:
-        
-         - space - Pause/Play
-         - left/right - Seek by 5 seconds
-         - up/down - Seek by 1 minute
-         - s - Take a screenshot
-         - S - Take a screenshot without subtitles
-         - f - Toggle fullscreen
-         - ,/. - Seek by individual frames
-         - \[/\] - Change video speed by 10%
-         - {/} - Change video speed by 50%
-         - backspace - Reset speed
-         - m - Mute
-         - d - Enable/disable deinterlace
-         - Ctrl+Shift+Left/Right - Adjust subtitle delay.
-        
-        ## Configuration
-        
-        The configuration file is located in different places depending on your platform. You can also open the
-        configuration folder using the systray icon if you are using the shim version. When you launch the program
-        on Linux or macOS from the terminal, the location of the config file will be printed. The locations are:
-         - Windows - `%appdata%\jellyfin-mpv-shim\conf.json`
-         - Linux - `~/.config/jellyfin-mpv-shim/conf.json`
-         - Linux (Flatpak) - `~/.var/app/com.github.iwalton3.jellyfin-mpv-shim/config/jellyfin-mpv-shim/conf.json`
-         - macOS - `~/Library/Application Support/jellyfin-mpv-shim/conf.json`
-         - CygWin - `~/.config/jellyfin-mpv-shim/conf.json`
-        
-        You can specify a custom configuration folder with the `--config` option.
-        
-        ### Transcoding
-        
-        You can adjust the basic transcoder settings via the menu.
-        
-        - `always_transcode` - This will tell the client to always transcode. Default: `false`
-            - This may be useful if you are using limited hardware that cannot handle advanced codecs.
-            - Please note that Jellyfin may still direct play files that meet the transcode profile
-              requirements. There is nothing I can do on my end to disable this, but you can reduce
-              the bandwidth setting to force a transcode.
-        - `transcode_hdr` - Force transcode HDR videos to SDR. Default: `false`
-        - `transcode_dolby_vision` - Force transcode Dolby Vision videos to SDR. Default: `true`
-            - If your computer can handle it, you can get tone mapping to work for this using `vo=gpu-next`.
-            - Note that `vo=gpu-next` is considered experimental by MPV at this time.
-        - `transcode_hi10p` - Force transcode 10 bit color videos to 8 bit color. Default: `false`
-        - `remote_kbps` - Bandwidth to permit for remote streaming. Default: `10000`
-        - `local_kbps` - Bandwidth to permit for local streaming. Default: `2147483`
-        - `direct_paths` - Play media files directly from the SMB or NFS source. Default: `false`
-            - `remote_direct_paths` - Apply this even when the server is detected as remote. Default: `false`
-        - `allow_transcode_to_h265` - Allow the server to transcode media *to* `hevc`. Default: `false`
-            - If you enable this, it'll allow remuxing to HEVC but it'll also break force transcoding of Dolby Vision and HDR content if those settings are used. (See [this bug](https://github.com/jellyfin/jellyfin/issues/9313).)
-        - `prefer_transcode_to_h265` - Requests the server to transcode media *to* `hevc` as the default. Default: `false`
-        - `transcode_warning` - Display a warning the first time media transcodes in a session. Default: `true`
-        - `force_video_codec` - Force a specified video codec to be played. Default: `null`
-            - This can be used in tandem with `always_transcode` to force the client to transcode into
-              the specified format.
-            - This may have the same limitations as `always_transcode`.
-            - This will override `transcode_to_h265`, `transcode_h265` and `transcode_hi10p`.
-        - `force_audio_codec` - Force a specified audio codec to be played. Default: `null`
-            - This can be used in tandeom with `always_transcode` to force the client to transcode into
-              the specified format.
-            - This may have the same limitations as `always_transcode`.
-        
-        ### Features
-        
-        You can use the config file to enable and disable features.
-        
-         - `fullscreen` - Fullscreen the player when starting playback. Default: `true`
-         - `enable_gui` - Enable the system tray icon and GUI features. Default: `true`
-         - `enable_osc` - Enable the MPV on-screen controller. Default: `true`
-            - It may be useful to disable this if you are using an external player that already provides a user interface.
-         - `media_key_seek` - Use the media next/prev keys to seek instead of skip episodes. Default: `false`
-         - `use_web_seek` - Use the seek times set in Jellyfin web for arrow key seek. Default: `false`
-         - `display_mirroring` - Enable webview-based display mirroring (content preview). Default: `false`
-         - `screenshot_menu` - Allow taking screenshots from menu. Default: `true`
-         - `check_updates` - Check for updates via GitHub. Default: `true`
-            - This requests the GitHub releases page and checks for a new version.
-            - Update checks are performed when playing media, once per day.
-         - `notify_updates` - Display update notification when playing media. Default: `true`
-            - Notification will only display once until the application is restarted. 
-         - `discord_presence` - Enable Discord rich presence support. Default: `false`
-         - `menu_mouse` - Enable mouse support in the menu. Default: `true`
-             - This requires MPV to be compiled with lua support.
-        
-        ### Shell Command Triggers
-        
-        You can execute shell commands on media state using the config file:
-        
-         - `media_ended_cmd` - When all media has played.
-         - `pre_media_cmd` - Before the player displays. (Will wait for finish.)
-         - `stop_cmd` - After stopping the player.
-         - `idle_cmd` - After no activity for `idle_cmd_delay` seconds.
-         - `idle_when_paused` - Consider the player idle when paused. Default: `false`
-         - `stop_idle` - Stop the player when idle. (Requires `idle_when_paused`.) Default: `false`
-         - `play_cmd` - After playback starts.
-         - `idle_ended_cmd` - After player stops being idle.
-        
-        ### Subtitle Visual Settings
-        
-        These settings may not works for some subtitle codecs or if subtitles are being burned in
-        during a transcode. You can configure custom styled subtitle settings through the MPV config file.
-        
-         - `subtitle_size` - The size of the subtitles, in percent. Default: `100`
-         - `subtitle_color` - The color of the subtitles, in hex. Default: `#FFFFFFFF`
-         - `subtitle_position` - The position (top, bottom, middle). Default: `bottom`
-        
-        ### External MPV
-        
-        The client now supports using an external copy of MPV, including one that is running prior to starting
-        the client. This may be useful if your distribution only provides MPV as a binary executable (instead
-        of as a shared library), or to connect to MPV-based GUI players. Please note that SMPlayer exhibits
-        strange behaviour when controlled in this manner. External MPV is currently the only working backend
-        for media playback on macOS.
-        
-        - `mpv_ext` - Enable usage of the external player by default. Default: `false`
-            - The external player may still be used by default if `libmpv1` is not available.
-        - `mpv_ext_path` - The path to the `mpv` binary to use. By default it uses the one in the PATH. Default: `null`
-            - If you are using Windows, make sure to use two backslashes. Example: `C:\\path\\to\\mpv.exe`
-        - `mpv_ext_ipc` - The path to the socket to control MPV. Default: `null`
-            - If unset, the socket is a randomly selected temp file.
-            - On Windows, this is just a name for the socket, not a path like on Linux.
-        - `mpv_ext_start` - Start a managed copy of MPV with the client. Default: `true`
-            - If not specified, the user must start MPV prior to launching the client.
-            - MPV must be launched with `--input-ipc-server=[value of mpv_ext_ipc]`.
-        - `mpv_ext_no_ovr` - Disable built-in mpv configuration files and use user defaults.
-            - Please note that some scripts and settings, such as ones to keep MPV open, may break
-              functionality in MPV Shim.
-        
-        ### Keyboard Shortcuts
-        
-        You can reconfigure the custom keyboard shortcuts. You can also set them to `null` to disable the shortcut. Please note that disabling keyboard shortcuts may make some features unusable. Additionally, if you remap `q`, using the default shortcut will crash the player.
-        
-         - `kb_stop` - Stop playback and close MPV. (Default: `q`)
-         - `kb_prev` - Go to the previous video. (Default: `<`)
-         - `kb_next` - Go to the next video. (Default: `>`)
-         - `kb_watched` - Mark the video as watched and skip. (Default: `w`)
-         - `kb_unwatched` - Mark the video as unwatched and quit. (Default: `u`)
-         - `kb_menu` - Open the configuration menu. (Default: `c`)
-         - `kb_menu_esc` - Leave the menu. Exits fullscreen otherwise. (Default: `esc`)
-         - `kb_menu_ok` - "ok" for menu. (Default: `enter`)
-         - `kb_menu_left` - "left" for menu. Seeks otherwise. (Default: `left`)
-         - `kb_menu_right` - "right" for menu. Seeks otherwise. (Default: `right`)
-         - `kb_menu_up` - "up" for menu. Seeks otherwise. (Default: `up`)
-         - `kb_menu_down` - "down" for menu. Seeks otherwise. (Default: `down`)
-         - `kb_pause` - Pause. Also "ok" for menu. (Default: `space`)
-         - `kb_fullscreen` - Toggle fullscreen. (Default: `f`)
-         - `kb_debug` - Trigger `pdb` debugger. (Default: `~`)
-         - `kb_kill_shader` - Disable shader packs. (Default: `k`)
-         - `seek_up` - Time to seek for "up" key. (Default: `60`)
-         - `seek_down` - Time to seek for "down" key. (Default: `-60`)
-         - `seek_right` - Time to seek for "right" key. (Default: `5`)
-         - `seek_left` - Time to seek for "left" key. (Default: `-5`)
-         - `media_keys` - Enable binding of MPV to media keys. Default: `true`
-         - `seek_v_exact` - Use exact seek for up/down keys. Default: `false`
-         - `seek_h_exact` - Use exact seek for left/right keys. Default: `false`
-        
-        ### Shader Packs
-        
-        Shader packs allow you to import MPV config and shader presets into MPV Shim and easily switch
-        between them at runtime through the built-in menu. This enables easy usage and switching of
-        advanced MPV video playback options, such as video upscaling, while being easy to use.
-        
-        If you select one of the presets from the shader pack, it will override some MPV configurations
-        and any shaders manually specified in `mpv.conf`. If you would like to customize the shader pack,
-        use `shader_pack_custom`.
-        
-         - `shader_pack_enable` - Enable shader pack. (Default: `true`)
-         - `shader_pack_custom` - Enable to use a custom shader pack. (Default: `false`)
-            - If you enable this, it will copy the default shader pack to the `shader_pack` config folder.
-            - This initial copy will only happen if the `shader_pack` folder didn't exist.
-            - This shader pack will then be used instead of the built-in one from then on.
-         - `shader_pack_remember` - Automatically remember the last used shader profile. (Default: `true`)
-         - `shader_pack_profile` - The default profile to use. (Default: `null`)
-            - If you use `shader_pack_remember`, this will be updated when you set a profile through the UI.
-         - `shader_pack_subtype` - The profile group to use. The default pack contains `lq` and `hq` groups. Use `hq` if you have a fancy graphics card.
-        
-        ### Trickplay Thumbnails
-        
-        MPV will automatically display thumbnail previews. By default it uses the Jellyfin chapter images
-        but it can also use JellyScrub as the source. Please note that this feature will download and
-        uncompress all of the chapter images before it becomes available for a video. For a 4 hour movie this
-        causes disk usage of about 250 MB, but for the average TV episode it is around 40 MB. It also requires
-        overriding the default MPV OSC, which may conflict with some custom user script. Trickplay is compatible
-        with any OSC that uses [thumbfast](https://github.com/po5/thumbfast), as I have added a [compatibility layer](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/jellyfin_mpv_shim/thumbfast.lua).
-        
-         - `thumbnail_enable` - Enable thumbnail feature. (Default: `true`)
-         - `thumbnail_jellyscrub` - Use JellyScrub as the thumbnail source instead of chapter images. (Default: `false`)
-         - `thumbnail_osc_builtin` - Disable this setting if you want to use your own custom osc but leave trickplay enabled. (Default: `true`)
-         - `thumbnail_preferred_size` - The ideal size for thumbnails. (Default: `320`)
-        
-        ### SVP Integration
-        
-        To enable SVP integration, set `svp_enable` to `true` and enable "External control via HTTP" within SVP
-        under Settings > Control options. Adjust the `svp_url` and `svp_socket` settings if needed.
-        
-         - `svp_enable` - Enable SVP integration. (Default: `false`)
-         - `svp_url` - URL for SVP web API. (Default: `http://127.0.0.1:9901/`)
-         - `svp_socket` - Custom MPV socket to use for SVP.
-            - Default on Windows: `mpvpipe`
-            - Default on other platforms: `/tmp/mpvsocket`
-        
-        Currently on Windows the built-in MPV does not work with SVP. You must download MPV yourself.
-        
-         - Download the latest MPV build [from here](https://sourceforge.net/projects/mpv-player-windows/files/64bit/).
-         - Follow the [vapoursynth instructions](https://github.com/shinchiro/mpv-winbuild-cmake/wiki/Setup-vapoursynth-for-mpv).
-             - Make sure to use the latest Python, not Python 3.7.
-         - In the config file, set `mpv_ext` to `true` and `mpv_ext_path` to the path to `mpv.exe`.
-             - Make sure to use two backslashes per each backslash in the path.
-        
-        ### SyncPlay
-        
-        You probably don't need to change these, but they are defined here in case you
-        need to.
-        
-         - `sync_max_delay_speed` - Delay in ms before changing video speed to sync playback. Default: `50`
-         - `sync_max_delay_skip` - Delay in ms before skipping through the video to sync playback. Default: `300`
-         - `sync_method_thresh` - Delay in ms before switching sync method. Default: `2000`
-         - `sync_speed_time` - Duration in ms to change playback speed. Default: `1000`
-         - `sync_speed_attempts` - Number of attempts before speed changes are disabled. Default: `3`
-         - `sync_attempts` - Number of attempts before disabling sync play. Default: `5`
-         - `sync_revert_seek` - Attempt to revert seek via MPV OSC. Default: `true`
-             - This could break if you use revert-seek markers or scripts that use it.
-         - `sync_osd_message` - Write syncplay status messages to OSD. Default: `true`
-        
-        ### Debugging
-        
-        These settings assist with debugging. You will often be asked to configure them when reporting an issue.
-        
-         - `log_decisions` - Log the full media decisions and playback URLs. Default: `false`
-         - `mpv_log_level` - Log level to use for mpv. Default: `info`
-            - Options: fatal, error, warn, info, v, debug, trace
-         - `sanitize_output` - Prevent the writing of server auth tokens to logs. Default: `true`
-         - `write_logs` - Write logs to the config directory for debugging. Default: `false`
-        
-        ### Other Configuration Options
-        
-        Other miscellaneous configuration options. You probably won't have to change these.
-        
-         - `player_name` - The name of the player that appears in the cast menu. Initially set from your hostname.
-         - `client_uuid` - The identifier for the client. Set to a random value on first run.
-         - `audio_output` - Currently has no effect. Default: `hdmi`
-         - `playback_timeout` - Timeout to wait for MPV to start loading video in seconds. Default: `30`
-            - If you're hitting this, it means files on your server probably got corrupted or deleted.
-            - It could also happen if you try to play an unsupported video format. These are rare.
-         - `lang` - Allows overriding system locale. (Enter a language code.) Default: `null`
-            - MPV Shim should use your OS language by default.
-         - `ignore_ssl_cert` - Ignore SSL certificates. Default: `false`
-            - Please consider getting a certificate from Let's Encrypt instead of using this.
-         - `connect_retry_mins` - Number of minutes to retry connecting before showing login window. Default: `0`
-            - This only applies for when you first launch the program.
-         - `lang_filter` - Limit track selection to desired languages. Default: `und,eng,jpn,mis,mul,zxx`
-            - Note that you need to turn on the options below for this to actually do something.
-            - If you remove `und` from the list, it will ignore untagged items.
-            - Languages are typically in [ISO 639-2/B](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes),
-              but if you have strange files this may not be the case.
-         - `lang_filter_sub` - Apply the language filter to subtitle selection. Default: `False`
-         - `lang_filter_audio` - Apply the language filter to audio selection. Default: `False`
-         - `screenshot_dir` - Sets where screenshots go.
-            - Default is the desktop on Windows and unset (current directory) on other platforms.
-         - `force_set_played` - This forcibly sets items as played when MPV playback finished.
-            - If you have files with malformed timestamps that don't get marked as played, enable this.
-         - `raise_mpv` - Windows only. Disable this if you are fine with MPV sometimes appearing behind other windows when playing.
-         - `health_check_interval` - The number of seconds between each client health check. Null disables it. Default: `300`
-        
-        ### Skip Intro Support
-        
-        This functionality is considered experimental and requires the third-party [SkipIntro server plugin](https://github.com/ConfusedPolarBear/intro-skipper). It works the same ways as it did on MPV Shim for Plex.
-        
-         - `skip_intro_always` - Always skip intros, without asking. Default: `false`
-         - `skip_intro_prompt` - Prompt to skip intro via seeking. Default: `false`
-        
-        ### MPV Configuration
-        
-        You can configure mpv directly using the `mpv.conf` and `input.conf` files. (It is in the same folder as `conf.json`.)
-        This may be useful for customizing video upscaling, keyboard shortcuts, or controlling the application
-        via the mpv IPC server.
-        
-        ### Authorization
-        
-        The `cred.json` file contains the authorization information. If you are having problems with the client,
-        such as the Now Playing not appearing or want to delete a server, you can delete this file and add the
-        servers again.
-        
-        ## Tips and Tricks
-        
-        Various tips have been found that allow the media player to support special
-        functionality, albeit with more configuration required.
-        
-        ### Open on Specific Monitor (#19)
-        
-        Please note: Edits to the `mpv.conf` will not take effect until you restart the application. You can open the config directory by using the menu option in the system tray icon.
-        
-        **Option 1**: Select fullscreen output screen through MPV.
-        Determine which screen you would like MPV to show up on.
-         - If you are on Windows, right click the desktop and select "Display Settings". Take the monitor number and subtract one.
-         - If you are on Linux, run `xrandr`. The screen number is the number you want. If there is only one proceed to **Option 2**.
-        
-        Add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration), replacing `0` with the number from the previous step:
-        ```
-        fs=yes
-        fs-screen=0
-        ```
-        
-        **Option 2**: (Linux Only) If option 1 does not work, both of your monitors are likely configured as a single "screen".
-        
-        Run `xrandr`. It should look something like this:
-        
-        ```
-        Screen 0: minimum 8 x 8, current 3520 x 1080, maximum 16384 x 16384
-        VGA-0 connected 1920x1080+0+0 (normal left inverted right x axis y axis) 521mm x 293mm
-           1920x1080     60.00*+
-           1680x1050     59.95  
-           1440x900      59.89  
-           1280x1024     75.02    60.02  
-           1280x960      60.00  
-           1280x800      59.81  
-           1280x720      60.00  
-           1152x864      75.00  
-           1024x768      75.03    70.07    60.00  
-           800x600       75.00    72.19    60.32    56.25  
-           640x480       75.00    59.94  
-        LVDS-0 connected 1600x900+1920+180 (normal left inverted right x axis y axis) 309mm x 174mm
-           1600x900      59.98*+
-        ```
-        
-        If you want MPV to open on VGA-0 for instance, add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration):
-        ```
-        fs=yes
-        geometry=1920x1080+0+0
-        ```
-        **Option 3**: (Linux Only) If your window manager supports it, you can tell the window manager to always open on a specific screen.
-        
-         - For OpenBox: https://forums.bunsenlabs.org/viewtopic.php?id=1199
-         - For i3: https://unix.stackexchange.com/questions/96798/i3wm-start-applications-on-specific-workspaces-when-i3-starts/363848#363848
-        
-        ### Control Volume with Mouse Wheel (#48)
-        
-        Add the following to `input.conf`:
-        ```
-        WHEEL_UP add volume 5
-        WHEEL_DOWN add volume -5
-        ```
-        
-        ### MPRIS Plugin (#54)
-        
-        Set `mpv_ext` to `true` in the config. Add `script=/path/to/mpris.so` to `mpv.conf`.
-        
-        ### Run Multiple Instances (#45)
-        
-        You can pass `--config /path/to/folder` to run another copy of the player. Please 
-        note that running multiple copies of the desktop client is currently not supported. 
-        
-        ### Audio Passthrough
-        
-        You can edit `mpv.conf` to support audio passthrough. A [user on Reddit](https://reddit.com/r/jellyfin/comments/fru6xo/new_cross_platform_desktop_client_jellyfin_mpv/fns7vyp) had luck with this config:
-        ```
-        audio-spdif=ac3,dts,eac3 # (to use the passthrough to receiver over hdmi)
-        audio-channels=2 # (not sure this is necessary, but i keep it in because it works)
-        af=scaletempo,lavcac3enc=yes:640:3 # (for aac 5.1 tracks to the receiver)
-        ```
-        
-        ### MPV Crashes with "The sub-scale option must be a floating point number or a ratio"
-        
-        Run the jellyfin-mpv-shim program with LC_NUMERIC=C.
-        
-        ### Use with gnome-mpv/celluloid (#61)
-        
-        You can use `gnome-mpv` with MPV Shim, but you must launch `gnome-mpv` separately before MPV Shim. (`gnome-mpv` doesn't support the MPV command options directly.)
-        
-        Configure MPV Shim with the following options (leave the other ones):
-        ```json
-        {
-            "mpv_ext": true,
-            "mpv_ext_ipc": "/tmp/gmpv-socket",
-            "mpv_ext_path": null,
-            "mpv_ext_start": false,
-            "enable_osc": false
-        }
-        ```
-        Then within `gnome-mpv`, click the application icon (top left) > Preferences. Configure the following Extra MPV Options:
-        ```
-        --idle --input-ipc-server=/tmp/gmpv-socket
-        ```
-        
-        ### Heavy Memory Usage
-        
-        A problem has been identified where MPV can use a ton of RAM after media has been played,
-        and this RAM is not always freed when the player goes into idle mode. Some users have
-        found that using external MPV lessens the memory leak. To enable external MPV on Windows:
-        
-         - [Download a copy of MPV](https://sourceforge.net/projects/mpv-player-windows/files/64bit/)
-         - Unzip it with 7zip.
-         - Configure `mpv_ext` to `true`. (See the config section.)
-         - Configure `mpv_ext_path` to `C:\\replace\\with\\path\\to\\mpv.exe`. (Note usage of two `\\`.)
-         - Run the program and wait. (You'll probably have to use it for a while.)
-         - Let me know if the high memory usage is with `mpv.exe` or the shim itself.
-        
-        On Linux, the process is similar, except that you don't need to set the `mpv_ext_path` variable.
-        On macOS, external MPV is already the default and is the only supported player mode.
-        
-        In the long term, I may look into a method of terminating MPV when not in use. This will require
-        a lot of changes to the software. 
-        
-        ### Player Sizing (#91)
-        
-        MPV by default may force the window size to match the video aspect ratio, instead of allowing
-        resizing and centering the video accordingly. Add the following to `mpv.conf` to enable resizing
-        of the window freely, if desired:
-        ```
-        no-keepaspect-window
-        ```
-        
-        ## Development
-        
-        If you'd like to run the application without installing it, run `./run.py`.
-        The project is written entirely in Python 3. There are no closed-source
-        components in this project. It is fully hackable.
-        
-        The project is dependent on `python-mpv`, `python-mpv-jsonipc`, and `jellyfin-apiclient-python`. If you are
-        using Windows and would like mpv to be maximize properly, `pywin32` is also needed. The GUI
-        component uses `pystray` and `tkinter`, but there is a fallback cli mode. The mirroring dependencies
-        are `Jinja2` and `pywebview`, along with platform-specific dependencies. (See the installation and building
-        guides for details on platform-specific dependencies for display mirroring.)
-        
-        This project is based Plex MPV Shim, which is based on https://github.com/wnielson/omplex, which
-        is available under the terms of the MIT License. The project was ported to python3, modified to
-        use mpv as the player, and updated to allow all features of the remote control api for video playback.
-        
-        The Jellyfin API client comes from [Jellyfin for Kodi](https://github.com/jellyfin/jellyfin-kodi/tree/master/jellyfin_kodi).
-        The API client was originally forked for this project and is now a [separate package](https://github.com/iwalton3/jellyfin-apiclient-python).
-        
-        The css file for desktop mirroring is from [jellyfin-chromecast](https://github.com/jellyfin/jellyfin-chromecast/tree/5194d2b9f0120e0eb8c7a81fe546cb9e92fcca2b) and is subject to GPL v2.0.
-        
-        The shaders included in the shader pack are also available under verious open source licenses,
-        [which you can read about here](https://github.com/iwalton3/default-shader-pack/blob/master/LICENSE.md).
-        
-        ### Local Dev Installation
-        
-        If you are on Windows there are additional dependencies. Please see the Windows Build Instructions.
-        
-        1. Install the dependencies: `sudo pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
-            - If you run `./gen_pkg.sh --install`, it will also fetch these for you.
-        2. Clone this repository: `git clone https://github.com/jellyfin/jellyfin-mpv-shim`
-            - You can also download a zip build.
-        3. `cd` to the repository: `cd jellyfin-mpv-shim`
-        4. Run prepare script: `./gen_pkg.sh`
-            - To do this manually, download the web client, shader pack, and build the language files.
-        5. Ensure you have a copy of `libmpv1` or `mpv` available.
-        6. Install any platform-specific dependencies from the respective install tutorials.
-        7. You should now be able to run the program with `./run.py`. Installation is possible with `sudo pip3 install .`.
-            - You can also install the package with `./gen_pkg.sh --install`.
-        
-        ### Translation
-        
-        This project uses gettext for translation. The current template language file is `base.pot` in `jellyfin_mpv_shim/messages/`.
-        
-        To regenerate `base.pot` and update an existing translation with new strings:
-        ```bash
-        ./regen_pot.sh
-        ```
-        
-        To compile all `*.po` files to `*.mo`:
-        ```bash
-        ./gen_pkg.sh --skip-build
-        ```
-        
-        ## Linux Installation
-        
-        You can [install the software from flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim). The pip installation is less integrated but takes up less space if you're not already using flatpak.
-        
-        If you are on Linux, you can install via pip. You'll need [libmpv1](https://github.com/Kagami/mpv.js/blob/master/README.md#get-libmpv) or `mpv` installed.
-        ```bash
-        sudo pip3 install --upgrade jellyfin-mpv-shim
-        ```
-        If you would like the GUI and systray features, also install `pystray` and `tkinter`:
-        ```bash
-        sudo pip3 install pystray
-        sudo apt install python3-tk
-        ```
-        If you would like display mirroring support, install the mirroring dependencies:
-        ```bash
-        sudo apt install python3-jinja2 python3-webview
-        # -- OR --
-        sudo pip3 install jellyfin-mpv-shim[mirror]
-        sudo apt install gir1.2-webkit2-4.0
-        ```
-        Discord rich presence support:
-        ```bash
-        sudo pip3 install jellyfin-mpv-shim[discord]
-        ```
-        You can build mpv from source to get better codec support. Execute the following:
-        ```bash
-        sudo pip3 install --upgrade python-mpv
-        sudo apt install autoconf automake libtool libharfbuzz-dev libfreetype6-dev libfontconfig1-dev libx11-dev libxrandr-dev libvdpau-dev libva-dev mesa-common-dev libegl1-mesa-dev yasm libasound2-dev libpulse-dev libuchardet-dev zlib1g-dev libfribidi-dev git libgnutls28-dev libgl1-mesa-dev libsdl2-dev cmake wget python g++ libluajit-5.1-dev
-        git clone https://github.com/mpv-player/mpv-build.git
-        cd mpv-build
-        echo --enable-libmpv-shared > mpv_options
-        ./rebuild -j4
-        sudo ./install
-        sudo ldconfig
-        ```
-        
-        ## <h2 id="osx-installation">macOS Installation</h2>
-        Currently on macOS only the external MPV backend seems to be working. I cannot test on macOS, so please report any issues you find.
-        
-        To install the CLI version:
-        
-        1. Install brew. ([Instructions](https://brew.sh/))
-        2. Install python3 and mpv. `brew install python mpv`
-        3. Install jellyfin-mpv-shim. `pip3 install --upgrade jellyfin-mpv-shim`
-        4. Run `jellyfin-mpv-shim`.
-        
-        If you'd like to install the GUI version, you need a working copy of tkinter.
-        
-        1. Install pyenv. ([Instructions](https://medium.com/python-every-day/python-development-on-macos-with-pyenv-2509c694a808))
-        2. Install TK and mpv. `brew install tcl-tk mpv`
-        3. Install python3 with TK support. `FLAGS="-I$(brew --prefix tcl-tk)/include" pyenv install 3.8.1`
-        4. Set this python3 as the default. `pyenv global 3.8.1`
-        5. Install jellyfin-mpv-shim and pystray. `pip3 install --upgrade 'jellyfin-mpv-shim[gui]'`
-        6. Run `jellyfin-mpv-shim`.
-        
-        Display mirroring is not tested on macOS, but may be installable with 'pip3 install --upgrade 'jellyfin-mpv-shim[mirror]'`.
-        
-        ## Building on Windows
-        
-        There is a prebuilt version for Windows in the releases section. When
-        following these directions, please take care to ensure both the python
-        and libmpv libraries are either 64 or 32 bit. (Don't mismatch them.)
-        
-        If you'd like to build the installer, please install [Inno Setup](https://jrsoftware.org/isinfo.php) to build
-        the installer. If you'd like to build a 32 bit version, download the 32 bit version of mpv-1.dll and
-        copy it into a new folder called mpv32. You'll also need [WebBrowserInterop.x86.dll](https://github.com/r0x0r/pywebview/blob/master/webview/lib/WebBrowserInterop.x86.dll?raw=true).
-        You may also need to edit the batch file for 32 bit builds to point to the right python executable.
-        
-        1. Install Git for Windows. Open Git Bash and run `git clone https://github.com/jellyfin/jellyfin-mpv-shim; cd jellyfin-mpv-shim`.
-            - You can update the project later with `git pull`.
-        2. Install [Python3](https://www.python.org/downloads/) with PATH enabled. Install [7zip](https://ninite.com/7zip/).
-        3. After installing python3, open `cmd` as admin and run `pip install --upgrade pyinstaller python-mpv jellyfin-apiclient-python pywin32 pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
-            - Details: https://github.com/pyinstaller/pyinstaller/issues/4346
-        4. Download [libmpv](https://sourceforge.net/projects/mpv-player-windows/files/libmpv/).
-        5. Extract the `mpv-2.dll` from the file and move it to the `jellyfin-mpv-shim` folder.
-        6. Open a regular `cmd` prompt. Navigate to the `jellyfin-mpv-shim` folder.
-        7. Run `get_pywebview_natives.py`.
-        8. Run `./gen_pkg.sh --skip-build` using the Git for Windows console.
-            - This builds the translation files and downloads the shader packs.
-        9. Run `build-win.bat`.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: discord
 Provides-Extra: gui
 Provides-Extra: mirror
+License-File: LICENSE.md
+
+# Jellyfin MPV Shim
+
+[![Current Release](https://img.shields.io/github/release/jellyfin/jellyfin-mpv-shim.svg)](https://github.com/jellyfin/jellyfin-mpv-shim/releases)
+[![PyPI](https://img.shields.io/pypi/v/jellyfin-mpv-shim)](https://pypi.org/project/jellyfin-mpv-shim/)
+[![Translation Status](https://translate.jellyfin.org/widgets/jellyfin/-/jellyfin-mpv-shim/svg-badge.svg)](https://translate.jellyfin.org/projects/jellyfin/jellyfin-mpv-shim/)
+[![Code Stype](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Jellyfin MPV Shim is a cross-platform cast client for Jellyfin.
+It has support for all your advanced media files without transcoding, as well as tons of
+features which set it apart from other multimedia clients:
+
+ - Direct play most media using MPV.
+ - Watch videos with friends using SyncPlay.
+ - Offers a shim mode which runs in the background.
+ - The Jellyfin mobile apps can fully control the client.
+ - [Reconfigure subtitles](https://github.com/jellyfin/jellyfin-mpv-shim#menu) for an entire season at once.
+ - Supports all of the [MPV keyboard shortcuts](https://github.com/jellyfin/jellyfin-mpv-shim#keyboard-shortcuts).
+ - Enhance your video with [Shader Packs](https://github.com/jellyfin/jellyfin-mpv-shim#menu) and [SVP Integration](https://github.com/jellyfin/jellyfin-mpv-shim#svp-integration).
+ - Optionally share your media activity with friends using Discord Rich Presence.
+ - Most features, as well as MPV itself, [can be extensively configured](https://github.com/jellyfin/jellyfin-mpv-shim#configuration).
+ - You can configure the player to use an [external MPV player](https://github.com/jellyfin/jellyfin-mpv-shim#external-mpv) of your choice.
+ - Enable a chromecast-like experience with [Display Mirroring](https://github.com/jellyfin/jellyfin-mpv-shim#display-mirroring).
+ - You can [trigger commands to run](https://github.com/jellyfin/jellyfin-mpv-shim#shell-command-triggers) when certain events happen.
+
+To learn more, keep reading. This README explains everything, including [configuration](https://github.com/jellyfin/jellyfin-mpv-shim#configuration), [tips & tricks](https://github.com/jellyfin/jellyfin-mpv-shim#tips-and-tricks), and [development information](https://github.com/jellyfin/jellyfin-mpv-shim#development).
+
+## Getting Started
+
+If you are on Windows, simply [download the binary](https://github.com/jellyfin/jellyfin-mpv-shim/releases).
+If you are using Linux, you can [install via flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim) or [install via pip](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#linux-installation). If you are on macOS, see the [macOS Installation](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/README.md#osx-installation)
+section below.
+
+To use the client, simply launch it and log into your Jellyfin server. You’ll need to enter the
+URL to your server, for example `http://server_ip:8096` or `https://secure_domain`. Make sure to
+include the subdirectory and port number if applicable. You can then cast your media
+from another Jellyfin application.
+
+The application runs with a notification icon by default. You can use this to edit the server settings,
+view the application log, open the config folder, and open the application menu. Unlike Plex MPV Shim,
+authorization tokens for your server are stored on your device, but you are able to cast to the player
+regardless of location.
+
+Note: Due to the huge number of questions and issues that have been submitted about URLs, I now tolerate
+bare IP addresses and not specifying the port by default. If you want to connect to port 80 instead of
+8096, you must add the `:80` to the URL because `:8096` is now the default.
+
+## Limitations
+
+ - Music playback and Live TV are not supported.
+ - The client can’t be shared seamlessly between multiple users on the same server. ([Link to issue.](https://features.jellyfin.org/posts/319/mark-device-as-shared))
+
+### Known Issues
+
+Please also note that the on-screen controller for MPV (if available) cannot change the
+audio and subtitle track configurations for transcoded media. It also cannot load external
+subtitles. You must either [use the menu](https://github.com/jellyfin/jellyfin-mpv-shim#menu) or the application you casted from.
+
+Please note the following issues with controlling SyncPlay:
+ - If you attempt to join a SyncPlay group when casting to MPV Shim, it will play the media but it will not activate SyncPlay.
+     - You can, however, proceed to activate SyncPlay [using the menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
+ - If you would like to create a group or join a group for currently playing media, [use menu within MPV](https://github.com/jellyfin/jellyfin-mpv-shim#menu).
+ - SyncPlay as of 10.7.0 is new and kind of fragile. You may need to rejoin or even restart the client. Please report any issues you find.
+
+Music playback sort-of works, but repeat, shuffle, and gapless playback have not been implemented and
+would require major changes to the application to properly support, as it was built for video.
+
+The shader packs feature is sensitive to graphics hardware. It may simply just not work on your computer.
+You may be able to use the log files to get some more diagnostic information. If you're really unlucky,
+you'll have to disable the feature by pressing `k` to restore basic functionality.
+If you find the solution for your case, *please* send me any information you can provide, as every test case helps.
+
+## Advanced Features
+
+### Menu
+
+To open the menu, press **c** on your computer or use the navigation controls
+in the mobile/web app.
+
+The menu enables you to:
+ - Adjust video transcoding quality.
+ - Change the default transcoder settings.
+ - Change subtitles or audio, while knowing the track names.
+ - Change subtitles or audio for an entire series at once.
+ - Mark the media as unwatched and quit.
+ - Enable and disable SyncPlay.
+ - Configure shader packs and SVP profiles.
+ - Take screenshots.
+
+On your computer, use the mouse or arrow keys, enter, and escape to navigate.
+On your phone, use the arrow buttons, ok, back, and home to navigate.
+
+### Shader Packs
+
+Shader packs are a recent feature addition that allows you to easily use advanced video
+shaders and video quality settings. These usually require a lot of configuration to use,
+but MPV Shim's default shader pack comes with [FSRCNNX](https://github.com/igv/FSRCNN-TensorFlow)
+and [Anime4K](https://github.com/bloc97/Anime4K) preconfigured. Try experimenting with video
+profiles! It may greatly improve your experience.
+
+Shader Packs are ready to use as of the most recent MPV Shim version. To use, simply
+navigate to the **Video Playback Profiles** option and select a profile.
+
+For details on the shader settings, please see [default-shader-pack](https://github.com/iwalton3/default-shader-pack).
+If you would like to customize the shader pack, there are details in the configuration section.
+
+### SVP Integration
+
+SVP integration allows you to easily configure SVP support, change profiles, and enable/disable
+SVP without having to exit the player. It is not enabled by default, please see the configuration
+instructions for instructions on how to enable it.
+
+### Display Mirroring
+
+This feature allows media previews to show on your display before you cast the media,
+similar to Chromecast. It is not enabled by default. To enable it, do one of the following:
+
+ - Using the systray icon, click "Application Menu". Go to preferences and enable display mirroring.
+     - Use the arrow keys, escape, and enter to navigate the menu.
+ - Cast media to the player and press `c`. Go to preferences and enable display mirroring.
+ - In the config file (see below), change `display_mirroring` to `true`.
+
+Then restart the application for the change to take effect. To quit the application on Windows with
+display mirroring enabled, press Alt+F4.
+
+### Keyboard Shortcuts
+
+This program supports most of the [keyboard shortcuts from MPV](https://mpv.io/manual/stable/#interactive-control). The custom keyboard shortcuts are:
+
+ - < > to skip episodes
+ - q to close player
+ - w to mark watched and skip
+ - u to mark unwatched and quit
+ - c to open the menu
+ - k disable shader packs
+
+Here are the notable MPV keyboard shortcuts:
+
+ - space - Pause/Play
+ - left/right - Seek by 5 seconds
+ - up/down - Seek by 1 minute
+ - s - Take a screenshot
+ - S - Take a screenshot without subtitles
+ - f - Toggle fullscreen
+ - ,/. - Seek by individual frames
+ - \[/\] - Change video speed by 10%
+ - {/} - Change video speed by 50%
+ - backspace - Reset speed
+ - m - Mute
+ - d - Enable/disable deinterlace
+ - Ctrl+Shift+Left/Right - Adjust subtitle delay.
+
+## Configuration
+
+The configuration file is located in different places depending on your platform. You can also open the
+configuration folder using the systray icon if you are using the shim version. When you launch the program
+on Linux or macOS from the terminal, the location of the config file will be printed. The locations are:
+ - Windows - `%appdata%\jellyfin-mpv-shim\conf.json`
+ - Linux - `~/.config/jellyfin-mpv-shim/conf.json`
+ - Linux (Flatpak) - `~/.var/app/com.github.iwalton3.jellyfin-mpv-shim/config/jellyfin-mpv-shim/conf.json`
+ - macOS - `~/Library/Application Support/jellyfin-mpv-shim/conf.json`
+ - CygWin - `~/.config/jellyfin-mpv-shim/conf.json`
+
+You can specify a custom configuration folder with the `--config` option.
+
+### Transcoding
+
+You can adjust the basic transcoder settings via the menu.
+
+- `always_transcode` - This will tell the client to always transcode. Default: `false`
+    - This may be useful if you are using limited hardware that cannot handle advanced codecs.
+    - Please note that Jellyfin may still direct play files that meet the transcode profile
+      requirements. There is nothing I can do on my end to disable this, but you can reduce
+      the bandwidth setting to force a transcode.
+- `transcode_hdr` - Force transcode HDR videos to SDR. Default: `false`
+- `transcode_dolby_vision` - Force transcode Dolby Vision videos to SDR. Default: `true`
+    - If your computer can handle it, you can get tone mapping to work for this using `vo=gpu-next`.
+    - Note that `vo=gpu-next` is considered experimental by MPV at this time.
+- `transcode_hi10p` - Force transcode 10 bit color videos to 8 bit color. Default: `false`
+- `transcode_hevc` - Force transcode HEVC videos. Default: `false`
+- `transcode_av1` - Force transcode AV1 videos. Default: `false`
+- `transcode_4k` - Force transcode videos over 1080p. Default: `false`
+- `remote_kbps` - Bandwidth to permit for remote streaming. Default: `10000`
+- `local_kbps` - Bandwidth to permit for local streaming. Default: `2147483`
+- `direct_paths` - Play media files directly from the SMB or NFS source. Default: `false`
+    - `remote_direct_paths` - Apply this even when the server is detected as remote. Default: `false`
+- `allow_transcode_to_h265` - Allow the server to transcode media *to* `hevc`. Default: `false`
+    - If you enable this, it'll allow remuxing to HEVC but it'll also break force transcoding of Dolby Vision and HDR content if those settings are used. (See [this bug](https://github.com/jellyfin/jellyfin/issues/9313).)
+- `prefer_transcode_to_h265` - Requests the server to transcode media *to* `hevc` as the default. Default: `false`
+- `transcode_warning` - Display a warning the first time media transcodes in a session. Default: `true`
+- `force_video_codec` - Force a specified video codec to be played. Default: `null`
+    - This can be used in tandem with `always_transcode` to force the client to transcode into
+      the specified format.
+    - This may have the same limitations as `always_transcode`.
+    - This will override `transcode_to_h265`, `transcode_h265` and `transcode_hi10p`.
+- `force_audio_codec` - Force a specified audio codec to be played. Default: `null`
+    - This can be used in tandeom with `always_transcode` to force the client to transcode into
+      the specified format.
+    - This may have the same limitations as `always_transcode`.
+
+### Features
+
+You can use the config file to enable and disable features.
+
+ - `fullscreen` - Fullscreen the player when starting playback. Default: `true`
+ - `enable_gui` - Enable the system tray icon and GUI features. Default: `true`
+ - `enable_osc` - Enable the MPV on-screen controller. Default: `true`
+    - It may be useful to disable this if you are using an external player that already provides a user interface.
+ - `media_key_seek` - Use the media next/prev keys to seek instead of skip episodes. Default: `false`
+ - `use_web_seek` - Use the seek times set in Jellyfin web for arrow key seek. Default: `false`
+ - `display_mirroring` - Enable webview-based display mirroring (content preview). Default: `false`
+ - `screenshot_menu` - Allow taking screenshots from menu. Default: `true`
+ - `check_updates` - Check for updates via GitHub. Default: `true`
+    - This requests the GitHub releases page and checks for a new version.
+    - Update checks are performed when playing media, once per day.
+ - `notify_updates` - Display update notification when playing media. Default: `true`
+    - Notification will only display once until the application is restarted.
+ - `discord_presence` - Enable Discord rich presence support. Default: `false`
+ - `menu_mouse` - Enable mouse support in the menu. Default: `true`
+     - This requires MPV to be compiled with lua support.
+
+### Shell Command Triggers
+
+You can execute shell commands on media state using the config file:
+
+ - `media_ended_cmd` - When all media has played.
+ - `pre_media_cmd` - Before the player displays. (Will wait for finish.)
+ - `stop_cmd` - After stopping the player.
+ - `idle_cmd` - After no activity for `idle_cmd_delay` seconds.
+ - `idle_when_paused` - Consider the player idle when paused. Default: `false`
+ - `stop_idle` - Stop the player when idle. (Requires `idle_when_paused`.) Default: `false`
+ - `play_cmd` - After playback starts.
+ - `idle_ended_cmd` - After player stops being idle.
+
+### Subtitle Visual Settings
+
+These settings may not works for some subtitle codecs or if subtitles are being burned in
+during a transcode. You can configure custom styled subtitle settings through the MPV config file.
+
+ - `subtitle_size` - The size of the subtitles, in percent. Default: `100`
+ - `subtitle_color` - The color of the subtitles, in hex. Default: `#FFFFFFFF`
+ - `subtitle_position` - The position (top, bottom, middle). Default: `bottom`
+
+### External MPV
+
+The client now supports using an external copy of MPV, including one that is running prior to starting
+the client. This may be useful if your distribution only provides MPV as a binary executable (instead
+of as a shared library), or to connect to MPV-based GUI players. Please note that SMPlayer exhibits
+strange behaviour when controlled in this manner. External MPV is currently the only working backend
+for media playback on macOS. Additionally, due to Flatpak sandbox restrictions, external mpv is not
+practical to use in most cases for the Flatpak version.
+
+- `mpv_ext` - Enable usage of the external player by default. Default: `false`
+    - The external player may still be used by default if `libmpv1` is not available.
+- `mpv_ext_path` - The path to the `mpv` binary to use. By default it uses the one in the PATH. Default: `null`
+    - If you are using Windows, make sure to use two backslashes. Example: `C:\\path\\to\\mpv.exe`
+- `mpv_ext_ipc` - The path to the socket to control MPV. Default: `null`
+    - If unset, the socket is a randomly selected temp file.
+    - On Windows, this is just a name for the socket, not a path like on Linux.
+- `mpv_ext_start` - Start a managed copy of MPV with the client. Default: `true`
+    - If not specified, the user must start MPV prior to launching the client.
+    - MPV must be launched with `--input-ipc-server=[value of mpv_ext_ipc]`.
+- `mpv_ext_no_ovr` - Disable built-in mpv configuration files and use user defaults.
+    - Please note that some scripts and settings, such as ones to keep MPV open, may break
+      functionality in MPV Shim.
+
+### Keyboard Shortcuts
+
+You can reconfigure the custom keyboard shortcuts. You can also set them to `null` to disable the shortcut. Please note that disabling keyboard shortcuts may make some features unusable. Additionally, if you remap `q`, using the default shortcut will crash the player.
+
+ - `kb_stop` - Stop playback and close MPV. (Default: `q`)
+ - `kb_prev` - Go to the previous video. (Default: `<`)
+ - `kb_next` - Go to the next video. (Default: `>`)
+ - `kb_watched` - Mark the video as watched and skip. (Default: `w`)
+ - `kb_unwatched` - Mark the video as unwatched and quit. (Default: `u`)
+ - `kb_menu` - Open the configuration menu. (Default: `c`)
+ - `kb_menu_esc` - Leave the menu. Exits fullscreen otherwise. (Default: `esc`)
+ - `kb_menu_ok` - "ok" for menu. (Default: `enter`)
+ - `kb_menu_left` - "left" for menu. Seeks otherwise. (Default: `left`)
+ - `kb_menu_right` - "right" for menu. Seeks otherwise. (Default: `right`)
+ - `kb_menu_up` - "up" for menu. Seeks otherwise. (Default: `up`)
+ - `kb_menu_down` - "down" for menu. Seeks otherwise. (Default: `down`)
+ - `kb_pause` - Pause. Also "ok" for menu. (Default: `space`)
+ - `kb_fullscreen` - Toggle fullscreen. (Default: `f`)
+ - `kb_debug` - Trigger `pdb` debugger. (Default: `~`)
+ - `kb_kill_shader` - Disable shader packs. (Default: `k`)
+ - `seek_up` - Time to seek for "up" key. (Default: `60`)
+ - `seek_down` - Time to seek for "down" key. (Default: `-60`)
+ - `seek_right` - Time to seek for "right" key. (Default: `5`)
+ - `seek_left` - Time to seek for "left" key. (Default: `-5`)
+ - `media_keys` - Enable binding of MPV to media keys. Default: `true`
+ - `seek_v_exact` - Use exact seek for up/down keys. Default: `false`
+ - `seek_h_exact` - Use exact seek for left/right keys. Default: `false`
+
+### Shader Packs
+
+Shader packs allow you to import MPV config and shader presets into MPV Shim and easily switch
+between them at runtime through the built-in menu. This enables easy usage and switching of
+advanced MPV video playback options, such as video upscaling, while being easy to use.
+
+If you select one of the presets from the shader pack, it will override some MPV configurations
+and any shaders manually specified in `mpv.conf`. If you would like to customize the shader pack,
+use `shader_pack_custom`.
+
+ - `shader_pack_enable` - Enable shader pack. (Default: `true`)
+ - `shader_pack_custom` - Enable to use a custom shader pack. (Default: `false`)
+    - If you enable this, it will copy the default shader pack to the `shader_pack` config folder.
+    - This initial copy will only happen if the `shader_pack` folder didn't exist.
+    - This shader pack will then be used instead of the built-in one from then on.
+ - `shader_pack_remember` - Automatically remember the last used shader profile. (Default: `true`)
+ - `shader_pack_profile` - The default profile to use. (Default: `null`)
+    - If you use `shader_pack_remember`, this will be updated when you set a profile through the UI.
+ - `shader_pack_subtype` - The profile group to use. The default pack contains `lq` and `hq` groups. Use `hq` if you have a fancy graphics card.
+
+### Trickplay Thumbnails
+
+MPV will automatically display thumbnail previews. By default it uses the Trickplay images and falls back to chapter images. Please note that this feature will download and
+uncompress all of the chapter images before it becomes available for a video. For a 4 hour movie this
+causes disk usage of about 250 MB, but for the average TV episode it is around 40 MB. It also requires
+overriding the default MPV OSC, which may conflict with some custom user script. Trickplay is compatible
+with any OSC that uses [thumbfast](https://github.com/po5/thumbfast), as I have added a [compatibility layer](https://github.com/jellyfin/jellyfin-mpv-shim/blob/master/jellyfin_mpv_shim/thumbfast.lua).
+
+ - `thumbnail_enable` - Enable thumbnail feature. (Default: `true`)
+ - `thumbnail_osc_builtin` - Disable this setting if you want to use your own custom osc but leave trickplay enabled. (Default: `true`)
+ - `thumbnail_preferred_size` - The ideal size for thumbnails. (Default: `320`)
+
+### SVP Integration
+
+To enable SVP integration, set `svp_enable` to `true` and enable "External control via HTTP" within SVP
+under Settings > Control options. Adjust the `svp_url` and `svp_socket` settings if needed.
+
+ - `svp_enable` - Enable SVP integration. (Default: `false`)
+ - `svp_url` - URL for SVP web API. (Default: `http://127.0.0.1:9901/`)
+ - `svp_socket` - Custom MPV socket to use for SVP.
+    - Default on Windows: `mpvpipe`
+    - Default on other platforms: `/tmp/mpvsocket`
+
+Currently on Windows the built-in MPV does not work with SVP. You must download MPV yourself.
+
+ - Download the latest MPV build [from here](https://sourceforge.net/projects/mpv-player-windows/files/64bit/).
+ - Follow the [vapoursynth instructions](https://github.com/shinchiro/mpv-winbuild-cmake/wiki/Setup-vapoursynth-for-mpv).
+     - Make sure to use the latest Python, not Python 3.7.
+ - In the config file, set `mpv_ext` to `true` and `mpv_ext_path` to the path to `mpv.exe`.
+     - Make sure to use two backslashes per each backslash in the path.
+
+### SyncPlay
+
+You probably don't need to change these, but they are defined here in case you
+need to.
+
+ - `sync_max_delay_speed` - Delay in ms before changing video speed to sync playback. Default: `50`
+ - `sync_max_delay_skip` - Delay in ms before skipping through the video to sync playback. Default: `300`
+ - `sync_method_thresh` - Delay in ms before switching sync method. Default: `2000`
+ - `sync_speed_time` - Duration in ms to change playback speed. Default: `1000`
+ - `sync_speed_attempts` - Number of attempts before speed changes are disabled. Default: `3`
+ - `sync_attempts` - Number of attempts before disabling sync play. Default: `5`
+ - `sync_revert_seek` - Attempt to revert seek via MPV OSC. Default: `true`
+     - This could break if you use revert-seek markers or scripts that use it.
+ - `sync_osd_message` - Write syncplay status messages to OSD. Default: `true`
+
+### Debugging
+
+These settings assist with debugging. You will often be asked to configure them when reporting an issue.
+
+ - `log_decisions` - Log the full media decisions and playback URLs. Default: `false`
+ - `mpv_log_level` - Log level to use for mpv. Default: `info`
+    - Options: fatal, error, warn, info, v, debug, trace
+ - `sanitize_output` - Prevent the writing of server auth tokens to logs. Default: `true`
+ - `write_logs` - Write logs to the config directory for debugging. Default: `false`
+
+### Other Configuration Options
+
+Other miscellaneous configuration options. You probably won't have to change these.
+
+ - `player_name` - The name of the player that appears in the cast menu. Initially set from your hostname.
+ - `client_uuid` - The identifier for the client. Set to a random value on first run.
+ - `audio_output` - Currently has no effect. Default: `hdmi`
+ - `playback_timeout` - Timeout to wait for MPV to start loading video in seconds. Default: `30`
+    - If you're hitting this, it means files on your server probably got corrupted or deleted.
+    - It could also happen if you try to play an unsupported video format. These are rare.
+ - `lang` - Allows overriding system locale. (Enter a language code.) Default: `null`
+    - MPV Shim should use your OS language by default.
+ - `ignore_ssl_cert` - Ignore SSL certificates. Default: `false`
+    - Please consider getting a certificate from Let's Encrypt instead of using this.
+ - `connect_retry_mins` - Number of minutes to retry connecting before showing login window. Default: `0`
+    - This only applies for when you first launch the program.
+ - `lang_filter` - Limit track selection to desired languages. Default: `und,eng,jpn,mis,mul,zxx`
+    - Note that you need to turn on the options below for this to actually do something.
+    - If you remove `und` from the list, it will ignore untagged items.
+    - Languages are typically in [ISO 639-2/B](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes),
+      but if you have strange files this may not be the case.
+ - `lang_filter_sub` - Apply the language filter to subtitle selection. Default: `False`
+ - `lang_filter_audio` - Apply the language filter to audio selection. Default: `False`
+ - `screenshot_dir` - Sets where screenshots go.
+    - Default is the desktop on Windows and unset (current directory) on other platforms.
+ - `force_set_played` - This forcibly sets items as played when MPV playback finished.
+    - If you have files with malformed timestamps that don't get marked as played, enable this.
+ - `raise_mpv` - Windows only. Disable this if you are fine with MPV sometimes appearing behind other windows when playing.
+ - `health_check_interval` - The number of seconds between each client health check. Null disables it. Default: `300`
+
+### Skip Intro Support
+
+This functionality is considered experimental and requires the third-party [SkipIntro server plugin](https://github.com/ConfusedPolarBear/intro-skipper). It works the same ways as it did on MPV Shim for Plex.
+
+ - `skip_intro_always` - Always skip intros, without asking. Default: `false`
+ - `skip_intro_prompt` - Prompt to skip intro via seeking. Default: `false`
+
+### MPV Configuration
+
+You can configure mpv directly using the `mpv.conf` and `input.conf` files. (It is in the same folder as `conf.json`.)
+This may be useful for customizing video upscaling, keyboard shortcuts, or controlling the application
+via the mpv IPC server.
+
+### Authorization
+
+The `cred.json` file contains the authorization information. If you are having problems with the client,
+such as the Now Playing not appearing or want to delete a server, you can delete this file and add the
+servers again.
+
+## Tips and Tricks
+
+Various tips have been found that allow the media player to support special
+functionality, albeit with more configuration required.
+
+### Open on Specific Monitor (#19)
+
+Please note: Edits to the `mpv.conf` will not take effect until you restart the application. You can open the config directory by using the menu option in the system tray icon.
+
+**Option 1**: Select fullscreen output screen through MPV.
+Determine which screen you would like MPV to show up on.
+ - If you are on Windows, right click the desktop and select "Display Settings". Take the monitor number and subtract one.
+ - If you are on Linux, run `xrandr`. The screen number is the number you want. If there is only one proceed to **Option 2**.
+
+Add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration), replacing `0` with the number from the previous step:
+```
+fs=yes
+fs-screen=0
+```
+
+**Option 2**: (Linux Only) If option 1 does not work, both of your monitors are likely configured as a single "screen".
+
+Run `xrandr`. It should look something like this:
+
+```
+Screen 0: minimum 8 x 8, current 3520 x 1080, maximum 16384 x 16384
+VGA-0 connected 1920x1080+0+0 (normal left inverted right x axis y axis) 521mm x 293mm
+   1920x1080     60.00*+
+   1680x1050     59.95
+   1440x900      59.89
+   1280x1024     75.02    60.02
+   1280x960      60.00
+   1280x800      59.81
+   1280x720      60.00
+   1152x864      75.00
+   1024x768      75.03    70.07    60.00
+   800x600       75.00    72.19    60.32    56.25
+   640x480       75.00    59.94
+LVDS-0 connected 1600x900+1920+180 (normal left inverted right x axis y axis) 309mm x 174mm
+   1600x900      59.98*+
+```
+
+If you want MPV to open on VGA-0 for instance, add the following to your `mpv.conf` in the [config directory](https://github.com/jellyfin/jellyfin-mpv-shim#mpv-configuration):
+```
+fs=yes
+geometry=1920x1080+0+0
+```
+**Option 3**: (Linux Only) If your window manager supports it, you can tell the window manager to always open on a specific screen.
+
+ - For OpenBox: https://forums.bunsenlabs.org/viewtopic.php?id=1199
+ - For i3: https://unix.stackexchange.com/questions/96798/i3wm-start-applications-on-specific-workspaces-when-i3-starts/363848#363848
+
+### Control Volume with Mouse Wheel (#48)
+
+Add the following to `input.conf`:
+```
+WHEEL_UP add volume 5
+WHEEL_DOWN add volume -5
+```
+
+### MPRIS Plugin (#54)
+
+Set `mpv_ext` to `true` in the config. Add `script=/path/to/mpris.so` to `mpv.conf`.
+
+### Run Multiple Instances (#45)
+
+You can pass `--config /path/to/folder` to run another copy of the player. Please
+note that running multiple copies of the desktop client is currently not supported.
+
+### Audio Passthrough
+
+You can edit `mpv.conf` to support audio passthrough. A [user on Reddit](https://reddit.com/r/jellyfin/comments/fru6xo/new_cross_platform_desktop_client_jellyfin_mpv/fns7vyp) had luck with this config:
+```
+audio-spdif=ac3,dts,eac3 # (to use the passthrough to receiver over hdmi)
+audio-channels=2 # (not sure this is necessary, but i keep it in because it works)
+af=scaletempo,lavcac3enc=yes:640:3 # (for aac 5.1 tracks to the receiver)
+```
+
+### MPV Crashes with "The sub-scale option must be a floating point number or a ratio"
+
+Run the jellyfin-mpv-shim program with LC_NUMERIC=C.
+
+### Use with gnome-mpv/celluloid (#61)
+
+You can use `gnome-mpv` with MPV Shim, but you must launch `gnome-mpv` separately before MPV Shim. (`gnome-mpv` doesn't support the MPV command options directly.)
+
+Configure MPV Shim with the following options (leave the other ones):
+```json
+{
+    "mpv_ext": true,
+    "mpv_ext_ipc": "/tmp/gmpv-socket",
+    "mpv_ext_path": null,
+    "mpv_ext_start": false,
+    "enable_osc": false
+}
+```
+Then within `gnome-mpv`, click the application icon (top left) > Preferences. Configure the following Extra MPV Options:
+```
+--idle --input-ipc-server=/tmp/gmpv-socket
+```
+
+### Heavy Memory Usage
+
+A problem has been identified where MPV can use a ton of RAM after media has been played,
+and this RAM is not always freed when the player goes into idle mode. Some users have
+found that using external MPV lessens the memory leak. To enable external MPV on Windows:
+
+ - [Download a copy of MPV](https://sourceforge.net/projects/mpv-player-windows/files/64bit/)
+ - Unzip it with 7zip.
+ - Configure `mpv_ext` to `true`. (See the config section.)
+ - Configure `mpv_ext_path` to `C:\\replace\\with\\path\\to\\mpv.exe`. (Note usage of two `\\`.)
+ - Run the program and wait. (You'll probably have to use it for a while.)
+ - Let me know if the high memory usage is with `mpv.exe` or the shim itself.
+
+On Linux, the process is similar, except that you don't need to set the `mpv_ext_path` variable.
+On macOS, external MPV is already the default and is the only supported player mode.
+
+In the long term, I may look into a method of terminating MPV when not in use. This will require
+a lot of changes to the software.
+
+### Player Sizing (#91)
+
+MPV by default may force the window size to match the video aspect ratio, instead of allowing
+resizing and centering the video accordingly. Add the following to `mpv.conf` to enable resizing
+of the window freely, if desired:
+```
+no-keepaspect-window
+```
+
+## Development
+
+If you'd like to run the application without installing it, run `./run.py`.
+The project is written entirely in Python 3. There are no closed-source
+components in this project. It is fully hackable.
+
+The project is dependent on `python-mpv`, `python-mpv-jsonipc`, and `jellyfin-apiclient-python`. If you are
+using Windows and would like mpv to be maximize properly, `pywin32` is also needed. The GUI
+component uses `pystray` and `tkinter`, but there is a fallback cli mode. The mirroring dependencies
+are `Jinja2` and `pywebview`, along with platform-specific dependencies. (See the installation and building
+guides for details on platform-specific dependencies for display mirroring.)
+
+This project is based Plex MPV Shim, which is based on https://github.com/wnielson/omplex, which
+is available under the terms of the MIT License. The project was ported to python3, modified to
+use mpv as the player, and updated to allow all features of the remote control api for video playback.
+
+The Jellyfin API client comes from [Jellyfin for Kodi](https://github.com/jellyfin/jellyfin-kodi/tree/master/jellyfin_kodi).
+The API client was originally forked for this project and is now a [separate package](https://github.com/iwalton3/jellyfin-apiclient-python).
+
+The css file for desktop mirroring is from [jellyfin-chromecast](https://github.com/jellyfin/jellyfin-chromecast/tree/5194d2b9f0120e0eb8c7a81fe546cb9e92fcca2b) and is subject to GPL v2.0.
+
+The shaders included in the shader pack are also available under verious open source licenses,
+[which you can read about here](https://github.com/iwalton3/default-shader-pack/blob/master/LICENSE.md).
+
+### Local Dev Installation
+
+If you are on Windows there are additional dependencies. Please see the Windows Build Instructions.
+
+1. Install the dependencies: `pip3 install --upgrade python-mpv jellyfin-apiclient-python pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
+    - If you run `./gen_pkg.sh --install`, it will also fetch these for you.
+    - Note: Recent distributions make pip unusable by default. Consider using conda or add a virtualenv to your user's path.
+2. Clone this repository: `git clone https://github.com/jellyfin/jellyfin-mpv-shim`
+    - You can also download a zip build.
+3. `cd` to the repository: `cd jellyfin-mpv-shim`
+4. Run prepare script: `./gen_pkg.sh`
+    - To do this manually, download the web client, shader pack, and build the language files.
+5. Ensure you have a copy of `libmpv1` or `mpv` available.
+6. Install any platform-specific dependencies from the respective install tutorials.
+7. You should now be able to run the program with `./run.py`. Installation is possible with `sudo pip3 install .`.
+    - You can also install the package with `./gen_pkg.sh --install`.
+
+### Translation
+
+This project uses gettext for translation. The current template language file is `base.pot` in `jellyfin_mpv_shim/messages/`.
+
+To regenerate `base.pot` and update an existing translation with new strings:
+```bash
+./regen_pot.sh
+```
+
+To compile all `*.po` files to `*.mo`:
+```bash
+./gen_pkg.sh --skip-build
+```
+
+## Linux Installation
+
+You can [install the software from flathub](https://flathub.org/apps/details/com.github.iwalton3.jellyfin-mpv-shim). The pip installation is less integrated but takes up less space if you're not already using flatpak.
+
+If you are on Linux, you can install via pip. You'll need [libmpv1](https://github.com/Kagami/mpv.js/blob/master/README.md#get-libmpv) or `mpv` installed.
+```bash
+sudo pip3 install --upgrade jellyfin-mpv-shim
+```
+If you would like the GUI and systray features, also install `pystray` and `tkinter`:
+```bash
+sudo pip3 install pystray
+sudo apt install python3-tk
+```
+If you would like display mirroring support, install the mirroring dependencies:
+```bash
+sudo apt install python3-jinja2 python3-webview
+# -- OR --
+sudo pip3 install jellyfin-mpv-shim[mirror]
+sudo apt install gir1.2-webkit2-4.0
+```
+Discord rich presence support:
+```bash
+sudo pip3 install jellyfin-mpv-shim[discord]
+```
+You can build mpv from source to get better codec support. Execute the following:
+```bash
+sudo pip3 install --upgrade python-mpv
+sudo apt install autoconf automake libtool libharfbuzz-dev libfreetype6-dev libfontconfig1-dev libx11-dev libxrandr-dev libvdpau-dev libva-dev mesa-common-dev libegl1-mesa-dev yasm libasound2-dev libpulse-dev libuchardet-dev zlib1g-dev libfribidi-dev git libgnutls28-dev libgl1-mesa-dev libsdl2-dev cmake wget python g++ libluajit-5.1-dev
+git clone https://github.com/mpv-player/mpv-build.git
+cd mpv-build
+echo --enable-libmpv-shared > mpv_options
+./rebuild -j4
+sudo ./install
+sudo ldconfig
+```
+
+## <h2 id="osx-installation">macOS Installation</h2>
+Currently on macOS only the external MPV backend seems to be working. I cannot test on macOS, so please report any issues you find.
+
+To install the CLI version:
+
+1. Install brew. ([Instructions](https://brew.sh/))
+2. Install python3 and mpv. `brew install python mpv`
+3. Install jellyfin-mpv-shim. `pip3 install --upgrade jellyfin-mpv-shim`
+4. Run `jellyfin-mpv-shim`.
+
+If you'd like to install the GUI version, you need a working copy of tkinter.
+
+1. Install pyenv. ([Instructions](https://medium.com/python-every-day/python-development-on-macos-with-pyenv-2509c694a808))
+2. Install TK and mpv. `brew install tcl-tk mpv`
+3. Install python3 with TK support. `FLAGS="-I$(brew --prefix tcl-tk)/include" pyenv install 3.8.1`
+4. Set this python3 as the default. `pyenv global 3.8.1`
+5. Install jellyfin-mpv-shim and pystray. `pip3 install --upgrade 'jellyfin-mpv-shim[gui]'`
+6. Run `jellyfin-mpv-shim`.
+
+Display mirroring is not tested on macOS, but may be installable with 'pip3 install --upgrade 'jellyfin-mpv-shim[mirror]'`.
+
+## Building on Windows
+
+There is a prebuilt version for Windows in the releases section. When
+following these directions, please take care to ensure both the python
+and libmpv libraries are either 64 or 32 bit. (Don't mismatch them.)
+
+If you'd like to build the installer, please install [Inno Setup](https://jrsoftware.org/isinfo.php) to build
+the installer. If you'd like to build a 32 bit version, download the 32 bit version of mpv-1.dll and
+copy it into a new folder called mpv32. You'll also need [WebBrowserInterop.x86.dll](https://github.com/r0x0r/pywebview/blob/master/webview/lib/WebBrowserInterop.x86.dll?raw=true).
+You may also need to edit the batch file for 32 bit builds to point to the right python executable.
+
+1. Install Git for Windows. Open Git Bash and run `git clone https://github.com/jellyfin/jellyfin-mpv-shim; cd jellyfin-mpv-shim`.
+    - You can update the project later with `git pull`.
+2. Install [Python3](https://www.python.org/downloads/) with PATH enabled. Install [7zip](https://ninite.com/7zip/).
+3. After installing python3, open `cmd` as admin and run `pip install --upgrade pyinstaller python-mpv jellyfin-apiclient-python pywin32 pystray Jinja2 pywebview python-mpv-jsonipc pypresence`.
+    - Details: https://github.com/pyinstaller/pyinstaller/issues/4346
+4. Download [libmpv](https://sourceforge.net/projects/mpv-player-windows/files/libmpv/).
+5. Extract the `mpv-2.dll` from the file and move it to the `jellyfin-mpv-shim` folder.
+6. Open a regular `cmd` prompt. Navigate to the `jellyfin-mpv-shim` folder.
+7. Run `get_pywebview_natives.py`.
+8. Run `./gen_pkg.sh --skip-build` using the Git for Windows console.
+    - This builds the translation files and downloads the shader packs.
+9. Run `build-win.bat`.
```

### Comparing `jellyfin-mpv-shim-2.6.0/jellyfin_mpv_shim.egg-info/SOURCES.txt` & `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.md
 MANIFEST.in
 README.md
 setup.py
 jellyfin_mpv_shim/__init__.py
 jellyfin_mpv_shim/action_thread.py
 jellyfin_mpv_shim/bifdecode.py
 jellyfin_mpv_shim/bulk_subtitle.py
@@ -96,14 +97,16 @@
 jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook
 jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook
 jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook
 jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook
 jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook
 jellyfin_mpv_shim/display_mirror/__init__.py
 jellyfin_mpv_shim/display_mirror/helpers.py
+jellyfin_mpv_shim/display_mirror/index.html
+jellyfin_mpv_shim/display_mirror/jellyfin.css
 jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml
 jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.desktop
 jellyfin_mpv_shim/integration/jellyfin-128.png
 jellyfin_mpv_shim/integration/jellyfin-16.png
 jellyfin_mpv_shim/integration/jellyfin-256.png
 jellyfin_mpv_shim/integration/jellyfin-32.png
 jellyfin_mpv_shim/integration/jellyfin-48.png
@@ -111,14 +114,15 @@
 jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo
@@ -126,30 +130,36 @@
 jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/km/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo
+jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo
 jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo
```

### Comparing `jellyfin-mpv-shim-2.6.0/setup.py` & `jellyfin-mpv-shim-2.7.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from setuptools import setup
 import sys
+import os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extras = {
     "gui": ["pystray", "pillow"],
     "mirror": ["Jinja2", "pywebview>=3.3.1"],
@@ -12,25 +13,43 @@
 }
 
 if sys.platform.startswith("win32"):
     win_extra = ["pywin32", "clr-loader==0.1.7", "pythonnet==3.0.0a2"]
     extras["all"] += win_extra
     extras["mirror"] += win_extra
 
+packages = [
+    "jellyfin_mpv_shim",
+    "jellyfin_mpv_shim.display_mirror",
+
+]
+
+if not sys.platform.startswith("win32"):
+    packages.extend([
+        "jellyfin_mpv_shim.messages",
+        "jellyfin_mpv_shim.default_shader_pack",
+        "jellyfin_mpv_shim.default_shader_pack.shaders",
+        "jellyfin_mpv_shim.integration"
+    ])
+
+    for dir in os.listdir("jellyfin_mpv_shim/messages"):
+        if os.path.isdir("jellyfin_mpv_shim/messages/" + dir + "/LC_MESSAGES"):
+            packages.append("jellyfin_mpv_shim.messages." + dir + ".LC_MESSAGES")
+
 setup(
     name="jellyfin-mpv-shim",
-    version="2.6.0",
-    author="Ian Walton",
-    author_email="iwalton3@gmail.com",
+    version="2.7.0",
+    author="Izzie Walton",
+    author_email="izzie@iwalton.com",
     description="Cast media from Jellyfin Mobile and Web apps to MPV.",
     license="GPLv3",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/jellyfin/jellyfin-mpv-shim",
-    packages=["jellyfin_mpv_shim", "jellyfin_mpv_shim.display_mirror"],
+    packages=packages,
     package_data={
         "jellyfin_mpv_shim.display_mirror": ["*.css", "*.html"],
         "jellyfin_mpv_shim": ["systray.png"],
     },
     entry_points={
         "console_scripts": ["jellyfin-mpv-shim=jellyfin_mpv_shim.mpv_shim:main"]
     },
```

