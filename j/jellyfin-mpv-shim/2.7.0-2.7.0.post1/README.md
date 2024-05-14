# Comparing `tmp/jellyfin-mpv-shim-2.7.0.tar.gz` & `tmp/jellyfin-mpv-shim-2.7.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jellyfin-mpv-shim-2.7.0.tar", last modified: Tue May 14 01:36:02 2024, max compression
+gzip compressed data, was "jellyfin-mpv-shim-2.7.0.post1.tar", last modified: Tue May 14 06:38:37 2024, max compression
```

## Comparing `jellyfin-mpv-shim-2.7.0.tar` & `jellyfin-mpv-shim-2.7.0.post1.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    36330 2024-05-13 18:21:11.000000 jellyfin-mpv-shim-2.7.0/LICENSE.md
--rw-r--r--   0 izzie     (1000) izzie     (1000)      316 2023-02-25 22:55:04.000000 jellyfin-mpv-shim-2.7.0/MANIFEST.in
--rw-r--r--   0 izzie     (1000) izzie     (1000)    39199 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/PKG-INFO
--rw-r--r--   0 izzie     (1000) izzie     (1000)    38603 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/README.md
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/
--rw-r--r--   0 izzie     (1000) izzie     (1000)       25 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/__init__.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)      660 2023-02-17 22:23:05.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/action_thread.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1704 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bifdecode.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8952 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bulk_subtitle.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)      352 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/cli_mgr.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    10750 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/clients.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6890 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conf.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1735 2023-02-24 22:10:52.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conffile.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)      593 2024-05-13 21:21:39.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/constants.py
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.596825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2160 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2971 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/README.md
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7249 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json
--rw-r--r--   0 izzie     (1000) izzie     (1000)    10428 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6781 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack.json
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1596 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1604 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2884 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6594 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6179 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4705 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6695 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2848 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4340 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     3923 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    69921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    35916 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    17136 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    70020 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    36016 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    17198 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   308873 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   144204 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   308660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   144075 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6482 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6184 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6571 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    73443 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    37685 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    18638 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   290257 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   146743 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    16063 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4988 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6590 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    73584 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    37714 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    18667 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   290040 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   146811 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4159 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6548 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    13921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    16217 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   246177 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    70598 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)    26173 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7444 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl
--rw-r--r--   0 izzie     (1000) izzie     (1000)   331721 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)    48421 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)   655609 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)    88885 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)   169871 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)      664 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)      666 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)      624 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook
--rw-r--r--   0 izzie     (1000) izzie     (1000)      625 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     5714 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/__init__.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9235 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/helpers.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7620 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/index.html
--rw-r--r--   0 izzie     (1000) izzie     (1000)    18550 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/jellyfin.css
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6149 2022-06-11 04:16:20.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/event_handler.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    14650 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/gui_mgr.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)      909 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/i18n.py
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    15961 2024-05-14 00:53:53.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml
--rw-r--r--   0 izzie     (1000) izzie     (1000)      160 2021-04-20 00:09:50.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.desktop
--rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-128.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-16.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)    19703 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-256.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1661 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-32.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2444 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-48.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)     6709 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-64.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2366 2024-05-14 00:00:06.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/log_utils.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    16222 2024-05-14 00:37:26.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/media.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    19810 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/menu.py
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4893 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      538 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    10706 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    11509 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    12209 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4358 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9722 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.600825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9098 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9569 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9197 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9129 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9408 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    12144 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.584824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8802 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8722 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9666 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9827 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9654 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9084 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    10970 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9443 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9524 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9653 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1645 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9245 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9992 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4272 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9532 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9735 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9024 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9305 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7698 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1956 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9136 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      329 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/km/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      541 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9349 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7522 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9544 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      330 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      547 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)      974 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8998 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1523 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    12586 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9259 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9404 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9626 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9514 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9661 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9432 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    11836 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9494 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9289 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9382 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8820 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9248 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.588824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.604825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    15084 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9425 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1289 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    11612 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9588 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8987 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 izzie     (1000) izzie     (1000)     8854 2024-05-14 01:36:01.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1249 2023-02-16 21:16:23.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mouse.lua
--rwxr-xr-x   0 izzie     (1000) izzie     (1000)     3226 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mpv_shim.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    38325 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/player.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1180 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/rich_presence.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2106 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/settings_base.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     5568 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/svp_integration.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    23065 2023-02-15 02:33:10.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/syncplay.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/systray.png
--rw-r--r--   0 izzie     (1000) izzie     (1000)     3412 2023-02-25 22:58:52.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/thumbfast.lua
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1974 2023-02-21 04:22:14.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/timeline.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)   101980 2024-05-13 21:22:11.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay-osc.lua
--rw-r--r--   0 izzie     (1000) izzie     (1000)     4780 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2740 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/update_check.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)    10115 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/utils.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     7835 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/video_profile.py
--rw-r--r--   0 izzie     (1000) izzie     (1000)     1385 2023-02-13 06:22:58.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/win_utils.py
-drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 01:36:02.592824 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/
--rw-r--r--   0 izzie     (1000) izzie     (1000)    39199 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/PKG-INFO
--rw-r--r--   0 izzie     (1000) izzie     (1000)     9452 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/SOURCES.txt
--rw-r--r--   0 izzie     (1000) izzie     (1000)        1 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/dependency_links.txt
--rw-r--r--   0 izzie     (1000) izzie     (1000)       70 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/entry_points.txt
--rw-r--r--   0 izzie     (1000) izzie     (1000)      214 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/requires.txt
--rw-r--r--   0 izzie     (1000) izzie     (1000)       18 2024-05-14 01:36:02.000000 jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/top_level.txt
--rw-r--r--   0 izzie     (1000) izzie     (1000)       38 2024-05-14 01:36:02.608825 jellyfin-mpv-shim-2.7.0/setup.cfg
--rw-r--r--   0 izzie     (1000) izzie     (1000)     2128 2024-05-13 22:26:09.000000 jellyfin-mpv-shim-2.7.0/setup.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    36330 2024-05-13 18:21:11.000000 jellyfin-mpv-shim-2.7.0.post1/LICENSE.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      316 2023-02-25 22:55:04.000000 jellyfin-mpv-shim-2.7.0.post1/MANIFEST.in
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    39205 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/PKG-INFO
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    38603 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0.post1/README.md
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.599019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       25 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/__init__.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      660 2023-02-17 22:23:05.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/action_thread.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1704 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/bifdecode.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8952 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/bulk_subtitle.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      352 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/cli_mgr.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10750 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/clients.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6890 2024-05-13 18:01:16.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/conf.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1735 2023-02-24 22:10:52.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/conffile.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      593 2024-05-13 21:21:39.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/constants.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.599019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2160 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/LICENSE.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2971 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/README.md
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7249 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack-hq.json
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10428 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack-next.json
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6781 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack.json
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1596 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1604 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2884 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6594 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6179 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4705 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6695 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2848 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4340 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     3923 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    69921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    35916 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    17136 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    70020 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    36016 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    17198 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   308873 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   144204 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   308660 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   144075 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6482 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6184 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6571 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    73443 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    37685 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18638 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   290257 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   146743 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16063 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4988 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6590 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    73584 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    37714 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18667 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   290040 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   146811 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4159 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6548 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    13921 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16217 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   246177 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    70598 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    26173 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7444 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   331721 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    48421 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   655609 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    88885 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   169871 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      664 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      666 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      624 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      625 2023-03-07 06:40:19.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     5714 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/__init__.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9235 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/helpers.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7620 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/index.html
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    18550 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/jellyfin.css
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6149 2022-06-11 04:16:20.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/event_handler.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    14650 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/gui_mgr.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      909 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/i18n.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16012 2024-05-14 06:36:24.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      160 2021-04-20 00:09:50.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.desktop
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12729 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-128.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-16.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    19703 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-256.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1661 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-32.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2444 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-48.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     6709 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-64.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2366 2024-05-14 00:00:06.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/log_utils.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    16222 2024-05-14 00:37:26.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/media.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    19810 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/menu.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/af/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/af/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4893 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/am/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/am/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      538 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ar/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10706 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/be/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/be/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11509 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bg/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12209 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4358 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ca/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9722 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ckb/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9098 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cs/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9569 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cy/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9197 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/da/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/da/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9129 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/de/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/de/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9408 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/el/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/el/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12144 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/en_GB/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8802 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/eo/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8722 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9666 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_419/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9827 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_AR/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9654 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/et/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/et/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9084 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fa/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.607020 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10970 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.591019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9443 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fil/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9524 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9653 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ga/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1645 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/gl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9245 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/he/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/he/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9992 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4272 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9532 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hu/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9735 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/id/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/id/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9024 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/it/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/it/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9305 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ja/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7698 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/jbo/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1956 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9136 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/km/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/km/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      329 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/km/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      541 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ko/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9349 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lt/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7522 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lv/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9544 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lzh/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      330 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lzh/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ml/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      547 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/mn/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      974 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nb_NO/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8998 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nds/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1523 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ne/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    12586 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9259 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9404 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9626 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_BR/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9514 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_PT/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9661 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ro/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9432 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ru/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11836 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9494 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sl/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9289 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sq/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9382 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8820 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sv/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9248 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ta/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    15084 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/tr/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9425 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ug/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1289 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/uk/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    11612 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/vi/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9588 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hans/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8987 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.595019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hant/
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     8854 2024-05-14 06:38:36.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1249 2023-02-16 21:16:23.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/mouse.lua
+-rwxr-xr-x   0 izzie     (1000) izzie     (1000)     3226 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/mpv_shim.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    38325 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/player.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1180 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/rich_presence.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2106 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/settings_base.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     5568 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/svp_integration.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    23065 2023-02-15 02:33:10.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/syncplay.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      787 2021-04-20 00:07:33.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/systray.png
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     3412 2023-02-25 22:58:52.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/thumbfast.lua
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1974 2023-02-21 04:22:14.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/timeline.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)   101980 2024-05-13 21:22:11.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/trickplay-osc.lua
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     4780 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/trickplay.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2740 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/update_check.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    10115 2024-05-13 23:59:41.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/utils.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     7835 2023-02-15 02:33:09.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/video_profile.py
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     1385 2023-02-13 06:22:58.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/win_utils.py
+drwxr-xr-x   0 izzie     (1000) izzie     (1000)        0 2024-05-14 06:38:37.599019 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/
+-rw-r--r--   0 izzie     (1000) izzie     (1000)    39205 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/PKG-INFO
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     9452 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/SOURCES.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)        1 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/dependency_links.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       70 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/entry_points.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)      214 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/requires.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       18 2024-05-14 06:38:37.000000 jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/top_level.txt
+-rw-r--r--   0 izzie     (1000) izzie     (1000)       38 2024-05-14 06:38:37.611019 jellyfin-mpv-shim-2.7.0.post1/setup.cfg
+-rw-r--r--   0 izzie     (1000) izzie     (1000)     2134 2024-05-14 06:37:31.000000 jellyfin-mpv-shim-2.7.0.post1/setup.py
```

### Comparing `jellyfin-mpv-shim-2.7.0/LICENSE.md` & `jellyfin-mpv-shim-2.7.0.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/PKG-INFO` & `jellyfin-mpv-shim-2.7.0.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyfin-mpv-shim
-Version: 2.7.0
+Version: 2.7.0.post1
 Summary: Cast media from Jellyfin Mobile and Web apps to MPV.
 Home-page: https://github.com/jellyfin/jellyfin-mpv-shim
 Author: Izzie Walton
 Author-email: izzie@iwalton.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jellyfin-mpv-shim-2.7.0/README.md` & `jellyfin-mpv-shim-2.7.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/action_thread.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/action_thread.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bifdecode.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/bifdecode.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/bulk_subtitle.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/bulk_subtitle.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/clients.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/clients.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conf.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/conf.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/conffile.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/conffile.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/constants.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/constants.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/LICENSE.md` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/README.md` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/README.md`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-hq.json` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack-hq.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack-next.json` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack-next.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/pack.json` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/pack.json`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_AutoDownscalePre_x4.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Clamp_Highlights.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_Fast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_HQ.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Darken_VeryFast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_DoG.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Deblur_Original.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mean.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Median.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Denoise_Bilateral_Mode.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_Soft_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Restore_CNN_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_Fast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_HQ.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Thin_VeryFast.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_CNN_x2_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DTD_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_DoG_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Deblur_Original_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_L.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_M.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_S.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_UL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Denoise_CNN_x2_VL.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_DoG_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/Anime4K_Upscale_Original_x2.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/CAS-scaled.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSR.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_16-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/FSRCNNX_x2_8-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/KrigBilateral.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/NVScaler.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/SSimDownscaler.glsl`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns128-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns16-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns256-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns32-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/nnedi3-nns64-win8x6.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_chroma_strong.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/default_shader_pack/shaders/noise_static_luma_strong.hook`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/__init__.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/__init__.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/helpers.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/helpers.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/index.html` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/index.html`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/display_mirror/jellyfin.css` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/display_mirror/jellyfin.css`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/event_handler.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/event_handler.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/gui_mgr.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/gui_mgr.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/i18n.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/i18n.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/com.github.iwalton3.jellyfin-mpv-shim.appdata.xml`

```diff
@@ -48,19 +48,22 @@
     <binary>jellyfin-mpv-shim</binary>
   </provides>
   <launchable type="desktop-id">com.github.iwalton3.jellyfin-mpv-shim.desktop</launchable>
   <content_rating type="oars-1.1"/>
   <releases>
     <release version="2.7.0" date="2024-05-13">
       <description>
-        <li>Switch to native Jellyfin Trickplay support.</li>
-        <li>Update mpv version to latest git version.</li>
-        <li>Fix support for newer MPV versions. (#377)</li>
-        <li>Make log level configurable. (#379)</li>
-        <li>Fix icon title. (#380)</li>
+        <p>Changes:</p>
+        <ul>
+          <li>Switch to native Jellyfin Trickplay support.</li>
+          <li>Update mpv version to latest git version.</li>
+          <li>Fix support for newer MPV versions. (#377)</li>
+          <li>Make log level configurable. (#379)</li>
+          <li>Fix icon title. (#380)</li>
+        </ul>
       </description>
     </release>
     <release version="2.6.0" date="2023-03-07">
       <description>
         <p>Disable built-in MPV playback resuming. (#323)</p>
         <p>Support IPv6 addressing with a protocol prefix (#306)</p>
         <p>Switch to mpv build 20230304 362256e with TLS 1.3 support.</p>
```

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-128.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-128.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-16.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-16.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-256.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-256.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-32.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-32.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-48.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-48.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/integration/jellyfin-64.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/integration/jellyfin-64.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/log_utils.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/log_utils.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/media.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/media.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/menu.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/menu.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/af/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/am/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ar/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/be/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bg/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/bn/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ca/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ckb/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cs/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/cy/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/da/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/de/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/el/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/en_GB/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/eo/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_419/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/es_AR/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/et/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fa/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fil/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/fr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ga/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/gl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/he/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/hu/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/id/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/it/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ja/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/jbo/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kk/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/kn/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ko/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/lv/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ml/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/mn/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nb_NO/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nds/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ne/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/nl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_BR/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/pt_PT/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ro/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ru/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sk/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sl/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sq/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/sv/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ta/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/tr/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/ug/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/uk/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/vi/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hans/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/messages/zh_Hant/LC_MESSAGES/base.mo`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mouse.lua` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/mouse.lua`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/mpv_shim.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/mpv_shim.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/player.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/player.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/rich_presence.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/rich_presence.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/settings_base.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/settings_base.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/svp_integration.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/svp_integration.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/syncplay.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/syncplay.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/systray.png` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/systray.png`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/thumbfast.lua` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/thumbfast.lua`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/timeline.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/timeline.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay-osc.lua` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/trickplay-osc.lua`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/trickplay.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/trickplay.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/update_check.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/update_check.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/utils.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/utils.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/video_profile.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/video_profile.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim/win_utils.py` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim/win_utils.py`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/PKG-INFO` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jellyfin-mpv-shim
-Version: 2.7.0
+Version: 2.7.0.post1
 Summary: Cast media from Jellyfin Mobile and Web apps to MPV.
 Home-page: https://github.com/jellyfin/jellyfin-mpv-shim
 Author: Izzie Walton
 Author-email: izzie@iwalton.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `jellyfin-mpv-shim-2.7.0/jellyfin_mpv_shim.egg-info/SOURCES.txt` & `jellyfin-mpv-shim-2.7.0.post1/jellyfin_mpv_shim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jellyfin-mpv-shim-2.7.0/setup.py` & `jellyfin-mpv-shim-2.7.0.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     for dir in os.listdir("jellyfin_mpv_shim/messages"):
         if os.path.isdir("jellyfin_mpv_shim/messages/" + dir + "/LC_MESSAGES"):
             packages.append("jellyfin_mpv_shim.messages." + dir + ".LC_MESSAGES")
 
 setup(
     name="jellyfin-mpv-shim",
-    version="2.7.0",
+    version="2.7.0.post1",
     author="Izzie Walton",
     author_email="izzie@iwalton.com",
     description="Cast media from Jellyfin Mobile and Web apps to MPV.",
     license="GPLv3",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/jellyfin/jellyfin-mpv-shim",
```

